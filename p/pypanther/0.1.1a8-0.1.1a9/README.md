# Comparing `tmp/pypanther-0.1.1a8.tar.gz` & `tmp/pypanther-0.1.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypanther-0.1.1a8.tar", max compression
+gzip compressed data, was "pypanther-0.1.1a9.tar", max compression
```

## Comparing `pypanther-0.1.1a8.tar` & `pypanther-0.1.1a9.tar`

### file list

```diff
@@ -1,566 +1,566 @@
--rw-r--r--   0        0        0    34523 2024-05-22 19:16:21.930547 pypanther-0.1.1a8/LICENSE.txt
--rw-r--r--   0        0        0       80 2024-05-03 18:47:26.705553 pypanther-0.1.1a8/README.md
--rw-r--r--   0        0        0      185 2024-05-23 22:00:33.237693 pypanther-0.1.1a8/pypanther/__init__.py
--rw-r--r--   0        0        0    24670 2024-05-28 19:11:58.339442 pypanther-0.1.1a8/pypanther/base.py
--rw-r--r--   0        0        0      490 2024-05-23 22:00:33.238107 pypanther-0.1.1a8/pypanther/cache.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:14.952849 pypanther-0.1.1a8/pypanther/data_models/__init__.py
--rw-r--r--   0        0        0     1387 2024-05-24 12:40:14.944512 pypanther-0.1.1a8/pypanther/data_models/asana_data_model.py
--rw-r--r--   0        0        0     1544 2024-05-24 12:40:14.933036 pypanther-0.1.1a8/pypanther/data_models/atlassian_data_model.py
--rw-r--r--   0        0        0      607 2024-05-24 12:40:14.942246 pypanther-0.1.1a8/pypanther/data_models/aws_alb_data_model.py
--rw-r--r--   0        0        0     2214 2024-05-24 12:40:14.938734 pypanther-0.1.1a8/pypanther/data_models/aws_cloudtrail_data_model.py
--rw-r--r--   0        0        0     1465 2024-05-24 12:40:14.929894 pypanther-0.1.1a8/pypanther/data_models/aws_eks_data_model.py
--rw-r--r--   0        0        0      630 2024-05-24 12:40:14.936327 pypanther-0.1.1a8/pypanther/data_models/aws_s3_data_model.py
--rw-r--r--   0        0        0      593 2024-05-24 12:40:14.939270 pypanther-0.1.1a8/pypanther/data_models/aws_vpcdns_data_model.py
--rw-r--r--   0        0        0      742 2024-05-24 12:40:14.928634 pypanther-0.1.1a8/pypanther/data_models/aws_vpcflow_data_model.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.927521 pypanther-0.1.1a8/pypanther/data_models/azure_signin_data_model.py
--rw-r--r--   0        0        0      941 2024-05-24 12:40:14.941146 pypanther-0.1.1a8/pypanther/data_models/box_data_model.py
--rw-r--r--   0        0        0      873 2024-05-24 12:40:14.939822 pypanther-0.1.1a8/pypanther/data_models/cisco_umbrella_data_model.py
--rw-r--r--   0        0        0      653 2024-05-24 12:40:14.943897 pypanther-0.1.1a8/pypanther/data_models/cloudflare_firewall_data_model.py
--rw-r--r--   0        0        0      729 2024-05-24 12:40:14.928057 pypanther-0.1.1a8/pypanther/data_models/cloudflare_httpreq_data_model.py
--rw-r--r--   0        0        0     1853 2024-05-24 12:40:14.943403 pypanther-0.1.1a8/pypanther/data_models/crowdstrike_fdr_data_model.py
--rw-r--r--   0        0        0     5215 2024-05-24 12:40:14.934292 pypanther-0.1.1a8/pypanther/data_models/gcp_data_model.py
--rw-r--r--   0        0        0     1613 2024-05-24 12:40:14.937900 pypanther-0.1.1a8/pypanther/data_models/github_data_model.py
--rw-r--r--   0        0        0     1669 2024-05-24 12:40:14.935584 pypanther-0.1.1a8/pypanther/data_models/gsuite_data_model.py
--rw-r--r--   0        0        0     1864 2024-05-24 12:40:14.940562 pypanther-0.1.1a8/pypanther/data_models/notion_data_model.py
--rw-r--r--   0        0        0     2070 2024-05-24 12:40:14.937166 pypanther-0.1.1a8/pypanther/data_models/okta_data_model.py
--rw-r--r--   0        0        0     1467 2024-05-24 12:40:14.932330 pypanther-0.1.1a8/pypanther/data_models/onelogin_data_model.py
--rw-r--r--   0        0        0      730 2024-05-24 12:40:14.934876 pypanther-0.1.1a8/pypanther/data_models/onepassword_itemusage_data_model.py
--rw-r--r--   0        0        0     1058 2024-05-24 12:40:14.941731 pypanther-0.1.1a8/pypanther/data_models/onepassword_signinattempt_data_model.py
--rw-r--r--   0        0        0     1742 2024-05-24 12:40:14.930685 pypanther-0.1.1a8/pypanther/data_models/panther_audit_data_model.py
--rw-r--r--   0        0        0      613 2024-05-24 12:40:14.929135 pypanther-0.1.1a8/pypanther/data_models/slack_accesslogs_data_model.py
--rw-r--r--   0        0        0      711 2024-05-24 12:40:14.942793 pypanther-0.1.1a8/pypanther/data_models/slack_auditlogs_data_model.py
--rw-r--r--   0        0        0      500 2024-05-24 12:40:14.926474 pypanther-0.1.1a8/pypanther/data_models/slack_integrationlogs_data_model.py
--rw-r--r--   0        0        0     2714 2024-05-24 12:40:14.931651 pypanther-0.1.1a8/pypanther/data_models/zendesk_data_model.py
--rw-r--r--   0        0        0      886 2024-05-24 12:40:14.926019 pypanther-0.1.1a8/pypanther/data_models/zoom_activity_data_model.py
--rw-r--r--   0        0        0     1887 2024-05-24 12:40:14.925345 pypanther-0.1.1a8/pypanther/data_models/zoom_operation_data_model.py
--rw-r--r--   0        0        0     2682 2024-05-23 22:00:33.243958 pypanther-0.1.1a8/pypanther/get.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:13.778915 pypanther-0.1.1a8/pypanther/helpers/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-24 12:40:14.169513 pypanther-0.1.1a8/pypanther/helpers/gcp_base_helpers.py
--rw-r--r--   0        0        0      781 2024-05-24 12:40:14.303335 pypanther-0.1.1a8/pypanther/helpers/gcp_environment.py
--rw-r--r--   0        0        0     1417 2024-05-24 12:40:13.948393 pypanther-0.1.1a8/pypanther/helpers/panther_asana_helpers.py
--rw-r--r--   0        0        0     1597 2024-05-24 12:40:14.156772 pypanther-0.1.1a8/pypanther/helpers/panther_audit.py
--rw-r--r--   0        0        0      555 2024-05-24 12:40:13.952837 pypanther-0.1.1a8/pypanther/helpers/panther_auth0_helpers.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.099017 pypanther-0.1.1a8/pypanther/helpers/panther_azuresignin_helpers.py
--rw-r--r--   0        0        0    19692 2024-05-24 12:40:14.264799 pypanther-0.1.1a8/pypanther/helpers/panther_base_helpers.py
--rw-r--r--   0        0        0     4529 2024-05-24 12:40:14.146111 pypanther-0.1.1a8/pypanther/helpers/panther_box_helpers.py
--rw-r--r--   0        0        0     2267 2024-05-24 12:40:13.916642 pypanther-0.1.1a8/pypanther/helpers/panther_cloudflare_helpers.py
--rw-r--r--   0        0        0      507 2024-05-24 12:40:14.148779 pypanther-0.1.1a8/pypanther/helpers/panther_config.py
--rw-r--r--   0        0        0      891 2024-05-24 12:40:14.103142 pypanther-0.1.1a8/pypanther/helpers/panther_config_defaults.py
--rw-r--r--   0        0        0     1043 2024-05-24 12:40:13.795713 pypanther-0.1.1a8/pypanther/helpers/panther_config_overrides.py
--rw-r--r--   0        0        0     3465 2024-05-24 12:40:13.831736 pypanther-0.1.1a8/pypanther/helpers/panther_default.py
--rw-r--r--   0        0        0     1288 2024-05-24 12:40:13.811022 pypanther-0.1.1a8/pypanther/helpers/panther_duo_helpers.py
--rw-r--r--   0        0        0     1118 2024-05-24 12:40:14.384435 pypanther-0.1.1a8/pypanther/helpers/panther_event_type_helpers.py
--rw-r--r--   0        0        0    12436 2024-05-24 12:40:14.482779 pypanther-0.1.1a8/pypanther/helpers/panther_greynoise_helpers.py
--rw-r--r--   0        0        0    38305 2024-05-24 12:40:13.902461 pypanther-0.1.1a8/pypanther/helpers/panther_iocs.py
--rw-r--r--   0        0        0     6497 2024-05-24 12:40:14.002454 pypanther-0.1.1a8/pypanther/helpers/panther_ipinfo_helpers.py
--rw-r--r--   0        0        0     2154 2024-05-24 12:40:14.015836 pypanther-0.1.1a8/pypanther/helpers/panther_lookuptable_helpers.py
--rw-r--r--   0        0        0      387 2024-05-24 12:40:14.270284 pypanther-0.1.1a8/pypanther/helpers/panther_mongodb_helpers.py
--rw-r--r--   0        0        0      340 2024-05-24 12:40:13.834434 pypanther-0.1.1a8/pypanther/helpers/panther_notion_helpers.py
--rw-r--r--   0        0        0    13096 2024-05-24 12:40:14.370655 pypanther-0.1.1a8/pypanther/helpers/panther_oss_helpers.py
--rw-r--r--   0        0        0      610 2024-05-24 12:40:13.801982 pypanther-0.1.1a8/pypanther/helpers/panther_snyk_helpers.py
--rw-r--r--   0        0        0      492 2024-05-24 12:40:14.307780 pypanther-0.1.1a8/pypanther/helpers/panther_tailscale_helpers.py
--rw-r--r--   0        0        0      567 2024-05-24 12:40:14.312664 pypanther-0.1.1a8/pypanther/helpers/panther_tines_helpers.py
--rw-r--r--   0        0        0     1542 2024-05-24 12:40:14.379643 pypanther-0.1.1a8/pypanther/helpers/panther_tor_helpers.py
--rw-r--r--   0        0        0     3084 2024-05-24 12:40:13.935600 pypanther-0.1.1a8/pypanther/helpers/panther_zoom_helpers.py
--rw-r--r--   0        0        0    13022 2024-05-23 22:06:29.350498 pypanther-0.1.1a8/pypanther/log_types.py
--rw-r--r--   0        0        0     1134 2024-05-28 18:40:51.829160 pypanther-0.1.1a8/pypanther/main.py
--rw-r--r--   0        0        0        0 2024-05-28 18:40:51.829203 pypanther-0.1.1a8/pypanther/py.typed
--rw-r--r--   0        0        0      824 2024-05-23 22:00:33.250813 pypanther-0.1.1a8/pypanther/register.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.351956 pypanther-0.1.1a8/pypanther/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356408 pypanther-0.1.1a8/pypanther/rules/asana_rules/__init__.py
--rw-r--r--   0        0        0     4069 2024-05-28 19:11:58.340050 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_service_account_created.py
--rw-r--r--   0        0        0     3241 2024-05-28 19:11:58.340466 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_team_privacy_public.py
--rw-r--r--   0        0        0     3263 2024-05-28 19:11:58.340767 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
--rw-r--r--   0        0        0     3232 2024-05-28 19:11:58.341082 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
--rw-r--r--   0        0        0     3420 2024-05-28 19:11:58.341520 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
--rw-r--r--   0        0        0     3399 2024-05-28 19:11:58.341677 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
--rw-r--r--   0        0        0     3747 2024-05-28 19:11:58.342105 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_new_admin.py
--rw-r--r--   0        0        0     3242 2024-05-28 19:11:58.342563 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_org_export.py
--rw-r--r--   0        0        0     3725 2024-05-28 19:11:58.342710 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
--rw-r--r--   0        0        0     3629 2024-05-28 19:11:58.342855 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
--rw-r--r--   0        0        0     3498 2024-05-28 19:11:58.343001 pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355786 pypanther-0.1.1a8/pypanther/rules/atlassian_rules/__init__.py
--rw-r--r--   0        0        0     4891 2024-05-28 19:11:58.343684 pypanther-0.1.1a8/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352374 pypanther-0.1.1a8/pypanther/rules/auth0_rules/__init__.py
--rw-r--r--   0        0        0    45000 2024-05-28 19:11:58.344253 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_custom_role_created.py
--rw-r--r--   0        0        0    15426 2024-05-28 19:11:58.344617 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_integration_installed.py
--rw-r--r--   0        0        0    23152 2024-05-28 19:11:58.344806 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
--rw-r--r--   0        0        0    23502 2024-05-28 19:11:58.345555 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
--rw-r--r--   0        0        0    34173 2024-05-28 19:11:58.345780 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
--rw-r--r--   0        0        0    23656 2024-05-28 19:11:58.346271 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
--rw-r--r--   0        0        0    22677 2024-05-28 19:11:58.346886 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
--rw-r--r--   0        0        0    19831 2024-05-28 19:11:58.347527 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
--rw-r--r--   0        0        0    17293 2024-05-28 19:11:58.347839 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
--rw-r--r--   0        0        0    18180 2024-05-28 19:11:58.348413 pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354895 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/__init__.py
--rw-r--r--   0        0        0    11023 2024-05-28 19:11:58.349277 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
--rw-r--r--   0        0        0     8203 2024-05-28 19:11:58.349480 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
--rw-r--r--   0        0        0     7052 2024-05-28 19:11:58.349705 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
--rw-r--r--   0        0        0     3387 2024-05-28 19:11:58.349922 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
--rw-r--r--   0        0        0     7226 2024-05-28 19:11:58.350335 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
--rw-r--r--   0        0        0     4474 2024-05-28 19:11:58.350937 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
--rw-r--r--   0        0        0     7006 2024-05-28 19:11:58.351155 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
--rw-r--r--   0        0        0     6565 2024-05-28 19:11:58.351374 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
--rw-r--r--   0        0        0     6552 2024-05-28 19:11:58.351972 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
--rw-r--r--   0        0        0    20565 2024-05-28 19:11:58.352382 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
--rw-r--r--   0        0        0     4041 2024-05-28 19:11:58.352970 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
--rw-r--r--   0        0        0     5610 2024-05-28 19:11:58.353229 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
--rw-r--r--   0        0        0     5713 2024-05-28 19:11:58.353455 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
--rw-r--r--   0        0        0     2295 2024-05-28 19:11:58.353621 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
--rw-r--r--   0        0        0     6726 2024-05-28 19:11:58.354018 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
--rw-r--r--   0        0        0    17207 2024-05-28 19:11:58.354349 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
--rw-r--r--   0        0        0    22420 2024-05-28 19:11:58.354703 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
--rw-r--r--   0        0        0     7258 2024-05-28 19:11:58.354938 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
--rw-r--r--   0        0        0     6888 2024-05-28 19:11:58.355449 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
--rw-r--r--   0        0        0     8185 2024-05-28 19:11:58.355672 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
--rw-r--r--   0        0        0     5173 2024-05-28 19:11:58.355869 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
--rw-r--r--   0        0        0    30283 2024-05-28 19:11:58.356080 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
--rw-r--r--   0        0        0     8614 2024-05-28 19:11:58.356309 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
--rw-r--r--   0        0        0    39743 2024-05-28 19:11:58.356657 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
--rw-r--r--   0        0        0    27333 2024-05-28 19:11:58.357147 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
--rw-r--r--   0        0        0    26742 2024-05-28 19:11:58.357329 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
--rw-r--r--   0        0        0     7276 2024-05-28 19:11:58.357539 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
--rw-r--r--   0        0        0     8595 2024-05-28 19:11:58.357722 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
--rw-r--r--   0        0        0     6119 2024-05-28 19:11:58.358232 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
--rw-r--r--   0        0        0    12719 2024-05-28 19:11:58.358560 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
--rw-r--r--   0        0        0    13763 2024-05-28 19:11:58.358785 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
--rw-r--r--   0        0        0     7154 2024-05-28 19:11:58.358990 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
--rw-r--r--   0        0        0    10491 2024-05-28 19:11:58.359146 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
--rw-r--r--   0        0        0     9050 2024-05-28 19:11:58.359334 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
--rw-r--r--   0        0        0     3389 2024-05-28 19:11:58.359556 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
--rw-r--r--   0        0        0     5216 2024-05-28 19:11:58.359740 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
--rw-r--r--   0        0        0    11264 2024-05-28 19:11:58.360006 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
--rw-r--r--   0        0        0     5730 2024-05-28 19:11:58.360189 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
--rw-r--r--   0        0        0     9734 2024-05-28 19:11:58.360403 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
--rw-r--r--   0        0        0    27000 2024-05-28 19:11:58.360729 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
--rw-r--r--   0        0        0     7827 2024-05-28 19:11:58.360968 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
--rw-r--r--   0        0        0    16376 2024-05-28 19:11:58.361181 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
--rw-r--r--   0        0        0    14639 2024-05-28 19:11:58.361366 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
--rw-r--r--   0        0        0    17400 2024-05-28 19:11:58.361535 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
--rw-r--r--   0        0        0     7480 2024-05-28 19:11:58.361741 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
--rw-r--r--   0        0        0    18982 2024-05-28 19:11:58.361903 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
--rw-r--r--   0        0        0     4669 2024-05-28 19:11:58.362111 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
--rw-r--r--   0        0        0    10753 2024-05-28 19:11:58.362414 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
--rw-r--r--   0        0        0     3934 2024-05-28 19:11:58.362563 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
--rw-r--r--   0        0        0     5825 2024-05-28 19:11:58.362754 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
--rw-r--r--   0        0        0     7516 2024-05-28 19:11:58.362968 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
--rw-r--r--   0        0        0    12289 2024-05-28 19:11:58.363162 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
--rw-r--r--   0        0        0    11516 2024-05-28 19:11:58.363357 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
--rw-r--r--   0        0        0     5570 2024-05-28 19:11:58.363567 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
--rw-r--r--   0        0        0     7558 2024-05-28 19:11:58.363804 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
--rw-r--r--   0        0        0     5191 2024-05-28 19:11:58.364017 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
--rw-r--r--   0        0        0     6478 2024-05-28 19:11:58.364344 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
--rw-r--r--   0        0        0     8697 2024-05-28 19:11:58.364595 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
--rw-r--r--   0        0        0     5976 2024-05-28 19:11:58.364841 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
--rw-r--r--   0        0        0     6782 2024-05-28 19:11:58.365067 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
--rw-r--r--   0        0        0     7024 2024-05-28 19:11:58.365361 pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352785 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/__init__.py
--rw-r--r--   0        0        0     9700 2024-05-28 19:11:58.365585 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
--rw-r--r--   0        0        0    17813 2024-05-28 19:11:58.365877 pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354748 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/__init__.py
--rw-r--r--   0        0        0     5370 2024-05-28 19:11:58.366101 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
--rw-r--r--   0        0        0     5391 2024-05-28 19:11:58.366424 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
--rw-r--r--   0        0        0     5417 2024-05-28 19:11:58.366618 pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355307 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/__init__.py
--rw-r--r--   0        0        0     4702 2024-05-28 19:11:58.366952 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
--rw-r--r--   0        0        0     2560 2024-05-28 19:11:58.367226 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
--rw-r--r--   0        0        0     6277 2024-05-28 19:11:58.367425 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
--rw-r--r--   0        0        0     1997 2024-05-28 19:11:58.367601 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
--rw-r--r--   0        0        0     8748 2024-05-28 19:11:58.367853 pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355429 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/__init__.py
--rw-r--r--   0        0        0     6790 2024-05-28 19:11:58.368287 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
--rw-r--r--   0        0        0     1340 2024-05-28 19:11:58.368494 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
--rw-r--r--   0        0        0     2538 2024-05-28 19:11:58.368664 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
--rw-r--r--   0        0        0     2498 2024-05-28 19:11:58.368815 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
--rw-r--r--   0        0        0     2927 2024-05-28 19:11:58.368969 pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355171 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/__init__.py
--rw-r--r--   0        0        0     7978 2024-05-28 19:11:58.369185 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_failed_signins.py
--rw-r--r--   0        0        0    15766 2024-05-28 19:11:58.369374 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_legacyauth.py
--rw-r--r--   0        0        0    17553 2024-05-28 19:11:58.369593 pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353050 pypanther-0.1.1a8/pypanther/rules/box_rules/__init__.py
--rw-r--r--   0        0        0     2134 2024-05-28 19:11:58.369784 pypanther-0.1.1a8/pypanther/rules/box_rules/box_access_granted.py
--rw-r--r--   0        0        0     2869 2024-05-28 19:11:58.369971 pypanther-0.1.1a8/pypanther/rules/box_rules/box_anomalous_download.py
--rw-r--r--   0        0        0     2744 2024-05-28 19:11:58.370506 pypanther-0.1.1a8/pypanther/rules/box_rules/box_event_triggered_externally.py
--rw-r--r--   0        0        0     3652 2024-05-28 19:11:58.370679 pypanther-0.1.1a8/pypanther/rules/box_rules/box_item_shared_externally.py
--rw-r--r--   0        0        0     4266 2024-05-28 19:11:58.371060 pypanther-0.1.1a8/pypanther/rules/box_rules/box_malicious_content.py
--rw-r--r--   0        0        0     2124 2024-05-28 19:11:58.371239 pypanther-0.1.1a8/pypanther/rules/box_rules/box_new_login.py
--rw-r--r--   0        0        0     2822 2024-05-28 19:11:58.371408 pypanther-0.1.1a8/pypanther/rules/box_rules/box_policy_violation.py
--rw-r--r--   0        0        0     4215 2024-05-28 19:11:58.371707 pypanther-0.1.1a8/pypanther/rules/box_rules/box_suspicious_login_or_session.py
--rw-r--r--   0        0        0     2226 2024-05-28 19:11:58.371941 pypanther-0.1.1a8/pypanther/rules/box_rules/box_untrusted_device.py
--rw-r--r--   0        0        0     2366 2024-05-28 19:11:58.372118 pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_downloads.py
--rw-r--r--   0        0        0     3179 2024-05-28 19:11:58.372430 pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_permission_updates.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355655 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/__init__.py
--rw-r--r--   0        0        0     3313 2024-05-28 19:11:58.372652 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
--rw-r--r--   0        0        0     3037 2024-05-28 19:11:58.372849 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
--rw-r--r--   0        0        0     3487 2024-05-28 19:11:58.373044 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
--rw-r--r--   0        0        0     2262 2024-05-28 19:11:58.373233 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
--rw-r--r--   0        0        0     2591 2024-05-28 19:11:58.373422 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
--rw-r--r--   0        0        0    11317 2024-05-28 19:11:58.373640 pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355556 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
--rw-r--r--   0        0        0     1801 2024-05-28 19:11:58.373825 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
--rw-r--r--   0        0        0     1428 2024-05-28 19:11:58.374022 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
--rw-r--r--   0        0        0     1917 2024-05-28 19:11:58.374212 pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354017 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/__init__.py
--rw-r--r--   0        0        0     4983 2024-05-28 19:11:58.374471 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
--rw-r--r--   0        0        0     7577 2024-05-28 19:11:58.374729 pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355030 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/__init__.py
--rw-r--r--   0        0        0    29399 2024-05-28 19:11:58.374939 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
--rw-r--r--   0        0        0     8191 2024-05-28 19:11:58.375218 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
--rw-r--r--   0        0        0     9907 2024-05-28 19:11:58.375469 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
--rw-r--r--   0        0        0     9869 2024-05-28 19:11:58.375719 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
--rw-r--r--   0        0        0    10434 2024-05-28 19:11:58.376157 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
--rw-r--r--   0        0        0    12191 2024-05-28 19:11:58.376404 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
--rw-r--r--   0        0        0    11725 2024-05-28 19:11:58.376639 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
--rw-r--r--   0        0        0    18694 2024-05-28 19:11:58.376794 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
--rw-r--r--   0        0        0    18901 2024-05-28 19:11:58.376982 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
--rw-r--r--   0        0        0    15628 2024-05-28 19:11:58.377171 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
--rw-r--r--   0        0        0     7222 2024-05-28 19:11:58.377382 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
--rw-r--r--   0        0        0     9736 2024-05-28 19:11:58.377566 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
--rw-r--r--   0        0        0    13608 2024-05-28 19:11:58.377757 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
--rw-r--r--   0        0        0     9717 2024-05-28 19:11:58.377927 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
--rw-r--r--   0        0        0    10020 2024-05-28 19:11:58.378100 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
--rw-r--r--   0        0        0    17371 2024-05-28 19:11:58.378268 pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354190 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/__init__.py
--rw-r--r--   0        0        0     6807 2024-05-28 19:11:58.378520 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
--rw-r--r--   0        0        0     9508 2024-05-28 19:11:58.378771 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_external_share.py
--rw-r--r--   0        0        0     8252 2024-05-28 19:11:58.379036 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
--rw-r--r--   0        0        0    11156 2024-05-28 19:11:58.379219 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
--rw-r--r--   0        0        0     5145 2024-05-28 19:11:58.379541 pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353471 pypanther-0.1.1a8/pypanther/rules/duo_rules/__init__.py
--rw-r--r--   0        0        0     2102 2024-05-28 19:11:58.379913 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
--rw-r--r--   0        0        0     2189 2024-05-28 19:11:58.380116 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
--rw-r--r--   0        0        0     2258 2024-05-28 19:11:58.380276 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
--rw-r--r--   0        0        0     2255 2024-05-28 19:11:58.380442 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_create_admin.py
--rw-r--r--   0        0        0     2522 2024-05-28 19:11:58.380597 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_lockout.py
--rw-r--r--   0        0        0     2672 2024-05-28 19:11:58.380740 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
--rw-r--r--   0        0        0     1982 2024-05-28 19:11:58.380887 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
--rw-r--r--   0        0        0     3158 2024-05-28 19:11:58.381045 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
--rw-r--r--   0        0        0     2222 2024-05-28 19:11:58.381189 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_policy_updated.py
--rw-r--r--   0        0        0     3390 2024-05-28 19:11:58.381334 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
--rw-r--r--   0        0        0     2916 2024-05-28 19:11:58.381485 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
--rw-r--r--   0        0        0     2042 2024-05-28 19:11:58.381623 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
--rw-r--r--   0        0        0     3166 2024-05-28 19:11:58.381800 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_anomalous_push.py
--rw-r--r--   0        0        0     3072 2024-05-28 19:11:58.381953 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
--rw-r--r--   0        0        0     5464 2024-05-28 19:11:58.382162 pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353698 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/__init__.py
--rw-r--r--   0        0        0     9853 2024-05-28 19:11:58.382382 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
--rw-r--r--   0        0        0    12347 2024-05-28 19:11:58.382595 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
--rw-r--r--   0        0        0     7059 2024-05-28 19:11:58.382832 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
--rw-r--r--   0        0        0     7853 2024-05-28 19:11:58.383041 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
--rw-r--r--   0        0        0     4141 2024-05-28 19:11:58.383240 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
--rw-r--r--   0        0        0     4141 2024-05-28 19:11:58.383531 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
--rw-r--r--   0        0        0    19142 2024-05-28 19:11:58.383866 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
--rw-r--r--   0        0        0    10446 2024-05-28 19:11:58.384113 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
--rw-r--r--   0        0        0    15447 2024-05-28 19:11:58.384321 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
--rw-r--r--   0        0        0     9163 2024-05-28 19:11:58.384509 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
--rw-r--r--   0        0        0     6832 2024-05-28 19:11:58.384716 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
--rw-r--r--   0        0        0     8955 2024-05-28 19:11:58.384901 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
--rw-r--r--   0        0        0     3845 2024-05-28 19:11:58.385062 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
--rw-r--r--   0        0        0     4541 2024-05-28 19:11:58.385247 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
--rw-r--r--   0        0        0    15807 2024-05-28 19:11:58.385445 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
--rw-r--r--   0        0        0     5283 2024-05-28 19:11:58.385683 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
--rw-r--r--   0        0        0     9955 2024-05-28 19:11:58.385873 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
--rw-r--r--   0        0        0     3593 2024-05-28 19:11:58.386054 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
--rw-r--r--   0        0        0     4129 2024-05-28 19:11:58.386250 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
--rw-r--r--   0        0        0     6799 2024-05-28 19:11:58.386458 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
--rw-r--r--   0        0        0     6599 2024-05-28 19:11:58.386658 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
--rw-r--r--   0        0        0     7318 2024-05-28 19:11:58.386850 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
--rw-r--r--   0        0        0     9277 2024-05-28 19:11:58.387038 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
--rw-r--r--   0        0        0    11308 2024-05-28 19:11:58.387279 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
--rw-r--r--   0        0        0     7629 2024-05-28 19:11:58.387601 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
--rw-r--r--   0        0        0     7093 2024-05-28 19:11:58.387853 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
--rw-r--r--   0        0        0    10621 2024-05-28 19:11:58.388047 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
--rw-r--r--   0        0        0     4082 2024-05-28 19:11:58.388203 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
--rw-r--r--   0        0        0     7728 2024-05-28 19:11:58.388401 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
--rw-r--r--   0        0        0    11756 2024-05-28 19:11:58.389095 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
--rw-r--r--   0        0        0    10830 2024-05-28 19:11:58.389332 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
--rw-r--r--   0        0        0     2289 2024-05-28 19:11:58.389500 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
--rw-r--r--   0        0        0     2925 2024-05-28 19:11:58.389669 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
--rw-r--r--   0        0        0    13072 2024-05-28 19:11:58.389871 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
--rw-r--r--   0        0        0    10924 2024-05-28 19:11:58.390057 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
--rw-r--r--   0        0        0     9640 2024-05-28 19:11:58.390240 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
--rw-r--r--   0        0        0    10178 2024-05-28 19:11:58.390442 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
--rw-r--r--   0        0        0    11781 2024-05-28 19:11:58.390626 pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352868 pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/__init__.py
--rw-r--r--   0        0        0     5922 2024-05-28 19:11:58.390838 pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356266 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/__init__.py
--rw-r--r--   0        0        0     4573 2024-05-28 19:11:58.391039 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
--rw-r--r--   0        0        0     6715 2024-05-28 19:11:58.391235 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
--rw-r--r--   0        0        0     2265 2024-05-28 19:11:58.391388 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
--rw-r--r--   0        0        0     3544 2024-05-28 19:11:58.391522 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
--rw-r--r--   0        0        0     3447 2024-05-28 19:11:58.391661 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
--rw-r--r--   0        0        0    12881 2024-05-28 19:11:58.391861 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
--rw-r--r--   0        0        0     3513 2024-05-28 19:11:58.391996 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
--rw-r--r--   0        0        0    14892 2024-05-28 19:11:58.392170 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
--rw-r--r--   0        0        0    11476 2024-05-28 19:11:58.392357 pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352570 pypanther-0.1.1a8/pypanther/rules/github_rules/__init__.py
--rw-r--r--   0        0        0     5255 2024-05-28 19:11:58.392814 pypanther-0.1.1a8/pypanther/rules/github_rules/github_action_failed.py
--rw-r--r--   0        0        0    14206 2024-05-28 19:11:58.393090 pypanther-0.1.1a8/pypanther/rules/github_rules/github_advanced_security_change.py
--rw-r--r--   0        0        0     2042 2024-05-28 19:11:58.393231 pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_policy_override.py
--rw-r--r--   0        0        0     2044 2024-05-28 19:11:58.393360 pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_protection_disabled.py
--rw-r--r--   0        0        0     2237 2024-05-28 19:11:58.393500 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_auth_modified.py
--rw-r--r--   0        0        0     2423 2024-05-28 19:11:58.393637 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_ip_allowlist.py
--rw-r--r--   0        0        0     2226 2024-05-28 19:11:58.393773 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_moderators_add.py
--rw-r--r--   0        0        0     2316 2024-05-28 19:11:58.393920 pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_modified.py
--rw-r--r--   0        0        0     3395 2024-05-28 19:11:58.394066 pypanther-0.1.1a8/pypanther/rules/github_rules/github_organization_app_integration_installed.py
--rw-r--r--   0        0        0     2861 2024-05-28 19:11:58.394265 pypanther-0.1.1a8/pypanther/rules/github_rules/github_public_repository_created.py
--rw-r--r--   0        0        0     2776 2024-05-28 19:11:58.394683 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_collaborator_change.py
--rw-r--r--   0        0        0     1460 2024-05-28 19:11:58.394854 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_created.py
--rw-r--r--   0        0        0     2515 2024-05-28 19:11:58.395035 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_hook_modified.py
--rw-r--r--   0        0        0     4225 2024-05-28 19:11:58.395329 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_initial_access.py
--rw-r--r--   0        0        0     1904 2024-05-28 19:11:58.395491 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_visibility_change.py
--rw-r--r--   0        0        0     5342 2024-05-28 19:11:58.395698 pypanther-0.1.1a8/pypanther/rules/github_rules/github_repository_transfer.py
--rw-r--r--   0        0        0     3334 2024-05-28 19:11:58.395864 pypanther-0.1.1a8/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
--rw-r--r--   0        0        0     3340 2024-05-28 19:11:58.396000 pypanther-0.1.1a8/pypanther/rules/github_rules/github_team_modified.py
--rw-r--r--   0        0        0     1636 2024-05-28 19:11:58.396133 pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_access_key_created.py
--rw-r--r--   0        0        0     1739 2024-05-28 19:11:58.396258 pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_role_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356132 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/__init__.py
--rw-r--r--   0        0        0     2347 2024-05-28 19:11:58.396411 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
--rw-r--r--   0        0        0     2803 2024-05-28 19:11:58.396546 pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352688 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/__init__.py
--rw-r--r--   0        0        0     2535 2024-05-28 19:11:58.396680 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
--rw-r--r--   0        0        0     2645 2024-05-28 19:11:58.396805 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
--rw-r--r--   0        0        0     3202 2024-05-28 19:11:58.396937 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
--rw-r--r--   0        0        0     2961 2024-05-28 19:11:58.397073 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
--rw-r--r--   0        0        0     1763 2024-05-28 19:11:58.397238 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
--rw-r--r--   0        0        0     6379 2024-05-28 19:11:58.397430 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
--rw-r--r--   0        0        0     4730 2024-05-28 19:11:58.397617 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
--rw-r--r--   0        0        0     1607 2024-05-28 19:11:58.397747 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
--rw-r--r--   0        0        0     2204 2024-05-28 19:11:58.397872 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
--rw-r--r--   0        0        0     1628 2024-05-28 19:11:58.397997 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
--rw-r--r--   0        0        0     2753 2024-05-28 19:11:58.398125 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
--rw-r--r--   0        0        0     4443 2024-05-28 19:11:58.398297 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
--rw-r--r--   0        0        0     3219 2024-05-28 19:11:58.398429 pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354403 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/__init__.py
--rw-r--r--   0        0        0     4374 2024-05-28 19:11:58.398625 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
--rw-r--r--   0        0        0     6493 2024-05-28 19:11:58.398814 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
--rw-r--r--   0        0        0     6706 2024-05-28 19:11:58.399004 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
--rw-r--r--   0        0        0     5283 2024-05-28 19:11:58.399187 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
--rw-r--r--   0        0        0     4645 2024-05-28 19:11:58.399359 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
--rw-r--r--   0        0        0     1961 2024-05-28 19:11:58.399479 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
--rw-r--r--   0        0        0     5786 2024-05-28 19:11:58.399651 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
--rw-r--r--   0        0        0     2339 2024-05-28 19:11:58.399800 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
--rw-r--r--   0        0        0     4338 2024-05-28 19:11:58.399992 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
--rw-r--r--   0        0        0     1465 2024-05-28 19:11:58.400185 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
--rw-r--r--   0        0        0     1998 2024-05-28 19:11:58.400339 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
--rw-r--r--   0        0        0     1963 2024-05-28 19:11:58.400491 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
--rw-r--r--   0        0        0     3049 2024-05-28 19:11:58.400629 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
--rw-r--r--   0        0        0     3473 2024-05-28 19:11:58.400857 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
--rw-r--r--   0        0        0     2742 2024-05-28 19:11:58.401165 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
--rw-r--r--   0        0        0     3387 2024-05-28 19:11:58.401491 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
--rw-r--r--   0        0        0     2020 2024-05-28 19:11:58.401680 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
--rw-r--r--   0        0        0     3457 2024-05-28 19:11:58.401841 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
--rw-r--r--   0        0        0     2587 2024-05-28 19:11:58.402024 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
--rw-r--r--   0        0        0     2203 2024-05-28 19:11:58.402185 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
--rw-r--r--   0        0        0     2721 2024-05-28 19:11:58.402352 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
--rw-r--r--   0        0        0     6834 2024-05-28 19:11:58.402566 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
--rw-r--r--   0        0        0     5013 2024-05-28 19:11:58.402760 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
--rw-r--r--   0        0        0     6052 2024-05-28 19:11:58.402956 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
--rw-r--r--   0        0        0     5452 2024-05-28 19:11:58.403242 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
--rw-r--r--   0        0        0     5222 2024-05-28 19:11:58.403587 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
--rw-r--r--   0        0        0     5172 2024-05-28 19:11:58.404059 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
--rw-r--r--   0        0        0     4977 2024-05-28 19:11:58.404328 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
--rw-r--r--   0        0        0     5223 2024-05-28 19:11:58.404574 pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353938 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/__init__.py
--rw-r--r--   0        0        0    10551 2024-05-28 19:11:58.404828 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
--rw-r--r--   0        0        0     4560 2024-05-28 19:11:58.405036 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
--rw-r--r--   0        0        0    25458 2024-05-28 19:11:58.405273 pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354103 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/__init__.py
--rw-r--r--   0        0        0     4663 2024-05-28 19:11:58.405686 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
--rw-r--r--   0        0        0     4410 2024-05-28 19:11:58.405924 pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353568 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/__init__.py
--rw-r--r--   0        0        0     4583 2024-05-28 19:11:58.406125 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
--rw-r--r--   0        0        0     9682 2024-05-28 19:11:58.406310 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
--rw-r--r--   0        0        0     6315 2024-05-28 19:11:58.406504 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
--rw-r--r--   0        0        0    10184 2024-05-28 19:11:58.406678 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
--rw-r--r--   0        0        0     5172 2024-05-28 19:11:58.406886 pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352474 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/__init__.py
--rw-r--r--   0        0        0     3363 2024-05-28 19:11:58.407204 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
--rw-r--r--   0        0        0     2868 2024-05-28 19:11:58.407445 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
--rw-r--r--   0        0        0     2711 2024-05-28 19:11:58.407846 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
--rw-r--r--   0        0        0     4174 2024-05-28 19:11:58.408092 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
--rw-r--r--   0        0        0     4371 2024-05-28 19:11:58.408451 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
--rw-r--r--   0        0        0     3958 2024-05-28 19:11:58.408751 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
--rw-r--r--   0        0        0     2284 2024-05-28 19:11:58.408958 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
--rw-r--r--   0        0        0     3355 2024-05-28 19:11:58.409180 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
--rw-r--r--   0        0        0     3215 2024-05-28 19:11:58.409325 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
--rw-r--r--   0        0        0     4770 2024-05-28 19:11:58.409546 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
--rw-r--r--   0        0        0     3435 2024-05-28 19:11:58.409835 pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352276 pypanther-0.1.1a8/pypanther/rules/netskope_rules/__init__.py
--rw-r--r--   0        0        0     2988 2024-05-28 19:11:58.410032 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
--rw-r--r--   0        0        0     3570 2024-05-28 19:11:58.410170 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_user_change.py
--rw-r--r--   0        0        0     2727 2024-05-28 19:11:58.410319 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_many_deletes.py
--rw-r--r--   0        0        0     2916 2024-05-28 19:11:58.410475 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_personnel_action.py
--rw-r--r--   0        0        0     3173 2024-05-28 19:11:58.410622 pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353782 pypanther-0.1.1a8/pypanther/rules/notion_rules/__init__.py
--rw-r--r--   0        0        0    16722 2024-05-28 19:11:58.410853 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_account_changed_after_login.py
--rw-r--r--   0        0        0     1543 2024-05-28 19:11:58.411187 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
--rw-r--r--   0        0        0    15424 2024-05-28 19:11:58.411442 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_new_location.py
--rw-r--r--   0        0        0     3287 2024-05-28 19:11:58.411704 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_deleted.py
--rw-r--r--   0        0        0     3283 2024-05-28 19:11:58.412121 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_exported.py
--rw-r--r--   0        0        0     1761 2024-05-28 19:11:58.412326 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
--rw-r--r--   0        0        0     5409 2024-05-28 19:11:58.412576 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
--rw-r--r--   0        0        0     1655 2024-05-28 19:11:58.412968 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_shared_to_web.py
--rw-r--r--   0        0        0     2883 2024-05-28 19:11:58.413158 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_scim_token_generated.py
--rw-r--r--   0        0        0     3886 2024-05-28 19:11:58.413330 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
--rw-r--r--   0        0        0     4484 2024-05-28 19:11:58.413592 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
--rw-r--r--   0        0        0     3009 2024-05-28 19:11:58.413814 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
--rw-r--r--   0        0        0     3278 2024-05-28 19:11:58.413989 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_exported.py
--rw-r--r--   0        0        0     4562 2024-05-28 19:11:58.414314 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
--rw-r--r--   0        0        0     4416 2024-05-28 19:11:58.414728 pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356572 pypanther-0.1.1a8/pypanther/rules/okta_rules/__init__.py
--rw-r--r--   0        0        0     3638 2024-05-28 19:11:58.414960 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_account_support_access.py
--rw-r--r--   0        0        0     3489 2024-05-28 19:11:58.415273 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
--rw-r--r--   0        0        0     7257 2024-05-28 19:11:58.416148 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_role_assigned.py
--rw-r--r--   0        0        0     7639 2024-05-28 19:11:58.416517 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
--rw-r--r--   0        0        0     2652 2024-05-28 19:11:58.416755 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_created.py
--rw-r--r--   0        0        0     2497 2024-05-28 19:11:58.416957 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_revoked.py
--rw-r--r--   0        0        0     9056 2024-05-28 19:11:58.417202 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
--rw-r--r--   0        0        0     7529 2024-05-28 19:11:58.417433 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
--rw-r--r--   0        0        0     7410 2024-05-28 19:11:58.417649 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
--rw-r--r--   0        0        0     8146 2024-05-28 19:11:58.417952 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_create_modify.py
--rw-r--r--   0        0        0     8236 2024-05-28 19:11:58.418501 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_signin.py
--rw-r--r--   0        0        0    13827 2024-05-28 19:11:58.418766 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
--rw-r--r--   0        0        0    13471 2024-05-28 19:11:58.419167 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
--rw-r--r--   0        0        0    10950 2024-05-28 19:11:58.419468 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_accessed.py
--rw-r--r--   0        0        0     7723 2024-05-28 19:11:58.419752 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
--rw-r--r--   0        0        0     7666 2024-05-28 19:11:58.420097 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
--rw-r--r--   0        0        0    19411 2024-05-28 19:11:58.420288 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
--rw-r--r--   0        0        0    10701 2024-05-28 19:11:58.420516 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_rate_limits.py
--rw-r--r--   0        0        0     5009 2024-05-28 19:11:58.420734 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_support_reset.py
--rw-r--r--   0        0        0     9212 2024-05-28 19:11:58.421054 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
--rw-r--r--   0        0        0     6860 2024-05-28 19:11:58.421255 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_account_locked.py
--rw-r--r--   0        0        0     7020 2024-05-28 19:11:58.421463 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
--rw-r--r--   0        0        0     4184 2024-05-28 19:11:58.422724 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset.py
--rw-r--r--   0        0        0     5466 2024-05-28 19:11:58.422989 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
--rw-r--r--   0        0        0     8402 2024-05-28 19:11:58.423208 pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352956 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/__init__.py
--rw-r--r--   0        0        0     3854 2024-05-28 19:11:58.423401 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
--rw-r--r--   0        0        0     1969 2024-05-28 19:11:58.423550 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
--rw-r--r--   0        0        0     2487 2024-05-28 19:11:58.423749 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
--rw-r--r--   0        0        0     2294 2024-05-28 19:11:58.424100 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
--rw-r--r--   0        0        0     2201 2024-05-28 19:11:58.424332 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_changed.py
--rw-r--r--   0        0        0     2670 2024-05-28 19:11:58.424491 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
--rw-r--r--   0        0        0     1893 2024-05-28 19:11:58.424643 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
--rw-r--r--   0        0        0     1935 2024-05-28 19:11:58.424964 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
--rw-r--r--   0        0        0     1862 2024-05-28 19:11:58.425132 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
--rw-r--r--   0        0        0     2559 2024-05-28 19:11:58.425286 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
--rw-r--r--   0        0        0     2009 2024-05-28 19:11:58.425435 pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353133 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/__init__.py
--rw-r--r--   0        0        0     4579 2024-05-28 19:11:58.425658 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
--rw-r--r--   0        0        0     3931 2024-05-28 19:11:58.425810 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
--rw-r--r--   0        0        0     4441 2024-05-28 19:11:58.426008 pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356027 pypanther-0.1.1a8/pypanther/rules/osquery_rules/__init__.py
--rw-r--r--   0        0        0     4052 2024-05-28 19:11:58.426279 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
--rw-r--r--   0        0        0     3412 2024-05-28 19:11:58.426542 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
--rw-r--r--   0        0        0     3594 2024-05-28 19:11:58.426693 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
--rw-r--r--   0        0        0     2979 2024-05-28 19:11:58.426836 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
--rw-r--r--   0        0        0     2610 2024-05-28 19:11:58.426984 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
--rw-r--r--   0        0        0     2217 2024-05-28 19:11:58.427130 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
--rw-r--r--   0        0        0     4071 2024-05-28 19:11:58.427265 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
--rw-r--r--   0        0        0     3684 2024-05-28 19:11:58.427400 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
--rw-r--r--   0        0        0     3486 2024-05-28 19:11:58.427530 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ossec.py
--rw-r--r--   0        0        0     3559 2024-05-28 19:11:58.427665 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated.py
--rw-r--r--   0        0        0     3688 2024-05-28 19:11:58.427798 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated_macos.py
--rw-r--r--   0        0        0     3744 2024-05-28 19:11:58.428233 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ssh_listener.py
--rw-r--r--   0        0        0     5597 2024-05-28 19:11:58.428534 pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353388 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/__init__.py
--rw-r--r--   0        0        0     4586 2024-05-28 19:11:58.428863 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
--rw-r--r--   0        0        0     2534 2024-05-28 19:11:58.429364 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_saml_modified.py
--rw-r--r--   0        0        0     8369 2024-05-28 19:11:58.429670 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
--rw-r--r--   0        0        0     9726 2024-05-28 19:11:58.429882 pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_user_modified.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354643 pypanther-0.1.1a8/pypanther/rules/salesforce_rules/__init__.py
--rw-r--r--   0        0        0     4586 2024-05-28 19:11:58.430146 pypanther-0.1.1a8/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353299 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/__init__.py
--rw-r--r--   0        0        0     7224 2024-05-28 19:11:58.430367 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
--rw-r--r--   0        0        0     6482 2024-05-28 19:11:58.430577 pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_threats.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355907 pypanther-0.1.1a8/pypanther/rules/slack_rules/__init__.py
--rw-r--r--   0        0        0    10111 2024-05-28 19:11:58.430815 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_access_expanded.py
--rw-r--r--   0        0        0     8853 2024-05-28 19:11:58.431014 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_added.py
--rw-r--r--   0        0        0     6590 2024-05-28 19:11:58.431418 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_removed.py
--rw-r--r--   0        0        0     4682 2024-05-28 19:11:58.431767 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_application_dos.py
--rw-r--r--   0        0        0     4947 2024-05-28 19:11:58.432063 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_dlp_modified.py
--rw-r--r--   0        0        0     3486 2024-05-28 19:11:58.432310 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_config_changed.py
--rw-r--r--   0        0        0     3429 2024-05-28 19:11:58.432516 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
--rw-r--r--   0        0        0     3334 2024-05-28 19:11:58.432687 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
--rw-r--r--   0        0        0     5895 2024-05-28 19:11:58.432918 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_idp_configuration_change.py
--rw-r--r--   0        0        0     4701 2024-05-28 19:11:58.433301 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_information_barrier_modified.py
--rw-r--r--   0        0        0     3331 2024-05-28 19:11:58.433529 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
--rw-r--r--   0        0        0     6999 2024-05-28 19:11:58.433717 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
--rw-r--r--   0        0        0     3454 2024-05-28 19:11:58.433852 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
--rw-r--r--   0        0        0     2843 2024-05-28 19:11:58.434062 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_created.py
--rw-r--r--   0        0        0     2843 2024-05-28 19:11:58.434228 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_deleted.py
--rw-r--r--   0        0        0     3315 2024-05-28 19:11:58.434385 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
--rw-r--r--   0        0        0     3412 2024-05-28 19:11:58.434559 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
--rw-r--r--   0        0        0     3592 2024-05-28 19:11:58.434722 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_private_channel_made_public.py
--rw-r--r--   0        0        0     4151 2024-05-28 19:11:58.434937 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
--rw-r--r--   0        0        0     3557 2024-05-28 19:11:58.435086 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_service_owner_transferred.py
--rw-r--r--   0        0        0     3399 2024-05-28 19:11:58.435367 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_sso_settings_changed.py
--rw-r--r--   0        0        0     7399 2024-05-28 19:11:58.435556 pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356824 pypanther-0.1.1a8/pypanther/rules/snyk_rules/__init__.py
--rw-r--r--   0        0        0     2626 2024-05-28 19:11:58.435716 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_misc_settings.py
--rw-r--r--   0        0        0     4571 2024-05-28 19:11:58.435902 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_org_settings.py
--rw-r--r--   0        0        0     4568 2024-05-28 19:11:58.436140 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_ou_change.py
--rw-r--r--   0        0        0     4884 2024-05-28 19:11:58.436378 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_project_settings.py
--rw-r--r--   0        0        0     5437 2024-05-28 19:11:58.436604 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_role_change.py
--rw-r--r--   0        0        0    12027 2024-05-28 19:11:58.436827 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_svcacct_change.py
--rw-r--r--   0        0        0     3971 2024-05-28 19:11:58.436998 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
--rw-r--r--   0        0        0     6266 2024-05-28 19:11:58.437211 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_policysetting.py
--rw-r--r--   0        0        0     2578 2024-05-28 19:11:58.437380 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_sso.py
--rw-r--r--   0        0        0     5851 2024-05-28 19:11:58.437713 pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_user_mgmt.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352089 pypanther-0.1.1a8/pypanther/rules/standard_rules/__init__.py
--rw-r--r--   0        0        0    10991 2024-05-28 19:11:58.437955 pypanther-0.1.1a8/pypanther/rules/standard_rules/admin_assigned.py
--rw-r--r--   0        0        0    16955 2024-05-28 19:11:58.438292 pypanther-0.1.1a8/pypanther/rules/standard_rules/brute_force_by_ip.py
--rw-r--r--   0        0        0    36758 2024-05-28 19:11:58.438611 pypanther-0.1.1a8/pypanther/rules/standard_rules/impossible_travel_login.py
--rw-r--r--   0        0        0     9779 2024-05-28 19:11:58.439137 pypanther-0.1.1a8/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
--rw-r--r--   0        0        0     8225 2024-05-28 19:11:58.439339 pypanther-0.1.1a8/pypanther/rules/standard_rules/mfa_disabled.py
--rw-r--r--   0        0        0     9943 2024-05-28 19:11:58.439546 pypanther-0.1.1a8/pypanther/rules/standard_rules/standard_dns_base64.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353861 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/__init__.py
--rw-r--r--   0        0        0     4649 2024-05-28 19:11:58.439749 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
--rw-r--r--   0        0        0     4885 2024-05-28 19:11:58.439960 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
--rw-r--r--   0        0        0     4666 2024-05-28 19:11:58.440234 pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356684 pypanther-0.1.1a8/pypanther/rules/tines_rules/__init__.py
--rw-r--r--   0        0        0     2584 2024-05-28 19:11:58.440442 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
--rw-r--r--   0        0        0     2824 2024-05-28 19:11:58.440763 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_custom_ca.py
--rw-r--r--   0        0        0     3540 2024-05-28 19:11:58.440948 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
--rw-r--r--   0        0        0     2887 2024-05-28 19:11:58.441094 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_global_resource_destruction.py
--rw-r--r--   0        0        0     2947 2024-05-28 19:11:58.441254 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_sso_settings.py
--rw-r--r--   0        0        0     2765 2024-05-28 19:11:58.441427 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_items_destruction.py
--rw-r--r--   0        0        0     2735 2024-05-28 19:11:58.441579 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
--rw-r--r--   0        0        0     2680 2024-05-28 19:11:58.441739 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_team_destruction.py
--rw-r--r--   0        0        0     3987 2024-05-28 19:11:58.441908 pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_tenant_authtoken.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352185 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/__init__.py
--rw-r--r--   0        0        0     3775 2024-05-28 19:11:58.442062 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
--rw-r--r--   0        0        0     2972 2024-05-28 19:11:58.442217 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
--rw-r--r--   0        0        0     3208 2024-05-28 19:11:58.442377 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_owner.py
--rw-r--r--   0        0        0     3717 2024-05-28 19:11:58.442531 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
--rw-r--r--   0        0        0     2962 2024-05-28 19:11:58.442682 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
--rw-r--r--   0        0        0     2774 2024-05-28 19:11:58.442830 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_role.py
--rw-r--r--   0        0        0     3927 2024-05-28 19:11:58.442983 pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353216 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-28 19:11:58.443143 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
--rw-r--r--   0        0        0     2359 2024-05-28 19:11:58.443509 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
--rw-r--r--   0        0        0     2830 2024-05-28 19:11:58.443740 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
--rw-r--r--   0        0        0     2760 2024-05-28 19:11:58.443955 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
--rw-r--r--   0        0        0     3358 2024-05-28 19:11:58.444132 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
--rw-r--r--   0        0        0     3558 2024-05-28 19:11:58.444298 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
--rw-r--r--   0        0        0     2620 2024-05-28 19:11:58.444442 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
--rw-r--r--   0        0        0     4620 2024-05-28 19:11:58.444656 pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
--rw-r--r--   0        0        0     4251 2024-05-28 18:40:51.829617 pypanther-0.1.1a8/pypanther/upload.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095097 pypanther-0.1.1a8/pypanther/vendor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095354 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095410 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/__init__.py
--rw-r--r--   0        0        0    16541 2024-05-24 13:47:47.095519 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/client.py
--rw-r--r--   0        0        0      624 2024-05-24 13:47:47.095629 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/errors.py
--rw-r--r--   0        0        0      159 2024-05-24 13:47:47.095796 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
--rw-r--r--   0        0        0      802 2024-05-24 13:47:47.095929 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
--rw-r--r--   0        0        0     1439 2024-05-24 17:25:24.652928 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql
--rw-r--r--   0        0        0    25446 2024-05-24 13:47:47.096146 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
--rw-r--r--   0        0        0     1606 2024-05-24 13:47:47.096405 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/cli_output.py
--rw-r--r--   0        0        0      493 2024-05-28 18:40:51.830002 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/command/standard_args.py
--rw-r--r--   0        0        0     1308 2024-05-28 18:40:51.830341 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/config.py
--rw-r--r--   0        0        0      714 2024-05-28 18:40:51.830732 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/constants.py
--rw-r--r--   0        0        0     2008 2024-05-28 18:40:51.831059 pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/util.py
--rw-r--r--   0        0        0      274 2024-05-23 22:00:33.355426 pypanther-0.1.1a8/pypanther/wrap.py
--rw-r--r--   0        0        0     1746 2024-05-28 19:11:58.444950 pypanther-0.1.1a8/pyproject.toml
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pypanther-0.1.1a8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-22 20:25:10.032196 pypanther-0.1.1a9/LICENSE.txt
+-rw-r--r--   0        0        0       80 2024-05-03 14:59:36.061341 pypanther-0.1.1a9/README.md
+-rw-r--r--   0        0        0      185 2024-05-23 22:40:02.087577 pypanther-0.1.1a9/pypanther/__init__.py
+-rw-r--r--   0        0        0    25688 2024-05-28 22:43:21.992934 pypanther-0.1.1a9/pypanther/base.py
+-rw-r--r--   0        0        0      490 2024-05-23 22:40:02.087802 pypanther-0.1.1a9/pypanther/cache.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.087892 pypanther-0.1.1a9/pypanther/data_models/__init__.py
+-rw-r--r--   0        0        0     1387 2024-05-23 22:40:02.088052 pypanther-0.1.1a9/pypanther/data_models/asana_data_model.py
+-rw-r--r--   0        0        0     1544 2024-05-23 22:40:02.088132 pypanther-0.1.1a9/pypanther/data_models/atlassian_data_model.py
+-rw-r--r--   0        0        0      607 2024-05-23 22:40:02.088229 pypanther-0.1.1a9/pypanther/data_models/aws_alb_data_model.py
+-rw-r--r--   0        0        0     2214 2024-05-23 22:40:02.088338 pypanther-0.1.1a9/pypanther/data_models/aws_cloudtrail_data_model.py
+-rw-r--r--   0        0        0     1465 2024-05-23 22:40:02.088467 pypanther-0.1.1a9/pypanther/data_models/aws_eks_data_model.py
+-rw-r--r--   0        0        0      630 2024-05-23 22:40:02.088667 pypanther-0.1.1a9/pypanther/data_models/aws_s3_data_model.py
+-rw-r--r--   0        0        0      593 2024-05-23 22:40:02.088783 pypanther-0.1.1a9/pypanther/data_models/aws_vpcdns_data_model.py
+-rw-r--r--   0        0        0      742 2024-05-23 22:40:02.088874 pypanther-0.1.1a9/pypanther/data_models/aws_vpcflow_data_model.py
+-rw-r--r--   0        0        0     1191 2024-05-23 22:40:02.088964 pypanther-0.1.1a9/pypanther/data_models/azure_signin_data_model.py
+-rw-r--r--   0        0        0      941 2024-05-23 22:40:02.089053 pypanther-0.1.1a9/pypanther/data_models/box_data_model.py
+-rw-r--r--   0        0        0      873 2024-05-23 22:40:02.089143 pypanther-0.1.1a9/pypanther/data_models/cisco_umbrella_data_model.py
+-rw-r--r--   0        0        0      653 2024-05-23 22:40:02.089238 pypanther-0.1.1a9/pypanther/data_models/cloudflare_firewall_data_model.py
+-rw-r--r--   0        0        0      729 2024-05-23 22:40:02.089315 pypanther-0.1.1a9/pypanther/data_models/cloudflare_httpreq_data_model.py
+-rw-r--r--   0        0        0     1853 2024-05-23 22:40:02.089395 pypanther-0.1.1a9/pypanther/data_models/crowdstrike_fdr_data_model.py
+-rw-r--r--   0        0        0     5215 2024-05-23 22:40:02.089505 pypanther-0.1.1a9/pypanther/data_models/gcp_data_model.py
+-rw-r--r--   0        0        0     1613 2024-05-23 22:40:02.089585 pypanther-0.1.1a9/pypanther/data_models/github_data_model.py
+-rw-r--r--   0        0        0     1669 2024-05-23 22:40:02.089672 pypanther-0.1.1a9/pypanther/data_models/gsuite_data_model.py
+-rw-r--r--   0        0        0     1864 2024-05-23 22:40:02.089746 pypanther-0.1.1a9/pypanther/data_models/notion_data_model.py
+-rw-r--r--   0        0        0     2070 2024-05-23 22:40:02.089823 pypanther-0.1.1a9/pypanther/data_models/okta_data_model.py
+-rw-r--r--   0        0        0     1467 2024-05-23 22:40:02.089912 pypanther-0.1.1a9/pypanther/data_models/onelogin_data_model.py
+-rw-r--r--   0        0        0      730 2024-05-23 22:40:02.089999 pypanther-0.1.1a9/pypanther/data_models/onepassword_itemusage_data_model.py
+-rw-r--r--   0        0        0     1058 2024-05-23 22:40:02.090085 pypanther-0.1.1a9/pypanther/data_models/onepassword_signinattempt_data_model.py
+-rw-r--r--   0        0        0     1742 2024-05-23 22:40:02.090180 pypanther-0.1.1a9/pypanther/data_models/panther_audit_data_model.py
+-rw-r--r--   0        0        0      613 2024-05-23 22:40:02.090269 pypanther-0.1.1a9/pypanther/data_models/slack_accesslogs_data_model.py
+-rw-r--r--   0        0        0      711 2024-05-23 22:40:02.090343 pypanther-0.1.1a9/pypanther/data_models/slack_auditlogs_data_model.py
+-rw-r--r--   0        0        0      500 2024-05-23 22:40:02.090417 pypanther-0.1.1a9/pypanther/data_models/slack_integrationlogs_data_model.py
+-rw-r--r--   0        0        0     2714 2024-05-23 22:40:02.090501 pypanther-0.1.1a9/pypanther/data_models/zendesk_data_model.py
+-rw-r--r--   0        0        0      886 2024-05-23 22:40:02.090588 pypanther-0.1.1a9/pypanther/data_models/zoom_activity_data_model.py
+-rw-r--r--   0        0        0     1887 2024-05-23 22:40:02.090677 pypanther-0.1.1a9/pypanther/data_models/zoom_operation_data_model.py
+-rw-r--r--   0        0        0     2682 2024-05-23 22:40:02.090760 pypanther-0.1.1a9/pypanther/get.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.090849 pypanther-0.1.1a9/pypanther/helpers/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-23 22:40:02.090945 pypanther-0.1.1a9/pypanther/helpers/gcp_base_helpers.py
+-rw-r--r--   0        0        0      781 2024-05-23 22:40:02.091403 pypanther-0.1.1a9/pypanther/helpers/gcp_environment.py
+-rw-r--r--   0        0        0     1417 2024-05-23 22:40:02.091523 pypanther-0.1.1a9/pypanther/helpers/panther_asana_helpers.py
+-rw-r--r--   0        0        0     1597 2024-05-23 22:40:02.091604 pypanther-0.1.1a9/pypanther/helpers/panther_audit.py
+-rw-r--r--   0        0        0      555 2024-05-23 22:40:02.091700 pypanther-0.1.1a9/pypanther/helpers/panther_auth0_helpers.py
+-rw-r--r--   0        0        0     1191 2024-05-23 22:40:02.091783 pypanther-0.1.1a9/pypanther/helpers/panther_azuresignin_helpers.py
+-rw-r--r--   0        0        0    19692 2024-05-23 22:40:02.091894 pypanther-0.1.1a9/pypanther/helpers/panther_base_helpers.py
+-rw-r--r--   0        0        0     4529 2024-05-23 22:40:02.092082 pypanther-0.1.1a9/pypanther/helpers/panther_box_helpers.py
+-rw-r--r--   0        0        0     2267 2024-05-23 22:40:02.092162 pypanther-0.1.1a9/pypanther/helpers/panther_cloudflare_helpers.py
+-rw-r--r--   0        0        0      507 2024-05-23 22:40:02.092238 pypanther-0.1.1a9/pypanther/helpers/panther_config.py
+-rw-r--r--   0        0        0      891 2024-05-23 22:40:02.092316 pypanther-0.1.1a9/pypanther/helpers/panther_config_defaults.py
+-rw-r--r--   0        0        0     1043 2024-05-23 22:40:02.092391 pypanther-0.1.1a9/pypanther/helpers/panther_config_overrides.py
+-rw-r--r--   0        0        0     3465 2024-05-23 22:40:02.092472 pypanther-0.1.1a9/pypanther/helpers/panther_default.py
+-rw-r--r--   0        0        0     1288 2024-05-23 22:40:02.092550 pypanther-0.1.1a9/pypanther/helpers/panther_duo_helpers.py
+-rw-r--r--   0        0        0     1118 2024-05-23 22:40:02.092632 pypanther-0.1.1a9/pypanther/helpers/panther_event_type_helpers.py
+-rw-r--r--   0        0        0    12436 2024-05-23 22:40:02.092782 pypanther-0.1.1a9/pypanther/helpers/panther_greynoise_helpers.py
+-rw-r--r--   0        0        0    38305 2024-05-23 22:40:02.092958 pypanther-0.1.1a9/pypanther/helpers/panther_iocs.py
+-rw-r--r--   0        0        0     6497 2024-05-23 22:40:02.093087 pypanther-0.1.1a9/pypanther/helpers/panther_ipinfo_helpers.py
+-rw-r--r--   0        0        0     2154 2024-05-23 22:40:02.093174 pypanther-0.1.1a9/pypanther/helpers/panther_lookuptable_helpers.py
+-rw-r--r--   0        0        0      387 2024-05-23 22:40:02.093255 pypanther-0.1.1a9/pypanther/helpers/panther_mongodb_helpers.py
+-rw-r--r--   0        0        0      340 2024-05-23 22:40:02.093335 pypanther-0.1.1a9/pypanther/helpers/panther_notion_helpers.py
+-rw-r--r--   0        0        0    13096 2024-05-23 22:40:02.093464 pypanther-0.1.1a9/pypanther/helpers/panther_oss_helpers.py
+-rw-r--r--   0        0        0      610 2024-05-23 22:40:02.093544 pypanther-0.1.1a9/pypanther/helpers/panther_snyk_helpers.py
+-rw-r--r--   0        0        0      492 2024-05-23 22:40:02.093712 pypanther-0.1.1a9/pypanther/helpers/panther_tailscale_helpers.py
+-rw-r--r--   0        0        0      567 2024-05-23 22:40:02.093837 pypanther-0.1.1a9/pypanther/helpers/panther_tines_helpers.py
+-rw-r--r--   0        0        0     1542 2024-05-23 22:40:02.093932 pypanther-0.1.1a9/pypanther/helpers/panther_tor_helpers.py
+-rw-r--r--   0        0        0     3084 2024-05-23 22:40:02.094025 pypanther-0.1.1a9/pypanther/helpers/panther_zoom_helpers.py
+-rw-r--r--   0        0        0    13022 2024-05-23 22:40:02.094175 pypanther-0.1.1a9/pypanther/log_types.py
+-rw-r--r--   0        0        0     1134 2024-05-28 19:02:33.404845 pypanther-0.1.1a9/pypanther/main.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:02:33.404888 pypanther-0.1.1a9/pypanther/py.typed
+-rw-r--r--   0        0        0      824 2024-05-28 17:53:54.258143 pypanther-0.1.1a9/pypanther/register.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.094340 pypanther-0.1.1a9/pypanther/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.094443 pypanther-0.1.1a9/pypanther/rules/asana_rules/__init__.py
+-rw-r--r--   0        0        0     4069 2024-05-28 19:02:33.405420 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_service_account_created.py
+-rw-r--r--   0        0        0     3241 2024-05-28 19:02:33.405768 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_team_privacy_public.py
+-rw-r--r--   0        0        0     3263 2024-05-28 19:02:33.406224 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
+-rw-r--r--   0        0        0     3232 2024-05-28 19:02:33.406628 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
+-rw-r--r--   0        0        0     3420 2024-05-28 19:02:33.406988 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
+-rw-r--r--   0        0        0     3399 2024-05-28 19:02:33.407290 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
+-rw-r--r--   0        0        0     3747 2024-05-28 19:02:33.407541 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_new_admin.py
+-rw-r--r--   0        0        0     3242 2024-05-28 19:02:33.407832 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_org_export.py
+-rw-r--r--   0        0        0     3725 2024-05-28 19:02:33.408073 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
+-rw-r--r--   0        0        0     3629 2024-05-28 19:02:33.408335 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
+-rw-r--r--   0        0        0     3498 2024-05-28 19:02:33.408578 pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.095444 pypanther-0.1.1a9/pypanther/rules/atlassian_rules/__init__.py
+-rw-r--r--   0        0        0     4891 2024-05-28 19:02:33.409308 pypanther-0.1.1a9/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.095651 pypanther-0.1.1a9/pypanther/rules/auth0_rules/__init__.py
+-rw-r--r--   0        0        0    45000 2024-05-28 19:02:33.409955 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_custom_role_created.py
+-rw-r--r--   0        0        0    15426 2024-05-28 19:02:33.410503 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_integration_installed.py
+-rw-r--r--   0        0        0    23152 2024-05-28 19:02:33.410975 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
+-rw-r--r--   0        0        0    23502 2024-05-28 19:02:33.411442 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
+-rw-r--r--   0        0        0    34173 2024-05-28 19:02:33.411737 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
+-rw-r--r--   0        0        0    23656 2024-05-28 19:02:33.412004 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
+-rw-r--r--   0        0        0    22677 2024-05-28 19:02:33.412298 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
+-rw-r--r--   0        0        0    19831 2024-05-28 19:02:33.412623 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
+-rw-r--r--   0        0        0    17293 2024-05-28 19:02:33.412941 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
+-rw-r--r--   0        0        0    18180 2024-05-28 19:02:33.413239 pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.096916 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/__init__.py
+-rw-r--r--   0        0        0    11023 2024-05-28 19:02:33.413528 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
+-rw-r--r--   0        0        0     8203 2024-05-28 19:02:33.413793 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
+-rw-r--r--   0        0        0     7052 2024-05-28 19:02:33.414760 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
+-rw-r--r--   0        0        0     3387 2024-05-28 19:02:33.415294 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
+-rw-r--r--   0        0        0     7226 2024-05-28 19:02:33.415595 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
+-rw-r--r--   0        0        0     4474 2024-05-28 19:02:33.416009 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
+-rw-r--r--   0        0        0     7006 2024-05-28 19:02:33.416328 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
+-rw-r--r--   0        0        0     6565 2024-05-28 19:02:33.416628 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
+-rw-r--r--   0        0        0     6552 2024-05-28 19:02:33.416880 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
+-rw-r--r--   0        0        0    20565 2024-05-28 19:02:33.417356 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
+-rw-r--r--   0        0        0     4041 2024-05-28 19:02:33.417611 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
+-rw-r--r--   0        0        0     5610 2024-05-28 19:02:33.417896 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
+-rw-r--r--   0        0        0     5713 2024-05-28 19:02:33.418201 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
+-rw-r--r--   0        0        0     2295 2024-05-28 19:02:33.418516 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
+-rw-r--r--   0        0        0     6726 2024-05-28 19:02:33.418866 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
+-rw-r--r--   0        0        0    17207 2024-05-28 19:02:33.419147 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
+-rw-r--r--   0        0        0    22420 2024-05-28 19:02:33.419718 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
+-rw-r--r--   0        0        0     7258 2024-05-28 19:02:33.420077 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
+-rw-r--r--   0        0        0     6888 2024-05-28 19:02:33.420346 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
+-rw-r--r--   0        0        0     8185 2024-05-28 19:02:33.420641 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
+-rw-r--r--   0        0        0     5173 2024-05-28 19:02:33.421239 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
+-rw-r--r--   0        0        0    30283 2024-05-28 19:02:33.421784 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
+-rw-r--r--   0        0        0     8614 2024-05-28 19:02:33.422108 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
+-rw-r--r--   0        0        0    39743 2024-05-28 19:02:33.422500 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
+-rw-r--r--   0        0        0    27333 2024-05-28 19:02:33.422861 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
+-rw-r--r--   0        0        0    26742 2024-05-28 19:02:33.423259 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
+-rw-r--r--   0        0        0     7276 2024-05-28 19:02:33.423766 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
+-rw-r--r--   0        0        0     8595 2024-05-28 19:02:33.424015 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
+-rw-r--r--   0        0        0     6119 2024-05-28 19:02:33.424304 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
+-rw-r--r--   0        0        0    12719 2024-05-28 19:02:33.424718 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
+-rw-r--r--   0        0        0    13763 2024-05-28 19:02:33.425064 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
+-rw-r--r--   0        0        0     7154 2024-05-28 19:02:33.425640 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
+-rw-r--r--   0        0        0    10491 2024-05-28 19:02:33.425951 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
+-rw-r--r--   0        0        0     9050 2024-05-28 19:02:33.426220 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
+-rw-r--r--   0        0        0     3389 2024-05-28 19:02:33.426463 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
+-rw-r--r--   0        0        0     5216 2024-05-28 19:02:33.426785 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
+-rw-r--r--   0        0        0    11264 2024-05-28 19:02:33.427150 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
+-rw-r--r--   0        0        0     5730 2024-05-28 19:02:33.427564 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
+-rw-r--r--   0        0        0     9734 2024-05-28 19:02:33.428155 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
+-rw-r--r--   0        0        0    27000 2024-05-28 19:02:33.428462 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
+-rw-r--r--   0        0        0     7827 2024-05-28 19:02:33.428861 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
+-rw-r--r--   0        0        0    16376 2024-05-28 19:02:33.429219 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
+-rw-r--r--   0        0        0    14639 2024-05-28 19:02:33.429491 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
+-rw-r--r--   0        0        0    17400 2024-05-28 19:02:33.429793 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
+-rw-r--r--   0        0        0     7480 2024-05-28 19:02:33.430325 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
+-rw-r--r--   0        0        0    18982 2024-05-28 19:02:33.430574 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
+-rw-r--r--   0        0        0     4669 2024-05-28 19:02:33.430950 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
+-rw-r--r--   0        0        0    10753 2024-05-28 19:02:33.431347 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
+-rw-r--r--   0        0        0     3934 2024-05-28 19:02:33.431594 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
+-rw-r--r--   0        0        0     5825 2024-05-28 19:02:33.431863 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
+-rw-r--r--   0        0        0     7516 2024-05-28 19:02:33.432250 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
+-rw-r--r--   0        0        0    12289 2024-05-28 19:02:33.432657 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
+-rw-r--r--   0        0        0    11516 2024-05-28 19:02:33.433348 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
+-rw-r--r--   0        0        0     5570 2024-05-28 19:02:33.433738 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
+-rw-r--r--   0        0        0     7558 2024-05-28 19:02:33.434200 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
+-rw-r--r--   0        0        0     5191 2024-05-28 19:02:33.434438 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
+-rw-r--r--   0        0        0     6478 2024-05-28 19:02:33.434693 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
+-rw-r--r--   0        0        0     8697 2024-05-28 19:02:33.434950 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
+-rw-r--r--   0        0        0     5976 2024-05-28 19:02:33.435378 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
+-rw-r--r--   0        0        0     6782 2024-05-28 19:02:33.435653 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
+-rw-r--r--   0        0        0     7024 2024-05-28 19:02:33.436030 pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.103613 pypanther-0.1.1a9/pypanther/rules/aws_eks_rules/__init__.py
+-rw-r--r--   0        0        0     9700 2024-05-28 19:02:33.436463 pypanther-0.1.1a9/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
+-rw-r--r--   0        0        0    17813 2024-05-28 19:02:33.436741 pypanther-0.1.1a9/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.103988 pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/__init__.py
+-rw-r--r--   0        0        0     5370 2024-05-28 19:02:33.437065 pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
+-rw-r--r--   0        0        0     5391 2024-05-28 19:02:33.437332 pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
+-rw-r--r--   0        0        0     5417 2024-05-28 19:02:33.437716 pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.104373 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/__init__.py
+-rw-r--r--   0        0        0     4702 2024-05-28 19:02:33.438067 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
+-rw-r--r--   0        0        0     2560 2024-05-28 19:02:33.438309 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
+-rw-r--r--   0        0        0     6277 2024-05-28 19:02:33.438566 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
+-rw-r--r--   0        0        0     1997 2024-05-28 19:02:33.440154 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
+-rw-r--r--   0        0        0     8748 2024-05-28 19:02:33.440433 pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.105046 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/__init__.py
+-rw-r--r--   0        0        0     6790 2024-05-28 19:02:33.440713 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
+-rw-r--r--   0        0        0     1340 2024-05-28 19:02:33.440979 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
+-rw-r--r--   0        0        0     2538 2024-05-28 19:02:33.441269 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
+-rw-r--r--   0        0        0     2498 2024-05-28 19:02:33.441547 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
+-rw-r--r--   0        0        0     2927 2024-05-28 19:02:33.441787 pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.105687 pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/__init__.py
+-rw-r--r--   0        0        0     7978 2024-05-28 19:02:33.442130 pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_failed_signins.py
+-rw-r--r--   0        0        0    15766 2024-05-28 19:02:33.442541 pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_legacyauth.py
+-rw-r--r--   0        0        0    17553 2024-05-28 19:02:33.443046 pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.106335 pypanther-0.1.1a9/pypanther/rules/box_rules/__init__.py
+-rw-r--r--   0        0        0     2134 2024-05-28 19:02:33.443664 pypanther-0.1.1a9/pypanther/rules/box_rules/box_access_granted.py
+-rw-r--r--   0        0        0     2869 2024-05-28 19:02:33.443939 pypanther-0.1.1a9/pypanther/rules/box_rules/box_anomalous_download.py
+-rw-r--r--   0        0        0     2744 2024-05-28 19:02:33.444235 pypanther-0.1.1a9/pypanther/rules/box_rules/box_event_triggered_externally.py
+-rw-r--r--   0        0        0     3652 2024-05-28 19:02:33.444526 pypanther-0.1.1a9/pypanther/rules/box_rules/box_item_shared_externally.py
+-rw-r--r--   0        0        0     4266 2024-05-28 19:02:33.444841 pypanther-0.1.1a9/pypanther/rules/box_rules/box_malicious_content.py
+-rw-r--r--   0        0        0     2124 2024-05-28 19:02:33.445245 pypanther-0.1.1a9/pypanther/rules/box_rules/box_new_login.py
+-rw-r--r--   0        0        0     2822 2024-05-28 19:02:33.445497 pypanther-0.1.1a9/pypanther/rules/box_rules/box_policy_violation.py
+-rw-r--r--   0        0        0     4215 2024-05-28 19:02:33.445795 pypanther-0.1.1a9/pypanther/rules/box_rules/box_suspicious_login_or_session.py
+-rw-r--r--   0        0        0     2226 2024-05-28 19:02:33.446178 pypanther-0.1.1a9/pypanther/rules/box_rules/box_untrusted_device.py
+-rw-r--r--   0        0        0     2366 2024-05-28 19:02:33.446613 pypanther-0.1.1a9/pypanther/rules/box_rules/box_user_downloads.py
+-rw-r--r--   0        0        0     3179 2024-05-28 19:02:33.447248 pypanther-0.1.1a9/pypanther/rules/box_rules/box_user_permission_updates.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.107410 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/__init__.py
+-rw-r--r--   0        0        0     3313 2024-05-28 19:02:33.447648 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
+-rw-r--r--   0        0        0     3037 2024-05-28 19:02:33.448560 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
+-rw-r--r--   0        0        0     3487 2024-05-28 19:02:33.448798 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
+-rw-r--r--   0        0        0     2262 2024-05-28 19:02:33.449059 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
+-rw-r--r--   0        0        0     2591 2024-05-28 19:02:33.449299 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
+-rw-r--r--   0        0        0    11317 2024-05-28 19:02:33.449575 pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.108062 pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-28 19:02:33.449964 pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
+-rw-r--r--   0        0        0     1428 2024-05-28 19:02:33.450275 pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
+-rw-r--r--   0        0        0     1917 2024-05-28 19:02:33.450523 pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.108466 pypanther-0.1.1a9/pypanther/rules/cloudflare_rules/__init__.py
+-rw-r--r--   0        0        0     4983 2024-05-28 19:02:33.450822 pypanther-0.1.1a9/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
+-rw-r--r--   0        0        0     7577 2024-05-28 19:02:33.451295 pypanther-0.1.1a9/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.108788 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/__init__.py
+-rw-r--r--   0        0        0    29399 2024-05-28 19:02:33.451613 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
+-rw-r--r--   0        0        0     8191 2024-05-28 19:02:33.451905 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
+-rw-r--r--   0        0        0     9907 2024-05-28 19:02:33.452194 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
+-rw-r--r--   0        0        0     9869 2024-05-28 19:02:33.452666 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
+-rw-r--r--   0        0        0    10434 2024-05-28 19:02:33.452935 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
+-rw-r--r--   0        0        0    12191 2024-05-28 19:02:33.453181 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
+-rw-r--r--   0        0        0    11725 2024-05-28 19:02:33.453440 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
+-rw-r--r--   0        0        0    18694 2024-05-28 19:02:33.453711 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
+-rw-r--r--   0        0        0    18901 2024-05-28 19:02:33.454170 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
+-rw-r--r--   0        0        0    15628 2024-05-28 19:02:33.454546 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
+-rw-r--r--   0        0        0     7222 2024-05-28 19:02:33.454964 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
+-rw-r--r--   0        0        0     9736 2024-05-28 19:02:33.455341 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
+-rw-r--r--   0        0        0    13608 2024-05-28 19:02:33.455615 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
+-rw-r--r--   0        0        0     9717 2024-05-28 19:02:33.455874 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
+-rw-r--r--   0        0        0    10020 2024-05-28 19:02:33.456124 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
+-rw-r--r--   0        0        0    17371 2024-05-28 19:02:33.456367 pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.111033 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/__init__.py
+-rw-r--r--   0        0        0     6807 2024-05-28 19:02:33.456696 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
+-rw-r--r--   0        0        0     9508 2024-05-28 19:02:33.456948 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_external_share.py
+-rw-r--r--   0        0        0     8252 2024-05-28 19:02:33.457222 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
+-rw-r--r--   0        0        0    11156 2024-05-28 19:02:33.457648 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
+-rw-r--r--   0        0        0     5145 2024-05-28 19:02:33.457953 pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.111687 pypanther-0.1.1a9/pypanther/rules/duo_rules/__init__.py
+-rw-r--r--   0        0        0     2102 2024-05-28 19:02:33.458274 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
+-rw-r--r--   0        0        0     2189 2024-05-28 19:02:33.458612 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
+-rw-r--r--   0        0        0     2258 2024-05-28 19:02:33.458892 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
+-rw-r--r--   0        0        0     2255 2024-05-28 19:02:33.459384 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_create_admin.py
+-rw-r--r--   0        0        0     2522 2024-05-28 19:02:33.459616 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_lockout.py
+-rw-r--r--   0        0        0     2672 2024-05-28 19:02:33.459844 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
+-rw-r--r--   0        0        0     1982 2024-05-28 19:02:33.460083 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
+-rw-r--r--   0        0        0     3158 2024-05-28 19:02:33.460337 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
+-rw-r--r--   0        0        0     2222 2024-05-28 19:02:33.460724 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_policy_updated.py
+-rw-r--r--   0        0        0     3390 2024-05-28 19:02:33.460985 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
+-rw-r--r--   0        0        0     2916 2024-05-28 19:02:33.461219 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
+-rw-r--r--   0        0        0     2042 2024-05-28 19:02:33.461496 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
+-rw-r--r--   0        0        0     3166 2024-05-28 19:02:33.461791 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_anomalous_push.py
+-rw-r--r--   0        0        0     3072 2024-05-28 19:02:33.462239 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
+-rw-r--r--   0        0        0     5464 2024-05-28 19:02:33.462711 pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.113049 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/__init__.py
+-rw-r--r--   0        0        0     9853 2024-05-28 19:02:33.463173 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
+-rw-r--r--   0        0        0    12347 2024-05-28 19:02:33.463465 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
+-rw-r--r--   0        0        0     7059 2024-05-28 19:02:33.463940 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
+-rw-r--r--   0        0        0     7853 2024-05-28 19:02:33.464337 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
+-rw-r--r--   0        0        0     4141 2024-05-28 19:02:33.464719 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
+-rw-r--r--   0        0        0     4141 2024-05-28 19:02:33.465002 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
+-rw-r--r--   0        0        0    19142 2024-05-28 19:02:33.465280 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
+-rw-r--r--   0        0        0    10446 2024-05-28 19:02:33.465578 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
+-rw-r--r--   0        0        0    15447 2024-05-28 19:02:33.465896 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
+-rw-r--r--   0        0        0     9163 2024-05-28 19:02:33.468285 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
+-rw-r--r--   0        0        0     6832 2024-05-28 19:02:33.468601 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
+-rw-r--r--   0        0        0     8955 2024-05-28 19:02:33.468922 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
+-rw-r--r--   0        0        0     3845 2024-05-28 19:02:33.469251 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
+-rw-r--r--   0        0        0     4541 2024-05-28 19:02:33.469556 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
+-rw-r--r--   0        0        0    15807 2024-05-28 19:02:33.469834 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
+-rw-r--r--   0        0        0     5283 2024-05-28 19:02:33.470296 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
+-rw-r--r--   0        0        0     9955 2024-05-28 19:02:33.470775 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
+-rw-r--r--   0        0        0     3593 2024-05-28 19:02:33.471106 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
+-rw-r--r--   0        0        0     4129 2024-05-28 19:02:33.471454 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
+-rw-r--r--   0        0        0     6799 2024-05-28 19:02:33.471944 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
+-rw-r--r--   0        0        0     6599 2024-05-28 19:02:33.472367 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
+-rw-r--r--   0        0        0     7318 2024-05-28 19:02:33.473111 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
+-rw-r--r--   0        0        0     9277 2024-05-28 19:02:33.473482 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
+-rw-r--r--   0        0        0    11308 2024-05-28 19:02:33.473855 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
+-rw-r--r--   0        0        0     7629 2024-05-28 19:02:33.474099 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
+-rw-r--r--   0        0        0     7093 2024-05-28 19:02:33.474472 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
+-rw-r--r--   0        0        0    10621 2024-05-28 19:02:33.474795 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
+-rw-r--r--   0        0        0     4082 2024-05-28 19:02:33.475121 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
+-rw-r--r--   0        0        0     7728 2024-05-28 19:02:33.475371 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
+-rw-r--r--   0        0        0    11756 2024-05-28 19:02:33.475783 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
+-rw-r--r--   0        0        0    10830 2024-05-28 19:02:33.476061 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
+-rw-r--r--   0        0        0     2289 2024-05-28 19:02:33.476301 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
+-rw-r--r--   0        0        0     2925 2024-05-28 19:02:33.476628 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
+-rw-r--r--   0        0        0    13072 2024-05-28 19:02:33.476936 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
+-rw-r--r--   0        0        0    10924 2024-05-28 19:02:33.477368 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
+-rw-r--r--   0        0        0     9640 2024-05-28 19:02:33.477654 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
+-rw-r--r--   0        0        0    10178 2024-05-28 19:02:33.478042 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
+-rw-r--r--   0        0        0    11781 2024-05-28 19:02:33.478319 pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.118371 pypanther-0.1.1a9/pypanther/rules/gcp_http_lb_rules/__init__.py
+-rw-r--r--   0        0        0     5922 2024-05-28 19:02:33.478642 pypanther-0.1.1a9/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.118592 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/__init__.py
+-rw-r--r--   0        0        0     4573 2024-05-28 19:02:33.478953 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
+-rw-r--r--   0        0        0     6715 2024-05-28 19:02:33.479218 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
+-rw-r--r--   0        0        0     2265 2024-05-28 19:02:33.479472 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
+-rw-r--r--   0        0        0     3544 2024-05-28 19:02:33.479706 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
+-rw-r--r--   0        0        0     3447 2024-05-28 19:02:33.479939 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
+-rw-r--r--   0        0        0    12881 2024-05-28 19:02:33.480201 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
+-rw-r--r--   0        0        0     3513 2024-05-28 19:02:33.480553 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
+-rw-r--r--   0        0        0    14892 2024-05-28 19:02:33.480799 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
+-rw-r--r--   0        0        0    11476 2024-05-28 19:02:33.481053 pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.119696 pypanther-0.1.1a9/pypanther/rules/github_rules/__init__.py
+-rw-r--r--   0        0        0     5255 2024-05-28 19:02:33.481294 pypanther-0.1.1a9/pypanther/rules/github_rules/github_action_failed.py
+-rw-r--r--   0        0        0    14206 2024-05-28 19:02:33.481529 pypanther-0.1.1a9/pypanther/rules/github_rules/github_advanced_security_change.py
+-rw-r--r--   0        0        0     2042 2024-05-28 19:02:33.481725 pypanther-0.1.1a9/pypanther/rules/github_rules/github_branch_policy_override.py
+-rw-r--r--   0        0        0     2044 2024-05-28 19:02:33.481924 pypanther-0.1.1a9/pypanther/rules/github_rules/github_branch_protection_disabled.py
+-rw-r--r--   0        0        0     2237 2024-05-28 19:02:33.482157 pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_auth_modified.py
+-rw-r--r--   0        0        0     2423 2024-05-28 19:02:33.482387 pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_ip_allowlist.py
+-rw-r--r--   0        0        0     2226 2024-05-28 19:02:33.482613 pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_moderators_add.py
+-rw-r--r--   0        0        0     2316 2024-05-28 19:02:33.482963 pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_modified.py
+-rw-r--r--   0        0        0     3395 2024-05-28 19:02:33.483236 pypanther-0.1.1a9/pypanther/rules/github_rules/github_organization_app_integration_installed.py
+-rw-r--r--   0        0        0     2861 2024-05-28 19:02:33.483473 pypanther-0.1.1a9/pypanther/rules/github_rules/github_public_repository_created.py
+-rw-r--r--   0        0        0     2776 2024-05-28 19:02:33.483745 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_collaborator_change.py
+-rw-r--r--   0        0        0     1460 2024-05-28 19:02:33.483998 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_created.py
+-rw-r--r--   0        0        0     2515 2024-05-28 19:02:33.484232 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_hook_modified.py
+-rw-r--r--   0        0        0     4225 2024-05-28 19:02:33.484516 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_initial_access.py
+-rw-r--r--   0        0        0     1904 2024-05-28 19:02:33.484804 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_visibility_change.py
+-rw-r--r--   0        0        0     5342 2024-05-28 19:02:33.485101 pypanther-0.1.1a9/pypanther/rules/github_rules/github_repository_transfer.py
+-rw-r--r--   0        0        0     3334 2024-05-28 19:02:33.485353 pypanther-0.1.1a9/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
+-rw-r--r--   0        0        0     3340 2024-05-28 19:02:33.485586 pypanther-0.1.1a9/pypanther/rules/github_rules/github_team_modified.py
+-rw-r--r--   0        0        0     1636 2024-05-28 19:02:33.486001 pypanther-0.1.1a9/pypanther/rules/github_rules/github_user_access_key_created.py
+-rw-r--r--   0        0        0     1739 2024-05-28 19:02:33.486257 pypanther-0.1.1a9/pypanther/rules/github_rules/github_user_role_updated.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.121588 pypanther-0.1.1a9/pypanther/rules/gitlab_rules/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-28 19:02:33.486513 pypanther-0.1.1a9/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0     2803 2024-05-28 19:02:33.486776 pypanther-0.1.1a9/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.121882 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/__init__.py
+-rw-r--r--   0        0        0     2535 2024-05-28 19:02:33.487032 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
+-rw-r--r--   0        0        0     2645 2024-05-28 19:02:33.487422 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
+-rw-r--r--   0        0        0     3202 2024-05-28 19:02:33.487662 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
+-rw-r--r--   0        0        0     2961 2024-05-28 19:02:33.487890 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
+-rw-r--r--   0        0        0     1763 2024-05-28 19:02:33.488125 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
+-rw-r--r--   0        0        0     6379 2024-05-28 19:02:33.488399 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
+-rw-r--r--   0        0        0     4730 2024-05-28 19:02:33.488631 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
+-rw-r--r--   0        0        0     1607 2024-05-28 19:02:33.488882 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
+-rw-r--r--   0        0        0     2204 2024-05-28 19:02:33.489120 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
+-rw-r--r--   0        0        0     1628 2024-05-28 19:02:33.489351 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
+-rw-r--r--   0        0        0     2753 2024-05-28 19:02:33.489603 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
+-rw-r--r--   0        0        0     4443 2024-05-28 19:02:33.489870 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
+-rw-r--r--   0        0        0     3219 2024-05-28 19:02:33.490083 pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.123166 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/__init__.py
+-rw-r--r--   0        0        0     4374 2024-05-28 19:02:33.490340 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
+-rw-r--r--   0        0        0     6493 2024-05-28 19:02:33.490605 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
+-rw-r--r--   0        0        0     6706 2024-05-28 19:02:33.490863 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
+-rw-r--r--   0        0        0     5283 2024-05-28 19:02:33.491281 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
+-rw-r--r--   0        0        0     4645 2024-05-28 19:02:33.491620 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
+-rw-r--r--   0        0        0     1961 2024-05-28 19:02:33.491916 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
+-rw-r--r--   0        0        0     5786 2024-05-28 19:02:33.492216 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
+-rw-r--r--   0        0        0     2339 2024-05-28 19:02:33.492460 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
+-rw-r--r--   0        0        0     4338 2024-05-28 19:02:33.492727 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
+-rw-r--r--   0        0        0     1465 2024-05-28 19:02:33.493018 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
+-rw-r--r--   0        0        0     1998 2024-05-28 19:02:33.493278 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
+-rw-r--r--   0        0        0     1963 2024-05-28 19:02:33.493677 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
+-rw-r--r--   0        0        0     3049 2024-05-28 19:02:33.493888 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
+-rw-r--r--   0        0        0     3473 2024-05-28 19:02:33.494124 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
+-rw-r--r--   0        0        0     2742 2024-05-28 19:02:33.494340 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
+-rw-r--r--   0        0        0     3387 2024-05-28 19:02:33.494569 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
+-rw-r--r--   0        0        0     2020 2024-05-28 19:02:33.494866 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
+-rw-r--r--   0        0        0     3457 2024-05-28 19:02:33.495107 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
+-rw-r--r--   0        0        0     2587 2024-05-28 19:02:33.495369 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
+-rw-r--r--   0        0        0     2203 2024-05-28 19:02:33.495610 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
+-rw-r--r--   0        0        0     2721 2024-05-28 19:02:33.495829 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
+-rw-r--r--   0        0        0     6834 2024-05-28 19:02:33.496095 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
+-rw-r--r--   0        0        0     5013 2024-05-28 19:02:33.496553 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
+-rw-r--r--   0        0        0     6052 2024-05-28 19:02:33.496812 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
+-rw-r--r--   0        0        0     5452 2024-05-28 19:02:33.497085 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
+-rw-r--r--   0        0        0     5222 2024-05-28 19:02:33.497344 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
+-rw-r--r--   0        0        0     5172 2024-05-28 19:02:33.497578 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
+-rw-r--r--   0        0        0     4977 2024-05-28 19:02:33.497796 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
+-rw-r--r--   0        0        0     5223 2024-05-28 19:02:33.498036 pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.126155 pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/__init__.py
+-rw-r--r--   0        0        0    10551 2024-05-28 19:02:33.498310 pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
+-rw-r--r--   0        0        0     4560 2024-05-28 19:02:33.498575 pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
+-rw-r--r--   0        0        0    25458 2024-05-28 19:02:33.498809 pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.126690 pypanther-0.1.1a9/pypanther/rules/indicator_creation_rules/__init__.py
+-rw-r--r--   0        0        0     4663 2024-05-28 19:02:33.499301 pypanther-0.1.1a9/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
+-rw-r--r--   0        0        0     4410 2024-05-28 19:02:33.499549 pypanther-0.1.1a9/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.127036 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/__init__.py
+-rw-r--r--   0        0        0     4583 2024-05-28 19:02:33.499800 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
+-rw-r--r--   0        0        0     9682 2024-05-28 19:02:33.500038 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
+-rw-r--r--   0        0        0     6315 2024-05-28 19:02:33.500290 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
+-rw-r--r--   0        0        0    10184 2024-05-28 19:02:33.500537 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
+-rw-r--r--   0        0        0     5172 2024-05-28 19:02:33.500823 pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.127867 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-28 19:02:33.501070 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
+-rw-r--r--   0        0        0     2868 2024-05-28 19:02:33.501281 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
+-rw-r--r--   0        0        0     2711 2024-05-28 19:02:33.501503 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
+-rw-r--r--   0        0        0     4174 2024-05-28 19:02:33.501894 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
+-rw-r--r--   0        0        0     4371 2024-05-28 19:02:33.502158 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
+-rw-r--r--   0        0        0     3958 2024-05-28 19:02:33.502391 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
+-rw-r--r--   0        0        0     2284 2024-05-28 19:02:33.502622 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
+-rw-r--r--   0        0        0     3355 2024-05-28 19:02:33.502848 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
+-rw-r--r--   0        0        0     3215 2024-05-28 19:02:33.503078 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
+-rw-r--r--   0        0        0     4770 2024-05-28 19:02:33.503467 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
+-rw-r--r--   0        0        0     3435 2024-05-28 19:02:33.503771 pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.129134 pypanther-0.1.1a9/pypanther/rules/netskope_rules/__init__.py
+-rw-r--r--   0        0        0     2988 2024-05-28 19:02:33.504008 pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
+-rw-r--r--   0        0        0     3570 2024-05-28 19:02:33.504264 pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_admin_user_change.py
+-rw-r--r--   0        0        0     2727 2024-05-28 19:02:33.504642 pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_many_deletes.py
+-rw-r--r--   0        0        0     2916 2024-05-28 19:02:33.504894 pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_personnel_action.py
+-rw-r--r--   0        0        0     3173 2024-05-28 19:02:33.505132 pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.129710 pypanther-0.1.1a9/pypanther/rules/notion_rules/__init__.py
+-rw-r--r--   0        0        0    16722 2024-05-28 19:02:33.505395 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_account_changed_after_login.py
+-rw-r--r--   0        0        0     1543 2024-05-28 19:02:33.505617 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
+-rw-r--r--   0        0        0    15424 2024-05-28 19:02:33.505899 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_login_from_new_location.py
+-rw-r--r--   0        0        0     3287 2024-05-28 19:02:33.506103 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_many_pages_deleted.py
+-rw-r--r--   0        0        0     3283 2024-05-28 19:02:33.506312 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_many_pages_exported.py
+-rw-r--r--   0        0        0     1761 2024-05-28 19:02:33.506524 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
+-rw-r--r--   0        0        0     5409 2024-05-28 19:02:33.506846 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
+-rw-r--r--   0        0        0     1655 2024-05-28 19:02:33.507095 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_shared_to_web.py
+-rw-r--r--   0        0        0     2883 2024-05-28 19:02:33.507424 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_scim_token_generated.py
+-rw-r--r--   0        0        0     3886 2024-05-28 19:02:33.507836 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
+-rw-r--r--   0        0        0     4484 2024-05-28 19:02:33.508137 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
+-rw-r--r--   0        0        0     3009 2024-05-28 19:02:33.508375 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
+-rw-r--r--   0        0        0     3278 2024-05-28 19:02:33.508598 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_exported.py
+-rw-r--r--   0        0        0     4562 2024-05-28 19:02:33.508837 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
+-rw-r--r--   0        0        0     4416 2024-05-28 19:02:33.509133 pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.131277 pypanther-0.1.1a9/pypanther/rules/okta_rules/__init__.py
+-rw-r--r--   0        0        0     3638 2024-05-28 19:02:33.509419 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_account_support_access.py
+-rw-r--r--   0        0        0     3489 2024-05-28 19:02:33.509661 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
+-rw-r--r--   0        0        0     7257 2024-05-28 19:02:33.509919 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_admin_role_assigned.py
+-rw-r--r--   0        0        0     7639 2024-05-28 19:02:33.510167 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
+-rw-r--r--   0        0        0     2652 2024-05-28 19:02:33.510428 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_api_key_created.py
+-rw-r--r--   0        0        0     2497 2024-05-28 19:02:33.510675 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_api_key_revoked.py
+-rw-r--r--   0        0        0     9056 2024-05-28 19:02:33.510973 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
+-rw-r--r--   0        0        0     7529 2024-05-28 19:02:33.511242 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
+-rw-r--r--   0        0        0     7410 2024-05-28 19:02:33.511502 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
+-rw-r--r--   0        0        0     8146 2024-05-28 19:02:33.511745 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_idp_create_modify.py
+-rw-r--r--   0        0        0     8236 2024-05-28 19:02:33.512000 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_idp_signin.py
+-rw-r--r--   0        0        0    13827 2024-05-28 19:02:33.512351 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
+-rw-r--r--   0        0        0    13471 2024-05-28 19:02:33.512634 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
+-rw-r--r--   0        0        0    10950 2024-05-28 19:02:33.513023 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_password_accessed.py
+-rw-r--r--   0        0        0     7723 2024-05-28 19:02:33.513323 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
+-rw-r--r--   0        0        0     7666 2024-05-28 19:02:33.513593 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
+-rw-r--r--   0        0        0    19411 2024-05-28 19:02:33.513861 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
+-rw-r--r--   0        0        0    10701 2024-05-28 19:02:33.514125 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_rate_limits.py
+-rw-r--r--   0        0        0     5009 2024-05-28 19:02:33.514382 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_support_reset.py
+-rw-r--r--   0        0        0     9212 2024-05-28 19:02:33.514779 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
+-rw-r--r--   0        0        0     6860 2024-05-28 19:02:33.515040 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_account_locked.py
+-rw-r--r--   0        0        0     7020 2024-05-28 19:02:33.515276 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
+-rw-r--r--   0        0        0     4184 2024-05-28 19:02:33.515527 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_reset.py
+-rw-r--r--   0        0        0     5466 2024-05-28 19:02:33.515754 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
+-rw-r--r--   0        0        0     8402 2024-05-28 19:02:33.516379 pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.134657 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/__init__.py
+-rw-r--r--   0        0        0     3854 2024-05-28 19:02:33.516838 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
+-rw-r--r--   0        0        0     1969 2024-05-28 19:02:33.517121 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
+-rw-r--r--   0        0        0     2487 2024-05-28 19:02:33.517410 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
+-rw-r--r--   0        0        0     2294 2024-05-28 19:02:33.517675 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
+-rw-r--r--   0        0        0     2201 2024-05-28 19:02:33.517936 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_password_changed.py
+-rw-r--r--   0        0        0     2670 2024-05-28 19:02:33.518183 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
+-rw-r--r--   0        0        0     1893 2024-05-28 19:02:33.518410 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
+-rw-r--r--   0        0        0     1935 2024-05-28 19:02:33.518641 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
+-rw-r--r--   0        0        0     1862 2024-05-28 19:02:33.518848 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
+-rw-r--r--   0        0        0     2559 2024-05-28 19:02:33.519057 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
+-rw-r--r--   0        0        0     2009 2024-05-28 19:02:33.519256 pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.135637 pypanther-0.1.1a9/pypanther/rules/onepassword_rules/__init__.py
+-rw-r--r--   0        0        0     4579 2024-05-28 19:02:33.519520 pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
+-rw-r--r--   0        0        0     3931 2024-05-28 19:02:33.519725 pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
+-rw-r--r--   0        0        0     4441 2024-05-28 19:02:33.519946 pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.136004 pypanther-0.1.1a9/pypanther/rules/osquery_rules/__init__.py
+-rw-r--r--   0        0        0     4052 2024-05-28 19:02:33.520156 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
+-rw-r--r--   0        0        0     3412 2024-05-28 19:02:33.520368 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
+-rw-r--r--   0        0        0     3594 2024-05-28 19:02:33.520617 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
+-rw-r--r--   0        0        0     2979 2024-05-28 19:02:33.520864 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
+-rw-r--r--   0        0        0     2610 2024-05-28 19:02:33.521087 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
+-rw-r--r--   0        0        0     2217 2024-05-28 19:02:33.521327 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
+-rw-r--r--   0        0        0     4071 2024-05-28 19:02:33.521556 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
+-rw-r--r--   0        0        0     3684 2024-05-28 19:02:33.521763 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
+-rw-r--r--   0        0        0     3486 2024-05-28 19:02:33.521987 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_ossec.py
+-rw-r--r--   0        0        0     3559 2024-05-28 19:02:33.522578 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_outdated.py
+-rw-r--r--   0        0        0     3688 2024-05-28 19:02:33.522871 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_outdated_macos.py
+-rw-r--r--   0        0        0     3744 2024-05-28 19:02:33.523326 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_ssh_listener.py
+-rw-r--r--   0        0        0     5597 2024-05-28 19:02:33.523577 pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.137303 pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/__init__.py
+-rw-r--r--   0        0        0     4586 2024-05-28 19:02:33.523833 pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
+-rw-r--r--   0        0        0     2534 2024-05-28 19:02:33.524044 pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_saml_modified.py
+-rw-r--r--   0        0        0     8369 2024-05-28 19:02:33.524279 pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
+-rw-r--r--   0        0        0     9726 2024-05-28 19:02:33.524669 pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_user_modified.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.137903 pypanther-0.1.1a9/pypanther/rules/salesforce_rules/__init__.py
+-rw-r--r--   0        0        0     4586 2024-05-28 19:02:33.524942 pypanther-0.1.1a9/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.138119 pypanther-0.1.1a9/pypanther/rules/sentinelone_rules/__init__.py
+-rw-r--r--   0        0        0     7224 2024-05-28 19:02:33.525188 pypanther-0.1.1a9/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
+-rw-r--r--   0        0        0     6482 2024-05-28 19:02:33.525445 pypanther-0.1.1a9/pypanther/rules/sentinelone_rules/sentinelone_threats.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.138439 pypanther-0.1.1a9/pypanther/rules/slack_rules/__init__.py
+-rw-r--r--   0        0        0    10111 2024-05-28 19:02:33.525756 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_access_expanded.py
+-rw-r--r--   0        0        0     8853 2024-05-28 19:02:33.526140 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_added.py
+-rw-r--r--   0        0        0     6590 2024-05-28 19:02:33.526395 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_removed.py
+-rw-r--r--   0        0        0     4682 2024-05-28 19:02:33.526724 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_application_dos.py
+-rw-r--r--   0        0        0     4947 2024-05-28 19:02:33.527012 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_dlp_modified.py
+-rw-r--r--   0        0        0     3486 2024-05-28 19:02:33.527253 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_config_changed.py
+-rw-r--r--   0        0        0     3429 2024-05-28 19:02:33.527611 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
+-rw-r--r--   0        0        0     3334 2024-05-28 19:02:33.527871 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
+-rw-r--r--   0        0        0     5895 2024-05-28 19:02:33.528135 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_idp_configuration_change.py
+-rw-r--r--   0        0        0     4701 2024-05-28 19:02:33.528382 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_information_barrier_modified.py
+-rw-r--r--   0        0        0     3331 2024-05-28 19:02:33.528614 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
+-rw-r--r--   0        0        0     6999 2024-05-28 19:02:33.528953 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
+-rw-r--r--   0        0        0     3454 2024-05-28 19:02:33.529200 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
+-rw-r--r--   0        0        0     2843 2024-05-28 19:02:33.529472 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_org_created.py
+-rw-r--r--   0        0        0     2843 2024-05-28 19:02:33.529738 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_org_deleted.py
+-rw-r--r--   0        0        0     3315 2024-05-28 19:02:33.529995 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
+-rw-r--r--   0        0        0     3412 2024-05-28 19:02:33.530230 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
+-rw-r--r--   0        0        0     3592 2024-05-28 19:02:33.530468 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_private_channel_made_public.py
+-rw-r--r--   0        0        0     4151 2024-05-28 19:02:33.530743 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
+-rw-r--r--   0        0        0     3557 2024-05-28 19:02:33.530973 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_service_owner_transferred.py
+-rw-r--r--   0        0        0     3399 2024-05-28 19:02:33.531178 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_sso_settings_changed.py
+-rw-r--r--   0        0        0     7399 2024-05-28 19:02:33.531432 pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.140617 pypanther-0.1.1a9/pypanther/rules/snyk_rules/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-28 19:02:33.531661 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_misc_settings.py
+-rw-r--r--   0        0        0     4571 2024-05-28 19:02:33.531900 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_org_settings.py
+-rw-r--r--   0        0        0     4568 2024-05-28 19:02:33.532162 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_ou_change.py
+-rw-r--r--   0        0        0     4884 2024-05-28 19:02:33.532428 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_project_settings.py
+-rw-r--r--   0        0        0     5437 2024-05-28 19:02:33.532671 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_role_change.py
+-rw-r--r--   0        0        0    12027 2024-05-28 19:02:33.532922 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_svcacct_change.py
+-rw-r--r--   0        0        0     3971 2024-05-28 19:02:33.533349 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
+-rw-r--r--   0        0        0     6266 2024-05-28 19:02:33.533638 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_policysetting.py
+-rw-r--r--   0        0        0     2578 2024-05-28 19:02:33.533906 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_sso.py
+-rw-r--r--   0        0        0     5851 2024-05-28 19:02:33.534191 pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_user_mgmt.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.141863 pypanther-0.1.1a9/pypanther/rules/standard_rules/__init__.py
+-rw-r--r--   0        0        0    10991 2024-05-28 19:02:33.534500 pypanther-0.1.1a9/pypanther/rules/standard_rules/admin_assigned.py
+-rw-r--r--   0        0        0    16955 2024-05-28 19:02:33.534791 pypanther-0.1.1a9/pypanther/rules/standard_rules/brute_force_by_ip.py
+-rw-r--r--   0        0        0    36758 2024-05-28 19:02:33.535233 pypanther-0.1.1a9/pypanther/rules/standard_rules/impossible_travel_login.py
+-rw-r--r--   0        0        0     9779 2024-05-28 19:02:33.535518 pypanther-0.1.1a9/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
+-rw-r--r--   0        0        0     8225 2024-05-28 19:02:33.535777 pypanther-0.1.1a9/pypanther/rules/standard_rules/mfa_disabled.py
+-rw-r--r--   0        0        0     9943 2024-05-28 19:02:33.536054 pypanther-0.1.1a9/pypanther/rules/standard_rules/standard_dns_base64.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.142861 pypanther-0.1.1a9/pypanther/rules/tailscale_rules/__init__.py
+-rw-r--r--   0        0        0     4649 2024-05-28 19:02:33.536425 pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
+-rw-r--r--   0        0        0     4885 2024-05-28 19:02:33.536687 pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
+-rw-r--r--   0        0        0     4666 2024-05-28 19:02:33.536950 pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.143230 pypanther-0.1.1a9/pypanther/rules/tines_rules/__init__.py
+-rw-r--r--   0        0        0     2584 2024-05-28 19:02:33.537183 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
+-rw-r--r--   0        0        0     2824 2024-05-28 19:02:33.537416 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_custom_ca.py
+-rw-r--r--   0        0        0     3540 2024-05-28 19:02:33.537640 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
+-rw-r--r--   0        0        0     2887 2024-05-28 19:02:33.537876 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_global_resource_destruction.py
+-rw-r--r--   0        0        0     2947 2024-05-28 19:02:33.538113 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_sso_settings.py
+-rw-r--r--   0        0        0     2765 2024-05-28 19:02:33.538333 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_story_items_destruction.py
+-rw-r--r--   0        0        0     2735 2024-05-28 19:02:33.538539 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
+-rw-r--r--   0        0        0     2680 2024-05-28 19:02:33.538771 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_team_destruction.py
+-rw-r--r--   0        0        0     3987 2024-05-28 19:02:33.539254 pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_tenant_authtoken.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.144069 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/__init__.py
+-rw-r--r--   0        0        0     3775 2024-05-28 19:02:33.539579 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
+-rw-r--r--   0        0        0     2972 2024-05-28 19:02:33.539811 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
+-rw-r--r--   0        0        0     3208 2024-05-28 19:02:33.540006 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_new_owner.py
+-rw-r--r--   0        0        0     3717 2024-05-28 19:02:33.540216 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
+-rw-r--r--   0        0        0     2962 2024-05-28 19:02:33.540422 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
+-rw-r--r--   0        0        0     2774 2024-05-28 19:02:33.540679 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_role.py
+-rw-r--r--   0        0        0     3927 2024-05-28 19:02:33.540886 pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
+-rw-r--r--   0        0        0        0 2024-05-23 22:40:02.144949 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-28 19:02:33.541119 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
+-rw-r--r--   0        0        0     2359 2024-05-28 19:02:33.541342 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
+-rw-r--r--   0        0        0     2830 2024-05-28 19:02:33.541571 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
+-rw-r--r--   0        0        0     2760 2024-05-28 19:02:33.541784 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
+-rw-r--r--   0        0        0     3358 2024-05-28 19:02:33.542013 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
+-rw-r--r--   0        0        0     3558 2024-05-28 19:02:33.542213 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
+-rw-r--r--   0        0        0     2620 2024-05-28 19:02:33.542453 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
+-rw-r--r--   0        0        0     4620 2024-05-28 19:02:33.542768 pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
+-rw-r--r--   0        0        0     4251 2024-05-28 19:02:33.543103 pypanther-0.1.1a9/pypanther/upload.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:55:34.856583 pypanther-0.1.1a9/pypanther/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:55:34.856930 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:55:34.857033 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/__init__.py
+-rw-r--r--   0        0        0    16541 2024-05-28 17:53:54.391608 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/client.py
+-rw-r--r--   0        0        0      624 2024-05-24 15:55:34.857276 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/errors.py
+-rw-r--r--   0        0        0      159 2024-05-24 15:55:34.857420 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
+-rw-r--r--   0        0        0      802 2024-05-24 15:55:34.857511 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
+-rw-r--r--   0        0        0     1439 2024-05-28 16:14:33.845103 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql
+-rw-r--r--   0        0        0    25446 2024-05-28 17:58:55.813542 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
+-rw-r--r--   0        0        0     1606 2024-05-24 15:55:34.857904 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/cli_output.py
+-rw-r--r--   0        0        0      493 2024-05-28 19:02:33.543543 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/command/standard_args.py
+-rw-r--r--   0        0        0     1308 2024-05-28 19:02:33.544297 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/config.py
+-rw-r--r--   0        0        0      714 2024-05-28 19:02:33.544534 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/constants.py
+-rw-r--r--   0        0        0     2008 2024-05-28 19:02:33.544794 pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/util.py
+-rw-r--r--   0        0        0      274 2024-05-23 22:40:02.145879 pypanther-0.1.1a9/pypanther/wrap.py
+-rw-r--r--   0        0        0     1775 2024-05-28 22:43:21.993213 pypanther-0.1.1a9/pyproject.toml
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pypanther-0.1.1a9/PKG-INFO
```

### Comparing `pypanther-0.1.1a8/LICENSE.txt` & `pypanther-0.1.1a9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/base.py` & `pypanther-0.1.1a9/pypanther/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,41 @@
         return {key: try_asdict(getattr(cls, key)) for key in PANTHER_RULE_ALL_ATTRS}
 
     @classmethod
     def validate(cls):
         PantherRuleAdapter.validate_python(cls.asdict())
 
     @classmethod
