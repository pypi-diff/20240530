# Comparing `tmp/authentik_client-2024.4.2.post1716550398.tar.gz` & `tmp/authentik_client-2024.4.2.post1717033274.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.4.2.post1716550398.tar", max compression
+gzip compressed data, was "authentik_client-2024.4.2.post1717033274.tar", max compression
```

## Comparing `authentik_client-2024.4.2.post1716550398.tar` & `authentik_client-2024.4.2.post1717033274.tar`

### file list

```diff
@@ -1,629 +1,625 @@
--rw-r--r--   0        0        0   157814 2024-05-24 11:33:32.409699 authentik_client-2024.4.2.post1716550398/README.md
--rw-r--r--   0        0        0    52224 2024-05-24 11:33:32.421699 authentik_client-2024.4.2.post1716550398/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-05-24 11:33:32.421699 authentik_client-2024.4.2.post1716550398/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-05-24 11:33:32.081702 authentik_client-2024.4.2.post1716550398/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-05-24 11:33:32.101702 authentik_client-2024.4.2.post1716550398/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701822 2024-05-24 11:33:32.129701 authentik_client-2024.4.2.post1716550398/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-05-24 11:33:32.141701 authentik_client-2024.4.2.post1716550398/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-05-24 11:33:32.153701 authentik_client-2024.4.2.post1716550398/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-05-24 11:33:32.173701 authentik_client-2024.4.2.post1716550398/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-05-24 11:33:32.185701 authentik_client-2024.4.2.post1716550398/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-05-24 11:33:32.197701 authentik_client-2024.4.2.post1716550398/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-05-24 11:33:32.205701 authentik_client-2024.4.2.post1716550398/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413244 2024-05-24 11:33:32.221701 authentik_client-2024.4.2.post1716550398/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725180 2024-05-24 11:33:32.241701 authentik_client-2024.4.2.post1716550398/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   721894 2024-05-24 11:33:32.261700 authentik_client-2024.4.2.post1716550398/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0  1235052 2024-05-24 11:33:32.289700 authentik_client-2024.4.2.post1716550398/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-05-24 11:33:32.301700 authentik_client-2024.4.2.post1716550398/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-05-24 11:33:32.313700 authentik_client-2024.4.2.post1716550398/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-05-24 11:33:32.317700 authentik_client-2024.4.2.post1716550398/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-05-24 11:33:32.321700 authentik_client-2024.4.2.post1716550398/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037175 2024-05-24 11:33:32.341700 authentik_client-2024.4.2.post1716550398/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945968 2024-05-24 11:33:32.381699 authentik_client-2024.4.2.post1716550398/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-05-24 11:33:32.397699 authentik_client-2024.4.2.post1716550398/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-05-24 11:33:32.425699 authentik_client-2024.4.2.post1716550398/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-05-24 11:33:32.425699 authentik_client-2024.4.2.post1716550398/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-05-24 11:33:32.417699 authentik_client-2024.4.2.post1716550398/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-05-24 11:33:32.421699 authentik_client-2024.4.2.post1716550398/authentik_client/exceptions.py
--rw-r--r--   0        0        0    50526 2024-05-24 11:33:32.421699 authentik_client-2024.4.2.post1716550398/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-05-24 11:33:29.097727 authentik_client-2024.4.2.post1716550398/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0      688 2024-05-24 11:33:29.105727 authentik_client-2024.4.2.post1716550398/authentik_client/models/alg_enum.py
--rw-r--r--   0        0        0     2482 2024-05-24 11:33:29.117726 authentik_client-2024.4.2.post1716550398/authentik_client/models/app.py
--rw-r--r--   0        0        0     4460 2024-05-24 11:33:29.121726 authentik_client-2024.4.2.post1716550398/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-05-24 11:33:29.129726 authentik_client-2024.4.2.post1716550398/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-05-24 11:33:29.141726 authentik_client-2024.4.2.post1716550398/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-05-24 11:33:29.149726 authentik_client-2024.4.2.post1716550398/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-05-24 11:33:29.157726 authentik_client-2024.4.2.post1716550398/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-05-24 11:33:29.161726 authentik_client-2024.4.2.post1716550398/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-05-24 11:33:29.165726 authentik_client-2024.4.2.post1716550398/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-05-24 11:33:29.173726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-05-24 11:33:29.177726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-05-24 11:33:29.185726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-05-24 11:33:29.189726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-05-24 11:33:29.193726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-05-24 11:33:29.201726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-05-24 11:33:29.209726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-05-24 11:33:29.213726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-05-24 11:33:29.213726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-05-24 11:33:29.221726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-05-24 11:33:29.229725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-05-24 11:33:29.237725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-05-24 11:33:29.241726 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-05-24 11:33:29.245725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-05-24 11:33:29.253725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-24 11:33:29.257725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-05-24 11:33:29.265725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-05-24 11:33:29.269725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-05-24 11:33:29.277725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-05-24 11:33:29.285725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-05-24 11:33:29.293725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-05-24 11:33:29.297725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-05-24 11:33:29.305725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-05-24 11:33:29.313725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-05-24 11:33:29.317725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-05-24 11:33:29.325725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-05-24 11:33:29.337725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-05-24 11:33:29.341724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-05-24 11:33:29.349725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-05-24 11:33:29.357725 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-05-24 11:33:29.369724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-05-24 11:33:29.373724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-05-24 11:33:29.381724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-05-24 11:33:29.385724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-05-24 11:33:29.393724 authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-05-24 11:33:29.401724 authentik_client-2024.4.2.post1716550398/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-05-24 11:33:29.405724 authentik_client-2024.4.2.post1716550398/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-05-24 11:33:29.409724 authentik_client-2024.4.2.post1716550398/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-05-24 11:33:29.413724 authentik_client-2024.4.2.post1716550398/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-05-24 11:33:29.417724 authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-05-24 11:33:29.417724 authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-05-24 11:33:29.421724 authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-05-24 11:33:29.425724 authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-05-24 11:33:29.429724 authentik_client-2024.4.2.post1716550398/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-05-24 11:33:29.437724 authentik_client-2024.4.2.post1716550398/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-05-24 11:33:29.441724 authentik_client-2024.4.2.post1716550398/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-05-24 11:33:29.445724 authentik_client-2024.4.2.post1716550398/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-05-24 11:33:29.449724 authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-05-24 11:33:29.453724 authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-05-24 11:33:29.461724 authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-05-24 11:33:29.465724 authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-05-24 11:33:29.473724 authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2990 2024-05-24 11:33:29.477723 authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-05-24 11:33:29.481723 authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-05-24 11:33:29.485723 authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-05-24 11:33:29.489723 authentik_client-2024.4.2.post1716550398/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-05-24 11:33:29.497723 authentik_client-2024.4.2.post1716550398/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-05-24 11:33:29.497723 authentik_client-2024.4.2.post1716550398/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-05-24 11:33:29.505723 authentik_client-2024.4.2.post1716550398/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-05-24 11:33:29.509723 authentik_client-2024.4.2.post1716550398/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-05-24 11:33:29.513723 authentik_client-2024.4.2.post1716550398/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-05-24 11:33:29.517723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-05-24 11:33:29.521723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-05-24 11:33:29.529723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-05-24 11:33:29.533723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-05-24 11:33:29.537723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-05-24 11:33:29.541723 authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-05-24 11:33:29.545723 authentik_client-2024.4.2.post1716550398/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-05-24 11:33:29.553723 authentik_client-2024.4.2.post1716550398/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-05-24 11:33:29.557723 authentik_client-2024.4.2.post1716550398/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-05-24 11:33:29.561723 authentik_client-2024.4.2.post1716550398/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-05-24 11:33:29.565723 authentik_client-2024.4.2.post1716550398/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-05-24 11:33:29.573723 authentik_client-2024.4.2.post1716550398/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-05-24 11:33:29.577723 authentik_client-2024.4.2.post1716550398/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-05-24 11:33:29.585723 authentik_client-2024.4.2.post1716550398/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-05-24 11:33:29.589722 authentik_client-2024.4.2.post1716550398/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-05-24 11:33:29.593722 authentik_client-2024.4.2.post1716550398/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-05-24 11:33:29.597722 authentik_client-2024.4.2.post1716550398/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-05-24 11:33:29.597722 authentik_client-2024.4.2.post1716550398/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-05-24 11:33:29.601722 authentik_client-2024.4.2.post1716550398/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-05-24 11:33:29.605722 authentik_client-2024.4.2.post1716550398/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-05-24 11:33:29.609722 authentik_client-2024.4.2.post1716550398/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-05-24 11:33:29.613722 authentik_client-2024.4.2.post1716550398/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-05-24 11:33:29.617722 authentik_client-2024.4.2.post1716550398/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-05-24 11:33:29.621722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-05-24 11:33:29.625722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-05-24 11:33:29.629722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-05-24 11:33:29.633722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-05-24 11:33:29.637722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-05-24 11:33:29.641722 authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-05-24 11:33:29.645722 authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-05-24 11:33:29.649722 authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-05-24 11:33:29.653722 authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-05-24 11:33:29.657722 authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-05-24 11:33:29.661722 authentik_client-2024.4.2.post1716550398/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-05-24 11:33:29.665722 authentik_client-2024.4.2.post1716550398/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-05-24 11:33:29.669722 authentik_client-2024.4.2.post1716550398/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-05-24 11:33:29.677722 authentik_client-2024.4.2.post1716550398/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-05-24 11:33:29.681722 authentik_client-2024.4.2.post1716550398/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-05-24 11:33:29.685722 authentik_client-2024.4.2.post1716550398/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-05-24 11:33:29.689722 authentik_client-2024.4.2.post1716550398/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-05-24 11:33:29.693722 authentik_client-2024.4.2.post1716550398/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-05-24 11:33:29.697722 authentik_client-2024.4.2.post1716550398/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-05-24 11:33:29.697722 authentik_client-2024.4.2.post1716550398/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-05-24 11:33:29.701722 authentik_client-2024.4.2.post1716550398/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-05-24 11:33:29.709721 authentik_client-2024.4.2.post1716550398/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-05-24 11:33:29.713722 authentik_client-2024.4.2.post1716550398/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-05-24 11:33:29.717722 authentik_client-2024.4.2.post1716550398/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-05-24 11:33:29.725721 authentik_client-2024.4.2.post1716550398/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-05-24 11:33:29.729721 authentik_client-2024.4.2.post1716550398/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-05-24 11:33:29.733721 authentik_client-2024.4.2.post1716550398/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-05-24 11:33:29.737721 authentik_client-2024.4.2.post1716550398/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-05-24 11:33:29.741721 authentik_client-2024.4.2.post1716550398/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-05-24 11:33:29.745721 authentik_client-2024.4.2.post1716550398/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-05-24 11:33:29.753721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-05-24 11:33:29.757721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-05-24 11:33:29.761721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-05-24 11:33:29.765721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-05-24 11:33:29.769721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-05-24 11:33:29.777721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-05-24 11:33:29.781721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-05-24 11:33:29.785721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-05-24 11:33:29.789721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-05-24 11:33:29.793721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-05-24 11:33:29.797721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-05-24 11:33:29.801721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-05-24 11:33:29.805721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-05-24 11:33:29.809721 authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-05-24 11:33:29.813721 authentik_client-2024.4.2.post1716550398/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-05-24 11:33:29.817721 authentik_client-2024.4.2.post1716550398/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-05-24 11:33:29.817721 authentik_client-2024.4.2.post1716550398/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     6418 2024-05-24 11:33:29.821721 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider.py
--rw-r--r--   0        0        0     3083 2024-05-24 11:33:29.825721 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_group.py
--rw-r--r--   0        0        0     2526 2024-05-24 11:33:29.829721 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_group_request.py
--rw-r--r--   0        0        0     4324 2024-05-24 11:33:29.833721 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_mapping.py
--rw-r--r--   0        0        0     3385 2024-05-24 11:33:29.837720 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_mapping_request.py
--rw-r--r--   0        0        0     4740 2024-05-24 11:33:29.841720 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_request.py
--rw-r--r--   0        0        0     3084 2024-05-24 11:33:29.845720 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_user.py
--rw-r--r--   0        0        0     2518 2024-05-24 11:33:29.849720 authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_user_request.py
--rw-r--r--   0        0        0     5445 2024-05-24 11:33:29.853720 authentik_client-2024.4.2.post1716550398/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-05-24 11:33:29.857720 authentik_client-2024.4.2.post1716550398/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-05-24 11:33:29.861720 authentik_client-2024.4.2.post1716550398/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-05-24 11:33:29.865720 authentik_client-2024.4.2.post1716550398/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-05-24 11:33:29.869720 authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-05-24 11:33:29.873720 authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-05-24 11:33:29.877720 authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-05-24 11:33:29.885720 authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-05-24 11:33:29.885720 authentik_client-2024.4.2.post1716550398/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-05-24 11:33:29.889720 authentik_client-2024.4.2.post1716550398/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-05-24 11:33:29.889720 authentik_client-2024.4.2.post1716550398/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-05-24 11:33:29.893720 authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-05-24 11:33:29.901720 authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-05-24 11:33:29.905720 authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-05-24 11:33:29.909720 authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-05-24 11:33:29.909720 authentik_client-2024.4.2.post1716550398/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-05-24 11:33:29.913720 authentik_client-2024.4.2.post1716550398/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-05-24 11:33:29.917720 authentik_client-2024.4.2.post1716550398/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-05-24 11:33:29.921720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-05-24 11:33:29.925720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-05-24 11:33:29.929720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-05-24 11:33:29.933720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-05-24 11:33:29.937720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-05-24 11:33:29.941720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11470 2024-05-24 11:33:29.945720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-05-24 11:33:29.953719 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0      726 2024-05-24 11:33:29.917720 authentik_client-2024.4.2.post1716550398/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-05-24 11:33:29.957719 authentik_client-2024.4.2.post1716550398/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-05-24 11:33:29.957719 authentik_client-2024.4.2.post1716550398/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-05-24 11:33:29.961719 authentik_client-2024.4.2.post1716550398/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-05-24 11:33:29.965719 authentik_client-2024.4.2.post1716550398/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-05-24 11:33:29.969719 authentik_client-2024.4.2.post1716550398/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-05-24 11:33:29.973719 authentik_client-2024.4.2.post1716550398/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-05-24 11:33:29.977719 authentik_client-2024.4.2.post1716550398/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-05-24 11:33:29.981719 authentik_client-2024.4.2.post1716550398/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-05-24 11:33:29.985719 authentik_client-2024.4.2.post1716550398/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-05-24 11:33:29.989719 authentik_client-2024.4.2.post1716550398/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-05-24 11:33:29.989719 authentik_client-2024.4.2.post1716550398/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     5920 2024-05-24 11:33:29.993719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider.py
--rw-r--r--   0        0        0     3079 2024-05-24 11:33:29.997719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_group.py
--rw-r--r--   0        0        0     2522 2024-05-24 11:33:30.001719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_group_request.py
--rw-r--r--   0        0        0     4320 2024-05-24 11:33:30.005719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_mapping.py
--rw-r--r--   0        0        0     3381 2024-05-24 11:33:30.009719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_mapping_request.py
--rw-r--r--   0        0        0     4307 2024-05-24 11:33:30.013719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_request.py
--rw-r--r--   0        0        0     3080 2024-05-24 11:33:30.017719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_user.py
--rw-r--r--   0        0        0     2514 2024-05-24 11:33:30.017719 authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_user_request.py
--rw-r--r--   0        0        0     8160 2024-05-24 11:33:30.021719 authentik_client-2024.4.2.post1716550398/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0    11885 2024-05-24 11:33:30.025719 authentik_client-2024.4.2.post1716550398/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-05-24 11:33:30.025719 authentik_client-2024.4.2.post1716550398/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-05-24 11:33:30.029719 authentik_client-2024.4.2.post1716550398/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-05-24 11:33:30.029719 authentik_client-2024.4.2.post1716550398/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-05-24 11:33:30.033719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-05-24 11:33:30.037719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-05-24 11:33:30.041719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-05-24 11:33:30.045719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-05-24 11:33:30.049719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-05-24 11:33:30.053719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-05-24 11:33:30.057719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-05-24 11:33:30.057719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-05-24 11:33:30.061719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-05-24 11:33:30.065719 authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-05-24 11:33:30.069718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-05-24 11:33:30.073718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-05-24 11:33:30.077719 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-05-24 11:33:30.085718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-05-24 11:33:30.093718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-05-24 11:33:30.097718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-05-24 11:33:30.101718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10451 2024-05-24 11:33:30.109718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-05-24 11:33:30.113718 authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-05-24 11:33:30.117718 authentik_client-2024.4.2.post1716550398/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0      779 2024-05-24 11:33:30.121718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outgoing_sync_delete_action.py
--rw-r--r--   0        0        0     5545 2024-05-24 11:33:30.125718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-05-24 11:33:30.129718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     4497 2024-05-24 11:33:30.133718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-05-24 11:33:30.137718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-05-24 11:33:30.141718 authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-05-24 11:33:30.145718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-05-24 11:33:30.149718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-05-24 11:33:30.153718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-05-24 11:33:30.157718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-05-24 11:33:30.157718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-05-24 11:33:30.161718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-05-24 11:33:30.165718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-05-24 11:33:30.169718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-05-24 11:33:30.173718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-05-24 11:33:30.177718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.181718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-05-24 11:33:30.185718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-05-24 11:33:30.185718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.189718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-24 11:33:30.193718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-05-24 11:33:30.197718 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-05-24 11:33:30.201717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.205717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.209717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-24 11:33:30.213717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.217717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-05-24 11:33:30.221717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-05-24 11:33:30.221717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-05-24 11:33:30.225717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-05-24 11:33:30.229717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-05-24 11:33:30.233717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-05-24 11:33:30.237717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-05-24 11:33:30.241717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-24 11:33:30.245717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-05-24 11:33:30.249717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3461 2024-05-24 11:33:30.253717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_group_list.py
--rw-r--r--   0        0        0     3420 2024-05-24 11:33:30.257717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_list.py
--rw-r--r--   0        0        0     3477 2024-05-24 11:33:30.261717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_mapping_list.py
--rw-r--r--   0        0        0     3453 2024-05-24 11:33:30.265717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_user_list.py
--rw-r--r--   0        0        0     3274 2024-05-24 11:33:30.265717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-05-24 11:33:30.269717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-24 11:33:30.273717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-05-24 11:33:30.277717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-05-24 11:33:30.281717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-05-24 11:33:30.281717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-05-24 11:33:30.285717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.289717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.293717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-24 11:33:30.297717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3453 2024-05-24 11:33:30.301717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_group_list.py
--rw-r--r--   0        0        0     3412 2024-05-24 11:33:30.305717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_list.py
--rw-r--r--   0        0        0     3469 2024-05-24 11:33:30.309717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py
--rw-r--r--   0        0        0     3445 2024-05-24 11:33:30.313717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_user_list.py
--rw-r--r--   0        0        0     3330 2024-05-24 11:33:30.313717 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-05-24 11:33:30.317716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-05-24 11:33:30.321716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-05-24 11:33:30.325716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-05-24 11:33:30.329716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-05-24 11:33:30.333716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-24 11:33:30.337716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-05-24 11:33:30.341716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-05-24 11:33:30.341716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-05-24 11:33:30.345716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-24 11:33:30.349716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-05-24 11:33:30.353716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.357716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-05-24 11:33:30.361716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-05-24 11:33:30.365716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-05-24 11:33:30.365716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.369716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-05-24 11:33:30.373716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-05-24 11:33:30.377716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-24 11:33:30.381716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-05-24 11:33:30.385716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-24 11:33:30.389716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.389716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-05-24 11:33:30.393716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-05-24 11:33:30.397716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-05-24 11:33:30.397716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-05-24 11:33:30.401716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-05-24 11:33:30.405716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-24 11:33:30.405716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-05-24 11:33:30.409716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.413716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.417716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.417716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.421716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-05-24 11:33:30.425716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.425716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-05-24 11:33:30.429715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.437715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-05-24 11:33:30.437715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-05-24 11:33:30.433715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-05-24 11:33:30.441716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.445716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-05-24 11:33:30.445716 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-05-24 11:33:30.449715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.453715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-05-24 11:33:30.457715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-05-24 11:33:30.461715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.465715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-05-24 11:33:30.457715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-05-24 11:33:30.465715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-05-24 11:33:30.469715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-05-24 11:33:30.473715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-05-24 11:33:30.473715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-05-24 11:33:30.477715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-05-24 11:33:30.481715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-05-24 11:33:30.485715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-05-24 11:33:30.485715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-05-24 11:33:30.489715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-05-24 11:33:30.493715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-05-24 11:33:30.493715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-05-24 11:33:30.497715 authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-05-24 11:33:30.501715 authentik_client-2024.4.2.post1716550398/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-05-24 11:33:30.505715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-05-24 11:33:30.505715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-05-24 11:33:30.509715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-05-24 11:33:30.513715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-05-24 11:33:30.517715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-05-24 11:33:30.521715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-05-24 11:33:30.525715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-05-24 11:33:30.529715 authentik_client-2024.4.2.post1716550398/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-24 11:33:30.533715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-05-24 11:33:30.537715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-05-24 11:33:30.541715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-05-24 11:33:30.541715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-05-24 11:33:30.545715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-05-24 11:33:30.549715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-05-24 11:33:30.553715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-05-24 11:33:30.557715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-05-24 11:33:30.561715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-05-24 11:33:30.561715 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-05-24 11:33:30.565714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-05-24 11:33:30.569714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-05-24 11:33:30.573714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-05-24 11:33:30.573714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-05-24 11:33:30.577714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-05-24 11:33:30.581714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-05-24 11:33:30.585714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-05-24 11:33:30.585714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-05-24 11:33:30.589714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-05-24 11:33:30.593714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-05-24 11:33:30.597714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-05-24 11:33:30.597714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-05-24 11:33:30.601714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-05-24 11:33:30.605714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-05-24 11:33:30.609714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-05-24 11:33:30.613714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     2574 2024-05-24 11:33:30.617714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_group_request.py
--rw-r--r--   0        0        0     3440 2024-05-24 11:33:30.617714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_mapping_request.py
--rw-r--r--   0        0        0     4819 2024-05-24 11:33:30.621714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_request.py
--rw-r--r--   0        0        0     2566 2024-05-24 11:33:30.625714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_user_request.py
--rw-r--r--   0        0        0     3385 2024-05-24 11:33:30.629714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-05-24 11:33:30.629714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-05-24 11:33:30.633714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-05-24 11:33:30.637714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-05-24 11:33:30.637714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-05-24 11:33:30.641714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-05-24 11:33:30.645714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-05-24 11:33:30.649714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-05-24 11:33:30.653714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2570 2024-05-24 11:33:30.657714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_group_request.py
--rw-r--r--   0        0        0     3436 2024-05-24 11:33:30.661714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py
--rw-r--r--   0        0        0     4396 2024-05-24 11:33:30.665714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_request.py
--rw-r--r--   0        0        0     2562 2024-05-24 11:33:30.669714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_user_request.py
--rw-r--r--   0        0        0     2879 2024-05-24 11:33:30.673714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-05-24 11:33:30.673714 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-05-24 11:33:30.677713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-05-24 11:33:30.681713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-05-24 11:33:30.685713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-05-24 11:33:30.685713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-05-24 11:33:30.689713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-05-24 11:33:30.693713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-05-24 11:33:30.697713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-05-24 11:33:30.697713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-05-24 11:33:30.701713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-05-24 11:33:30.705713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-05-24 11:33:30.709713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-05-24 11:33:30.709713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-05-24 11:33:30.713713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-05-24 11:33:30.717713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-05-24 11:33:30.721713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-05-24 11:33:30.725713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-05-24 11:33:30.725713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-05-24 11:33:30.729713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-05-24 11:33:30.733713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-05-24 11:33:30.733713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-05-24 11:33:30.737713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-05-24 11:33:30.741713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-05-24 11:33:30.745713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-05-24 11:33:30.745713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-05-24 11:33:30.749713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-05-24 11:33:30.753713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-05-24 11:33:30.757713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-05-24 11:33:30.761713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-05-24 11:33:30.765713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-05-24 11:33:30.769713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-05-24 11:33:30.765713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-05-24 11:33:30.773713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-05-24 11:33:30.777713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-05-24 11:33:30.781713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-05-24 11:33:30.785713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-05-24 11:33:30.777713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-05-24 11:33:30.785713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-05-24 11:33:30.789713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-05-24 11:33:30.793712 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-05-24 11:33:30.793712 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-05-24 11:33:30.797712 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-05-24 11:33:30.801712 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-05-24 11:33:30.805713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-05-24 11:33:30.805713 authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-05-24 11:33:30.809713 authentik_client-2024.4.2.post1716550398/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-05-24 11:33:30.813712 authentik_client-2024.4.2.post1716550398/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-05-24 11:33:30.817712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-05-24 11:33:30.817712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7431 2024-05-24 11:33:30.821712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-05-24 11:33:30.821712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-05-24 11:33:30.825712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-05-24 11:33:30.829712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-05-24 11:33:30.829712 authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-05-24 11:33:30.829712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-05-24 11:33:30.833712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-05-24 11:33:30.837712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-05-24 11:33:30.837712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-05-24 11:33:30.837712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-05-24 11:33:30.841712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-05-24 11:33:30.841712 authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-05-24 11:33:30.845712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-05-24 11:33:30.845712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-05-24 11:33:30.849712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-05-24 11:33:30.849712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-05-24 11:33:30.853712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-05-24 11:33:30.857712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-05-24 11:33:30.857712 authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-05-24 11:33:30.861712 authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-05-24 11:33:30.861712 authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2740 2024-05-24 11:33:30.865712 authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_test_request.py
--rw-r--r--   0        0        0     2744 2024-05-24 11:33:30.869712 authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-05-24 11:33:30.869712 authentik_client-2024.4.2.post1716550398/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-05-24 11:33:30.873712 authentik_client-2024.4.2.post1716550398/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-05-24 11:33:30.873712 authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1578 2024-05-24 11:33:30.873712 authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-05-24 11:33:30.877712 authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-05-24 11:33:30.877712 authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-05-24 11:33:30.881712 authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-05-24 11:33:30.881712 authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-05-24 11:33:30.885712 authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-05-24 11:33:30.889712 authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-05-24 11:33:30.889712 authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-05-24 11:33:30.893712 authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-05-24 11:33:30.897712 authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-05-24 11:33:30.897712 authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-05-24 11:33:30.901712 authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-05-24 11:33:30.901712 authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-05-24 11:33:30.905712 authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-05-24 11:33:30.909712 authentik_client-2024.4.2.post1716550398/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-05-24 11:33:30.913712 authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-05-24 11:33:30.913712 authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-05-24 11:33:30.917712 authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-05-24 11:33:30.917712 authentik_client-2024.4.2.post1716550398/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-05-24 11:33:30.917712 authentik_client-2024.4.2.post1716550398/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-05-24 11:33:30.921712 authentik_client-2024.4.2.post1716550398/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-05-24 11:33:30.921712 authentik_client-2024.4.2.post1716550398/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-05-24 11:33:30.925711 authentik_client-2024.4.2.post1716550398/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-05-24 11:33:30.925711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-05-24 11:33:30.929711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-05-24 11:33:30.929711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-05-24 11:33:30.933711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-05-24 11:33:30.933711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10242 2024-05-24 11:33:30.937711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-05-24 11:33:30.937711 authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-05-24 11:33:30.941711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-05-24 11:33:30.941711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-05-24 11:33:30.945711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-05-24 11:33:30.945711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-05-24 11:33:30.949711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-05-24 11:33:30.953711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-05-24 11:33:30.953711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-05-24 11:33:30.957711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-05-24 11:33:30.961711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-05-24 11:33:30.965711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     4629 2024-05-24 11:33:30.973711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-05-24 11:33:30.973711 authentik_client-2024.4.2.post1716550398/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-05-24 11:33:30.977711 authentik_client-2024.4.2.post1716550398/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-05-24 11:33:30.977711 authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-05-24 11:33:30.977711 authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-05-24 11:33:30.981711 authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-05-24 11:33:30.981711 authentik_client-2024.4.2.post1716550398/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-05-24 11:33:30.985711 authentik_client-2024.4.2.post1716550398/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-05-24 11:33:30.989711 authentik_client-2024.4.2.post1716550398/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-05-24 11:33:30.989711 authentik_client-2024.4.2.post1716550398/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-05-24 11:33:30.993711 authentik_client-2024.4.2.post1716550398/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     2172 2024-05-24 11:33:30.993711 authentik_client-2024.4.2.post1716550398/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-05-24 11:33:30.965711 authentik_client-2024.4.2.post1716550398/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-05-24 11:33:30.969711 authentik_client-2024.4.2.post1716550398/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-05-24 11:33:30.997711 authentik_client-2024.4.2.post1716550398/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-05-24 11:33:31.001711 authentik_client-2024.4.2.post1716550398/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-05-24 11:33:31.001711 authentik_client-2024.4.2.post1716550398/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-05-24 11:33:31.005711 authentik_client-2024.4.2.post1716550398/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-05-24 11:33:31.009711 authentik_client-2024.4.2.post1716550398/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-05-24 11:33:31.009711 authentik_client-2024.4.2.post1716550398/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-05-24 11:33:31.013711 authentik_client-2024.4.2.post1716550398/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-05-24 11:33:31.017711 authentik_client-2024.4.2.post1716550398/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-05-24 11:33:31.017711 authentik_client-2024.4.2.post1716550398/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-05-24 11:33:31.021711 authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-05-24 11:33:31.025711 authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-05-24 11:33:31.025711 authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-05-24 11:33:31.029711 authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-05-24 11:33:31.029711 authentik_client-2024.4.2.post1716550398/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     3114 2024-05-24 11:33:31.033711 authentik_client-2024.4.2.post1716550398/authentik_client/models/sync_status.py
--rw-r--r--   0        0        0     4463 2024-05-24 11:33:31.033711 authentik_client-2024.4.2.post1716550398/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     3177 2024-05-24 11:33:31.037711 authentik_client-2024.4.2.post1716550398/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4701 2024-05-24 11:33:31.037711 authentik_client-2024.4.2.post1716550398/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-05-24 11:33:31.041710 authentik_client-2024.4.2.post1716550398/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-05-24 11:33:31.045710 authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-05-24 11:33:31.049710 authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-05-24 11:33:31.053710 authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-05-24 11:33:31.053710 authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-05-24 11:33:31.057710 authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-05-24 11:33:31.057710 authentik_client-2024.4.2.post1716550398/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-05-24 11:33:31.061710 authentik_client-2024.4.2.post1716550398/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-05-24 11:33:31.065710 authentik_client-2024.4.2.post1716550398/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-05-24 11:33:31.065710 authentik_client-2024.4.2.post1716550398/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-05-24 11:33:31.069710 authentik_client-2024.4.2.post1716550398/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-05-24 11:33:31.041710 authentik_client-2024.4.2.post1716550398/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-05-24 11:33:31.045710 authentik_client-2024.4.2.post1716550398/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-05-24 11:33:31.069710 authentik_client-2024.4.2.post1716550398/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-05-24 11:33:31.073710 authentik_client-2024.4.2.post1716550398/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     3034 2024-05-24 11:33:31.073710 authentik_client-2024.4.2.post1716550398/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-05-24 11:33:31.073710 authentik_client-2024.4.2.post1716550398/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-05-24 11:33:31.077710 authentik_client-2024.4.2.post1716550398/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-05-24 11:33:31.077710 authentik_client-2024.4.2.post1716550398/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5459 2024-05-24 11:33:31.081710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-05-24 11:33:31.081710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-05-24 11:33:31.085710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-05-24 11:33:31.085710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-05-24 11:33:31.089710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-05-24 11:33:31.089710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-05-24 11:33:31.093710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-05-24 11:33:31.093710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-05-24 11:33:31.097710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-05-24 11:33:31.097710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-05-24 11:33:31.101710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-05-24 11:33:31.101710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-05-24 11:33:31.105710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-05-24 11:33:31.109710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-05-24 11:33:31.109710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-05-24 11:33:31.113710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-05-24 11:33:31.113710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-05-24 11:33:31.117710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-05-24 11:33:31.117710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-05-24 11:33:31.121710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-05-24 11:33:31.121710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-05-24 11:33:31.125710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-05-24 11:33:31.125710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-05-24 11:33:31.129710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-05-24 11:33:31.133710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-05-24 11:33:31.137710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-05-24 11:33:31.137710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-05-24 11:33:31.141710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-05-24 11:33:31.141710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-05-24 11:33:31.145710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-05-24 11:33:31.145710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-05-24 11:33:31.149710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-05-24 11:33:31.149710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-05-24 11:33:31.149710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-05-24 11:33:31.153710 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-05-24 11:33:31.157709 authentik_client-2024.4.2.post1716550398/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-05-24 11:33:31.157709 authentik_client-2024.4.2.post1716550398/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-05-24 11:33:31.161709 authentik_client-2024.4.2.post1716550398/authentik_client/models/version.py
--rw-r--r--   0        0        0     3786 2024-05-24 11:33:31.161709 authentik_client-2024.4.2.post1716550398/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-05-24 11:33:31.165709 authentik_client-2024.4.2.post1716550398/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-05-24 11:33:31.165709 authentik_client-2024.4.2.post1716550398/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-05-24 11:33:31.169709 authentik_client-2024.4.2.post1716550398/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-05-24 11:33:31.169709 authentik_client-2024.4.2.post1716550398/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-05-24 11:33:32.413699 authentik_client-2024.4.2.post1716550398/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-05-24 11:33:32.425699 authentik_client-2024.4.2.post1716550398/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-05-24 11:33:32.413699 authentik_client-2024.4.2.post1716550398/pyproject.toml
--rw-r--r--   0        0        0   158766 1970-01-01 00:00:00.000000 authentik_client-2024.4.2.post1716550398/PKG-INFO
+-rw-r--r--   0        0        0   155926 2024-05-30 01:41:27.649966 authentik_client-2024.4.2.post1717033274/README.md
+-rw-r--r--   0        0        0    51724 2024-05-30 01:41:27.661966 authentik_client-2024.4.2.post1717033274/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-05-30 01:41:27.661966 authentik_client-2024.4.2.post1717033274/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-05-30 01:41:27.349960 authentik_client-2024.4.2.post1717033274/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-05-30 01:41:27.373961 authentik_client-2024.4.2.post1717033274/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701822 2024-05-30 01:41:27.397961 authentik_client-2024.4.2.post1717033274/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-05-30 01:41:27.413962 authentik_client-2024.4.2.post1717033274/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-05-30 01:41:27.421962 authentik_client-2024.4.2.post1717033274/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-05-30 01:41:27.433962 authentik_client-2024.4.2.post1717033274/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-05-30 01:41:27.449962 authentik_client-2024.4.2.post1717033274/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-05-30 01:41:27.457962 authentik_client-2024.4.2.post1717033274/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-05-30 01:41:27.465963 authentik_client-2024.4.2.post1717033274/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413244 2024-05-30 01:41:27.473963 authentik_client-2024.4.2.post1717033274/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725180 2024-05-30 01:41:27.493963 authentik_client-2024.4.2.post1717033274/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   721894 2024-05-30 01:41:27.509963 authentik_client-2024.4.2.post1717033274/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0  1136128 2024-05-30 01:41:27.529964 authentik_client-2024.4.2.post1717033274/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-05-30 01:41:27.553964 authentik_client-2024.4.2.post1717033274/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-05-30 01:41:27.565964 authentik_client-2024.4.2.post1717033274/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-05-30 01:41:27.569965 authentik_client-2024.4.2.post1717033274/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-05-30 01:41:27.573964 authentik_client-2024.4.2.post1717033274/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037175 2024-05-30 01:41:27.593965 authentik_client-2024.4.2.post1717033274/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945968 2024-05-30 01:41:27.625965 authentik_client-2024.4.2.post1717033274/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-05-30 01:41:27.641966 authentik_client-2024.4.2.post1717033274/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-05-30 01:41:27.665966 authentik_client-2024.4.2.post1717033274/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-30 01:41:27.665966 authentik_client-2024.4.2.post1717033274/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-05-30 01:41:27.657966 authentik_client-2024.4.2.post1717033274/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-05-30 01:41:27.661966 authentik_client-2024.4.2.post1717033274/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    50026 2024-05-30 01:41:27.661966 authentik_client-2024.4.2.post1717033274/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-05-30 01:41:24.521909 authentik_client-2024.4.2.post1717033274/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0      688 2024-05-30 01:41:24.533909 authentik_client-2024.4.2.post1717033274/authentik_client/models/alg_enum.py
+-rw-r--r--   0        0        0     2482 2024-05-30 01:41:24.541909 authentik_client-2024.4.2.post1717033274/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4460 2024-05-30 01:41:24.549909 authentik_client-2024.4.2.post1717033274/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-05-30 01:41:24.557910 authentik_client-2024.4.2.post1717033274/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-05-30 01:41:24.569910 authentik_client-2024.4.2.post1717033274/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-05-30 01:41:24.585910 authentik_client-2024.4.2.post1717033274/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-05-30 01:41:24.593910 authentik_client-2024.4.2.post1717033274/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-05-30 01:41:24.597910 authentik_client-2024.4.2.post1717033274/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-05-30 01:41:24.605910 authentik_client-2024.4.2.post1717033274/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-05-30 01:41:24.609911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-05-30 01:41:24.617911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-05-30 01:41:24.625911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-05-30 01:41:24.633911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-05-30 01:41:24.637911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-05-30 01:41:24.645911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-05-30 01:41:24.653911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-05-30 01:41:24.657911 authentik_client-2024.4.2.post1717033274/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-05-30 01:41:24.661912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-05-30 01:41:24.669912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-05-30 01:41:24.677912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-05-30 01:41:24.685912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-05-30 01:41:24.693912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-05-30 01:41:24.697912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-05-30 01:41:24.705912 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-30 01:41:24.713913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-05-30 01:41:24.721913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-05-30 01:41:24.729913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-05-30 01:41:24.737913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-05-30 01:41:24.741913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-05-30 01:41:24.749913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-05-30 01:41:24.753913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-05-30 01:41:24.761913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-05-30 01:41:24.765913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-05-30 01:41:24.769914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-05-30 01:41:24.773913 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-05-30 01:41:24.785914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-05-30 01:41:24.789914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-05-30 01:41:24.797914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-05-30 01:41:24.801914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-05-30 01:41:24.805914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-05-30 01:41:24.813914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-05-30 01:41:24.817914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-05-30 01:41:24.821915 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-05-30 01:41:24.825914 authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-05-30 01:41:24.829915 authentik_client-2024.4.2.post1717033274/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-05-30 01:41:24.833915 authentik_client-2024.4.2.post1717033274/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-05-30 01:41:24.837915 authentik_client-2024.4.2.post1717033274/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-05-30 01:41:24.841915 authentik_client-2024.4.2.post1717033274/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-05-30 01:41:24.845915 authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-05-30 01:41:24.849915 authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-05-30 01:41:24.853915 authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-05-30 01:41:24.857915 authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-05-30 01:41:24.861915 authentik_client-2024.4.2.post1717033274/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-05-30 01:41:24.865915 authentik_client-2024.4.2.post1717033274/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-05-30 01:41:24.869915 authentik_client-2024.4.2.post1717033274/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-05-30 01:41:24.873915 authentik_client-2024.4.2.post1717033274/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-05-30 01:41:24.877915 authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-05-30 01:41:24.881915 authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-05-30 01:41:24.885916 authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-05-30 01:41:24.889916 authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-05-30 01:41:24.893916 authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2990 2024-05-30 01:41:24.897916 authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-05-30 01:41:24.901916 authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-05-30 01:41:24.905916 authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-05-30 01:41:24.909916 authentik_client-2024.4.2.post1717033274/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-05-30 01:41:24.917916 authentik_client-2024.4.2.post1717033274/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-05-30 01:41:24.921916 authentik_client-2024.4.2.post1717033274/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-05-30 01:41:24.925916 authentik_client-2024.4.2.post1717033274/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-05-30 01:41:24.929916 authentik_client-2024.4.2.post1717033274/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-05-30 01:41:24.933916 authentik_client-2024.4.2.post1717033274/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-05-30 01:41:24.941917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-05-30 01:41:24.945917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-05-30 01:41:24.949917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-05-30 01:41:24.957917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-05-30 01:41:24.957917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-05-30 01:41:24.961917 authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-05-30 01:41:24.965917 authentik_client-2024.4.2.post1717033274/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-05-30 01:41:24.969917 authentik_client-2024.4.2.post1717033274/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-05-30 01:41:24.973917 authentik_client-2024.4.2.post1717033274/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-05-30 01:41:24.977917 authentik_client-2024.4.2.post1717033274/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-05-30 01:41:24.981917 authentik_client-2024.4.2.post1717033274/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-05-30 01:41:24.985917 authentik_client-2024.4.2.post1717033274/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-05-30 01:41:24.993918 authentik_client-2024.4.2.post1717033274/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-05-30 01:41:24.993918 authentik_client-2024.4.2.post1717033274/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-05-30 01:41:25.001918 authentik_client-2024.4.2.post1717033274/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-05-30 01:41:25.005918 authentik_client-2024.4.2.post1717033274/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-05-30 01:41:25.009918 authentik_client-2024.4.2.post1717033274/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-05-30 01:41:25.009918 authentik_client-2024.4.2.post1717033274/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-05-30 01:41:25.013918 authentik_client-2024.4.2.post1717033274/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-05-30 01:41:25.017918 authentik_client-2024.4.2.post1717033274/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-05-30 01:41:25.021918 authentik_client-2024.4.2.post1717033274/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-05-30 01:41:25.025918 authentik_client-2024.4.2.post1717033274/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-05-30 01:41:25.029918 authentik_client-2024.4.2.post1717033274/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-05-30 01:41:25.037918 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-05-30 01:41:25.041918 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-05-30 01:41:25.045919 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-05-30 01:41:25.049919 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-05-30 01:41:25.053919 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-05-30 01:41:25.065919 authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-05-30 01:41:25.069919 authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-05-30 01:41:25.077919 authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-05-30 01:41:25.085919 authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-05-30 01:41:25.089919 authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-05-30 01:41:25.097920 authentik_client-2024.4.2.post1717033274/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-05-30 01:41:25.101920 authentik_client-2024.4.2.post1717033274/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-05-30 01:41:25.109920 authentik_client-2024.4.2.post1717033274/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-05-30 01:41:25.117920 authentik_client-2024.4.2.post1717033274/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-05-30 01:41:25.125920 authentik_client-2024.4.2.post1717033274/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-05-30 01:41:25.133920 authentik_client-2024.4.2.post1717033274/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-05-30 01:41:25.137920 authentik_client-2024.4.2.post1717033274/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-05-30 01:41:25.145920 authentik_client-2024.4.2.post1717033274/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-05-30 01:41:25.149920 authentik_client-2024.4.2.post1717033274/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-05-30 01:41:25.153921 authentik_client-2024.4.2.post1717033274/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-05-30 01:41:25.161921 authentik_client-2024.4.2.post1717033274/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-05-30 01:41:25.165921 authentik_client-2024.4.2.post1717033274/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-05-30 01:41:25.173921 authentik_client-2024.4.2.post1717033274/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-05-30 01:41:25.177921 authentik_client-2024.4.2.post1717033274/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-05-30 01:41:25.185921 authentik_client-2024.4.2.post1717033274/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-05-30 01:41:25.193921 authentik_client-2024.4.2.post1717033274/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-05-30 01:41:25.197921 authentik_client-2024.4.2.post1717033274/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-05-30 01:41:25.205922 authentik_client-2024.4.2.post1717033274/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-05-30 01:41:25.209921 authentik_client-2024.4.2.post1717033274/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-05-30 01:41:25.217922 authentik_client-2024.4.2.post1717033274/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-05-30 01:41:25.225922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-05-30 01:41:25.233922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-05-30 01:41:25.233922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-05-30 01:41:25.241922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-05-30 01:41:25.249922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-05-30 01:41:25.253922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-05-30 01:41:25.261922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-05-30 01:41:25.265922 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-05-30 01:41:25.269923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-05-30 01:41:25.273923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-05-30 01:41:25.277923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-05-30 01:41:25.281923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-05-30 01:41:25.285923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-05-30 01:41:25.289923 authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-05-30 01:41:25.293923 authentik_client-2024.4.2.post1717033274/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-05-30 01:41:25.297923 authentik_client-2024.4.2.post1717033274/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-05-30 01:41:25.297923 authentik_client-2024.4.2.post1717033274/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     6418 2024-05-30 01:41:25.301923 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider.py
+-rw-r--r--   0        0        0     3577 2024-05-30 01:41:25.305923 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_group.py
+-rw-r--r--   0        0        0     2618 2024-05-30 01:41:25.309923 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_group_request.py
+-rw-r--r--   0        0        0     4324 2024-05-30 01:41:25.313923 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_mapping.py
+-rw-r--r--   0        0        0     3385 2024-05-30 01:41:25.317923 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_mapping_request.py
+-rw-r--r--   0        0        0     4740 2024-05-30 01:41:25.321924 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_request.py
+-rw-r--r--   0        0        0     3567 2024-05-30 01:41:25.325924 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_user.py
+-rw-r--r--   0        0        0     2599 2024-05-30 01:41:25.329924 authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_user_request.py
+-rw-r--r--   0        0        0     5445 2024-05-30 01:41:25.333924 authentik_client-2024.4.2.post1717033274/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-05-30 01:41:25.337924 authentik_client-2024.4.2.post1717033274/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-05-30 01:41:25.341924 authentik_client-2024.4.2.post1717033274/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-05-30 01:41:25.345924 authentik_client-2024.4.2.post1717033274/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-05-30 01:41:25.349924 authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-05-30 01:41:25.353924 authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-05-30 01:41:25.357924 authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-05-30 01:41:25.361924 authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-05-30 01:41:25.365924 authentik_client-2024.4.2.post1717033274/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-05-30 01:41:25.369924 authentik_client-2024.4.2.post1717033274/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-05-30 01:41:25.369924 authentik_client-2024.4.2.post1717033274/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-05-30 01:41:25.373925 authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-05-30 01:41:25.377925 authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-05-30 01:41:25.381925 authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-05-30 01:41:25.385925 authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-05-30 01:41:25.389925 authentik_client-2024.4.2.post1717033274/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-05-30 01:41:25.393925 authentik_client-2024.4.2.post1717033274/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-05-30 01:41:25.397925 authentik_client-2024.4.2.post1717033274/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-05-30 01:41:25.401925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-05-30 01:41:25.405925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-05-30 01:41:25.409925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-05-30 01:41:25.417925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-05-30 01:41:25.421925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-05-30 01:41:25.425925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11470 2024-05-30 01:41:25.429926 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-05-30 01:41:25.429926 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0      726 2024-05-30 01:41:25.397925 authentik_client-2024.4.2.post1717033274/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-05-30 01:41:25.433925 authentik_client-2024.4.2.post1717033274/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-05-30 01:41:25.437926 authentik_client-2024.4.2.post1717033274/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-05-30 01:41:25.437926 authentik_client-2024.4.2.post1717033274/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-05-30 01:41:25.441926 authentik_client-2024.4.2.post1717033274/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-05-30 01:41:25.445926 authentik_client-2024.4.2.post1717033274/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-05-30 01:41:25.449926 authentik_client-2024.4.2.post1717033274/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-05-30 01:41:25.449926 authentik_client-2024.4.2.post1717033274/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-05-30 01:41:25.453926 authentik_client-2024.4.2.post1717033274/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-05-30 01:41:25.453926 authentik_client-2024.4.2.post1717033274/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-05-30 01:41:25.457926 authentik_client-2024.4.2.post1717033274/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-05-30 01:41:25.461926 authentik_client-2024.4.2.post1717033274/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     5920 2024-05-30 01:41:25.465926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider.py
+-rw-r--r--   0        0        0     3573 2024-05-30 01:41:25.465926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_group.py
+-rw-r--r--   0        0        0     2614 2024-05-30 01:41:25.469926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_group_request.py
+-rw-r--r--   0        0        0     4320 2024-05-30 01:41:25.473926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_mapping.py
+-rw-r--r--   0        0        0     3381 2024-05-30 01:41:25.477926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_mapping_request.py
+-rw-r--r--   0        0        0     4307 2024-05-30 01:41:25.477926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_request.py
+-rw-r--r--   0        0        0     3563 2024-05-30 01:41:25.481927 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_user.py
+-rw-r--r--   0        0        0     2595 2024-05-30 01:41:25.485926 authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_user_request.py
+-rw-r--r--   0        0        0     8160 2024-05-30 01:41:25.485926 authentik_client-2024.4.2.post1717033274/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0    11885 2024-05-30 01:41:25.489927 authentik_client-2024.4.2.post1717033274/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-05-30 01:41:25.489927 authentik_client-2024.4.2.post1717033274/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-05-30 01:41:25.493927 authentik_client-2024.4.2.post1717033274/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-05-30 01:41:25.493927 authentik_client-2024.4.2.post1717033274/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-05-30 01:41:25.497927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-05-30 01:41:25.497927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-05-30 01:41:25.501927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-05-30 01:41:25.505927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-05-30 01:41:25.509927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-05-30 01:41:25.509927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-05-30 01:41:25.513927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-05-30 01:41:25.517927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-05-30 01:41:25.517927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-05-30 01:41:25.521927 authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-05-30 01:41:25.525927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-05-30 01:41:25.525927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-05-30 01:41:25.529927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-05-30 01:41:25.533927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-05-30 01:41:25.537927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-05-30 01:41:25.541927 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-05-30 01:41:25.545928 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10451 2024-05-30 01:41:25.549928 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-05-30 01:41:25.553928 authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-05-30 01:41:25.553928 authentik_client-2024.4.2.post1717033274/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0      779 2024-05-30 01:41:25.557928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outgoing_sync_delete_action.py
+-rw-r--r--   0        0        0     5545 2024-05-30 01:41:25.557928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-05-30 01:41:25.561928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     4497 2024-05-30 01:41:25.565928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-05-30 01:41:25.569928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-05-30 01:41:25.569928 authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-05-30 01:41:25.573928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-05-30 01:41:25.573928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-05-30 01:41:25.577928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-05-30 01:41:25.581928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-05-30 01:41:25.581928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-05-30 01:41:25.585928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-05-30 01:41:25.589928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-05-30 01:41:25.589928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-05-30 01:41:25.593928 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-05-30 01:41:25.597929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.601929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-05-30 01:41:25.601929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-05-30 01:41:25.605929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.609929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-30 01:41:25.613929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-05-30 01:41:25.617929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-05-30 01:41:25.621929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.625929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.625929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-30 01:41:25.629929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.633929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-05-30 01:41:25.637929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-05-30 01:41:25.637929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-05-30 01:41:25.641929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-05-30 01:41:25.645929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-05-30 01:41:25.645929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-05-30 01:41:25.649929 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-05-30 01:41:25.653930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-30 01:41:25.653930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-05-30 01:41:25.657930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3461 2024-05-30 01:41:25.665930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_group_list.py
+-rw-r--r--   0        0        0     3420 2024-05-30 01:41:25.669930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_list.py
+-rw-r--r--   0        0        0     3477 2024-05-30 01:41:25.673930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_mapping_list.py
+-rw-r--r--   0        0        0     3453 2024-05-30 01:41:25.677930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_user_list.py
+-rw-r--r--   0        0        0     3274 2024-05-30 01:41:25.681930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-05-30 01:41:25.681930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-30 01:41:25.685930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-05-30 01:41:25.689930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-05-30 01:41:25.689930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-05-30 01:41:25.693930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-05-30 01:41:25.697930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.697930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.701930 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-30 01:41:25.705931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3453 2024-05-30 01:41:25.705931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_group_list.py
+-rw-r--r--   0        0        0     3412 2024-05-30 01:41:25.709931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_list.py
+-rw-r--r--   0        0        0     3469 2024-05-30 01:41:25.713931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py
+-rw-r--r--   0        0        0     3445 2024-05-30 01:41:25.717931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_user_list.py
+-rw-r--r--   0        0        0     3330 2024-05-30 01:41:25.717931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-05-30 01:41:25.721931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-05-30 01:41:25.725931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-05-30 01:41:25.725931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-05-30 01:41:25.729931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-05-30 01:41:25.733931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-30 01:41:25.733931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-05-30 01:41:25.737931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-05-30 01:41:25.741931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-05-30 01:41:25.745931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-30 01:41:25.749931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-05-30 01:41:25.753931 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.757932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-05-30 01:41:25.761932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-05-30 01:41:25.761932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-05-30 01:41:25.765932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.769932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-05-30 01:41:25.773932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-05-30 01:41:25.777932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-30 01:41:25.777932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-05-30 01:41:25.781932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-30 01:41:25.785932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.789932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-05-30 01:41:25.789932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-05-30 01:41:25.793932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-05-30 01:41:25.797932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-05-30 01:41:25.797932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-05-30 01:41:25.801932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-30 01:41:25.801932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-05-30 01:41:25.805932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.805932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.809932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.813933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.813933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-05-30 01:41:25.817932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.817932 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-05-30 01:41:25.821933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.825933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-05-30 01:41:25.829933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-05-30 01:41:25.821933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-05-30 01:41:25.829933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.833933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-05-30 01:41:25.833933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-05-30 01:41:25.837933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.841933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-05-30 01:41:25.845933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-05-30 01:41:25.849933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.849933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:41:25.841933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-05-30 01:41:25.853933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-05-30 01:41:25.853933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-05-30 01:41:25.857933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-05-30 01:41:25.857933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-05-30 01:41:25.861933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-05-30 01:41:25.861933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-05-30 01:41:25.865934 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-05-30 01:41:25.869933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-05-30 01:41:25.869933 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-05-30 01:41:25.873934 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-05-30 01:41:25.873934 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-05-30 01:41:25.877934 authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-05-30 01:41:25.877934 authentik_client-2024.4.2.post1717033274/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-05-30 01:41:25.881934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-05-30 01:41:25.885934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-05-30 01:41:25.885934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-05-30 01:41:25.889934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-05-30 01:41:25.893934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-05-30 01:41:25.893934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-05-30 01:41:25.897934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-05-30 01:41:25.901934 authentik_client-2024.4.2.post1717033274/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-30 01:41:25.905934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-05-30 01:41:25.909934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-05-30 01:41:25.913934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-05-30 01:41:25.913934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-05-30 01:41:25.917934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-05-30 01:41:25.921934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-05-30 01:41:25.921934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-05-30 01:41:25.925934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-05-30 01:41:25.925934 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-05-30 01:41:25.929935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-05-30 01:41:25.929935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-05-30 01:41:25.933935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-05-30 01:41:25.933935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-05-30 01:41:25.937935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-05-30 01:41:25.937935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-05-30 01:41:25.941935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-05-30 01:41:25.941935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-05-30 01:41:25.945935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-05-30 01:41:25.949935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-05-30 01:41:25.949935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-05-30 01:41:25.953935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-05-30 01:41:25.957935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-05-30 01:41:25.957935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-05-30 01:41:25.961935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-05-30 01:41:25.965935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-05-30 01:41:25.965935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3440 2024-05-30 01:41:25.969935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_google_workspace_provider_mapping_request.py
+-rw-r--r--   0        0        0     4819 2024-05-30 01:41:25.969935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_google_workspace_provider_request.py
+-rw-r--r--   0        0        0     3385 2024-05-30 01:41:25.973935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-05-30 01:41:25.977935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-05-30 01:41:25.977935 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-05-30 01:41:25.981936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-05-30 01:41:25.981936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-05-30 01:41:25.985936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-05-30 01:41:25.985936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-05-30 01:41:25.989936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-05-30 01:41:25.989936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     3436 2024-05-30 01:41:25.993936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py
+-rw-r--r--   0        0        0     4396 2024-05-30 01:41:25.993936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_microsoft_entra_provider_request.py
+-rw-r--r--   0        0        0     2879 2024-05-30 01:41:25.997936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-05-30 01:41:25.997936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-05-30 01:41:26.001936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-05-30 01:41:26.005936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-05-30 01:41:26.005936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-05-30 01:41:26.009936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-05-30 01:41:26.009936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-05-30 01:41:26.013936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-05-30 01:41:26.017936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-05-30 01:41:26.017936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-05-30 01:41:26.021936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-05-30 01:41:26.021936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-05-30 01:41:26.025936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-05-30 01:41:26.025936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-05-30 01:41:26.029936 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-05-30 01:41:26.033937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-05-30 01:41:26.033937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-05-30 01:41:26.037937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-05-30 01:41:26.037937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-05-30 01:41:26.041937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-05-30 01:41:26.041937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-05-30 01:41:26.045937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-05-30 01:41:26.049937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-05-30 01:41:26.049937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-05-30 01:41:26.053937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-05-30 01:41:26.057937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-05-30 01:41:26.061937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-05-30 01:41:26.065937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-05-30 01:41:26.065937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-05-30 01:41:26.069937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-05-30 01:41:26.077937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-05-30 01:41:26.077937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-05-30 01:41:26.073937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-05-30 01:41:26.081937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-05-30 01:41:26.085937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-05-30 01:41:26.089938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-05-30 01:41:26.089938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-05-30 01:41:26.085937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-05-30 01:41:26.093937 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-05-30 01:41:26.097938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-05-30 01:41:26.097938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-05-30 01:41:26.101938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-05-30 01:41:26.101938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-05-30 01:41:26.105938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-05-30 01:41:26.105938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-05-30 01:41:26.105938 authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-05-30 01:41:26.109938 authentik_client-2024.4.2.post1717033274/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-05-30 01:41:26.109938 authentik_client-2024.4.2.post1717033274/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-05-30 01:41:26.113938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-05-30 01:41:26.117938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7431 2024-05-30 01:41:26.121938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-05-30 01:41:26.125938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-05-30 01:41:26.125938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-05-30 01:41:26.129938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-05-30 01:41:26.133938 authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-05-30 01:41:26.133938 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-05-30 01:41:26.137938 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-05-30 01:41:26.141939 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-05-30 01:41:26.141939 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-05-30 01:41:26.141939 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-05-30 01:41:26.145938 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-05-30 01:41:26.149939 authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-05-30 01:41:26.149939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-05-30 01:41:26.153939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-05-30 01:41:26.157939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-05-30 01:41:26.157939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-05-30 01:41:26.161939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-05-30 01:41:26.161939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-05-30 01:41:26.165939 authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-05-30 01:41:26.165939 authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-05-30 01:41:26.169939 authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2740 2024-05-30 01:41:26.169939 authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_test_request.py
+-rw-r--r--   0        0        0     2744 2024-05-30 01:41:26.173939 authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-05-30 01:41:26.173939 authentik_client-2024.4.2.post1717033274/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-05-30 01:41:26.177939 authentik_client-2024.4.2.post1717033274/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-05-30 01:41:26.177939 authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1578 2024-05-30 01:41:26.181939 authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-05-30 01:41:26.181939 authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-05-30 01:41:26.181939 authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-05-30 01:41:26.185939 authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-05-30 01:41:26.185939 authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-05-30 01:41:26.189939 authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-05-30 01:41:26.193939 authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-05-30 01:41:26.193939 authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-05-30 01:41:26.197939 authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-05-30 01:41:26.201939 authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-05-30 01:41:26.201939 authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-05-30 01:41:26.205940 authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-05-30 01:41:26.209940 authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-05-30 01:41:26.209940 authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-05-30 01:41:26.213940 authentik_client-2024.4.2.post1717033274/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-05-30 01:41:26.217940 authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-05-30 01:41:26.217940 authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-05-30 01:41:26.221940 authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-05-30 01:41:26.221940 authentik_client-2024.4.2.post1717033274/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-05-30 01:41:26.225940 authentik_client-2024.4.2.post1717033274/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-05-30 01:41:26.229940 authentik_client-2024.4.2.post1717033274/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-05-30 01:41:26.233940 authentik_client-2024.4.2.post1717033274/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-05-30 01:41:26.237940 authentik_client-2024.4.2.post1717033274/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-05-30 01:41:26.241940 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-05-30 01:41:26.245940 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-05-30 01:41:26.245940 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-05-30 01:41:26.249940 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-05-30 01:41:26.253940 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10242 2024-05-30 01:41:26.257941 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-05-30 01:41:26.261941 authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-05-30 01:41:26.265941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-05-30 01:41:26.265941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-05-30 01:41:26.269941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-05-30 01:41:26.269941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-05-30 01:41:26.273941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-05-30 01:41:26.277941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-05-30 01:41:26.277941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-05-30 01:41:26.281941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-05-30 01:41:26.281941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-05-30 01:41:26.285941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     4629 2024-05-30 01:41:26.289941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-05-30 01:41:26.293941 authentik_client-2024.4.2.post1717033274/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-05-30 01:41:26.293941 authentik_client-2024.4.2.post1717033274/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-05-30 01:41:26.297941 authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-05-30 01:41:26.297941 authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-05-30 01:41:26.301941 authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-05-30 01:41:26.301941 authentik_client-2024.4.2.post1717033274/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-05-30 01:41:26.305941 authentik_client-2024.4.2.post1717033274/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-05-30 01:41:26.305941 authentik_client-2024.4.2.post1717033274/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-05-30 01:41:26.309941 authentik_client-2024.4.2.post1717033274/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-05-30 01:41:26.309941 authentik_client-2024.4.2.post1717033274/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     2172 2024-05-30 01:41:26.313942 authentik_client-2024.4.2.post1717033274/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-05-30 01:41:26.285941 authentik_client-2024.4.2.post1717033274/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-05-30 01:41:26.289941 authentik_client-2024.4.2.post1717033274/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-05-30 01:41:26.313942 authentik_client-2024.4.2.post1717033274/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-05-30 01:41:26.317942 authentik_client-2024.4.2.post1717033274/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-05-30 01:41:26.317942 authentik_client-2024.4.2.post1717033274/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-05-30 01:41:26.321942 authentik_client-2024.4.2.post1717033274/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-05-30 01:41:26.321942 authentik_client-2024.4.2.post1717033274/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-05-30 01:41:26.325942 authentik_client-2024.4.2.post1717033274/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-05-30 01:41:26.325942 authentik_client-2024.4.2.post1717033274/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-05-30 01:41:26.329942 authentik_client-2024.4.2.post1717033274/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-05-30 01:41:26.329942 authentik_client-2024.4.2.post1717033274/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-05-30 01:41:26.333942 authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-05-30 01:41:26.333942 authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-05-30 01:41:26.337942 authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-05-30 01:41:26.337942 authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-05-30 01:41:26.341942 authentik_client-2024.4.2.post1717033274/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     3114 2024-05-30 01:41:26.341942 authentik_client-2024.4.2.post1717033274/authentik_client/models/sync_status.py
+-rw-r--r--   0        0        0     4463 2024-05-30 01:41:26.345942 authentik_client-2024.4.2.post1717033274/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     3177 2024-05-30 01:41:26.345942 authentik_client-2024.4.2.post1717033274/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4701 2024-05-30 01:41:26.349942 authentik_client-2024.4.2.post1717033274/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-05-30 01:41:26.349942 authentik_client-2024.4.2.post1717033274/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-05-30 01:41:26.357942 authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-05-30 01:41:26.361942 authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-05-30 01:41:26.361942 authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-05-30 01:41:26.365943 authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-05-30 01:41:26.365943 authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-05-30 01:41:26.369943 authentik_client-2024.4.2.post1717033274/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-05-30 01:41:26.373943 authentik_client-2024.4.2.post1717033274/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-05-30 01:41:26.377943 authentik_client-2024.4.2.post1717033274/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-05-30 01:41:26.377943 authentik_client-2024.4.2.post1717033274/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-05-30 01:41:26.381943 authentik_client-2024.4.2.post1717033274/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-05-30 01:41:26.353942 authentik_client-2024.4.2.post1717033274/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-05-30 01:41:26.353942 authentik_client-2024.4.2.post1717033274/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-05-30 01:41:26.381943 authentik_client-2024.4.2.post1717033274/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-05-30 01:41:26.385943 authentik_client-2024.4.2.post1717033274/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     3034 2024-05-30 01:41:26.389943 authentik_client-2024.4.2.post1717033274/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-05-30 01:41:26.389943 authentik_client-2024.4.2.post1717033274/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-05-30 01:41:26.393943 authentik_client-2024.4.2.post1717033274/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-05-30 01:41:26.393943 authentik_client-2024.4.2.post1717033274/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-05-30 01:41:26.397943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-05-30 01:41:26.401943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-05-30 01:41:26.405943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-05-30 01:41:26.405943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-05-30 01:41:26.405943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-05-30 01:41:26.409943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-30 01:41:26.413943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-05-30 01:41:26.413943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-05-30 01:41:26.413943 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-05-30 01:41:26.417944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-05-30 01:41:26.421944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-05-30 01:41:26.421944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-05-30 01:41:26.425944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-05-30 01:41:26.429944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-05-30 01:41:26.429944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-30 01:41:26.433944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-05-30 01:41:26.433944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-05-30 01:41:26.437944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-05-30 01:41:26.437944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-05-30 01:41:26.441944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-05-30 01:41:26.441944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-05-30 01:41:26.441944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-05-30 01:41:26.445944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-05-30 01:41:26.445944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-05-30 01:41:26.449944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-05-30 01:41:26.449944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-05-30 01:41:26.453944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-05-30 01:41:26.453944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-05-30 01:41:26.457944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-05-30 01:41:26.457944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-05-30 01:41:26.457944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-05-30 01:41:26.461944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-05-30 01:41:26.461944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-05-30 01:41:26.461944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-05-30 01:41:26.465944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-05-30 01:41:26.465944 authentik_client-2024.4.2.post1717033274/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-05-30 01:41:26.469944 authentik_client-2024.4.2.post1717033274/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-05-30 01:41:26.469944 authentik_client-2024.4.2.post1717033274/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3786 2024-05-30 01:41:26.473945 authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-05-30 01:41:26.473945 authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-05-30 01:41:26.473945 authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-05-30 01:41:26.477944 authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-05-30 01:41:26.477944 authentik_client-2024.4.2.post1717033274/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-05-30 01:41:27.657966 authentik_client-2024.4.2.post1717033274/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-05-30 01:41:27.665966 authentik_client-2024.4.2.post1717033274/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-05-30 01:41:27.657966 authentik_client-2024.4.2.post1717033274/pyproject.toml
+-rw-r--r--   0        0        0   156878 1970-01-01 00:00:00.000000 authentik_client-2024.4.2.post1717033274/PKG-INFO
```

### Comparing `authentik_client-2024.4.2.post1716550398/README.md` & `authentik_client-2024.4.2.post1717033274/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.4.2
-- Package version: 2024.4.2-1716550398
+- Package version: 2024.4.2-1717033274
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -491,59 +491,51 @@
 *ProvidersApi* | [**providers_all_types_list**](docs/ProvidersApi.md#providers_all_types_list) | **GET** /providers/all/types/ | 
 *ProvidersApi* | [**providers_all_used_by_list**](docs/ProvidersApi.md#providers_all_used_by_list) | **GET** /providers/all/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_create**](docs/ProvidersApi.md#providers_google_workspace_create) | **POST** /providers/google_workspace/ | 
 *ProvidersApi* | [**providers_google_workspace_destroy**](docs/ProvidersApi.md#providers_google_workspace_destroy) | **DELETE** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_create**](docs/ProvidersApi.md#providers_google_workspace_groups_create) | **POST** /providers/google_workspace_groups/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_destroy**](docs/ProvidersApi.md#providers_google_workspace_groups_destroy) | **DELETE** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_list**](docs/ProvidersApi.md#providers_google_workspace_groups_list) | **GET** /providers/google_workspace_groups/ | 
-*ProvidersApi* | [**providers_google_workspace_groups_partial_update**](docs/ProvidersApi.md#providers_google_workspace_groups_partial_update) | **PATCH** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_retrieve**](docs/ProvidersApi.md#providers_google_workspace_groups_retrieve) | **GET** /providers/google_workspace_groups/{id}/ | 
-*ProvidersApi* | [**providers_google_workspace_groups_update**](docs/ProvidersApi.md#providers_google_workspace_groups_update) | **PUT** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_groups_used_by_list) | **GET** /providers/google_workspace_groups/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_list**](docs/ProvidersApi.md#providers_google_workspace_list) | **GET** /providers/google_workspace/ | 
 *ProvidersApi* | [**providers_google_workspace_partial_update**](docs/ProvidersApi.md#providers_google_workspace_partial_update) | **PATCH** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_retrieve**](docs/ProvidersApi.md#providers_google_workspace_retrieve) | **GET** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_sync_status_retrieve**](docs/ProvidersApi.md#providers_google_workspace_sync_status_retrieve) | **GET** /providers/google_workspace/{id}/sync/status/ | 
 *ProvidersApi* | [**providers_google_workspace_update**](docs/ProvidersApi.md#providers_google_workspace_update) | **PUT** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_used_by_list) | **GET** /providers/google_workspace/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_users_create**](docs/ProvidersApi.md#providers_google_workspace_users_create) | **POST** /providers/google_workspace_users/ | 
 *ProvidersApi* | [**providers_google_workspace_users_destroy**](docs/ProvidersApi.md#providers_google_workspace_users_destroy) | **DELETE** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_list**](docs/ProvidersApi.md#providers_google_workspace_users_list) | **GET** /providers/google_workspace_users/ | 
-*ProvidersApi* | [**providers_google_workspace_users_partial_update**](docs/ProvidersApi.md#providers_google_workspace_users_partial_update) | **PATCH** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_retrieve**](docs/ProvidersApi.md#providers_google_workspace_users_retrieve) | **GET** /providers/google_workspace_users/{id}/ | 
-*ProvidersApi* | [**providers_google_workspace_users_update**](docs/ProvidersApi.md#providers_google_workspace_users_update) | **PUT** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_users_used_by_list) | **GET** /providers/google_workspace_users/{id}/used_by/ | 
 *ProvidersApi* | [**providers_ldap_create**](docs/ProvidersApi.md#providers_ldap_create) | **POST** /providers/ldap/ | 
 *ProvidersApi* | [**providers_ldap_destroy**](docs/ProvidersApi.md#providers_ldap_destroy) | **DELETE** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_list**](docs/ProvidersApi.md#providers_ldap_list) | **GET** /providers/ldap/ | 
 *ProvidersApi* | [**providers_ldap_partial_update**](docs/ProvidersApi.md#providers_ldap_partial_update) | **PATCH** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_retrieve**](docs/ProvidersApi.md#providers_ldap_retrieve) | **GET** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_update**](docs/ProvidersApi.md#providers_ldap_update) | **PUT** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_used_by_list**](docs/ProvidersApi.md#providers_ldap_used_by_list) | **GET** /providers/ldap/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_create**](docs/ProvidersApi.md#providers_microsoft_entra_create) | **POST** /providers/microsoft_entra/ | 
 *ProvidersApi* | [**providers_microsoft_entra_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_destroy) | **DELETE** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_create**](docs/ProvidersApi.md#providers_microsoft_entra_groups_create) | **POST** /providers/microsoft_entra_groups/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_groups_destroy) | **DELETE** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_list**](docs/ProvidersApi.md#providers_microsoft_entra_groups_list) | **GET** /providers/microsoft_entra_groups/ | 
-*ProvidersApi* | [**providers_microsoft_entra_groups_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_groups_partial_update) | **PATCH** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_groups_retrieve) | **GET** /providers/microsoft_entra_groups/{id}/ | 
-*ProvidersApi* | [**providers_microsoft_entra_groups_update**](docs/ProvidersApi.md#providers_microsoft_entra_groups_update) | **PUT** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_groups_used_by_list) | **GET** /providers/microsoft_entra_groups/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_list**](docs/ProvidersApi.md#providers_microsoft_entra_list) | **GET** /providers/microsoft_entra/ | 
 *ProvidersApi* | [**providers_microsoft_entra_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_partial_update) | **PATCH** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_retrieve) | **GET** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_sync_status_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_sync_status_retrieve) | **GET** /providers/microsoft_entra/{id}/sync/status/ | 
 *ProvidersApi* | [**providers_microsoft_entra_update**](docs/ProvidersApi.md#providers_microsoft_entra_update) | **PUT** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_used_by_list) | **GET** /providers/microsoft_entra/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_create**](docs/ProvidersApi.md#providers_microsoft_entra_users_create) | **POST** /providers/microsoft_entra_users/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_users_destroy) | **DELETE** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_list**](docs/ProvidersApi.md#providers_microsoft_entra_users_list) | **GET** /providers/microsoft_entra_users/ | 
-*ProvidersApi* | [**providers_microsoft_entra_users_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_users_partial_update) | **PATCH** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_users_retrieve) | **GET** /providers/microsoft_entra_users/{id}/ | 
-*ProvidersApi* | [**providers_microsoft_entra_users_update**](docs/ProvidersApi.md#providers_microsoft_entra_users_update) | **PUT** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_users_used_by_list) | **GET** /providers/microsoft_entra_users/{id}/used_by/ | 
 *ProvidersApi* | [**providers_oauth2_create**](docs/ProvidersApi.md#providers_oauth2_create) | **POST** /providers/oauth2/ | 
 *ProvidersApi* | [**providers_oauth2_destroy**](docs/ProvidersApi.md#providers_oauth2_destroy) | **DELETE** /providers/oauth2/{id}/ | 
 *ProvidersApi* | [**providers_oauth2_list**](docs/ProvidersApi.md#providers_oauth2_list) | **GET** /providers/oauth2/ | 
 *ProvidersApi* | [**providers_oauth2_partial_update**](docs/ProvidersApi.md#providers_oauth2_partial_update) | **PATCH** /providers/oauth2/{id}/ | 
 *ProvidersApi* | [**providers_oauth2_preview_user_retrieve**](docs/ProvidersApi.md#providers_oauth2_preview_user_retrieve) | **GET** /providers/oauth2/{id}/preview_user/ | 
 *ProvidersApi* | [**providers_oauth2_retrieve**](docs/ProvidersApi.md#providers_oauth2_retrieve) | **GET** /providers/oauth2/{id}/ | 
@@ -1262,31 +1254,27 @@
  - [PatchedEmailStageRequest](docs/PatchedEmailStageRequest.md)
  - [PatchedEndpointRequest](docs/PatchedEndpointRequest.md)
  - [PatchedEventMatcherPolicyRequest](docs/PatchedEventMatcherPolicyRequest.md)
  - [PatchedEventRequest](docs/PatchedEventRequest.md)
  - [PatchedExpressionPolicyRequest](docs/PatchedExpressionPolicyRequest.md)
  - [PatchedFlowRequest](docs/PatchedFlowRequest.md)
  - [PatchedFlowStageBindingRequest](docs/PatchedFlowStageBindingRequest.md)
- - [PatchedGoogleWorkspaceProviderGroupRequest](docs/PatchedGoogleWorkspaceProviderGroupRequest.md)
  - [PatchedGoogleWorkspaceProviderMappingRequest](docs/PatchedGoogleWorkspaceProviderMappingRequest.md)
  - [PatchedGoogleWorkspaceProviderRequest](docs/PatchedGoogleWorkspaceProviderRequest.md)
- - [PatchedGoogleWorkspaceProviderUserRequest](docs/PatchedGoogleWorkspaceProviderUserRequest.md)
  - [PatchedGroupRequest](docs/PatchedGroupRequest.md)
  - [PatchedIdentificationStageRequest](docs/PatchedIdentificationStageRequest.md)
  - [PatchedInvitationRequest](docs/PatchedInvitationRequest.md)
  - [PatchedInvitationStageRequest](docs/PatchedInvitationStageRequest.md)
  - [PatchedKubernetesServiceConnectionRequest](docs/PatchedKubernetesServiceConnectionRequest.md)
  - [PatchedLDAPPropertyMappingRequest](docs/PatchedLDAPPropertyMappingRequest.md)
  - [PatchedLDAPProviderRequest](docs/PatchedLDAPProviderRequest.md)
  - [PatchedLDAPSourceRequest](docs/PatchedLDAPSourceRequest.md)
  - [PatchedLicenseRequest](docs/PatchedLicenseRequest.md)
- - [PatchedMicrosoftEntraProviderGroupRequest](docs/PatchedMicrosoftEntraProviderGroupRequest.md)
  - [PatchedMicrosoftEntraProviderMappingRequest](docs/PatchedMicrosoftEntraProviderMappingRequest.md)
  - [PatchedMicrosoftEntraProviderRequest](docs/PatchedMicrosoftEntraProviderRequest.md)
- - [PatchedMicrosoftEntraProviderUserRequest](docs/PatchedMicrosoftEntraProviderUserRequest.md)
  - [PatchedNotificationRequest](docs/PatchedNotificationRequest.md)
  - [PatchedNotificationRuleRequest](docs/PatchedNotificationRuleRequest.md)
  - [PatchedNotificationTransportRequest](docs/PatchedNotificationTransportRequest.md)
  - [PatchedNotificationWebhookMappingRequest](docs/PatchedNotificationWebhookMappingRequest.md)
  - [PatchedOAuth2ProviderRequest](docs/PatchedOAuth2ProviderRequest.md)
  - [PatchedOAuthSourceRequest](docs/PatchedOAuthSourceRequest.md)
  - [PatchedOutpostRequest](docs/PatchedOutpostRequest.md)
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/__init__.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.4.2-1716550398"
+__version__ = "2024.4.2-1717033274"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
@@ -417,31 +417,27 @@
 from authentik_client.models.patched_email_stage_request import PatchedEmailStageRequest
 from authentik_client.models.patched_endpoint_request import PatchedEndpointRequest
 from authentik_client.models.patched_event_matcher_policy_request import PatchedEventMatcherPolicyRequest
 from authentik_client.models.patched_event_request import PatchedEventRequest
 from authentik_client.models.patched_expression_policy_request import PatchedExpressionPolicyRequest
 from authentik_client.models.patched_flow_request import PatchedFlowRequest
 from authentik_client.models.patched_flow_stage_binding_request import PatchedFlowStageBindingRequest
-from authentik_client.models.patched_google_workspace_provider_group_request import PatchedGoogleWorkspaceProviderGroupRequest
 from authentik_client.models.patched_google_workspace_provider_mapping_request import PatchedGoogleWorkspaceProviderMappingRequest
 from authentik_client.models.patched_google_workspace_provider_request import PatchedGoogleWorkspaceProviderRequest
-from authentik_client.models.patched_google_workspace_provider_user_request import PatchedGoogleWorkspaceProviderUserRequest
 from authentik_client.models.patched_group_request import PatchedGroupRequest
 from authentik_client.models.patched_identification_stage_request import PatchedIdentificationStageRequest
 from authentik_client.models.patched_invitation_request import PatchedInvitationRequest
 from authentik_client.models.patched_invitation_stage_request import PatchedInvitationStageRequest
 from authentik_client.models.patched_kubernetes_service_connection_request import PatchedKubernetesServiceConnectionRequest
 from authentik_client.models.patched_ldap_property_mapping_request import PatchedLDAPPropertyMappingRequest
 from authentik_client.models.patched_ldap_provider_request import PatchedLDAPProviderRequest
 from authentik_client.models.patched_ldap_source_request import PatchedLDAPSourceRequest
 from authentik_client.models.patched_license_request import PatchedLicenseRequest
-from authentik_client.models.patched_microsoft_entra_provider_group_request import PatchedMicrosoftEntraProviderGroupRequest
 from authentik_client.models.patched_microsoft_entra_provider_mapping_request import PatchedMicrosoftEntraProviderMappingRequest
 from authentik_client.models.patched_microsoft_entra_provider_request import PatchedMicrosoftEntraProviderRequest
-from authentik_client.models.patched_microsoft_entra_provider_user_request import PatchedMicrosoftEntraProviderUserRequest
 from authentik_client.models.patched_notification_request import PatchedNotificationRequest
 from authentik_client.models.patched_notification_rule_request import PatchedNotificationRuleRequest
 from authentik_client.models.patched_notification_transport_request import PatchedNotificationTransportRequest
 from authentik_client.models.patched_notification_webhook_mapping_request import PatchedNotificationWebhookMappingRequest
 from authentik_client.models.patched_o_auth2_provider_request import PatchedOAuth2ProviderRequest
 from authentik_client.models.patched_o_auth_source_request import PatchedOAuthSourceRequest
 from authentik_client.models.patched_outpost_request import PatchedOutpostRequest
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/__init__.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/admin_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/authenticators_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/authenticators_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/core_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/crypto_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/crypto_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/enterprise_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/enterprise_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/events_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/flows_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/managed_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/managed_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/oauth2_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/oauth2_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/outposts_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/outposts_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/policies_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/propertymappings_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/providers_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/providers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,17 @@
 from authentik_client.models.paginated_o_auth2_provider_list import PaginatedOAuth2ProviderList
 from authentik_client.models.paginated_provider_list import PaginatedProviderList
 from authentik_client.models.paginated_proxy_provider_list import PaginatedProxyProviderList
 from authentik_client.models.paginated_rac_provider_list import PaginatedRACProviderList
 from authentik_client.models.paginated_radius_provider_list import PaginatedRadiusProviderList
 from authentik_client.models.paginated_saml_provider_list import PaginatedSAMLProviderList
 from authentik_client.models.paginated_scim_provider_list import PaginatedSCIMProviderList
-from authentik_client.models.patched_google_workspace_provider_group_request import PatchedGoogleWorkspaceProviderGroupRequest
 from authentik_client.models.patched_google_workspace_provider_request import PatchedGoogleWorkspaceProviderRequest
-from authentik_client.models.patched_google_workspace_provider_user_request import PatchedGoogleWorkspaceProviderUserRequest
 from authentik_client.models.patched_ldap_provider_request import PatchedLDAPProviderRequest
-from authentik_client.models.patched_microsoft_entra_provider_group_request import PatchedMicrosoftEntraProviderGroupRequest
 from authentik_client.models.patched_microsoft_entra_provider_request import PatchedMicrosoftEntraProviderRequest
-from authentik_client.models.patched_microsoft_entra_provider_user_request import PatchedMicrosoftEntraProviderUserRequest
 from authentik_client.models.patched_o_auth2_provider_request import PatchedOAuth2ProviderRequest
 from authentik_client.models.patched_proxy_provider_request import PatchedProxyProviderRequest
 from authentik_client.models.patched_rac_provider_request import PatchedRACProviderRequest
 from authentik_client.models.patched_radius_provider_request import PatchedRadiusProviderRequest
 from authentik_client.models.patched_saml_provider_request import PatchedSAMLProviderRequest
 from authentik_client.models.patched_scim_provider_request import PatchedSCIMProviderRequest
 from authentik_client.models.property_mapping_preview import PropertyMappingPreview
@@ -2938,306 +2934,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_google_workspace_groups_partial_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        patched_google_workspace_provider_group_request: Optional[PatchedGoogleWorkspaceProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GoogleWorkspaceProviderGroup:
-        """providers_google_workspace_groups_partial_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param patched_google_workspace_provider_group_request:
-        :type patched_google_workspace_provider_group_request: PatchedGoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_group_request=patched_google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_google_workspace_groups_partial_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        patched_google_workspace_provider_group_request: Optional[PatchedGoogleWorkspaceProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GoogleWorkspaceProviderGroup]:
-        """providers_google_workspace_groups_partial_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param patched_google_workspace_provider_group_request:
-        :type patched_google_workspace_provider_group_request: PatchedGoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_group_request=patched_google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_google_workspace_groups_partial_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        patched_google_workspace_provider_group_request: Optional[PatchedGoogleWorkspaceProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_google_workspace_groups_partial_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param patched_google_workspace_provider_group_request:
-        :type patched_google_workspace_provider_group_request: PatchedGoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_group_request=patched_google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_google_workspace_groups_partial_update_serialize(
-        self,
-        id,
-        patched_google_workspace_provider_group_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if patched_google_workspace_provider_group_request is not None:
-            _body_params = patched_google_workspace_provider_group_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/providers/google_workspace_groups/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_google_workspace_groups_retrieve(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -3494,306 +3198,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_google_workspace_groups_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GoogleWorkspaceProviderGroup:
-        """providers_google_workspace_groups_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param google_workspace_provider_group_request: (required)
-        :type google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_update_serialize(
-            id=id,
-            google_workspace_provider_group_request=google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_google_workspace_groups_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GoogleWorkspaceProviderGroup]:
-        """providers_google_workspace_groups_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param google_workspace_provider_group_request: (required)
-        :type google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_update_serialize(
-            id=id,
-            google_workspace_provider_group_request=google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_google_workspace_groups_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
-        google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_google_workspace_groups_update
-
-        GoogleWorkspaceProviderGroup Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider Group. (required)
-        :type id: str
-        :param google_workspace_provider_group_request: (required)
-        :type google_workspace_provider_group_request: GoogleWorkspaceProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_groups_update_serialize(
-            id=id,
-            google_workspace_provider_group_request=google_workspace_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_google_workspace_groups_update_serialize(
-        self,
-        id,
-        google_workspace_provider_group_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if google_workspace_provider_group_request is not None:
-            _body_params = google_workspace_provider_group_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/providers/google_workspace_groups/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_google_workspace_groups_used_by_list(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider Group.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -6723,306 +6135,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_google_workspace_users_partial_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        patched_google_workspace_provider_user_request: Optional[PatchedGoogleWorkspaceProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GoogleWorkspaceProviderUser:
-        """providers_google_workspace_users_partial_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param patched_google_workspace_provider_user_request:
-        :type patched_google_workspace_provider_user_request: PatchedGoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_user_request=patched_google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_google_workspace_users_partial_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        patched_google_workspace_provider_user_request: Optional[PatchedGoogleWorkspaceProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GoogleWorkspaceProviderUser]:
-        """providers_google_workspace_users_partial_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param patched_google_workspace_provider_user_request:
-        :type patched_google_workspace_provider_user_request: PatchedGoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_user_request=patched_google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_google_workspace_users_partial_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        patched_google_workspace_provider_user_request: Optional[PatchedGoogleWorkspaceProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_google_workspace_users_partial_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param patched_google_workspace_provider_user_request:
-        :type patched_google_workspace_provider_user_request: PatchedGoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_partial_update_serialize(
-            id=id,
-            patched_google_workspace_provider_user_request=patched_google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_google_workspace_users_partial_update_serialize(
-        self,
-        id,
-        patched_google_workspace_provider_user_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if patched_google_workspace_provider_user_request is not None:
-            _body_params = patched_google_workspace_provider_user_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/providers/google_workspace_users/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_google_workspace_users_retrieve(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -7279,306 +6399,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_google_workspace_users_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GoogleWorkspaceProviderUser:
-        """providers_google_workspace_users_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param google_workspace_provider_user_request: (required)
-        :type google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_update_serialize(
-            id=id,
-            google_workspace_provider_user_request=google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_google_workspace_users_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GoogleWorkspaceProviderUser]:
-        """providers_google_workspace_users_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param google_workspace_provider_user_request: (required)
-        :type google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_update_serialize(
-            id=id,
-            google_workspace_provider_user_request=google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_google_workspace_users_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
-        google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_google_workspace_users_update
-
-        GoogleWorkspaceProviderUser Viewset
-
-        :param id: A UUID string identifying this Google Workspace Provider User. (required)
-        :type id: str
-        :param google_workspace_provider_user_request: (required)
-        :type google_workspace_provider_user_request: GoogleWorkspaceProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_google_workspace_users_update_serialize(
-            id=id,
-            google_workspace_provider_user_request=google_workspace_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GoogleWorkspaceProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_google_workspace_users_update_serialize(
-        self,
-        id,
-        google_workspace_provider_user_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if google_workspace_provider_user_request is not None:
-            _body_params = google_workspace_provider_user_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/providers/google_workspace_users/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_google_workspace_users_used_by_list(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Google Workspace Provider User.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -11442,306 +10270,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_microsoft_entra_groups_partial_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        patched_microsoft_entra_provider_group_request: Optional[PatchedMicrosoftEntraProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MicrosoftEntraProviderGroup:
-        """providers_microsoft_entra_groups_partial_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_group_request:
-        :type patched_microsoft_entra_provider_group_request: PatchedMicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_group_request=patched_microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_microsoft_entra_groups_partial_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        patched_microsoft_entra_provider_group_request: Optional[PatchedMicrosoftEntraProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MicrosoftEntraProviderGroup]:
-        """providers_microsoft_entra_groups_partial_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_group_request:
-        :type patched_microsoft_entra_provider_group_request: PatchedMicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_group_request=patched_microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_microsoft_entra_groups_partial_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        patched_microsoft_entra_provider_group_request: Optional[PatchedMicrosoftEntraProviderGroupRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_microsoft_entra_groups_partial_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_group_request:
-        :type patched_microsoft_entra_provider_group_request: PatchedMicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_group_request=patched_microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_microsoft_entra_groups_partial_update_serialize(
-        self,
-        id,
-        patched_microsoft_entra_provider_group_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if patched_microsoft_entra_provider_group_request is not None:
-            _body_params = patched_microsoft_entra_provider_group_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/providers/microsoft_entra_groups/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_microsoft_entra_groups_retrieve(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -11998,306 +10534,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_microsoft_entra_groups_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MicrosoftEntraProviderGroup:
-        """providers_microsoft_entra_groups_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param microsoft_entra_provider_group_request: (required)
-        :type microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_update_serialize(
-            id=id,
-            microsoft_entra_provider_group_request=microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_microsoft_entra_groups_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MicrosoftEntraProviderGroup]:
-        """providers_microsoft_entra_groups_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param microsoft_entra_provider_group_request: (required)
-        :type microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_update_serialize(
-            id=id,
-            microsoft_entra_provider_group_request=microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_microsoft_entra_groups_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
-        microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_microsoft_entra_groups_update
-
-        MicrosoftEntraProviderGroup Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider Group. (required)
-        :type id: str
-        :param microsoft_entra_provider_group_request: (required)
-        :type microsoft_entra_provider_group_request: MicrosoftEntraProviderGroupRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_groups_update_serialize(
-            id=id,
-            microsoft_entra_provider_group_request=microsoft_entra_provider_group_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderGroup",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_microsoft_entra_groups_update_serialize(
-        self,
-        id,
-        microsoft_entra_provider_group_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if microsoft_entra_provider_group_request is not None:
-            _body_params = microsoft_entra_provider_group_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/providers/microsoft_entra_groups/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_microsoft_entra_groups_used_by_list(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider Group.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -15210,306 +13454,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def providers_microsoft_entra_users_partial_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        patched_microsoft_entra_provider_user_request: Optional[PatchedMicrosoftEntraProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MicrosoftEntraProviderUser:
-        """providers_microsoft_entra_users_partial_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_user_request:
-        :type patched_microsoft_entra_provider_user_request: PatchedMicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_user_request=patched_microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_microsoft_entra_users_partial_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        patched_microsoft_entra_provider_user_request: Optional[PatchedMicrosoftEntraProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MicrosoftEntraProviderUser]:
-        """providers_microsoft_entra_users_partial_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_user_request:
-        :type patched_microsoft_entra_provider_user_request: PatchedMicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_user_request=patched_microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_microsoft_entra_users_partial_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        patched_microsoft_entra_provider_user_request: Optional[PatchedMicrosoftEntraProviderUserRequest] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_microsoft_entra_users_partial_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param patched_microsoft_entra_provider_user_request:
-        :type patched_microsoft_entra_provider_user_request: PatchedMicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_partial_update_serialize(
-            id=id,
-            patched_microsoft_entra_provider_user_request=patched_microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_microsoft_entra_users_partial_update_serialize(
-        self,
-        id,
-        patched_microsoft_entra_provider_user_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if patched_microsoft_entra_provider_user_request is not None:
-            _body_params = patched_microsoft_entra_provider_user_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/providers/microsoft_entra_users/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def providers_microsoft_entra_users_retrieve(
         self,
         id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -15756,306 +13708,14 @@
             resource_path='/providers/microsoft_entra_users/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def providers_microsoft_entra_users_update(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MicrosoftEntraProviderUser:
-        """providers_microsoft_entra_users_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param microsoft_entra_provider_user_request: (required)
-        :type microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_update_serialize(
-            id=id,
-            microsoft_entra_provider_user_request=microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def providers_microsoft_entra_users_update_with_http_info(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MicrosoftEntraProviderUser]:
-        """providers_microsoft_entra_users_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param microsoft_entra_provider_user_request: (required)
-        :type microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_update_serialize(
-            id=id,
-            microsoft_entra_provider_user_request=microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def providers_microsoft_entra_users_update_without_preload_content(
-        self,
-        id: Annotated[StrictStr, Field(description="A UUID string identifying this Microsoft Entra Provider User.")],
-        microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """providers_microsoft_entra_users_update
-
-        MicrosoftEntraProviderUser Viewset
-
-        :param id: A UUID string identifying this Microsoft Entra Provider User. (required)
-        :type id: str
-        :param microsoft_entra_provider_user_request: (required)
-        :type microsoft_entra_provider_user_request: MicrosoftEntraProviderUserRequest
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._providers_microsoft_entra_users_update_serialize(
-            id=id,
-            microsoft_entra_provider_user_request=microsoft_entra_provider_user_request,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MicrosoftEntraProviderUser",
-            '400': "ValidationError",
-            '403': "GenericError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _providers_microsoft_entra_users_update_serialize(
-        self,
-        id,
-        microsoft_entra_provider_user_request,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if microsoft_entra_provider_user_request is not None:
-            _body_params = microsoft_entra_provider_user_request
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'authentik'
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/providers/microsoft_entra_users/{id}/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
             auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/rac_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/rac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/rbac_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/rbac_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/root_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/root_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/schema_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/sources_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/stages_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/stages_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api/tenants_api.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api_client.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.4.2-1716550398/python'
+        self.user_agent = 'OpenAPI-Generator/2024.4.2-1717033274/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/api_response.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/configuration.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024.4.2\n"\
-               "SDK Package Version: 2024.4.2-1716550398".\
+               "SDK Package Version: 2024.4.2-1717033274".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/exceptions.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/__init__.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,31 +381,27 @@
 from authentik_client.models.patched_email_stage_request import PatchedEmailStageRequest
 from authentik_client.models.patched_endpoint_request import PatchedEndpointRequest
 from authentik_client.models.patched_event_matcher_policy_request import PatchedEventMatcherPolicyRequest
 from authentik_client.models.patched_event_request import PatchedEventRequest
 from authentik_client.models.patched_expression_policy_request import PatchedExpressionPolicyRequest
 from authentik_client.models.patched_flow_request import PatchedFlowRequest
 from authentik_client.models.patched_flow_stage_binding_request import PatchedFlowStageBindingRequest
-from authentik_client.models.patched_google_workspace_provider_group_request import PatchedGoogleWorkspaceProviderGroupRequest
 from authentik_client.models.patched_google_workspace_provider_mapping_request import PatchedGoogleWorkspaceProviderMappingRequest
 from authentik_client.models.patched_google_workspace_provider_request import PatchedGoogleWorkspaceProviderRequest
-from authentik_client.models.patched_google_workspace_provider_user_request import PatchedGoogleWorkspaceProviderUserRequest
 from authentik_client.models.patched_group_request import PatchedGroupRequest
 from authentik_client.models.patched_identification_stage_request import PatchedIdentificationStageRequest
 from authentik_client.models.patched_invitation_request import PatchedInvitationRequest
 from authentik_client.models.patched_invitation_stage_request import PatchedInvitationStageRequest
 from authentik_client.models.patched_kubernetes_service_connection_request import PatchedKubernetesServiceConnectionRequest
 from authentik_client.models.patched_ldap_property_mapping_request import PatchedLDAPPropertyMappingRequest
 from authentik_client.models.patched_ldap_provider_request import PatchedLDAPProviderRequest
 from authentik_client.models.patched_ldap_source_request import PatchedLDAPSourceRequest
 from authentik_client.models.patched_license_request import PatchedLicenseRequest
-from authentik_client.models.patched_microsoft_entra_provider_group_request import PatchedMicrosoftEntraProviderGroupRequest
 from authentik_client.models.patched_microsoft_entra_provider_mapping_request import PatchedMicrosoftEntraProviderMappingRequest
 from authentik_client.models.patched_microsoft_entra_provider_request import PatchedMicrosoftEntraProviderRequest
-from authentik_client.models.patched_microsoft_entra_provider_user_request import PatchedMicrosoftEntraProviderUserRequest
 from authentik_client.models.patched_notification_request import PatchedNotificationRequest
 from authentik_client.models.patched_notification_rule_request import PatchedNotificationRuleRequest
 from authentik_client.models.patched_notification_transport_request import PatchedNotificationTransportRequest
 from authentik_client.models.patched_notification_webhook_mapping_request import PatchedNotificationWebhookMappingRequest
 from authentik_client.models.patched_o_auth2_provider_request import PatchedOAuth2ProviderRequest
 from authentik_client.models.patched_o_auth_source_request import PatchedOAuthSourceRequest
 from authentik_client.models.patched_outpost_request import PatchedOutpostRequest
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/access_denied_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/alg_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/alg_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/app.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/app.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/app_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/app_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/apple_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/apple_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/application.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/application.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/application_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/auth_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/auth_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_asn.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authentication_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authentication_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_attachment_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validate_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validation_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/autosubmit_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/backends_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/backends_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/binding_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_file.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_file.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/brand.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/brand_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/cache.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/cache.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/capabilities_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_data.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_data.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_generation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_key_pair.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/challenge_choices.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/challenge_choices.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/challenge_types.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/client_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/client_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/connection_token.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/connection_token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/connection_token_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/contextual_flow_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/coordinate.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/current_brand.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/current_brand.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/denied_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/deny_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/deny_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/device_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/device_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/device_challenge_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/device_classes_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/digest_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/digits_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/digits_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/docker_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/domain.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/domain_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device_enrollment_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/duo_response_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/email_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/email_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/email_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/email_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/email_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/email_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/endpoint.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/endpoint_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/error_detail.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/error_reporting_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event_actions.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event_actions.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event_matcher_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/event_top_per_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/expiring_base_grant_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/expression_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/expression_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/extra_role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/extra_user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/file_path_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/file_path_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_designation_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_diagram.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_diagram.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_error_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_import_result.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_import_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_inspection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_inspection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_inspector_plan.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_layout_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_set.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_set.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_set_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_set_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_stage_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/footer_link.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/footer_link.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/generic_error.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/generic_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/geoip_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_group.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 from authentik_client.models.user_group import UserGroup
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GoogleWorkspaceProviderGroup(BaseModel):
+class SCIMSourceGroup(BaseModel):
     """
-    GoogleWorkspaceProviderGroup Serializer
+    SCIMSourceGroup Serializer
     """ # noqa: E501
     id: StrictStr
     group: StrictStr
     group_obj: UserGroup
-    __properties: ClassVar[List[str]] = ["id", "group", "group_obj"]
+    source: StrictStr
+    attributes: Optional[Any] = None
+    __properties: ClassVar[List[str]] = ["id", "group", "group_obj", "source", "attributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,54 +49,59 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderGroup from a JSON string"""
+        """Create an instance of SCIMSourceGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "id",
             "group_obj",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of group_obj
         if self.group_obj:
             _dict['group_obj'] = self.group_obj.to_dict()
+        # set to None if attributes (nullable) is None
+        # and model_fields_set contains the field
+        if self.attributes is None and "attributes" in self.model_fields_set:
+            _dict['attributes'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderGroup from a dict"""
+        """Create an instance of SCIMSourceGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "group": obj.get("group"),
-            "group_obj": UserGroup.from_dict(obj["group_obj"]) if obj.get("group_obj") is not None else None
+            "group_obj": UserGroup.from_dict(obj["group_obj"]) if obj.get("group_obj") is not None else None,
+            "source": obj.get("source"),
+            "attributes": obj.get("attributes")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GoogleWorkspaceProviderGroupRequest(BaseModel):
+class Link(BaseModel):
     """
-    GoogleWorkspaceProviderGroup Serializer
+    Returns a single link
     """ # noqa: E501
-    group: StrictStr
-    __properties: ClassVar[List[str]] = ["group"]
+    link: StrictStr
+    __properties: ClassVar[List[str]] = ["link"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderGroupRequest from a JSON string"""
+        """Create an instance of Link from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderGroupRequest from a dict"""
+        """Create an instance of Link from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "group": obj.get("group")
+            "link": obj.get("link")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/token_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.group_member import GroupMember
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GoogleWorkspaceProviderUser(BaseModel):
+class TokenView(BaseModel):
     """
-    GoogleWorkspaceProviderUser Serializer
+    Show token's current key
     """ # noqa: E501
-    id: StrictStr
-    user: StrictInt
-    user_obj: GroupMember
-    __properties: ClassVar[List[str]] = ["id", "user", "user_obj"]
+    key: StrictStr
+    __properties: ClassVar[List[str]] = ["key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,54 +44,47 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderUser from a JSON string"""
+        """Create an instance of TokenView from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "id",
-            "user_obj",
+            "key",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of user_obj
-        if self.user_obj:
-            _dict['user_obj'] = self.user_obj.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderUser from a dict"""
+        """Create an instance of TokenView from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "user": obj.get("user"),
-            "user_obj": GroupMember.from_dict(obj["user_obj"]) if obj.get("user_obj") is not None else None
+            "key": obj.get("key")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/google_workspace_provider_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/license_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GoogleWorkspaceProviderUserRequest(BaseModel):
+class LicenseRequest(BaseModel):
     """
-    GoogleWorkspaceProviderUser Serializer
+    License Serializer
     """ # noqa: E501
-    user: StrictInt
-    __properties: ClassVar[List[str]] = ["user"]
+    key: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderUserRequest from a JSON string"""
+        """Create an instance of LicenseRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GoogleWorkspaceProviderUserRequest from a dict"""
+        """Create an instance of LicenseRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user")
+            "key": obj.get("key")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/group.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/group_member.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/group_member_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/group_member_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/install_id.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/install_id.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/intent_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/intent_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/invalid_response_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/issuer_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/kubernetes_service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_debug.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_debug.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ldapapi_access_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/license.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/license.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/license_forecast.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/license_forecast.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/license_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LicenseRequest(BaseModel):
+class WebAuthnDeviceRequest(BaseModel):
     """
-    License Serializer
+    Serializer for WebAuthn authenticator devices
     """ # noqa: E501
-    key: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["key"]
+    name: Annotated[str, Field(min_length=1, strict=True, max_length=200)]
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LicenseRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LicenseRequest from a dict"""
+        """Create an instance of WebAuthnDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "key": obj.get("key")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/license_summary.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/license_summary.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/link.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Link(BaseModel):
+class StaticDeviceToken(BaseModel):
     """
-    Returns a single link
+    Serializer for static device's tokens
     """ # noqa: E501
-    link: StrictStr
-    __properties: ClassVar[List[str]] = ["link"]
+    token: Annotated[str, Field(strict=True, max_length=16)]
+    __properties: ClassVar[List[str]] = ["token"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Link from a JSON string"""
+        """Create an instance of StaticDeviceToken from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Link from a dict"""
+        """Create an instance of StaticDeviceToken from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "link": obj.get("link")
+            "token": obj.get("token")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/log_event.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/log_event.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/log_level_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/log_level_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/login_challenge_types.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/login_metrics.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/login_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/login_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/login_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/metadata.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_group.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/sms_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.user_group import UserGroup
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MicrosoftEntraProviderGroup(BaseModel):
+class SMSDevice(BaseModel):
     """
-    MicrosoftEntraProviderGroup Serializer
+    Serializer for sms authenticator devices
     """ # noqa: E501
-    id: StrictStr
-    group: StrictStr
-    group_obj: UserGroup
-    __properties: ClassVar[List[str]] = ["id", "group", "group_obj"]
+    name: Annotated[str, Field(strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
+    pk: StrictInt
+    phone_number: StrictStr
+    __properties: ClassVar[List[str]] = ["name", "pk", "phone_number"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderGroup from a JSON string"""
+        """Create an instance of SMSDevice from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -63,38 +63,35 @@
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "id",
-            "group_obj",
+            "pk",
+            "phone_number",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of group_obj
-        if self.group_obj:
-            _dict['group_obj'] = self.group_obj.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderGroup from a dict"""
+        """Create an instance of SMSDevice from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "group": obj.get("group"),
-            "group_obj": UserGroup.from_dict(obj["group_obj"]) if obj.get("group_obj") is not None else None
+            "name": obj.get("name"),
+            "pk": obj.get("pk"),
+            "phone_number": obj.get("phone_number")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_recovery_key_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from datetime import datetime
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MicrosoftEntraProviderGroupRequest(BaseModel):
+class TenantRecoveryKeyResponse(BaseModel):
     """
-    MicrosoftEntraProviderGroup Serializer
+    Tenant recovery key creation response serializer
     """ # noqa: E501
-    group: StrictStr
-    __properties: ClassVar[List[str]] = ["group"]
+    expiry: datetime
+    url: StrictStr
+    __properties: ClassVar[List[str]] = ["expiry", "url"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderGroupRequest from a JSON string"""
+        """Create an instance of TenantRecoveryKeyResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderGroupRequest from a dict"""
+        """Create an instance of TenantRecoveryKeyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "group": obj.get("group")
+            "expiry": obj.get("expiry"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_test_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.group_member import GroupMember
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MicrosoftEntraProviderUser(BaseModel):
+class PropertyMappingTestResult(BaseModel):
     """
-    MicrosoftEntraProviderUser Serializer
+    Result of a Property-mapping test
     """ # noqa: E501
-    id: StrictStr
-    user: StrictInt
-    user_obj: GroupMember
-    __properties: ClassVar[List[str]] = ["id", "user", "user_obj"]
+    result: StrictStr
+    successful: StrictBool
+    __properties: ClassVar[List[str]] = ["result", "successful"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderUser from a JSON string"""
+        """Create an instance of PropertyMappingTestResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -63,38 +61,34 @@
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "id",
-            "user_obj",
+            "result",
+            "successful",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of user_obj
-        if self.user_obj:
-            _dict['user_obj'] = self.user_obj.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderUser from a dict"""
+        """Create an instance of PropertyMappingTestResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "user": obj.get("user"),
-            "user_obj": GroupMember.from_dict(obj["user_obj"]) if obj.get("user_obj") is not None else None
+            "result": obj.get("result"),
+            "successful": obj.get("successful")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/microsoft_entra_provider_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_group_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MicrosoftEntraProviderUserRequest(BaseModel):
+class MicrosoftEntraProviderGroupRequest(BaseModel):
     """
-    MicrosoftEntraProviderUser Serializer
+    MicrosoftEntraProviderGroup Serializer
     """ # noqa: E501
-    user: StrictInt
-    __properties: ClassVar[List[str]] = ["user"]
+    group: StrictStr
+    provider: StrictInt
+    __properties: ClassVar[List[str]] = ["group", "provider"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderUserRequest from a JSON string"""
+        """Create an instance of MicrosoftEntraProviderGroupRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MicrosoftEntraProviderUserRequest from a dict"""
+        """Create an instance of MicrosoftEntraProviderGroupRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user")
+            "group": obj.get("group"),
+            "provider": obj.get("provider")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/model_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/model_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/model_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/name_id_policy_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/network_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/not_configured_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_rule.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_rule.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_transport_test.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_webhook_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/open_id_connect_configuration.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outgoing_sync_delete_action.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outgoing_sync_delete_action.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_default_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_health.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_health.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/outpost_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_brand_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_connection_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_consent_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_deny_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_domain_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_duo_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_email_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_event_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_expression_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_flow_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_group_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_google_workspace_provider_user_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_google_workspace_provider_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_identification_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_invitation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_ldap_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_license_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_group_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_microsoft_entra_provider_user_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_microsoft_entra_provider_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_rule_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_transport_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_outpost_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_password_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_plex_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_prompt_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_rac_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_radius_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_reputation_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_saml_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_provider_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_service_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_sms_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_source_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_source_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_static_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_system_task_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_token_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_token_model_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_totp_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_consent_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/pagination.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_expiry_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/password_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_application_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_brand_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_captcha_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_connection_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_consent_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_deny_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_domain_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_dummy_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_dummy_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_duo_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_email_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_event_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_event_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_expression_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_flow_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_license_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedGoogleWorkspaceProviderGroupRequest(BaseModel):
+class PatchedLicenseRequest(BaseModel):
     """
-    GoogleWorkspaceProviderGroup Serializer
+    License Serializer
     """ # noqa: E501
-    group: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["group"]
+    key: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    __properties: ClassVar[List[str]] = ["key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedGoogleWorkspaceProviderGroupRequest from a JSON string"""
+        """Create an instance of PatchedLicenseRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedGoogleWorkspaceProviderGroupRequest from a dict"""
+        """Create an instance of PatchedLicenseRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "group": obj.get("group")
+            "key": obj.get("key")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_google_workspace_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_google_workspace_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_google_workspace_provider_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_group_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedGoogleWorkspaceProviderUserRequest(BaseModel):
+class GoogleWorkspaceProviderGroupRequest(BaseModel):
     """
-    GoogleWorkspaceProviderUser Serializer
+    GoogleWorkspaceProviderGroup Serializer
     """ # noqa: E501
-    user: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["user"]
+    group: StrictStr
+    provider: StrictInt
+    __properties: ClassVar[List[str]] = ["group", "provider"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedGoogleWorkspaceProviderUserRequest from a JSON string"""
+        """Create an instance of GoogleWorkspaceProviderGroupRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedGoogleWorkspaceProviderUserRequest from a dict"""
+        """Create an instance of GoogleWorkspaceProviderGroupRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user")
+            "group": obj.get("group"),
+            "provider": obj.get("provider")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_identification_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_invitation_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_invitation_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_ldap_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_license_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/token_set_key_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedLicenseRequest(BaseModel):
+class TokenSetKeyRequest(BaseModel):
     """
-    License Serializer
+    TokenSetKeyRequest
     """ # noqa: E501
-    key: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    key: Annotated[str, Field(min_length=1, strict=True)]
     __properties: ClassVar[List[str]] = ["key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedLicenseRequest from a JSON string"""
+        """Create an instance of TokenSetKeyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedLicenseRequest from a dict"""
+        """Create an instance of TokenSetKeyRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_web_authn_device_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List, Optional
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedMicrosoftEntraProviderGroupRequest(BaseModel):
+class PatchedWebAuthnDeviceRequest(BaseModel):
     """
-    MicrosoftEntraProviderGroup Serializer
+    Serializer for WebAuthn authenticator devices
     """ # noqa: E501
-    group: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["group"]
+    name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=200)]] = None
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedMicrosoftEntraProviderGroupRequest from a JSON string"""
+        """Create an instance of PatchedWebAuthnDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedMicrosoftEntraProviderGroupRequest from a dict"""
+        """Create an instance of PatchedWebAuthnDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "group": obj.get("group")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_microsoft_entra_provider_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_microsoft_entra_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_microsoft_entra_provider_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_user_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedMicrosoftEntraProviderUserRequest(BaseModel):
+class MicrosoftEntraProviderUserRequest(BaseModel):
     """
     MicrosoftEntraProviderUser Serializer
     """ # noqa: E501
-    user: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["user"]
+    user: StrictInt
+    provider: StrictInt
+    __properties: ClassVar[List[str]] = ["user", "provider"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedMicrosoftEntraProviderUserRequest from a JSON string"""
+        """Create an instance of MicrosoftEntraProviderUserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedMicrosoftEntraProviderUserRequest from a dict"""
+        """Create an instance of MicrosoftEntraProviderUserRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user")
+            "user": obj.get("user"),
+            "provider": obj.get("provider")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_rule_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_transport_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_o_auth_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_outpost_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_password_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_role_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_sms_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_tenant_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_token_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_totp_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/patched_user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedWebAuthnDeviceRequest(BaseModel):
+class ServiceConnectionRequest(BaseModel):
     """
-    Serializer for WebAuthn authenticator devices
+    ServiceConnection Serializer
     """ # noqa: E501
-    name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=200)]] = None
-    __properties: ClassVar[List[str]] = ["name"]
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    local: Optional[StrictBool] = Field(default=None, description="If enabled, use the local connection. Required Docker socket/Kubernetes Integration")
+    __properties: ClassVar[List[str]] = ["name", "local"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedWebAuthnDeviceRequest from a JSON string"""
+        """Create an instance of ServiceConnectionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedWebAuthnDeviceRequest from a dict"""
+        """Create an instance of ServiceConnectionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "local": obj.get("local")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/permission_assign_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_authentication_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/plex_token_redeem_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_binding.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_binding.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_binding_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_engine_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_test_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/policy_test_result.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/policy_test_result.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/prompt_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_preview.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_test_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/property_mapping_test_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_self_groups.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PropertyMappingTestResult(BaseModel):
+class UserSelfGroups(BaseModel):
     """
-    Result of a Property-mapping test
+    UserSelfGroups
     """ # noqa: E501
-    result: StrictStr
-    successful: StrictBool
-    __properties: ClassVar[List[str]] = ["result", "successful"]
+    name: StrictStr
+    pk: StrictStr
+    __properties: ClassVar[List[str]] = ["name", "pk"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PropertyMappingTestResult from a JSON string"""
+        """Create an instance of UserSelfGroups from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -61,34 +61,34 @@
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "result",
-            "successful",
+            "name",
+            "pk",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PropertyMappingTestResult from a dict"""
+        """Create an instance of UserSelfGroups from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "result": obj.get("result"),
-            "successful": obj.get("successful")
+            "name": obj.get("name"),
+            "pk": obj.get("pk")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/protocol_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/protocol_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_model_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/provider_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_mode.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_mode.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/proxy_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/rac_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_outpost_config.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/radius_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/redirect_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation_policy.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation_policy.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/reputation_policy_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/resident_key_requirement_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/role.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/role.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/role_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/role_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/role_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/role_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/role_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_metadata.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_property_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/saml_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/saml_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_provider.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_provider.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_provider_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_group.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from authentik_client.models.user_group import UserGroup
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SCIMSourceGroup(BaseModel):
+class GoogleWorkspaceProviderGroup(BaseModel):
     """
-    SCIMSourceGroup Serializer
+    GoogleWorkspaceProviderGroup Serializer
     """ # noqa: E501
     id: StrictStr
     group: StrictStr
     group_obj: UserGroup
-    source: StrictStr
-    attributes: Optional[Any] = None
-    __properties: ClassVar[List[str]] = ["id", "group", "group_obj", "source", "attributes"]
+    provider: StrictInt
+    attributes: Optional[Any]
+    __properties: ClassVar[List[str]] = ["id", "group", "group_obj", "provider", "attributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,30 +49,34 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SCIMSourceGroup from a JSON string"""
+        """Create an instance of GoogleWorkspaceProviderGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "id",
             "group_obj",
+            "attributes",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
@@ -84,24 +88,24 @@
         if self.attributes is None and "attributes" in self.model_fields_set:
             _dict['attributes'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SCIMSourceGroup from a dict"""
+        """Create an instance of GoogleWorkspaceProviderGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "group": obj.get("group"),
             "group_obj": UserGroup.from_dict(obj["group_obj"]) if obj.get("group_obj") is not None else None,
-            "source": obj.get("source"),
+            "provider": obj.get("provider"),
             "attributes": obj.get("attributes")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scim_source_user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scope_mapping.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scope_mapping.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/scope_mapping_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/selectable_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/selectable_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_saml_source_connection_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ServiceConnectionRequest(BaseModel):
+class UserSAMLSourceConnectionRequest(BaseModel):
     """
-    ServiceConnection Serializer
+    SAML Source Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    local: Optional[StrictBool] = Field(default=None, description="If enabled, use the local connection. Required Docker socket/Kubernetes Integration")
-    __properties: ClassVar[List[str]] = ["name", "local"]
+    user: StrictInt
+    identifier: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["user", "identifier"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ServiceConnectionRequest from a JSON string"""
+        """Create an instance of UserSAMLSourceConnectionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ServiceConnectionRequest from a dict"""
+        """Create an instance of UserSAMLSourceConnectionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "local": obj.get("local")
+            "user": obj.get("user"),
+            "identifier": obj.get("identifier")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/service_connection_state.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/service_connection_state.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/session_user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/session_user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/settings.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/settings.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/settings_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/settings_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/severity_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/severity_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/shell_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/shell_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/signature_algorithm_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/sms_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/sms_device_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SMSDevice(BaseModel):
+class SMSDeviceRequest(BaseModel):
     """
     Serializer for sms authenticator devices
     """ # noqa: E501
-    name: Annotated[str, Field(strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
-    pk: StrictInt
-    phone_number: StrictStr
-    __properties: ClassVar[List[str]] = ["name", "pk", "phone_number"]
+    name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,51 +45,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SMSDevice from a JSON string"""
+        """Create an instance of SMSDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "pk",
-            "phone_number",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SMSDevice from a dict"""
+        """Create an instance of SMSDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "pk": obj.get("pk"),
-            "phone_number": obj.get("phone_number")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/sms_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/totp_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SMSDeviceRequest(BaseModel):
+class TOTPDeviceRequest(BaseModel):
     """
-    Serializer for sms authenticator devices
+    Serializer for totp authenticator devices
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
     __properties: ClassVar[List[str]] = ["name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SMSDeviceRequest from a JSON string"""
+        """Create an instance of TOTPDeviceRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SMSDeviceRequest from a dict"""
+        """Create an instance of TOTPDeviceRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/source.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/source.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/source_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/source_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/source_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/source_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/source_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/source_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/source_type.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/sp_binding_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/stage_prompt.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/stage_prompt.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_token.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StaticDeviceToken(BaseModel):
+class TenantAdminGroupRequestRequest(BaseModel):
     """
-    Serializer for static device's tokens
+    Tenant admin group creation request serializer
     """ # noqa: E501
-    token: Annotated[str, Field(strict=True, max_length=16)]
-    __properties: ClassVar[List[str]] = ["token"]
+    user: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["user"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StaticDeviceToken from a JSON string"""
+        """Create an instance of TenantAdminGroupRequestRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StaticDeviceToken from a dict"""
+        """Create an instance of TenantAdminGroupRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "token": obj.get("token")
+            "user": obj.get("user")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/static_device_token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/sub_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/sync_status.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/sync_status.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/system_info.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/system_info_runtime.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/system_task.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/system_task.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/system_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TenantAdminGroupRequestRequest(BaseModel):
+class TenantRecoveryKeyRequestRequest(BaseModel):
     """
-    Tenant admin group creation request serializer
+    Tenant recovery key creation request serializer
     """ # noqa: E501
     user: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["user"]
+    duration_days: StrictInt
+    __properties: ClassVar[List[str]] = ["user", "duration_days"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TenantAdminGroupRequestRequest from a JSON string"""
+        """Create an instance of TenantRecoveryKeyRequestRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TenantAdminGroupRequestRequest from a dict"""
+        """Create an instance of TenantRecoveryKeyRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user")
+            "user": obj.get("user"),
+            "duration_days": obj.get("duration_days")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/tenant_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictBool
+from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TenantRecoveryKeyRequestRequest(BaseModel):
+class TenantRequest(BaseModel):
     """
-    Tenant recovery key creation request serializer
+    Tenant Serializer
     """ # noqa: E501
-    user: Annotated[str, Field(min_length=1, strict=True)]
-    duration_days: StrictInt
-    __properties: ClassVar[List[str]] = ["user", "duration_days"]
+    schema_name: Annotated[str, Field(min_length=1, strict=True, max_length=63)]
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    ready: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["schema_name", "name", "ready"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TenantRecoveryKeyRequestRequest from a JSON string"""
+        """Create an instance of TenantRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +72,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TenantRecoveryKeyRequestRequest from a dict"""
+        """Create an instance of TenantRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user"),
-            "duration_days": obj.get("duration_days")
+            "schema_name": obj.get("schema_name"),
+            "name": obj.get("name"),
+            "ready": obj.get("ready")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_account_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TenantRecoveryKeyResponse(BaseModel):
+class UserAccountRequest(BaseModel):
     """
-    Tenant recovery key creation response serializer
+    Account adding/removing operations
     """ # noqa: E501
-    expiry: datetime
-    url: StrictStr
-    __properties: ClassVar[List[str]] = ["expiry", "url"]
+    pk: StrictInt
+    __properties: ClassVar[List[str]] = ["pk"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TenantRecoveryKeyResponse from a JSON string"""
+        """Create an instance of UserAccountRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TenantRecoveryKeyResponse from a dict"""
+        """Create an instance of UserAccountRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "expiry": obj.get("expiry"),
-            "url": obj.get("url")
+            "pk": obj.get("pk")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/tenant_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_o_auth_source_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
+from authentik_client.models.source import Source
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TenantRequest(BaseModel):
+class UserOAuthSourceConnection(BaseModel):
     """
-    Tenant Serializer
+    OAuth Source Serializer
     """ # noqa: E501
-    schema_name: Annotated[str, Field(min_length=1, strict=True, max_length=63)]
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    ready: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["schema_name", "name", "ready"]
+    pk: StrictInt
+    user: StrictInt
+    source: Source
+    identifier: Annotated[str, Field(strict=True, max_length=255)]
+    __properties: ClassVar[List[str]] = ["pk", "user", "source", "identifier"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,47 +49,55 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TenantRequest from a JSON string"""
+        """Create an instance of UserOAuthSourceConnection from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "pk",
+            "source",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of source
+        if self.source:
+            _dict['source'] = self.source.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TenantRequest from a dict"""
+        """Create an instance of UserOAuthSourceConnection from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "schema_name": obj.get("schema_name"),
-            "name": obj.get("name"),
-            "ready": obj.get("ready")
+            "pk": obj.get("pk"),
+            "user": obj.get("user"),
+            "source": Source.from_dict(obj["source"]) if obj.get("source") is not None else None,
+            "identifier": obj.get("identifier")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/token.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/token.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/token_model.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/token_model.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/token_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_password_set_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TokenSetKeyRequest(BaseModel):
+class UserPasswordSetRequest(BaseModel):
     """
-    TokenSetKeyRequest
+    UserPasswordSetRequest
     """ # noqa: E501
-    key: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["key"]
+    password: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["password"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TokenSetKeyRequest from a JSON string"""
+        """Create an instance of UserPasswordSetRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +70,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TokenSetKeyRequest from a dict"""
+        """Create an instance of UserPasswordSetRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "key": obj.get("key")
+            "password": obj.get("password")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/token_view.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TokenView(BaseModel):
+class UserPath(BaseModel):
     """
-    Show token's current key
+    UserPath
     """ # noqa: E501
-    key: StrictStr
-    __properties: ClassVar[List[str]] = ["key"]
+    paths: List[StrictStr]
+    __properties: ClassVar[List[str]] = ["paths"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,47 +44,47 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TokenView from a JSON string"""
+        """Create an instance of UserPath from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "key",
+            "paths",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TokenView from a dict"""
+        """Create an instance of UserPath from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "key": obj.get("key")
+            "paths": obj.get("paths")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/totp_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/totp_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/totp_device_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_logout_stage_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
+from authentik_client.models.flow_set_request import FlowSetRequest
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TOTPDeviceRequest(BaseModel):
+class UserLogoutStageRequest(BaseModel):
     """
-    Serializer for totp authenticator devices
+    UserLogoutStage Serializer
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True, max_length=64)] = Field(description="The human-readable name of this device.")
-    __properties: ClassVar[List[str]] = ["name"]
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    flow_set: Optional[List[FlowSetRequest]] = None
+    __properties: ClassVar[List[str]] = ["name", "flow_set"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TOTPDeviceRequest from a JSON string"""
+        """Create an instance of UserLogoutStageRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,24 +68,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in flow_set (list)
+        _items = []
+        if self.flow_set:
+            for _item in self.flow_set:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['flow_set'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TOTPDeviceRequest from a dict"""
+        """Create an instance of UserLogoutStageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "flow_set": [FlowSetRequest.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/transaction_application_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/transaction_application_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/type_create.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/type_create.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/ui_theme_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/used_by.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/used_by.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/used_by_action_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_account_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserAccountRequest(BaseModel):
+class WebAuthnDeviceType(BaseModel):
     """
-    Account adding/removing operations
+    WebAuthnDeviceType Serializer
     """ # noqa: E501
-    pk: StrictInt
-    __properties: ClassVar[List[str]] = ["pk"]
+    aaguid: StrictStr
+    description: StrictStr
+    __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserAccountRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceType from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserAccountRequest from a dict"""
+        """Create an instance of WebAuthnDeviceType from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pk": obj.get("pk")
+            "aaguid": obj.get("aaguid"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_assigned_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_consent.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_consent.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_creation_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_delete_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_delete_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_fields_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_group.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_group.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_group_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_group_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_challenge.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_challenge_response_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_login_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_logout_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_service_account_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from authentik_client.models.flow_set_request import FlowSetRequest
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserLogoutStageRequest(BaseModel):
+class UserServiceAccountRequest(BaseModel):
     """
-    UserLogoutStage Serializer
+    UserServiceAccountRequest
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)]
-    flow_set: Optional[List[FlowSetRequest]] = None
-    __properties: ClassVar[List[str]] = ["name", "flow_set"]
+    create_group: Optional[StrictBool] = False
+    expiring: Optional[StrictBool] = True
+    expires: Optional[datetime] = Field(default=None, description="If not provided, valid for 360 days")
+    __properties: ClassVar[List[str]] = ["name", "create_group", "expiring", "expires"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserLogoutStageRequest from a JSON string"""
+        """Create an instance of UserServiceAccountRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,32 +70,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in flow_set (list)
-        _items = []
-        if self.flow_set:
-            for _item in self.flow_set:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['flow_set'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserLogoutStageRequest from a dict"""
+        """Create an instance of UserServiceAccountRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "flow_set": [FlowSetRequest.from_dict(_item) for _item in obj["flow_set"]] if obj.get("flow_set") is not None else None
+            "create_group": obj.get("create_group") if obj.get("create_group") is not None else False,
+            "expiring": obj.get("expiring") if obj.get("expiring") is not None else True,
+            "expires": obj.get("expires")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_matching_mode_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_metrics.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_metrics.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_source_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
 from authentik_client.models.source import Source
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserOAuthSourceConnection(BaseModel):
+class UserSourceConnection(BaseModel):
     """
     OAuth Source Serializer
     """ # noqa: E501
     pk: StrictInt
     user: StrictInt
     source: Source
-    identifier: Annotated[str, Field(strict=True, max_length=255)]
-    __properties: ClassVar[List[str]] = ["pk", "user", "source", "identifier"]
+    created: datetime
+    __properties: ClassVar[List[str]] = ["pk", "user", "source", "created"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,55 +49,59 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserOAuthSourceConnection from a JSON string"""
+        """Create an instance of UserSourceConnection from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "pk",
+            "user",
             "source",
+            "created",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of source
         if self.source:
             _dict['source'] = self.source.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserOAuthSourceConnection from a dict"""
+        """Create an instance of UserSourceConnection from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pk": obj.get("pk"),
             "user": obj.get("user"),
             "source": Source.from_dict(obj["source"]) if obj.get("source") is not None else None,
-            "identifier": obj.get("identifier")
+            "created": obj.get("created")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_object_permission.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_object_permission.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device_type_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPasswordSetRequest(BaseModel):
+class WebAuthnDeviceTypeRequest(BaseModel):
     """
-    UserPasswordSetRequest
+    WebAuthnDeviceType Serializer
     """ # noqa: E501
-    password: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["password"]
+    aaguid: StrictStr
+    description: Annotated[str, Field(min_length=1, strict=True)]
+    __properties: ClassVar[List[str]] = ["aaguid", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPasswordSetRequest from a JSON string"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,20 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPasswordSetRequest from a dict"""
+        """Create an instance of WebAuthnDeviceTypeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "password": obj.get("password")
+            "aaguid": obj.get("aaguid"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_path.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/workers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPath(BaseModel):
+class Workers(BaseModel):
     """
-    UserPath
+    Workers
     """ # noqa: E501
-    paths: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["paths"]
+    count: StrictInt
+    __properties: ClassVar[List[str]] = ["count"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,47 +44,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPath from a JSON string"""
+        """Create an instance of Workers from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "paths",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPath from a dict"""
+        """Create an instance of Workers from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "paths": obj.get("paths")
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_saml_source_connection.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_service_account_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
-from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserSAMLSourceConnectionRequest(BaseModel):
+class UserServiceAccountResponse(BaseModel):
     """
-    SAML Source Serializer
+    UserServiceAccountResponse
     """ # noqa: E501
-    user: StrictInt
-    identifier: Annotated[str, Field(min_length=1, strict=True)]
-    __properties: ClassVar[List[str]] = ["user", "identifier"]
+    username: StrictStr
+    token: StrictStr
+    user_uid: StrictStr
+    user_pk: StrictInt
+    group_pk: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["username", "token", "user_uid", "user_pk", "group_pk"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserSAMLSourceConnectionRequest from a JSON string"""
+        """Create an instance of UserServiceAccountResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +73,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserSAMLSourceConnectionRequest from a dict"""
+        """Create an instance of UserServiceAccountResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "user": obj.get("user"),
-            "identifier": obj.get("identifier")
+            "username": obj.get("username"),
+            "token": obj.get("token"),
+            "user_uid": obj.get("user_uid"),
+            "user_pk": obj.get("user_pk"),
+            "group_pk": obj.get("group_pk")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_self.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_self.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_self_groups.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from authentik_client.models.group_member import GroupMember
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserSelfGroups(BaseModel):
+class GoogleWorkspaceProviderUser(BaseModel):
     """
-    UserSelfGroups
+    GoogleWorkspaceProviderUser Serializer
     """ # noqa: E501
-    name: StrictStr
-    pk: StrictStr
-    __properties: ClassVar[List[str]] = ["name", "pk"]
+    id: StrictStr
+    user: StrictInt
+    user_obj: GroupMember
+    provider: StrictInt
+    attributes: Optional[Any]
+    __properties: ClassVar[List[str]] = ["id", "user", "user_obj", "provider", "attributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,50 +49,63 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserSelfGroups from a JSON string"""
+        """Create an instance of GoogleWorkspaceProviderUser from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "name",
-            "pk",
+            "id",
+            "user_obj",
+            "attributes",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of user_obj
+        if self.user_obj:
+            _dict['user_obj'] = self.user_obj.to_dict()
+        # set to None if attributes (nullable) is None
+        # and model_fields_set contains the field
+        if self.attributes is None and "attributes" in self.model_fields_set:
+            _dict['attributes'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserSelfGroups from a dict"""
+        """Create an instance of GoogleWorkspaceProviderUser from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "pk": obj.get("pk")
+            "id": obj.get("id"),
+            "user": obj.get("user"),
+            "user_obj": GroupMember.from_dict(obj["user_obj"]) if obj.get("user_obj") is not None else None,
+            "provider": obj.get("provider"),
+            "attributes": obj.get("attributes")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_setting.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictBool
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserServiceAccountRequest(BaseModel):
+class UserSetting(BaseModel):
     """
-    UserServiceAccountRequest
+    Serializer for User settings for stages and sources
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    create_group: Optional[StrictBool] = False
-    expiring: Optional[StrictBool] = True
-    expires: Optional[datetime] = Field(default=None, description="If not provided, valid for 360 days")
-    __properties: ClassVar[List[str]] = ["name", "create_group", "expiring", "expires"]
+    object_uid: StrictStr
+    component: StrictStr
+    title: StrictStr
+    configure_url: Optional[StrictStr] = None
+    icon_url: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["object_uid", "component", "title", "configure_url", "icon_url"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserServiceAccountRequest from a JSON string"""
+        """Create an instance of UserSetting from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,23 +73,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserServiceAccountRequest from a dict"""
+        """Create an instance of UserSetting from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "create_group": obj.get("create_group") if obj.get("create_group") is not None else False,
-            "expiring": obj.get("expiring") if obj.get("expiring") is not None else True,
-            "expires": obj.get("expires")
+            "object_uid": obj.get("object_uid"),
+            "component": obj.get("component"),
+            "title": obj.get("title"),
+            "configure_url": obj.get("configure_url"),
+            "icon_url": obj.get("icon_url")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from authentik_client.models.user_group import UserGroup
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserServiceAccountResponse(BaseModel):
+class MicrosoftEntraProviderGroup(BaseModel):
     """
-    UserServiceAccountResponse
+    MicrosoftEntraProviderGroup Serializer
     """ # noqa: E501
-    username: StrictStr
-    token: StrictStr
-    user_uid: StrictStr
-    user_pk: StrictInt
-    group_pk: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["username", "token", "user_uid", "user_pk", "group_pk"]
+    id: StrictStr
+    group: StrictStr
+    group_obj: UserGroup
+    provider: StrictInt
+    attributes: Optional[Any]
+    __properties: ClassVar[List[str]] = ["id", "group", "group_obj", "provider", "attributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,49 +49,63 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserServiceAccountResponse from a JSON string"""
+        """Create an instance of MicrosoftEntraProviderGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "id",
+            "group_obj",
+            "attributes",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of group_obj
+        if self.group_obj:
+            _dict['group_obj'] = self.group_obj.to_dict()
+        # set to None if attributes (nullable) is None
+        # and model_fields_set contains the field
+        if self.attributes is None and "attributes" in self.model_fields_set:
+            _dict['attributes'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserServiceAccountResponse from a dict"""
+        """Create an instance of MicrosoftEntraProviderGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "username": obj.get("username"),
-            "token": obj.get("token"),
-            "user_uid": obj.get("user_uid"),
-            "user_pk": obj.get("user_pk"),
-            "group_pk": obj.get("group_pk")
+            "id": obj.get("id"),
+            "group": obj.get("group"),
+            "group_obj": UserGroup.from_dict(obj["group_obj"]) if obj.get("group_obj") is not None else None,
+            "provider": obj.get("provider"),
+            "attributes": obj.get("attributes")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_setting.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/google_workspace_provider_user_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, StrictInt
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserSetting(BaseModel):
+class GoogleWorkspaceProviderUserRequest(BaseModel):
     """
-    Serializer for User settings for stages and sources
+    GoogleWorkspaceProviderUser Serializer
     """ # noqa: E501
-    object_uid: StrictStr
-    component: StrictStr
-    title: StrictStr
-    configure_url: Optional[StrictStr] = None
-    icon_url: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["object_uid", "component", "title", "configure_url", "icon_url"]
+    user: StrictInt
+    provider: StrictInt
+    __properties: ClassVar[List[str]] = ["user", "provider"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserSetting from a JSON string"""
+        """Create an instance of GoogleWorkspaceProviderUserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,24 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserSetting from a dict"""
+        """Create an instance of GoogleWorkspaceProviderUserRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "object_uid": obj.get("object_uid"),
-            "component": obj.get("component"),
-            "title": obj.get("title"),
-            "configure_url": obj.get("configure_url"),
-            "icon_url": obj.get("icon_url")
+            "user": obj.get("user"),
+            "provider": obj.get("provider")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_source_connection.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/microsoft_entra_provider_user.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, StrictInt
-from typing import Any, ClassVar, Dict, List
-from authentik_client.models.source import Source
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from authentik_client.models.group_member import GroupMember
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserSourceConnection(BaseModel):
+class MicrosoftEntraProviderUser(BaseModel):
     """
-    OAuth Source Serializer
+    MicrosoftEntraProviderUser Serializer
     """ # noqa: E501
-    pk: StrictInt
+    id: StrictStr
     user: StrictInt
-    source: Source
-    created: datetime
-    __properties: ClassVar[List[str]] = ["pk", "user", "source", "created"]
+    user_obj: GroupMember
+    provider: StrictInt
+    attributes: Optional[Any]
+    __properties: ClassVar[List[str]] = ["id", "user", "user_obj", "provider", "attributes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,59 +49,63 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserSourceConnection from a JSON string"""
+        """Create an instance of MicrosoftEntraProviderUser from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "pk",
-            "user",
-            "source",
-            "created",
+            "id",
+            "user_obj",
+            "attributes",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of source
-        if self.source:
-            _dict['source'] = self.source.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of user_obj
+        if self.user_obj:
+            _dict['user_obj'] = self.user_obj.to_dict()
+        # set to None if attributes (nullable) is None
+        # and model_fields_set contains the field
+        if self.attributes is None and "attributes" in self.model_fields_set:
+            _dict['attributes'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserSourceConnection from a dict"""
+        """Create an instance of MicrosoftEntraProviderUser from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pk": obj.get("pk"),
+            "id": obj.get("id"),
             "user": obj.get("user"),
-            "source": Source.from_dict(obj["source"]) if obj.get("source") is not None else None,
-            "created": obj.get("created")
+            "user_obj": GroupMember.from_dict(obj["user_obj"]) if obj.get("user_obj") is not None else None,
+            "provider": obj.get("provider"),
+            "attributes": obj.get("attributes")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_type_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_type_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_verification_enum.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_write_stage.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_write_stage.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/user_write_stage_request.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/validation_error.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/version.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/version.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/models/web_authn_device.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/models/web_authn_device.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/authentik_client/rest.py` & `authentik_client-2024.4.2.post1717033274/authentik_client/rest.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.2.post1716550398/pyproject.toml` & `authentik_client-2024.4.2.post1717033274/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.4.2-1716550398"
+version = "2024.4.2-1717033274"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.4.2.post1716550398/PKG-INFO` & `authentik_client-2024.4.2.post1717033274/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.4.2.post1716550398
+Version: 2024.4.2.post1717033274
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -25,15 +25,15 @@
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2024.4.2
-- Package version: 2024.4.2-1716550398
+- Package version: 2024.4.2-1717033274
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -516,59 +516,51 @@
 *ProvidersApi* | [**providers_all_types_list**](docs/ProvidersApi.md#providers_all_types_list) | **GET** /providers/all/types/ | 
 *ProvidersApi* | [**providers_all_used_by_list**](docs/ProvidersApi.md#providers_all_used_by_list) | **GET** /providers/all/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_create**](docs/ProvidersApi.md#providers_google_workspace_create) | **POST** /providers/google_workspace/ | 
 *ProvidersApi* | [**providers_google_workspace_destroy**](docs/ProvidersApi.md#providers_google_workspace_destroy) | **DELETE** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_create**](docs/ProvidersApi.md#providers_google_workspace_groups_create) | **POST** /providers/google_workspace_groups/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_destroy**](docs/ProvidersApi.md#providers_google_workspace_groups_destroy) | **DELETE** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_list**](docs/ProvidersApi.md#providers_google_workspace_groups_list) | **GET** /providers/google_workspace_groups/ | 
-*ProvidersApi* | [**providers_google_workspace_groups_partial_update**](docs/ProvidersApi.md#providers_google_workspace_groups_partial_update) | **PATCH** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_retrieve**](docs/ProvidersApi.md#providers_google_workspace_groups_retrieve) | **GET** /providers/google_workspace_groups/{id}/ | 
-*ProvidersApi* | [**providers_google_workspace_groups_update**](docs/ProvidersApi.md#providers_google_workspace_groups_update) | **PUT** /providers/google_workspace_groups/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_groups_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_groups_used_by_list) | **GET** /providers/google_workspace_groups/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_list**](docs/ProvidersApi.md#providers_google_workspace_list) | **GET** /providers/google_workspace/ | 
 *ProvidersApi* | [**providers_google_workspace_partial_update**](docs/ProvidersApi.md#providers_google_workspace_partial_update) | **PATCH** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_retrieve**](docs/ProvidersApi.md#providers_google_workspace_retrieve) | **GET** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_sync_status_retrieve**](docs/ProvidersApi.md#providers_google_workspace_sync_status_retrieve) | **GET** /providers/google_workspace/{id}/sync/status/ | 
 *ProvidersApi* | [**providers_google_workspace_update**](docs/ProvidersApi.md#providers_google_workspace_update) | **PUT** /providers/google_workspace/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_used_by_list) | **GET** /providers/google_workspace/{id}/used_by/ | 
 *ProvidersApi* | [**providers_google_workspace_users_create**](docs/ProvidersApi.md#providers_google_workspace_users_create) | **POST** /providers/google_workspace_users/ | 
 *ProvidersApi* | [**providers_google_workspace_users_destroy**](docs/ProvidersApi.md#providers_google_workspace_users_destroy) | **DELETE** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_list**](docs/ProvidersApi.md#providers_google_workspace_users_list) | **GET** /providers/google_workspace_users/ | 
-*ProvidersApi* | [**providers_google_workspace_users_partial_update**](docs/ProvidersApi.md#providers_google_workspace_users_partial_update) | **PATCH** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_retrieve**](docs/ProvidersApi.md#providers_google_workspace_users_retrieve) | **GET** /providers/google_workspace_users/{id}/ | 
-*ProvidersApi* | [**providers_google_workspace_users_update**](docs/ProvidersApi.md#providers_google_workspace_users_update) | **PUT** /providers/google_workspace_users/{id}/ | 
 *ProvidersApi* | [**providers_google_workspace_users_used_by_list**](docs/ProvidersApi.md#providers_google_workspace_users_used_by_list) | **GET** /providers/google_workspace_users/{id}/used_by/ | 
 *ProvidersApi* | [**providers_ldap_create**](docs/ProvidersApi.md#providers_ldap_create) | **POST** /providers/ldap/ | 
 *ProvidersApi* | [**providers_ldap_destroy**](docs/ProvidersApi.md#providers_ldap_destroy) | **DELETE** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_list**](docs/ProvidersApi.md#providers_ldap_list) | **GET** /providers/ldap/ | 
 *ProvidersApi* | [**providers_ldap_partial_update**](docs/ProvidersApi.md#providers_ldap_partial_update) | **PATCH** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_retrieve**](docs/ProvidersApi.md#providers_ldap_retrieve) | **GET** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_update**](docs/ProvidersApi.md#providers_ldap_update) | **PUT** /providers/ldap/{id}/ | 
 *ProvidersApi* | [**providers_ldap_used_by_list**](docs/ProvidersApi.md#providers_ldap_used_by_list) | **GET** /providers/ldap/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_create**](docs/ProvidersApi.md#providers_microsoft_entra_create) | **POST** /providers/microsoft_entra/ | 
 *ProvidersApi* | [**providers_microsoft_entra_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_destroy) | **DELETE** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_create**](docs/ProvidersApi.md#providers_microsoft_entra_groups_create) | **POST** /providers/microsoft_entra_groups/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_groups_destroy) | **DELETE** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_list**](docs/ProvidersApi.md#providers_microsoft_entra_groups_list) | **GET** /providers/microsoft_entra_groups/ | 
-*ProvidersApi* | [**providers_microsoft_entra_groups_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_groups_partial_update) | **PATCH** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_groups_retrieve) | **GET** /providers/microsoft_entra_groups/{id}/ | 
-*ProvidersApi* | [**providers_microsoft_entra_groups_update**](docs/ProvidersApi.md#providers_microsoft_entra_groups_update) | **PUT** /providers/microsoft_entra_groups/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_groups_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_groups_used_by_list) | **GET** /providers/microsoft_entra_groups/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_list**](docs/ProvidersApi.md#providers_microsoft_entra_list) | **GET** /providers/microsoft_entra/ | 
 *ProvidersApi* | [**providers_microsoft_entra_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_partial_update) | **PATCH** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_retrieve) | **GET** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_sync_status_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_sync_status_retrieve) | **GET** /providers/microsoft_entra/{id}/sync/status/ | 
 *ProvidersApi* | [**providers_microsoft_entra_update**](docs/ProvidersApi.md#providers_microsoft_entra_update) | **PUT** /providers/microsoft_entra/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_used_by_list) | **GET** /providers/microsoft_entra/{id}/used_by/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_create**](docs/ProvidersApi.md#providers_microsoft_entra_users_create) | **POST** /providers/microsoft_entra_users/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_destroy**](docs/ProvidersApi.md#providers_microsoft_entra_users_destroy) | **DELETE** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_list**](docs/ProvidersApi.md#providers_microsoft_entra_users_list) | **GET** /providers/microsoft_entra_users/ | 
-*ProvidersApi* | [**providers_microsoft_entra_users_partial_update**](docs/ProvidersApi.md#providers_microsoft_entra_users_partial_update) | **PATCH** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_retrieve**](docs/ProvidersApi.md#providers_microsoft_entra_users_retrieve) | **GET** /providers/microsoft_entra_users/{id}/ | 
-*ProvidersApi* | [**providers_microsoft_entra_users_update**](docs/ProvidersApi.md#providers_microsoft_entra_users_update) | **PUT** /providers/microsoft_entra_users/{id}/ | 
 *ProvidersApi* | [**providers_microsoft_entra_users_used_by_list**](docs/ProvidersApi.md#providers_microsoft_entra_users_used_by_list) | **GET** /providers/microsoft_entra_users/{id}/used_by/ | 
 *ProvidersApi* | [**providers_oauth2_create**](docs/ProvidersApi.md#providers_oauth2_create) | **POST** /providers/oauth2/ | 
 *ProvidersApi* | [**providers_oauth2_destroy**](docs/ProvidersApi.md#providers_oauth2_destroy) | **DELETE** /providers/oauth2/{id}/ | 
 *ProvidersApi* | [**providers_oauth2_list**](docs/ProvidersApi.md#providers_oauth2_list) | **GET** /providers/oauth2/ | 
 *ProvidersApi* | [**providers_oauth2_partial_update**](docs/ProvidersApi.md#providers_oauth2_partial_update) | **PATCH** /providers/oauth2/{id}/ | 
 *ProvidersApi* | [**providers_oauth2_preview_user_retrieve**](docs/ProvidersApi.md#providers_oauth2_preview_user_retrieve) | **GET** /providers/oauth2/{id}/preview_user/ | 
 *ProvidersApi* | [**providers_oauth2_retrieve**](docs/ProvidersApi.md#providers_oauth2_retrieve) | **GET** /providers/oauth2/{id}/ | 
@@ -1287,31 +1279,27 @@
  - [PatchedEmailStageRequest](docs/PatchedEmailStageRequest.md)
  - [PatchedEndpointRequest](docs/PatchedEndpointRequest.md)
  - [PatchedEventMatcherPolicyRequest](docs/PatchedEventMatcherPolicyRequest.md)
  - [PatchedEventRequest](docs/PatchedEventRequest.md)
  - [PatchedExpressionPolicyRequest](docs/PatchedExpressionPolicyRequest.md)
  - [PatchedFlowRequest](docs/PatchedFlowRequest.md)
  - [PatchedFlowStageBindingRequest](docs/PatchedFlowStageBindingRequest.md)
- - [PatchedGoogleWorkspaceProviderGroupRequest](docs/PatchedGoogleWorkspaceProviderGroupRequest.md)
  - [PatchedGoogleWorkspaceProviderMappingRequest](docs/PatchedGoogleWorkspaceProviderMappingRequest.md)
  - [PatchedGoogleWorkspaceProviderRequest](docs/PatchedGoogleWorkspaceProviderRequest.md)
- - [PatchedGoogleWorkspaceProviderUserRequest](docs/PatchedGoogleWorkspaceProviderUserRequest.md)
  - [PatchedGroupRequest](docs/PatchedGroupRequest.md)
  - [PatchedIdentificationStageRequest](docs/PatchedIdentificationStageRequest.md)
  - [PatchedInvitationRequest](docs/PatchedInvitationRequest.md)
  - [PatchedInvitationStageRequest](docs/PatchedInvitationStageRequest.md)
  - [PatchedKubernetesServiceConnectionRequest](docs/PatchedKubernetesServiceConnectionRequest.md)
  - [PatchedLDAPPropertyMappingRequest](docs/PatchedLDAPPropertyMappingRequest.md)
  - [PatchedLDAPProviderRequest](docs/PatchedLDAPProviderRequest.md)
  - [PatchedLDAPSourceRequest](docs/PatchedLDAPSourceRequest.md)
  - [PatchedLicenseRequest](docs/PatchedLicenseRequest.md)
- - [PatchedMicrosoftEntraProviderGroupRequest](docs/PatchedMicrosoftEntraProviderGroupRequest.md)
  - [PatchedMicrosoftEntraProviderMappingRequest](docs/PatchedMicrosoftEntraProviderMappingRequest.md)
  - [PatchedMicrosoftEntraProviderRequest](docs/PatchedMicrosoftEntraProviderRequest.md)
- - [PatchedMicrosoftEntraProviderUserRequest](docs/PatchedMicrosoftEntraProviderUserRequest.md)
  - [PatchedNotificationRequest](docs/PatchedNotificationRequest.md)
  - [PatchedNotificationRuleRequest](docs/PatchedNotificationRuleRequest.md)
  - [PatchedNotificationTransportRequest](docs/PatchedNotificationTransportRequest.md)
  - [PatchedNotificationWebhookMappingRequest](docs/PatchedNotificationWebhookMappingRequest.md)
  - [PatchedOAuth2ProviderRequest](docs/PatchedOAuth2ProviderRequest.md)
  - [PatchedOAuthSourceRequest](docs/PatchedOAuthSourceRequest.md)
  - [PatchedOutpostRequest](docs/PatchedOutpostRequest.md)
```

