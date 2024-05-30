# Comparing `tmp/pulumiverse_zitadel-0.1.7.tar.gz` & `tmp/pulumiverse_zitadel-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_zitadel-0.1.7.tar", last modified: Tue Mar 26 17:19:33 2024, max compression
+gzip compressed data, was "pulumiverse_zitadel-0.1.8.tar", last modified: Thu May 30 09:52:15 2024, max compression
```

## Comparing `pulumiverse_zitadel-0.1.7.tar` & `pulumiverse_zitadel-0.1.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:19:33.642310 pulumiverse_zitadel-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-26 17:19:33.642310 pulumiverse_zitadel-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:19:33.638310 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17390 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    54240 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_saml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:19:33.638310 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_domain_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    54760 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_label_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_lockout_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    63072 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_login_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_oidc_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_password_complexity_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_privacy_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/domain_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_oidcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_samls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_default_oidc_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_human_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (127)    18016 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_machine_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_machine_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_jwt_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_oidc_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_orgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_project_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/human_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    33931 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    26795 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    34673 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)    28893 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (127)    26741 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_google.py
--rw-r--r--   0 runner    (1001) docker     (127)    75757 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/instance_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    56698 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/label_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/lockout_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    64998 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/login_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/machine_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    25437 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/machine_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org.py
--rw-r--r--   0 runner    (1001) docker     (127)    36123 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    28987 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    36859 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_github_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    28935 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)    31085 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py
--rw-r--r--   0 runner    (1001) docker     (127)    28933 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_google.py
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)    77949 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    33859 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    19479 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/password_complexity_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/privacy_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_grant_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/sms_provider_twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/smtp_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/trigger_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/user_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:19:33.638310 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-26 17:19:33.000000 pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 17:19:33.642310 pulumiverse_zitadel-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-26 17:19:32.000000 pulumiverse_zitadel-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17390 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54240 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_domain_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54760 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_label_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_lockout_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63072 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_login_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_oidc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_password_complexity_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_privacy_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/domain_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_oidcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_samls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_default_oidc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_human_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18016 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_machine_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_machine_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_jwt_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_oidc_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_project_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/human_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33931 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26795 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34673 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28893 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26741 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75757 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/instance_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56698 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/label_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/lockout_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64998 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/login_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/machine_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25437 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/machine_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36123 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28987 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36859 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_github_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28935 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31085 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28933 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77949 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33859 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19479 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/password_complexity_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/privacy_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_grant_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/sms_provider_twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/smtp_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/trigger_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/user_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 09:52:15.000000 pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:52:15.171687 pulumiverse_zitadel-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-30 09:52:14.000000 pulumiverse_zitadel-0.1.8/setup.py
```

### Comparing `pulumiverse_zitadel-0.1.7/PKG-INFO` & `pulumiverse_zitadel-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: pulumiverse_zitadel
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Pulumi package for creating and managing zitadel cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-zitadel
 Keywords: pulumi zitadel category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Zitadel Resource Provider
 