+    def override(
+        cls,
+        LogTypes: Optional[List[str]] = None,
+        RuleID: Optional[str] = None,
+        Severity: Optional[PantherSeverity] = None,
+        Enabled: Optional[bool] = None,
+        Tags: Optional[List[str]] = None,
+        DedupPeriodMinutes: Optional[NonNegativeInt] = None,
+        Description: Optional[str] = None,
+        DisplayName: Optional[str] = None,
+        OutputIds: Optional[List[str]] = None,
+        Reference: Optional[str] = None,
+        Reports: Optional[Dict[str, List[str]]] = None,
+        Runbook: Optional[str] = None,
+        ScheduledQueries: Optional[List[str]] = None,
+        SummaryAttributes: Optional[List[str]] = None,
+        Tests: Optional[List[PantherRuleTest]] = None,
+        Threshold: Optional[PositiveInt] = None,
+    ):
+        for key, val in locals().items():
+            if key == "cls":
+                continue
+
+            if val is not None:
+                setattr(cls, key, val)
+
+    @classmethod
     def run_tests(
         cls,
         get_data_model: Callable[[str], Optional[DataModel]],
     ):
         cls.validate()
         rule = cls()
         for test in rule.Tests:
@@ -440,15 +467,19 @@
             for p in patches:
                 p.stop()
 
     def is_method_defined(self, name: str) -> bool:
         return callable(getattr(self, name))
 
     def run(
-        self, event: PantherEvent, outputs: Dict, outputs_names: Dict, batch_mode: bool = True
+        self,
+        event: PantherEvent,
+        outputs: Dict,
+        outputs_names: Dict,
+        batch_mode: bool = True,
     ) -> DetectionResult:
         result = DetectionResult(
             detection_id=self.RuleID,
             detection_severity=self.Severity,
             detection_type=TYPE_RULE,
             # set default to not alert
             trigger_alert=False,
```

### Comparing `pypanther-0.1.1a8/pypanther/data_models/asana_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/asana_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/atlassian_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/atlassian_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_alb_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_alb_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_cloudtrail_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_cloudtrail_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_eks_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_eks_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_s3_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_s3_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_vpcdns_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_vpcdns_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/aws_vpcflow_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/aws_vpcflow_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/azure_signin_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/azure_signin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/box_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/box_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/cisco_umbrella_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/cisco_umbrella_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/cloudflare_firewall_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/cloudflare_firewall_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/cloudflare_httpreq_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/cloudflare_httpreq_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/crowdstrike_fdr_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/crowdstrike_fdr_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/gcp_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/gcp_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/github_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/github_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/gsuite_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/gsuite_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/notion_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/notion_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/okta_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/okta_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/onelogin_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/onelogin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/onepassword_itemusage_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/onepassword_itemusage_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/onepassword_signinattempt_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/onepassword_signinattempt_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/panther_audit_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/panther_audit_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/slack_accesslogs_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/slack_accesslogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/slack_auditlogs_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/slack_auditlogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/zendesk_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/zendesk_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/zoom_activity_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/zoom_activity_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/data_models/zoom_operation_data_model.py` & `pypanther-0.1.1a9/pypanther/data_models/zoom_operation_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/get.py` & `pypanther-0.1.1a9/pypanther/get.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/gcp_base_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/gcp_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/gcp_environment.py` & `pypanther-0.1.1a9/pypanther/helpers/gcp_environment.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_asana_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_asana_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_audit.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_audit.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_auth0_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_auth0_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_azuresignin_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_azuresignin_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_base_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_box_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_box_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_cloudflare_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_cloudflare_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_config_defaults.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_config_defaults.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_config_overrides.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_config_overrides.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_default.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_default.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_duo_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_duo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_event_type_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_event_type_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_greynoise_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_greynoise_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_iocs.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_iocs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_ipinfo_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_ipinfo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_lookuptable_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_lookuptable_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_oss_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_oss_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_snyk_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_snyk_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_tines_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_tines_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_tor_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_tor_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/helpers/panther_zoom_helpers.py` & `pypanther-0.1.1a9/pypanther/helpers/panther_zoom_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/log_types.py` & `pypanther-0.1.1a9/pypanther/log_types.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/main.py` & `pypanther-0.1.1a9/pypanther/main.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/register.py` & `pypanther-0.1.1a9/pypanther/register.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_service_account_created.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_service_account_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_team_privacy_public.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_team_privacy_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_new_admin.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_new_admin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_org_export.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_org_export.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/asana_rules/asana_workspace_saml_optional.py` & `pypanther-0.1.1a9/pypanther/rules/asana_rules/asana_workspace_saml_optional.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/atlassian_rules/user_logged_in_as_user.py` & `pypanther-0.1.1a9/pypanther/rules/atlassian_rules/user_logged_in_as_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_custom_role_created.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_custom_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_integration_installed.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_integration_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_invitation_created.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_user_invitation_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py` & `pypanther-0.1.1a9/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py` & `pypanther-0.1.1a9/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py` & `pypanther-0.1.1a9/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py` & `pypanther-0.1.1a9/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py` & `pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py` & `pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py` & `pypanther-0.1.1a9/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_error.py` & `pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_access_error.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py` & `pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py` & `pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py` & `pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py` & `pypanther-0.1.1a9/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py` & `pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py` & `pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py` & `pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py` & `pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py` & `pypanther-0.1.1a9/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_failed_signins.py` & `pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_failed_signins.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_legacyauth.py` & `pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_legacyauth.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py` & `pypanther-0.1.1a9/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_access_granted.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_access_granted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_anomalous_download.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_anomalous_download.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_event_triggered_externally.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_event_triggered_externally.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_item_shared_externally.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_item_shared_externally.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_malicious_content.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_malicious_content.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_new_login.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_new_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_policy_violation.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_policy_violation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_suspicious_login_or_session.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_suspicious_login_or_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_untrusted_device.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_untrusted_device.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_downloads.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_user_downloads.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/box_rules/box_user_permission_updates.py` & `pypanther-0.1.1a9/pypanther/rules/box_rules/box_user_permission_updates.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_flagged.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_flagged.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/carbonblack_rules/cb_passthrough.py` & `pypanther-0.1.1a9/pypanther/rules/carbonblack_rules/cb_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py` & `pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py` & `pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py` & `pypanther-0.1.1a9/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py` & `pypanther-0.1.1a9/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py` & `pypanther-0.1.1a9/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py` & `pypanther-0.1.1a9/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py` & `pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_external_share.py` & `pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_external_share.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py` & `pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py` & `pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py` & `pypanther-0.1.1a9/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_create_admin.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_create_admin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_lockout.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_lockout.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_policy_updated.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_policy_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_action_fraudulent.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_action_fraudulent.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_anomalous_push.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_anomalous_push.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_bypass_code_used.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_bypass_code_used.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py` & `pypanther-0.1.1a9/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py` & `pypanther-0.1.1a9/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_action_failed.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_action_failed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_advanced_security_change.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_advanced_security_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_policy_override.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_branch_policy_override.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_branch_protection_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_branch_protection_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_auth_modified.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_auth_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_ip_allowlist.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_ip_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_moderators_add.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_moderators_add.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_org_modified.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_org_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_organization_app_integration_installed.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_organization_app_integration_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_public_repository_created.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_public_repository_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_collaborator_change.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_collaborator_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_created.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_hook_modified.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_hook_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_initial_access.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_initial_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repo_visibility_change.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repo_visibility_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_repository_transfer.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_repository_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_secret_scanning_alert_created.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_secret_scanning_alert_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_team_modified.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_team_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_access_key_created.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_user_access_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/github_rules/github_user_role_updated.py` & `pypanther-0.1.1a9/pypanther/rules/github_rules/github_user_role_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py` & `pypanther-0.1.1a9/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py` & `pypanther-0.1.1a9/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py` & `pypanther-0.1.1a9/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py` & `pypanther-0.1.1a9/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py` & `pypanther-0.1.1a9/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/indicator_creation_rules/new_user_account_logging.py` & `pypanther-0.1.1a9/pypanther/rules/indicator_creation_rules/new_user_account_logging.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py` & `pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py` & `pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py` & `pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py` & `pypanther-0.1.1a9/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py` & `pypanther-0.1.1a9/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_logged_out.py` & `pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_admin_logged_out.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_admin_user_change.py` & `pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_admin_user_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_many_deletes.py` & `pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_many_deletes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_personnel_action.py` & `pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_personnel_action.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py` & `pypanther-0.1.1a9/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_account_changed_after_login.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_account_changed_after_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_login_from_new_location.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_login_from_new_location.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_many_pages_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_many_pages_exported.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_many_pages_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_api.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_accessible_to_api.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_page_shared_to_web.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_page_shared_to_web.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_scim_token_generated.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_scim_token_generated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_sharing_settings_updated.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_sharing_settings_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_teamspace_owner_added.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_teamspace_owner_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_exported.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py` & `pypanther-0.1.1a9/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_account_support_access.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_account_support_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_admin_role_assigned.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_admin_role_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_created.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_api_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_api_key_revoked.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_api_key_revoked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_create_modify.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_idp_create_modify.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_idp_signin.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_idp_signin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_org2org_creation_modification.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_org2org_creation_modification.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_accessed.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_password_accessed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_potentially_stolen_session.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_potentially_stolen_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_rate_limits.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_rate_limits.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_support_reset.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_support_reset.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_account_locked.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_account_locked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_reset.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py` & `pypanther-0.1.1a9/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_accessed.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_password_accessed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_password_changed.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_password_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onelogin_rules/onelogin_user_assumed.py` & `pypanther-0.1.1a9/pypanther/rules/onelogin_rules/onelogin_user_assumed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py` & `pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py` & `pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/onepassword_rules/onepassword_unusual_client.py` & `pypanther-0.1.1a9/pypanther/rules/onepassword_rules/onepassword_unusual_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ossec.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_ossec.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_outdated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_outdated_macos.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_outdated_macos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_ssh_listener.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_ssh_listener.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/osquery_rules/osquery_suspicious_cron.py` & `pypanther-0.1.1a9/pypanther/rules/osquery_rules/osquery_suspicious_cron.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_detection_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_detection_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_saml_modified.py` & `pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_saml_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py` & `pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/panther_audit_rules/panther_user_modified.py` & `pypanther-0.1.1a9/pypanther/rules/panther_audit_rules/panther_user_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py` & `pypanther-0.1.1a9/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py` & `pypanther-0.1.1a9/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/sentinelone_rules/sentinelone_threats.py` & `pypanther-0.1.1a9/pypanther/rules/sentinelone_rules/sentinelone_threats.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_access_expanded.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_access_expanded.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_added.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_app_removed.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_app_removed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_application_dos.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_application_dos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_dlp_modified.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_dlp_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_config_changed.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_config_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_ekm_unenrolled.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_ekm_unenrolled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_idp_configuration_change.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_idp_configuration_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_information_barrier_modified.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_information_barrier_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_mfa_settings_changed.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_mfa_settings_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_created.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_org_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_org_deleted.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_org_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_passthrough_anomaly.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_passthrough_anomaly.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_private_channel_made_public.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_private_channel_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_service_owner_transferred.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_service_owner_transferred.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_sso_settings_changed.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_sso_settings_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/slack_rules/slack_user_privilege_escalation.py` & `pypanther-0.1.1a9/pypanther/rules/slack_rules/slack_user_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_misc_settings.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_misc_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_org_settings.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_org_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_ou_change.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_ou_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_project_settings.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_project_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_role_change.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_role_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_svcacct_change.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_svcacct_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_externalaccess.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_externalaccess.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_policysetting.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_policysetting.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_system_sso.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_system_sso.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/snyk_rules/snyk_user_mgmt.py` & `pypanther-0.1.1a9/pypanther/rules/snyk_rules/snyk_user_mgmt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/admin_assigned.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/admin_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/brute_force_by_ip.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/brute_force_by_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/impossible_travel_login.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/impossible_travel_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/mfa_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/mfa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/standard_rules/standard_dns_base64.py` & `pypanther-0.1.1a9/pypanther/rules/standard_rules/standard_dns_base64.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_https_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_https_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_actions_disabled_changes.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_actions_disabled_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_custom_ca.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_custom_ca.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_global_resource_destruction.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_global_resource_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_sso_settings.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_sso_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_items_destruction.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_story_items_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_story_jobs_clearance.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_story_jobs_clearance.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_team_destruction.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_team_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/tines_rules/tines_tenant_authtoken.py` & `pypanther-0.1.1a9/pypanther/rules/tines_rules/tines_tenant_authtoken.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_api_token.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_new_api_token.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_new_owner.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_new_owner.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_assumption.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_assumption.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_role.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zendesk_rules/zendesk_user_suspension.py` & `pypanther-0.1.1a9/pypanther/rules/zendesk_rules/zendesk_user_suspension.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py` & `pypanther-0.1.1a9/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/upload.py` & `pypanther-0.1.1a9/pypanther/upload.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/client.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/errors.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/errors.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/cli_output.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/cli_output.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/config.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/config.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/constants.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/constants.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pypanther/vendor/panther_analysis_tool/util.py` & `pypanther-0.1.1a9/pypanther/vendor/panther_analysis_tool/util.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a8/pyproject.toml` & `pypanther-0.1.1a9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypanther"
-version = "0.1.1a8"
+version = "0.1.1a9"
 description = ""
 authors = ["Panther Labs Inc <pypi@runpanther.io>"]
 readme = "README.md"
 keywords = ["Security", "CLI"]
 classifiers = ["Operating System :: OS Independent"]
 license = "AGPL-3.0-only"
 include = ["pypanther/py.typed"]
@@ -66,14 +66,15 @@
 module = "pypanther.rules.*"
 follow_imports = "skip"
 
 [tool.black]
 line-length = 100
 target-version = ['py311']
 include = '\.pyi?$'
+exclude = "pypanther/vendor"
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
```

### Comparing `pypanther-0.1.1a8/PKG-INFO` & `pypanther-0.1.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypanther
-Version: 0.1.1a8
+Version: 0.1.1a9
 Summary: 
 License: AGPL-3.0-only
 Keywords: Security,CLI
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