-**⚠️WARNING: [I](https://github.com/vavsab) do not maintain this repo anymore. [Wating for zitadel to respond](https://github.com/zitadel/terraform-provider-zitadel/issues/158)**
-
 The Zitadel Resource Provider lets you manage [Zitadel](https://zitadel.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumiverse_zitadel-0.1.7/README.md` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,20 @@
-# Zitadel Resource Provider
+Metadata-Version: 2.1
+Name: pulumiverse-zitadel
+Version: 0.1.8
+Summary: A Pulumi package for creating and managing zitadel cloud resources.
+Home-page: https://www.pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumiverse/pulumi-zitadel
+Keywords: pulumi zitadel category/cloud
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
-**⚠️WARNING: [I](https://github.com/vavsab) do not maintain this repo anymore. [Wating for zitadel to respond](https://github.com/zitadel/terraform-provider-zitadel/issues/158)**
+# Zitadel Resource Provider
 
 The Zitadel Resource Provider lets you manage [Zitadel](https://zitadel.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
@@ -56,7 +66,9 @@
 - `zitadel:jwtProfileJson` - JSON value of credentials to connect to ZITADEL. Either `jwtProfileFile` or `jwtProfileJson` is required
 - `zitadel:port` - used port if not the default ports 80 or 443 are configured
 - `zitadel:token` - path to the file containing credentials to connect to ZITADEL
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/zitadel/api-docs/).
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/__init__.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/_utilities.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/action.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_api.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_api.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_key.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_oidc.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/application_saml.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/application_saml.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/config/vars.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_domain_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_domain_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_label_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_label_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_lockout_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_lockout_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_login_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_login_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_notification_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_oidc_settings.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_oidc_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_password_complexity_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_password_complexity_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/default_privacy_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/default_privacy_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/domain.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/domain_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/domain_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_action.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_api.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_api.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_apis.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_apis.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_oidc.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_oidcs.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_oidcs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_saml.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_saml.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_application_samls.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_application_samls.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_default_oidc_settings.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_default_oidc_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_human_user.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_human_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_azure_ad.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_github.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_github_es.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_gitlab.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_google.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_idp_ldap.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_machine_user.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_machine_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_machine_users.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_machine_users.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_azure_ad.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_github.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_github_es.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_gitlab.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_google.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_idp_ldap.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_jwt_idp.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_jwt_idp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_org_oidc_idp.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_org_oidc_idp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_orgs.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_orgs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_project.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_project_role.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_project_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_projects.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/get_trigger_actions.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/get_trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/human_user.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/human_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_azure_ad.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_github.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_github_es.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_gitlab.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_google.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/idp_ldap.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/instance_member.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/instance_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/label_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/label_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/lockout_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/lockout_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/login_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/login_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/machine_key.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/machine_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/machine_user.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/machine_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/notification_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_azure_ad.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_github.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_github.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_github_es.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_github_es.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_gitlab.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_gitlab.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_gitlab_self_hosted.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_google.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_google.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_jwt.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_jwt.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_ldap.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_idp_oidc.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_idp_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/org_member.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/org_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/password_complexity_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/password_complexity_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/personal_access_token.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/privacy_policy.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/privacy_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_grant.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_grant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_grant_member.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_grant_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_member.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/project_role.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/project_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/provider.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/sms_provider_twilio.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/sms_provider_twilio.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/smtp_config.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/smtp_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/trigger_actions.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/trigger_actions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel/user_grant.py` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel/user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/PKG-INFO` & `pulumiverse_zitadel-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-Metadata-Version: 2.1
-Name: pulumiverse-zitadel
-Version: 0.1.7
-Summary: A Pulumi package for creating and managing zitadel cloud resources.
-Home-page: https://www.pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumiverse/pulumi-zitadel
-Keywords: pulumi zitadel category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Zitadel Resource Provider
 
-**⚠️WARNING: [I](https://github.com/vavsab) do not maintain this repo anymore. [Wating for zitadel to respond](https://github.com/zitadel/terraform-provider-zitadel/issues/158)**
-
 The Zitadel Resource Provider lets you manage [Zitadel](https://zitadel.com/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
@@ -68,9 +54,7 @@
 - `zitadel:jwtProfileJson` - JSON value of credentials to connect to ZITADEL. Either `jwtProfileFile` or `jwtProfileJson` is required
 - `zitadel:port` - used port if not the default ports 80 or 443 are configured
 - `zitadel:token` - path to the file containing credentials to connect to ZITADEL
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/zitadel/api-docs/).
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumiverse_zitadel-0.1.7/pulumiverse_zitadel.egg-info/SOURCES.txt` & `pulumiverse_zitadel-0.1.8/pulumiverse_zitadel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_zitadel-0.1.7/setup.py` & `pulumiverse_zitadel-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "zitadel Pulumi Package - Development Version"
```

