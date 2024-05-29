# Comparing `tmp/django_restit-4.2.9.tar.gz` & `tmp/django_restit-4.2.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.2.9.tar", max compression
+gzip compressed data, was "django_restit-4.2.90.tar", max compression
```

## Comparing `django_restit-4.2.9.tar` & `django_restit-4.2.90.tar`

### file list

```diff
@@ -1,491 +1,512 @@
--rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.2.9/LICENSE.md
--rw-r--r--   0        0        0     6240 2023-07-18 17:15:13.487162 django_restit-4.2.9/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.2.9/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.2.9/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.2.9/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.2.9/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.2.9/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.2.9/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.2.9/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.2.9/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.2.9/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.2.9/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.2.9/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.2.9/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.2.9/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.2.9/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0      418 2023-07-13 15:44:27.208937 django_restit-4.2.9/account/migrations/0013_memberdevice_ip.py
--rw-r--r--   0        0        0      541 2023-11-07 12:44:14.024459 django_restit-4.2.9/account/migrations/0014_alter_notificationmemberrecord_member.py
--rw-r--r--   0        0        0      460 2023-11-15 19:46:51.612834 django_restit-4.2.9/account/migrations/0015_memberdevice_buid.py
--rw-r--r--   0        0        0      424 2023-11-15 20:20:37.084916 django_restit-4.2.9/account/migrations/0016_authsession_buid.py
--rw-r--r--   0        0        0      375 2023-11-28 23:26:56.206776 django_restit-4.2.9/account/migrations/0017_rename_requires_topt_member_requires_totp.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.2.9/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.2.9/account/models/__init__.py
--rw-r--r--   0        0        0     4105 2023-11-15 20:24:03.414109 django_restit-4.2.9/account/models/device.py
--rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.2.9/account/models/feeds.py
--rw-r--r--   0        0        0    20064 2023-12-15 19:46:55.047382 django_restit-4.2.9/account/models/group.py
--rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.2.9/account/models/legacy.py
--rw-r--r--   0        0        0    49327 2023-12-19 20:43:30.083308 django_restit-4.2.9/account/models/member.py
--rw-r--r--   0        0        0     7763 2023-12-09 22:24:04.788938 django_restit-4.2.9/account/models/membership.py
--rw-r--r--   0        0        0    12078 2023-11-17 21:39:46.651560 django_restit-4.2.9/account/models/notify.py
--rw-r--r--   0        0        0     3509 2023-11-15 20:20:12.123435 django_restit-4.2.9/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.2.9/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.2.9/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.2.9/account/oauth/google.py
--rw-r--r--   0        0        0      874 2023-11-29 03:43:42.972754 django_restit-4.2.9/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.2.9/account/rpc/__init__.py
--rw-r--r--   0        0        0    14896 2023-12-19 15:38:33.959934 django_restit-4.2.9/account/rpc/auth.py
--rw-r--r--   0        0        0     2852 2023-07-13 15:33:42.583999 django_restit-4.2.9/account/rpc/device.py
--rw-r--r--   0        0        0     3472 2023-12-04 21:21:15.602286 django_restit-4.2.9/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.2.9/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.2.9/account/rpc/notify.py
--rw-r--r--   0        0        0     2669 2023-12-17 00:40:58.671312 django_restit-4.2.9/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.2.9/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.2.9/account/settings.py
--rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.2.9/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.2.9/account/templates/email/invite.html
--rw-r--r--   0        0        0    12609 2023-11-07 13:31:04.277159 django_restit-4.2.9/account/templates/email/plain/base.html
--rw-r--r--   0        0        0    15235 2023-09-13 21:51:42.921379 django_restit-4.2.9/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.2.9/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.2.9/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15147 2023-09-13 21:29:05.002359 django_restit-4.2.9/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.2.9/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.2.9/auditlog/README
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.2.9/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.2.9/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.2.9/auditlog/decorators.py
--rw-r--r--   0        0        0     1511 2023-12-17 00:38:09.426633 django_restit-4.2.9/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.2.9/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.2.9/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16294 2023-11-28 17:50:33.116663 django_restit-4.2.9/auditlog/models.py
--rw-r--r--   0        0        0      363 2023-11-06 22:55:59.417756 django_restit-4.2.9/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2023-12-09 17:40:20.663908 django_restit-4.2.9/auditlog/rpc.py
--rw-r--r--   0        0        0     2415 2023-11-06 23:04:22.220672 django_restit-4.2.9/auditlog/tq.py
--rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.2.9/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.2.9/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.2.9/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.2.9/inbox/admin.py
--rw-r--r--   0        0        0     5638 2023-11-17 19:40:32.512907 django_restit-4.2.9/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.2.9/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.2.9/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.2.9/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.2.9/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.2.9/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.2.9/inbox/models/__init__.py
--rw-r--r--   0        0        0     2881 2023-12-09 17:43:11.500207 django_restit-4.2.9/inbox/models/bounce.py
--rw-r--r--   0        0        0     2517 2023-12-09 17:43:15.908858 django_restit-4.2.9/inbox/models/complaint.py
--rw-r--r--   0        0        0     3003 2023-12-09 17:43:26.636118 django_restit-4.2.9/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.2.9/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.2.9/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.2.9/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4615 2023-11-17 22:20:26.650843 django_restit-4.2.9/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.2.9/inbox/utils/render.py
--rw-r--r--   0        0        0     2179 2023-11-09 19:28:02.561057 django_restit-4.2.9/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.2.9/incident/README.md
--rw-r--r--   0        0        0     3249 2023-12-09 16:49:33.350637 django_restit-4.2.9/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.2.9/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.2.9/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.2.9/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.2.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.2.9/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.2.9/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.2.9/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.2.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0      473 2023-08-22 19:29:15.953220 django_restit-4.2.9/incident/migrations/0009_incident_reporter_ip.py
--rw-r--r--   0        0        0      631 2023-11-20 03:38:24.557282 django_restit-4.2.9/incident/migrations/0010_incident_category_incident_component_id.py
--rw-r--r--   0        0        0     2142 2023-11-20 03:51:50.549436 django_restit-4.2.9/incident/migrations/0011_ticket.py
--rw-r--r--   0        0        0      372 2023-12-19 03:25:06.153029 django_restit-4.2.9/incident/migrations/0012_rule_match_by.py
--rw-r--r--   0        0        0      387 2023-12-19 17:40:50.828606 django_restit-4.2.9/incident/migrations/0013_rulecheck_is_required.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.2.9/incident/migrations/__init__.py
--rw-r--r--   0        0        0      209 2023-11-20 03:49:22.992273 django_restit-4.2.9/incident/models/__init__.py
--rw-r--r--   0        0        0     6849 2023-12-09 19:39:18.790758 django_restit-4.2.9/incident/models/event.py
--rw-r--r--   0        0        0    15294 2023-12-20 17:41:19.779521 django_restit-4.2.9/incident/models/incident.py
--rw-r--r--   0        0        0     2227 2023-12-09 16:28:25.375197 django_restit-4.2.9/incident/models/ossec.py
--rw-r--r--   0        0        0     6024 2023-12-19 17:45:22.401412 django_restit-4.2.9/incident/models/rules.py
--rw-r--r--   0        0        0     2302 2023-11-20 03:51:47.283232 django_restit-4.2.9/incident/models/ticket.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.2.9/incident/parsers/__init__.py
--rw-r--r--   0        0        0     6247 2023-12-19 21:01:44.694027 django_restit-4.2.9/incident/parsers/ossec.py
--rw-r--r--   0        0        0      227 2023-11-28 04:04:56.458420 django_restit-4.2.9/incident/periodic.py
--rw-r--r--   0        0        0     7546 2023-12-19 00:05:09.162867 django_restit-4.2.9/incident/rpc.py
--rw-r--r--   0        0        0    14178 2023-11-18 15:34:42.122382 django_restit-4.2.9/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.2.9/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    14727 2023-11-20 22:01:29.858057 django_restit-4.2.9/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0     4589 2023-12-21 04:40:51.784780 django_restit-4.2.9/incident/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.2.9/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.2.9/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.2.9/location/geolocate.py
--rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.2.9/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.2.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.2.9/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.2.9/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.2.9/location/models/address.py
--rw-r--r--   0        0        0     5984 2023-12-09 17:41:39.358207 django_restit-4.2.9/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.2.9/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.2.9/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.2.9/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.2.9/location/providers/__init__.py
--rw-r--r--   0        0        0      727 2023-08-07 06:30:37.235541 django_restit-4.2.9/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.2.9/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.2.9/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.2.9/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.2.9/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.2.9/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.2.9/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.2.9/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.2.9/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.2.9/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.2.9/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.2.9/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.2.9/location/rpc/__init__.py
--rw-r--r--   0        0        0     1305 2023-11-27 23:53:10.865156 django_restit-4.2.9/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.2.9/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.2.9/location/rpc/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.2.9/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.2.9/medialib/admin.py
--rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.2.9/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.2.9/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.2.9/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.2.9/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.2.9/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.2.9/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.2.9/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.2.9/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.2.9/medialib/forms.py
--rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.2.9/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.2.9/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52152 2023-10-09 22:04:22.261815 django_restit-4.2.9/medialib/models.py
--rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.2.9/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.2.9/medialib/pdf.py
--rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.2.9/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.2.9/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.2.9/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.2.9/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.2.9/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.2.9/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.2.9/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.2.9/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.2.9/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.2.9/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.2.9/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.2.9/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.2.9/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.2.9/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.2.9/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.2.9/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.2.9/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.2.9/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.2.9/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.2.9/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.2.9/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.2.9/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.2.9/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.2.9/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.2.9/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.2.9/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.2.9/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.2.9/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.2.9/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.2.9/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.2.9/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.2.9/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.2.9/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.2.9/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.2.9/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.2.9/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.2.9/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.2.9/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.2.9/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.2.9/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.2.9/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.2.9/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.2.9/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.2.9/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.2.9/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.2.9/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.2.9/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.2.9/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.2.9/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.2.9/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.2.9/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.2.9/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.2.9/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.2.9/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.2.9/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.2.9/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.2.9/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.2.9/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.2.9/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.2.9/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.2.9/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.2.9/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.2.9/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.2.9/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.2.9/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.2.9/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.2.9/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.2.9/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.2.9/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.2.9/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.2.9/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.2.9/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.2.9/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.2.9/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.2.9/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.2.9/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.2.9/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.2.9/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.2.9/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.2.9/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.2.9/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.2.9/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.2.9/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.2.9/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.2.9/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.2.9/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.2.9/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.2.9/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.2.9/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.2.9/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.2.9/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.2.9/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.2.9/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.2.9/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.2.9/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.2.9/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.2.9/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.2.9/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.2.9/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.2.9/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.2.9/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.2.9/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.2.9/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.2.9/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.2.9/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.2.9/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.2.9/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.2.9/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.2.9/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.2.9/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.2.9/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.2.9/medialib/tests.py
--rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.2.9/medialib/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.2.9/medialib/urls.py
--rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.2.9/medialib/utils.py
--rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.2.9/medialib/views.py
--rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.2.9/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.2.9/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.2.9/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.2.9/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.2.9/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.2.9/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.2.9/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.2.9/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.2.9/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.2.9/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.2.9/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.2.9/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.2.9/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.2.9/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.2.9/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.2.9/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.2.9/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.2.9/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.2.9/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.2.9/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.2.9/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.2.9/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.2.9/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.2.9/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.2.9/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.2.9/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.2.9/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.2.9/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.2.9/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.2.9/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.2.9/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.2.9/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.2.9/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.2.9/metrics/__init__.py
--rw-r--r--   0        0        0    24337 2023-11-12 22:00:50.439910 django_restit-4.2.9/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.2.9/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.2.9/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.2.9/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.2.9/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.2.9/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.2.9/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.2.9/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.2.9/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.2.9/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.2.9/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.2.9/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.2.9/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.2.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.2.9/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.2.9/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.2.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.2.9/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    13444 2023-11-14 19:47:33.877245 django_restit-4.2.9/metrics/models.py
--rw-r--r--   0        0        0      651 2023-08-07 16:07:55.926386 django_restit-4.2.9/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.2.9/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7432 2023-08-01 17:23:09.504050 django_restit-4.2.9/metrics/providers/aws.py
--rw-r--r--   0        0        0    17674 2023-12-17 00:39:40.117566 django_restit-4.2.9/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.2.9/metrics/settings.py
--rw-r--r--   0        0        0      799 2023-08-22 14:57:47.689025 django_restit-4.2.9/metrics/tq.py
--rw-r--r--   0        0        0    11995 2023-11-12 21:49:36.875626 django_restit-4.2.9/metrics/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.2.9/pushit/__init__.py
--rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.2.9/pushit/admin.py
--rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.2.9/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.2.9/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.2.9/pushit/models.py
--rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.2.9/pushit/rpc/__init__.py
--rw-r--r--   0        0        0     1756 2023-07-24 17:39:38.308118 django_restit-4.2.9/pushit/rpc/githooks.py
--rw-r--r--   0        0        0     5028 2023-12-09 19:07:40.680776 django_restit-4.2.9/pushit/rpc/legacy.py
--rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.2.9/pushit/rpc/products.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.2.9/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0      424 2023-08-01 06:36:56.109166 django_restit-4.2.9/pushit/tq.py
--rw-r--r--   0        0        0     2121 2023-07-24 17:36:54.438531 django_restit-4.2.9/pushit/utils.py
--rw-r--r--   0        0        0     1210 2023-12-21 05:47:30.691584 django_restit-4.2.9/pyproject.toml
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.2.9/rest/.gitignore
--rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.2.9/rest/README.md
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.2.9/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2023-12-21 05:47:30.734086 django_restit-4.2.9/rest/__init__.py
--rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.2.9/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.2.9/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.2.9/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.2.9/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.2.9/rest/crypto/privpub.py
--rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.2.9/rest/crypto/util.py
--rw-r--r--   0        0        0     9330 2023-11-25 04:40:03.230095 django_restit-4.2.9/rest/datem.py
--rw-r--r--   0        0        0    15082 2023-12-09 17:07:25.089133 django_restit-4.2.9/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.2.9/rest/encryption.py
--rw-r--r--   0        0        0      612 2023-12-19 00:02:03.767620 django_restit-4.2.9/rest/errors.py
--rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.2.9/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.2.9/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.2.9/rest/fields.py
--rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.2.9/rest/forms.py
--rw-r--r--   0        0        0    26563 2023-12-17 18:42:16.439687 django_restit-4.2.9/rest/helpers.py
--rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.2.9/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.2.9/rest/jwtoken.py
--rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.2.9/rest/log.py
--rw-r--r--   0        0        0     7737 2023-09-13 21:40:41.824715 django_restit-4.2.9/rest/mail.py
--rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.2.9/rest/mailman.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.2.9/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.2.9/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.2.9/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.2.9/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.2.9/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.2.9/rest/middleware/db_router.py
--rw-r--r--   0        0        0     6017 2023-11-29 03:51:44.491936 django_restit-4.2.9/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4189 2023-11-15 19:37:49.027885 django_restit-4.2.9/rest/middleware/request.py
--rw-r--r--   0        0        0    10240 2023-07-17 21:30:14.707861 django_restit-4.2.9/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.2.9/rest/middleware/session_store.py
--rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.2.9/rest/models/__init__.py
--rw-r--r--   0        0        0    66081 2023-12-09 19:57:57.872073 django_restit-4.2.9/rest/models/base.py
--rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.2.9/rest/models/cacher.py
--rw-r--r--   0        0        0    12631 2023-12-09 17:10:16.004033 django_restit-4.2.9/rest/models/metadata.py
--rw-r--r--   0        0        0     1691 2023-08-07 04:48:28.143401 django_restit-4.2.9/rest/net.py
--rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.2.9/rest/regexes.yaml
--rw-r--r--   0        0        0    15701 2023-12-20 17:18:00.376275 django_restit-4.2.9/rest/requestex.py
--rw-r--r--   0        0        0     3612 2023-08-07 04:26:49.350849 django_restit-4.2.9/rest/rpc.py
--rw-r--r--   0        0        0     8362 2023-11-14 19:35:31.737708 django_restit-4.2.9/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.2.9/rest/serializers/__init__.py
--rw-r--r--   0        0        0     4648 2023-11-15 20:41:11.119667 django_restit-4.2.9/rest/serializers/collection.py
--rw-r--r--   0        0        0     3251 2023-12-10 01:39:17.966410 django_restit-4.2.9/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.2.9/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.2.9/rest/serializers/json.py
--rw-r--r--   0        0        0    61981 2023-12-19 00:04:01.349514 django_restit-4.2.9/rest/serializers/legacy.py
--rw-r--r--   0        0        0     8598 2023-11-10 17:09:26.910604 django_restit-4.2.9/rest/serializers/model.py
--rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.2.9/rest/serializers/profiler.py
--rw-r--r--   0        0        0     7051 2023-12-19 00:03:41.185610 django_restit-4.2.9/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.2.9/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.2.9/rest/settings_helper.py
--rw-r--r--   0        0        0     1419 2023-08-07 05:26:37.128368 django_restit-4.2.9/rest/ssl_check.py
--rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.2.9/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.2.9/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.2.9/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.2.9/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.2.9/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.2.9/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.2.9/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.2.9/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10986 2023-12-17 18:47:10.126214 django_restit-4.2.9/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185398 2023-07-28 01:56:34.391352 django_restit-4.2.9/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.2.9/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.2.9/rest/url_docs.py
--rw-r--r--   0        0        0     1869 2023-12-17 00:13:41.075590 django_restit-4.2.9/rest/urls.py
--rw-r--r--   0        0        0     1115 2023-12-17 00:40:15.697924 django_restit-4.2.9/rest/views.py
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.2.9/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.2.9/sessionlog/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.2.9/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.2.9/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.2.9/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.2.9/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3662 2023-07-17 21:32:12.789126 django_restit-4.2.9/sessionlog/models.py
--rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.2.9/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.2.9/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.2.9/taskqueue/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.2.9/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.2.9/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.2.9/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.2.9/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    19306 2023-12-18 15:27:25.429795 django_restit-4.2.9/taskqueue/models.py
--rw-r--r--   0        0        0     3543 2023-08-11 17:40:15.804907 django_restit-4.2.9/taskqueue/periodic.py
--rw-r--r--   0        0        0     5736 2023-12-09 17:45:37.022351 django_restit-4.2.9/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.2.9/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.2.9/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.2.9/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2023-08-31 21:55:56.632266 django_restit-4.2.9/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1913 2023-10-30 22:13:38.540735 django_restit-4.2.9/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.2.9/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.2.9/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    16050 2023-12-16 21:45:01.773610 django_restit-4.2.9/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.2.9/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.2.9/telephony/admin.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.2.9/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.2.9/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0      424 2023-11-27 22:03:30.384417 django_restit-4.2.9/telephony/migrations/0002_alter_sms_sid.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.2.9/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     8248 2023-12-09 17:49:10.656587 django_restit-4.2.9/telephony/models.py
--rw-r--r--   0        0        0     2426 2023-11-28 15:55:05.388090 django_restit-4.2.9/telephony/phone_util.py
--rw-r--r--   0        0        0     3473 2023-12-09 17:49:26.483244 django_restit-4.2.9/telephony/rpc.py
--rw-r--r--   0        0        0        1 2023-08-03 14:28:08.854157 django_restit-4.2.9/wiki/__init__.py
--rw-r--r--   0        0        0     3606 2023-08-04 04:52:16.019699 django_restit-4.2.9/wiki/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-08-04 04:52:16.018799 django_restit-4.2.9/wiki/migrations/__init__.py
--rw-r--r--   0        0        0      132 2023-08-04 03:46:50.913857 django_restit-4.2.9/wiki/models/__init__.py
--rw-r--r--   0        0        0     1745 2023-08-03 15:41:23.854674 django_restit-4.2.9/wiki/models/faq.py
--rw-r--r--   0        0        0     7203 2023-08-16 18:23:17.138555 django_restit-4.2.9/wiki/models/page.py
--rw-r--r--   0        0        0      729 2023-08-04 03:47:46.129186 django_restit-4.2.9/wiki/models/revision.py
--rw-r--r--   0        0        0      334 2023-08-03 14:28:08.854499 django_restit-4.2.9/wiki/periodic.py
--rw-r--r--   0        0        0      461 2023-08-03 15:34:25.031919 django_restit-4.2.9/wiki/renderers/__init__.py
--rwxr-xr-x   0        0        0       84 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/__init__.py
--rwxr-xr-x   0        0        0     1264 2023-08-04 05:12:57.404938 django_restit-4.2.9/wiki/renderers/mistune/highlight.py
--rwxr-xr-x   0        0        0     1901 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/math.py
--rw-r--r--   0        0        0     2610 2023-08-14 06:50:10.268306 django_restit-4.2.9/wiki/renderers/mistune/media.py
--rwxr-xr-x   0        0        0      805 2022-09-24 04:49:32.000000 django_restit-4.2.9/wiki/renderers/mistune/meta.py
--rw-r--r--   0        0        0     1889 2023-08-16 00:38:11.894074 django_restit-4.2.9/wiki/renderers/mistune/task_list.py
--rwxr-xr-x   0        0        0     2302 2023-08-04 05:12:30.563520 django_restit-4.2.9/wiki/renderers/mistune/toc.py
--rw-r--r--   0        0        0       40 2023-08-04 00:19:22.669056 django_restit-4.2.9/wiki/rpc/__init__.py
--rw-r--r--   0        0        0     1333 2023-08-16 18:28:15.622351 django_restit-4.2.9/wiki/rpc/wiki.py
--rw-r--r--   0        0        0      313 2023-08-03 14:28:08.854423 django_restit-4.2.9/wiki/tq.py
--rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.2.9/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.2.9/ws4redis/__init__.py
--rw-r--r--   0        0        0     5049 2023-11-12 04:56:27.258942 django_restit-4.2.9/ws4redis/client.py
--rw-r--r--   0        0        0    13431 2023-08-14 17:22:44.326899 django_restit-4.2.9/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.2.9/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.2.9/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.2.9/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.2.9/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.2.9/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.2.9/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1536 2023-08-14 17:15:40.285934 django_restit-4.2.9/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.2.9/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.2.9/ws4redis/websocket.py
--rw-r--r--   0        0        0     7572 1970-01-01 00:00:00.000000 django_restit-4.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-13 20:28:15.628821 django_restit-4.2.90/LICENSE.md
+-rw-r--r--   0        0        0     6240 2024-04-13 20:28:15.628920 django_restit-4.2.90/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.629016 django_restit-4.2.90/account/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-13 20:28:15.629085 django_restit-4.2.90/account/admin.py
+-rw-r--r--   0        0        0      980 2024-04-13 20:28:15.629171 django_restit-4.2.90/account/fcm/__init__.py
+-rw-r--r--   0        0        0     1710 2024-04-13 20:28:15.629233 django_restit-4.2.90/account/fcm/google.py
+-rw-r--r--   0        0        0     1434 2024-04-13 20:28:15.629289 django_restit-4.2.90/account/fcm/v1.py
+-rw-r--r--   0        0        0    15894 2024-04-13 20:28:15.629493 django_restit-4.2.90/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2024-04-13 20:28:15.629557 django_restit-4.2.90/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2024-04-13 20:28:15.629612 django_restit-4.2.90/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2024-04-13 20:28:15.629669 django_restit-4.2.90/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2024-04-13 20:28:15.629735 django_restit-4.2.90/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2024-04-13 20:28:15.629793 django_restit-4.2.90/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2024-04-13 20:28:15.629858 django_restit-4.2.90/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2024-04-13 20:28:15.629909 django_restit-4.2.90/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2024-04-13 20:28:15.629961 django_restit-4.2.90/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2024-04-13 20:28:15.630006 django_restit-4.2.90/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2024-04-13 20:28:15.630059 django_restit-4.2.90/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0      418 2024-04-13 20:28:15.630114 django_restit-4.2.90/account/migrations/0013_memberdevice_ip.py
+-rw-r--r--   0        0        0      541 2024-04-13 20:28:15.630162 django_restit-4.2.90/account/migrations/0014_alter_notificationmemberrecord_member.py
+-rw-r--r--   0        0        0      460 2024-04-13 20:28:15.630211 django_restit-4.2.90/account/migrations/0015_memberdevice_buid.py
+-rw-r--r--   0        0        0      424 2024-04-13 20:28:15.630262 django_restit-4.2.90/account/migrations/0016_authsession_buid.py
+-rw-r--r--   0        0        0      375 2024-04-13 20:28:15.630324 django_restit-4.2.90/account/migrations/0017_rename_requires_topt_member_requires_totp.py
+-rw-r--r--   0        0        0     1475 2024-04-13 20:28:15.630382 django_restit-4.2.90/account/migrations/0018_userpasskey.py
+-rw-r--r--   0        0        0      601 2024-04-13 20:28:15.630452 django_restit-4.2.90/account/migrations/0019_group_location.py
+-rw-r--r--   0        0        0     2250 2024-04-25 16:09:54.723585 django_restit-4.2.90/account/migrations/0020_cloudcredentials_cloudcredentialsmetadata.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.630482 django_restit-4.2.90/account/migrations/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-13 20:28:15.630615 django_restit-4.2.90/account/models/__init__.py
+-rw-r--r--   0        0        0     5491 2024-05-03 22:34:25.131492 django_restit-4.2.90/account/models/device.py
+-rw-r--r--   0        0        0     2011 2024-04-13 20:28:15.630794 django_restit-4.2.90/account/models/feeds.py
+-rw-r--r--   0        0        0    22262 2024-05-16 16:56:19.272702 django_restit-4.2.90/account/models/group.py
+-rw-r--r--   0        0        0     2720 2024-04-13 20:28:15.631007 django_restit-4.2.90/account/models/legacy.py
+-rw-r--r--   0        0        0    53092 2024-05-14 19:14:54.930718 django_restit-4.2.90/account/models/member.py
+-rw-r--r--   0        0        0     9249 2024-05-08 01:17:16.122005 django_restit-4.2.90/account/models/membership.py
+-rw-r--r--   0        0        0    15306 2024-05-13 23:53:09.195555 django_restit-4.2.90/account/models/notify.py
+-rw-r--r--   0        0        0     1516 2024-04-13 20:28:15.631615 django_restit-4.2.90/account/models/passkeys.py
+-rw-r--r--   0        0        0     3737 2024-05-03 19:51:25.510322 django_restit-4.2.90/account/models/session.py
+-rw-r--r--   0        0        0     2137 2024-04-13 20:28:15.631753 django_restit-4.2.90/account/models/settings.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.631821 django_restit-4.2.90/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-13 20:28:15.631917 django_restit-4.2.90/account/oauth/google.py
+-rw-r--r--   0        0        0       89 2024-04-13 20:28:15.632026 django_restit-4.2.90/account/passkeys/__init__.py
+-rw-r--r--   0        0        0     4126 2024-04-25 16:09:54.725070 django_restit-4.2.90/account/passkeys/core.py
+-rw-r--r--   0        0        0      874 2024-04-13 20:28:15.632196 django_restit-4.2.90/account/periodic.py
+-rw-r--r--   0        0        0      336 2024-04-13 20:28:15.632316 django_restit-4.2.90/account/rpc/__init__.py
+-rw-r--r--   0        0        0    16615 2024-05-11 18:22:59.362744 django_restit-4.2.90/account/rpc/auth.py
+-rw-r--r--   0        0        0     3070 2024-05-03 21:17:34.200466 django_restit-4.2.90/account/rpc/device.py
+-rw-r--r--   0        0        0     4929 2024-05-23 02:25:37.963413 django_restit-4.2.90/account/rpc/group.py
+-rw-r--r--   0        0        0     1817 2024-05-11 00:18:44.008237 django_restit-4.2.90/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2024-04-13 20:28:15.632714 django_restit-4.2.90/account/rpc/notify.py
+-rw-r--r--   0        0        0     2864 2024-04-13 20:28:15.632792 django_restit-4.2.90/account/rpc/oauth.py
+-rw-r--r--   0        0        0     1729 2024-04-13 20:28:15.632847 django_restit-4.2.90/account/rpc/passkeys.py
+-rw-r--r--   0        0        0      271 2024-04-13 20:28:15.632903 django_restit-4.2.90/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2024-04-13 20:28:15.632953 django_restit-4.2.90/account/settings.py
+-rw-r--r--   0        0        0     9669 2024-05-10 19:31:50.813510 django_restit-4.2.90/account/templates/email/base.html
+-rw-r--r--   0        0        0    10346 2024-05-10 19:30:56.128429 django_restit-4.2.90/account/templates/email/invite.html
+-rw-r--r--   0        0        0    12600 2024-04-13 20:28:15.633509 django_restit-4.2.90/account/templates/email/plain/base.html
+-rw-r--r--   0        0        0    14692 2024-05-10 21:14:10.951606 django_restit-4.2.90/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13411 2024-05-10 21:08:49.022358 django_restit-4.2.90/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10040 2024-05-10 21:09:00.248228 django_restit-4.2.90/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    14604 2024-05-10 21:14:17.651731 django_restit-4.2.90/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13401 2024-05-10 21:08:38.943379 django_restit-4.2.90/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0    46361 2024-05-11 00:17:15.860611 django_restit-4.2.90/account/templates/unsubscribed.html
+-rw-r--r--   0        0        0      520 2024-04-13 20:28:15.634310 django_restit-4.2.90/auditlog/README
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.634338 django_restit-4.2.90/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2024-04-13 20:28:15.634405 django_restit-4.2.90/auditlog/admin.py
+-rw-r--r--   0        0        0     6788 2024-05-14 03:46:10.115535 django_restit-4.2.90/auditlog/cloudwatch.py
+-rw-r--r--   0        0        0     6553 2024-04-13 20:28:15.634534 django_restit-4.2.90/auditlog/decorators.py
+-rw-r--r--   0        0        0     1537 2024-04-13 20:28:15.634591 django_restit-4.2.90/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2024-04-13 20:28:15.634691 django_restit-4.2.90/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0      541 2024-05-13 02:34:55.168831 django_restit-4.2.90/auditlog/migrations/0002_alter_persistentlog_session.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.634715 django_restit-4.2.90/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16517 2024-04-13 20:28:15.634791 django_restit-4.2.90/auditlog/models.py
+-rw-r--r--   0        0        0      363 2024-04-13 20:28:15.634866 django_restit-4.2.90/auditlog/periodic.py
+-rw-r--r--   0        0        0     5592 2024-05-14 04:52:41.918784 django_restit-4.2.90/auditlog/rpc.py
+-rw-r--r--   0        0        0     2415 2024-04-13 20:28:15.634967 django_restit-4.2.90/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2024-04-13 20:28:15.635019 django_restit-4.2.90/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2024-04-13 20:28:15.636613 django_restit-4.2.90/inbox/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.636640 django_restit-4.2.90/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-13 20:28:15.636694 django_restit-4.2.90/inbox/admin.py
+-rw-r--r--   0        0        0     5638 2024-04-13 20:28:15.636750 django_restit-4.2.90/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2024-04-13 20:28:15.636826 django_restit-4.2.90/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2024-04-13 20:28:15.636873 django_restit-4.2.90/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2024-04-13 20:28:15.636925 django_restit-4.2.90/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2024-04-13 20:28:15.636990 django_restit-4.2.90/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0      393 2024-05-13 02:34:55.167916 django_restit-4.2.90/inbox/migrations/0005_alter_mailbox_state.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.637014 django_restit-4.2.90/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-13 20:28:15.637210 django_restit-4.2.90/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2881 2024-04-13 20:28:15.637278 django_restit-4.2.90/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2517 2024-04-13 20:28:15.637330 django_restit-4.2.90/inbox/models/complaint.py
+-rw-r--r--   0        0        0     3003 2024-04-13 20:28:15.637381 django_restit-4.2.90/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2024-04-13 20:28:15.637431 django_restit-4.2.90/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2024-04-13 20:28:15.637481 django_restit-4.2.90/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2024-04-13 20:28:15.637552 django_restit-4.2.90/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2024-04-13 20:28:15.637625 django_restit-4.2.90/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4331 2024-05-10 19:44:35.001421 django_restit-4.2.90/inbox/utils/render.py
+-rw-r--r--   0        0        0     2179 2024-04-13 20:28:15.637750 django_restit-4.2.90/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2024-04-13 20:28:15.637830 django_restit-4.2.90/incident/README.md
+-rw-r--r--   0        0        0     3455 2024-04-13 20:28:15.637889 django_restit-4.2.90/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2024-04-13 20:28:15.638179 django_restit-4.2.90/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2024-04-13 20:28:15.638252 django_restit-4.2.90/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2024-04-13 20:28:15.638305 django_restit-4.2.90/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2024-04-13 20:28:15.638359 django_restit-4.2.90/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2024-04-13 20:28:15.638414 django_restit-4.2.90/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2024-04-13 20:28:15.638467 django_restit-4.2.90/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2024-04-13 20:28:15.638518 django_restit-4.2.90/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2024-04-13 20:28:15.638569 django_restit-4.2.90/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0      473 2024-04-13 20:28:15.638617 django_restit-4.2.90/incident/migrations/0009_incident_reporter_ip.py
+-rw-r--r--   0        0        0      631 2024-04-13 20:28:15.638665 django_restit-4.2.90/incident/migrations/0010_incident_category_incident_component_id.py
+-rw-r--r--   0        0        0     2142 2024-04-13 20:28:15.638711 django_restit-4.2.90/incident/migrations/0011_ticket.py
+-rw-r--r--   0        0        0      372 2024-04-13 20:28:15.638757 django_restit-4.2.90/incident/migrations/0012_rule_match_by.py
+-rw-r--r--   0        0        0      387 2024-04-13 20:28:15.638814 django_restit-4.2.90/incident/migrations/0013_rulecheck_is_required.py
+-rw-r--r--   0        0        0      724 2024-04-13 20:28:15.638862 django_restit-4.2.90/incident/migrations/0014_event_group_alter_rulecheck_index.py
+-rw-r--r--   0        0        0      687 2024-05-13 02:35:36.839627 django_restit-4.2.90/incident/migrations/0015_rule_title_template_alter_incident_state.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.638883 django_restit-4.2.90/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-13 20:28:15.638963 django_restit-4.2.90/incident/models/__init__.py
+-rw-r--r--   0        0        0     7769 2024-05-13 02:54:01.165523 django_restit-4.2.90/incident/models/event.py
+-rw-r--r--   0        0        0    20030 2024-05-16 21:36:31.605873 django_restit-4.2.90/incident/models/incident.py
+-rw-r--r--   0        0        0     2252 2024-05-12 16:53:21.163497 django_restit-4.2.90/incident/models/ossec.py
+-rw-r--r--   0        0        0     7001 2024-05-13 04:25:42.761665 django_restit-4.2.90/incident/models/rules.py
+-rw-r--r--   0        0        0     2302 2024-04-13 20:28:15.639286 django_restit-4.2.90/incident/models/ticket.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.639341 django_restit-4.2.90/incident/parsers/__init__.py
+-rw-r--r--   0        0        0    11609 2024-05-15 16:28:34.609597 django_restit-4.2.90/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      381 2024-04-13 20:28:15.639464 django_restit-4.2.90/incident/periodic.py
+-rw-r--r--   0        0        0     8187 2024-05-14 15:21:12.014856 django_restit-4.2.90/incident/rpc.py
+-rw-r--r--   0        0        0    13895 2024-05-10 19:31:58.659471 django_restit-4.2.90/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    13780 2024-05-10 19:32:01.508597 django_restit-4.2.90/incident/templates/email/incident_msg.html
+-rw-r--r--   0        0        0    15185 2024-05-10 19:31:46.016828 django_restit-4.2.90/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    14739 2024-05-10 19:33:03.301598 django_restit-4.2.90/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0     5226 2024-04-13 20:28:15.640095 django_restit-4.2.90/incident/tq.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.640151 django_restit-4.2.90/location/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-13 20:28:15.640214 django_restit-4.2.90/location/admin.py
+-rw-r--r--   0        0        0     1694 2024-04-13 20:28:15.640298 django_restit-4.2.90/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2024-04-13 20:28:15.640408 django_restit-4.2.90/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2024-04-13 20:28:15.640461 django_restit-4.2.90/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0      443 2024-04-13 20:28:15.640514 django_restit-4.2.90/location/migrations/0003_address_postalcode_suffix.py
+-rw-r--r--   0        0        0     1270 2024-04-13 20:28:15.640575 django_restit-4.2.90/location/migrations/0004_remove_address_modified_by_address_group_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.640602 django_restit-4.2.90/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-13 20:28:15.640694 django_restit-4.2.90/location/models/__init__.py
+-rw-r--r--   0        0        0     3149 2024-04-13 20:28:15.640749 django_restit-4.2.90/location/models/address.py
+-rw-r--r--   0        0        0     6039 2024-05-13 17:28:14.894161 django_restit-4.2.90/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2024-04-13 20:28:15.640866 django_restit-4.2.90/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2024-04-13 20:28:15.640935 django_restit-4.2.90/location/models/location.py
+-rw-r--r--   0        0        0     1474 2024-04-13 20:28:15.640986 django_restit-4.2.90/location/models/track.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.641044 django_restit-4.2.90/location/providers/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-13 17:27:03.924591 django_restit-4.2.90/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2024-04-13 20:28:15.641198 django_restit-4.2.90/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2024-04-13 20:28:15.641249 django_restit-4.2.90/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2024-04-13 20:28:15.641301 django_restit-4.2.90/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2024-04-13 20:28:15.641374 django_restit-4.2.90/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2024-04-13 20:28:15.641436 django_restit-4.2.90/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2024-04-13 20:28:15.641497 django_restit-4.2.90/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2024-04-13 20:28:15.641582 django_restit-4.2.90/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2024-04-13 20:28:15.641633 django_restit-4.2.90/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2024-04-13 20:28:15.641713 django_restit-4.2.90/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-13 20:28:15.641760 django_restit-4.2.90/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2024-04-13 20:28:15.641810 django_restit-4.2.90/location/providers/zillow.py
+-rw-r--r--   0        0        0      166 2024-04-13 20:28:15.641885 django_restit-4.2.90/location/rpc/__init__.py
+-rw-r--r--   0        0        0      219 2024-04-13 20:28:15.641939 django_restit-4.2.90/location/rpc/address.py
+-rw-r--r--   0        0        0     1452 2024-05-15 01:10:30.262895 django_restit-4.2.90/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2024-04-13 20:28:15.642041 django_restit-4.2.90/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2024-04-13 20:28:15.642094 django_restit-4.2.90/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.642145 django_restit-4.2.90/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2024-04-13 20:28:15.642205 django_restit-4.2.90/medialib/admin.py
+-rw-r--r--   0        0        0       27 2024-04-13 20:28:15.642295 django_restit-4.2.90/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2024-04-13 20:28:15.642369 django_restit-4.2.90/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2024-04-13 20:28:15.642503 django_restit-4.2.90/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2024-04-13 20:28:15.642653 django_restit-4.2.90/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2024-04-13 20:28:15.642733 django_restit-4.2.90/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2024-04-13 20:28:15.642888 django_restit-4.2.90/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2024-04-13 20:28:15.643014 django_restit-4.2.90/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2024-04-13 20:28:15.643144 django_restit-4.2.90/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2024-04-13 20:28:15.643241 django_restit-4.2.90/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2024-04-13 20:28:15.643376 django_restit-4.2.90/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.643436 django_restit-4.2.90/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52201 2024-05-15 22:58:30.568579 django_restit-4.2.90/medialib/models.py
+-rw-r--r--   0        0        0     1189 2024-04-13 20:28:15.643657 django_restit-4.2.90/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2024-04-13 20:28:15.643716 django_restit-4.2.90/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2024-04-13 20:28:15.643772 django_restit-4.2.90/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2024-04-13 20:28:15.643954 django_restit-4.2.90/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.644014 django_restit-4.2.90/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-13 20:28:15.644086 django_restit-4.2.90/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2024-04-13 20:28:15.644158 django_restit-4.2.90/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2024-04-13 20:28:15.644218 django_restit-4.2.90/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2024-04-13 20:28:15.644276 django_restit-4.2.90/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2024-04-13 20:28:15.644333 django_restit-4.2.90/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2024-04-13 20:28:15.644417 django_restit-4.2.90/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.644448 django_restit-4.2.90/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2024-04-13 20:28:15.644516 django_restit-4.2.90/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2024-04-13 20:28:15.644579 django_restit-4.2.90/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2024-04-13 20:28:15.644647 django_restit-4.2.90/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2024-04-13 20:28:15.644704 django_restit-4.2.90/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2024-04-13 20:28:15.644758 django_restit-4.2.90/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2024-04-13 20:28:15.644812 django_restit-4.2.90/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.644870 django_restit-4.2.90/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2024-04-13 20:28:15.644935 django_restit-4.2.90/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2024-04-13 20:28:15.644999 django_restit-4.2.90/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2024-04-13 20:28:15.645068 django_restit-4.2.90/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2024-04-13 20:28:15.645127 django_restit-4.2.90/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2024-04-13 20:28:15.645209 django_restit-4.2.90/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2024-04-13 20:28:15.645283 django_restit-4.2.90/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2024-04-13 20:28:15.645345 django_restit-4.2.90/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2024-04-13 20:28:15.645404 django_restit-4.2.90/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2024-04-13 20:28:15.645468 django_restit-4.2.90/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2024-04-13 20:28:15.645531 django_restit-4.2.90/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2024-04-13 20:28:15.645582 django_restit-4.2.90/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2024-04-13 20:28:15.645637 django_restit-4.2.90/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2024-04-13 20:28:15.645717 django_restit-4.2.90/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2024-04-13 20:28:15.645800 django_restit-4.2.90/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2024-04-13 20:28:15.645892 django_restit-4.2.90/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2024-04-13 20:28:15.645993 django_restit-4.2.90/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2024-04-13 20:28:15.646082 django_restit-4.2.90/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2024-04-13 20:28:15.646147 django_restit-4.2.90/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2024-04-13 20:28:15.646262 django_restit-4.2.90/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2024-04-13 20:28:15.646422 django_restit-4.2.90/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2024-04-13 20:28:15.646484 django_restit-4.2.90/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2024-04-13 20:28:15.646541 django_restit-4.2.90/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2024-04-13 20:28:15.646618 django_restit-4.2.90/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2024-04-13 20:28:15.646683 django_restit-4.2.90/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2024-04-13 20:28:15.646733 django_restit-4.2.90/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2024-04-13 20:28:15.646785 django_restit-4.2.90/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2024-04-13 20:28:15.646841 django_restit-4.2.90/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2024-04-13 20:28:15.646891 django_restit-4.2.90/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2024-04-13 20:28:15.646947 django_restit-4.2.90/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2024-04-13 20:28:15.647004 django_restit-4.2.90/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2024-04-13 20:28:15.647047 django_restit-4.2.90/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2024-04-13 20:28:15.647097 django_restit-4.2.90/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2024-04-13 20:28:15.647168 django_restit-4.2.90/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2024-04-13 20:28:15.647217 django_restit-4.2.90/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2024-04-13 20:28:15.647266 django_restit-4.2.90/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2024-04-13 20:28:15.647317 django_restit-4.2.90/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2024-04-13 20:28:15.647497 django_restit-4.2.90/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2024-04-13 20:28:15.647608 django_restit-4.2.90/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2024-04-13 20:28:15.647726 django_restit-4.2.90/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2024-04-13 20:28:15.647801 django_restit-4.2.90/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2024-04-13 20:28:15.647890 django_restit-4.2.90/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2024-04-13 20:28:15.648085 django_restit-4.2.90/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2024-04-13 20:28:15.648292 django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2024-04-13 20:28:15.648356 django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2024-04-13 20:28:15.648462 django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2024-04-13 20:28:15.648520 django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2024-04-13 20:28:15.648620 django_restit-4.2.90/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-13 20:28:15.648728 django_restit-4.2.90/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2024-04-13 20:28:15.648872 django_restit-4.2.90/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2024-04-13 20:28:15.648982 django_restit-4.2.90/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2024-04-13 20:28:15.649082 django_restit-4.2.90/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2024-04-13 20:28:15.649208 django_restit-4.2.90/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2024-04-13 20:28:15.649279 django_restit-4.2.90/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2024-04-13 20:28:15.649414 django_restit-4.2.90/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2024-04-13 20:28:15.649474 django_restit-4.2.90/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2024-04-13 20:28:15.649619 django_restit-4.2.90/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2024-04-13 20:28:15.649685 django_restit-4.2.90/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2024-04-13 20:28:15.649881 django_restit-4.2.90/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2024-04-13 20:28:15.650027 django_restit-4.2.90/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2024-04-13 20:28:15.650118 django_restit-4.2.90/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2024-04-13 20:28:15.650205 django_restit-4.2.90/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2024-04-13 20:28:15.650292 django_restit-4.2.90/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2024-04-13 20:28:15.650355 django_restit-4.2.90/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2024-04-13 20:28:15.650459 django_restit-4.2.90/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2024-04-13 20:28:15.650539 django_restit-4.2.90/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2024-04-13 20:28:15.650636 django_restit-4.2.90/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2024-04-13 20:28:15.650760 django_restit-4.2.90/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2024-04-13 20:28:15.650827 django_restit-4.2.90/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2024-04-13 20:28:15.650953 django_restit-4.2.90/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2024-04-13 20:28:15.651011 django_restit-4.2.90/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2024-04-13 20:28:15.651090 django_restit-4.2.90/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2024-04-13 20:28:15.651142 django_restit-4.2.90/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2024-04-13 20:28:15.651203 django_restit-4.2.90/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2024-04-13 20:28:15.651337 django_restit-4.2.90/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2024-04-13 20:28:15.651445 django_restit-4.2.90/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2024-04-13 20:28:15.651500 django_restit-4.2.90/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2024-04-13 20:28:15.651633 django_restit-4.2.90/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2024-04-13 20:28:15.651698 django_restit-4.2.90/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2024-04-13 20:28:15.651754 django_restit-4.2.90/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2024-04-13 20:28:15.651802 django_restit-4.2.90/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2024-04-13 20:28:15.651859 django_restit-4.2.90/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2024-04-13 20:28:15.651952 django_restit-4.2.90/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-13 20:28:15.652008 django_restit-4.2.90/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2024-04-13 20:28:15.652134 django_restit-4.2.90/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2024-04-13 20:28:15.652198 django_restit-4.2.90/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2024-04-13 20:28:15.652246 django_restit-4.2.90/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2024-04-13 20:28:15.652381 django_restit-4.2.90/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2024-04-13 20:28:15.652434 django_restit-4.2.90/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2024-04-13 20:28:15.652482 django_restit-4.2.90/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2024-04-13 20:28:15.652541 django_restit-4.2.90/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2024-04-13 20:28:15.652606 django_restit-4.2.90/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2024-04-13 20:28:15.652663 django_restit-4.2.90/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2024-04-13 20:28:15.652727 django_restit-4.2.90/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2024-04-13 20:28:15.652785 django_restit-4.2.90/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2024-04-13 20:28:15.652835 django_restit-4.2.90/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2024-04-13 20:28:15.652886 django_restit-4.2.90/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2024-04-13 20:28:15.652934 django_restit-4.2.90/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2024-04-13 20:28:15.652984 django_restit-4.2.90/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2024-04-13 20:28:15.653031 django_restit-4.2.90/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2024-04-13 20:28:15.653082 django_restit-4.2.90/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2024-04-13 20:28:15.653133 django_restit-4.2.90/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2024-04-13 20:28:15.653202 django_restit-4.2.90/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2024-04-13 20:28:15.653257 django_restit-4.2.90/medialib/tests.py
+-rw-r--r--   0        0        0      544 2024-04-13 20:28:15.653311 django_restit-4.2.90/medialib/tq.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.653335 django_restit-4.2.90/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2024-04-13 20:28:15.653405 django_restit-4.2.90/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2024-04-13 20:28:15.653460 django_restit-4.2.90/medialib/views.py
+-rw-r--r--   0        0        0     4303 2024-04-13 20:28:15.653559 django_restit-4.2.90/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-13 20:28:15.653649 django_restit-4.2.90/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2024-04-13 20:28:15.653775 django_restit-4.2.90/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2024-04-13 20:28:15.653881 django_restit-4.2.90/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2024-04-13 20:28:15.653946 django_restit-4.2.90/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2024-04-13 20:28:15.654022 django_restit-4.2.90/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2024-04-13 20:28:15.654098 django_restit-4.2.90/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2024-04-13 20:28:15.654220 django_restit-4.2.90/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2024-04-13 20:28:15.654275 django_restit-4.2.90/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2024-04-13 20:28:15.654397 django_restit-4.2.90/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2024-04-13 20:28:15.654522 django_restit-4.2.90/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2024-04-13 20:28:15.654649 django_restit-4.2.90/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2024-04-13 20:28:15.654713 django_restit-4.2.90/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2024-04-13 20:28:15.654782 django_restit-4.2.90/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2024-04-13 20:28:15.654878 django_restit-4.2.90/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2024-04-13 20:28:15.654931 django_restit-4.2.90/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2024-04-13 20:28:15.655013 django_restit-4.2.90/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2024-04-13 20:28:15.655081 django_restit-4.2.90/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2024-04-13 20:28:15.655147 django_restit-4.2.90/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2024-04-13 20:28:15.655276 django_restit-4.2.90/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2024-04-13 20:28:15.655327 django_restit-4.2.90/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2024-04-13 20:28:15.655376 django_restit-4.2.90/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2024-04-13 20:28:15.655423 django_restit-4.2.90/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2024-04-13 20:28:15.655475 django_restit-4.2.90/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2024-04-13 20:28:15.655598 django_restit-4.2.90/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2024-04-13 20:28:15.655705 django_restit-4.2.90/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2024-04-13 20:28:15.655760 django_restit-4.2.90/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2024-04-13 20:28:15.655892 django_restit-4.2.90/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2024-04-13 20:28:15.655944 django_restit-4.2.90/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2024-04-13 20:28:15.655994 django_restit-4.2.90/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2024-04-13 20:28:15.656049 django_restit-4.2.90/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2024-04-13 20:28:15.656132 django_restit-4.2.90/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2024-04-13 20:28:15.656213 django_restit-4.2.90/metrics/README.md
+-rw-r--r--   0        0        0       90 2024-04-13 20:28:15.656260 django_restit-4.2.90/metrics/__init__.py
+-rw-r--r--   0        0        0    25251 2024-05-15 03:10:33.369045 django_restit-4.2.90/metrics/client.py
+-rw-r--r--   0        0        0     9182 2024-04-13 20:28:15.656504 django_restit-4.2.90/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2024-04-13 20:28:15.656581 django_restit-4.2.90/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.656631 django_restit-4.2.90/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.656688 django_restit-4.2.90/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-13 20:28:15.656742 django_restit-4.2.90/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2024-04-13 20:28:15.656786 django_restit-4.2.90/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2024-04-13 20:28:15.656837 django_restit-4.2.90/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2024-04-13 20:28:15.656890 django_restit-4.2.90/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2024-04-13 20:28:15.656939 django_restit-4.2.90/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2024-04-13 20:28:15.656985 django_restit-4.2.90/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2024-04-13 20:28:15.657038 django_restit-4.2.90/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2024-04-13 20:28:15.657120 django_restit-4.2.90/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2024-04-13 20:28:15.657174 django_restit-4.2.90/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2024-04-13 20:28:15.657215 django_restit-4.2.90/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2024-04-13 20:28:15.657266 django_restit-4.2.90/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2024-04-13 20:28:15.657318 django_restit-4.2.90/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.657341 django_restit-4.2.90/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    13444 2024-04-13 20:28:15.657464 django_restit-4.2.90/metrics/models.py
+-rw-r--r--   0        0        0      651 2024-04-13 20:28:15.657514 django_restit-4.2.90/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.657565 django_restit-4.2.90/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7432 2024-04-13 20:28:15.657627 django_restit-4.2.90/metrics/providers/aws.py
+-rw-r--r--   0        0        0    21300 2024-05-15 03:10:09.350305 django_restit-4.2.90/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2024-04-13 20:28:15.657771 django_restit-4.2.90/metrics/settings.py
+-rw-r--r--   0        0        0      825 2024-05-08 16:38:17.204112 django_restit-4.2.90/metrics/tq.py
+-rw-r--r--   0        0        0    12606 2024-05-15 02:58:12.813043 django_restit-4.2.90/metrics/utils.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.658051 django_restit-4.2.90/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-13 20:28:15.658105 django_restit-4.2.90/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2024-04-13 20:28:15.658188 django_restit-4.2.90/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.658208 django_restit-4.2.90/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5066 2024-04-13 20:28:15.658264 django_restit-4.2.90/pushit/models.py
+-rw-r--r--   0        0        0       88 2024-04-13 20:28:15.658337 django_restit-4.2.90/pushit/rpc/__init__.py
+-rw-r--r--   0        0        0     1756 2024-04-13 20:28:15.658394 django_restit-4.2.90/pushit/rpc/githooks.py
+-rw-r--r--   0        0        0     5028 2024-04-13 20:28:15.658451 django_restit-4.2.90/pushit/rpc/legacy.py
+-rw-r--r--   0        0        0      378 2024-04-13 20:28:15.658498 django_restit-4.2.90/pushit/rpc/products.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.658581 django_restit-4.2.90/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0      424 2024-04-13 20:28:15.658635 django_restit-4.2.90/pushit/tq.py
+-rw-r--r--   0        0        0     2121 2024-04-13 20:28:15.658692 django_restit-4.2.90/pushit/utils.py
+-rw-r--r--   0        0        0     1223 2024-05-29 18:24:05.704384 django_restit-4.2.90/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-13 20:28:15.658826 django_restit-4.2.90/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2024-04-13 20:28:15.658873 django_restit-4.2.90/rest/README.md
+-rw-r--r--   0        0        0       72 2024-04-13 20:28:15.658918 django_restit-4.2.90/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      121 2024-04-25 16:09:54.726545 django_restit-4.2.90/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2024-04-13 20:28:15.659011 django_restit-4.2.90/rest/arc4.py
+-rw-r--r--   0        0        0       83 2024-04-13 20:28:15.659054 django_restit-4.2.90/rest/cache.py
+-rw-r--r--   0        0        0       72 2024-04-13 20:28:15.659122 django_restit-4.2.90/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     4372 2024-04-13 20:28:15.659176 django_restit-4.2.90/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2024-04-13 20:28:15.659224 django_restit-4.2.90/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     4514 2024-04-13 20:28:15.659274 django_restit-4.2.90/rest/crypto/util.py
+-rw-r--r--   0        0        0    12335 2024-05-14 01:14:52.490579 django_restit-4.2.90/rest/datem.py
+-rw-r--r--   0        0        0    15082 2024-04-13 20:28:15.659521 django_restit-4.2.90/rest/decorators.py
+-rw-r--r--   0        0        0      788 2024-04-13 20:28:15.659585 django_restit-4.2.90/rest/encryption.py
+-rw-r--r--   0        0        0      612 2024-04-13 20:28:15.659638 django_restit-4.2.90/rest/errors.py
+-rw-r--r--   0        0        0       54 2024-04-13 20:28:15.659709 django_restit-4.2.90/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-13 20:28:15.659754 django_restit-4.2.90/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2024-04-13 20:28:15.659880 django_restit-4.2.90/rest/fields.py
+-rw-r--r--   0        0        0     6316 2024-04-13 20:28:15.659935 django_restit-4.2.90/rest/forms.py
+-rw-r--r--   0        0        0    29450 2024-05-16 16:51:41.779758 django_restit-4.2.90/rest/helpers.py
+-rw-r--r--   0        0        0      260 2024-04-13 20:28:15.660082 django_restit-4.2.90/rest/joke.py
+-rw-r--r--   0        0        0     2444 2024-05-11 18:15:45.432169 django_restit-4.2.90/rest/jwtoken.py
+-rw-r--r--   0        0        0    20930 2024-04-13 20:28:15.660211 django_restit-4.2.90/rest/log.py
+-rw-r--r--   0        0        0     7965 2024-04-30 22:59:33.205817 django_restit-4.2.90/rest/mail.py
+-rw-r--r--   0        0        0     9174 2024-04-13 20:28:15.660384 django_restit-4.2.90/rest/mailman.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.660446 django_restit-4.2.90/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.660519 django_restit-4.2.90/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-13 20:28:15.660585 django_restit-4.2.90/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2024-04-13 20:28:15.660670 django_restit-4.2.90/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2024-04-13 20:28:15.660732 django_restit-4.2.90/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2024-04-13 20:28:15.660813 django_restit-4.2.90/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     6017 2024-04-13 20:28:15.660879 django_restit-4.2.90/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4189 2024-04-13 20:28:15.660938 django_restit-4.2.90/rest/middleware/request.py
+-rw-r--r--   0        0        0    10240 2024-04-13 20:28:15.661058 django_restit-4.2.90/rest/middleware/session.py
+-rw-r--r--   0        0        0     1901 2024-04-13 20:28:15.661107 django_restit-4.2.90/rest/middleware/session_store.py
+-rw-r--r--   0        0        0      130 2024-04-13 20:28:15.661198 django_restit-4.2.90/rest/models/__init__.py
+-rw-r--r--   0        0        0    69675 2024-05-12 22:38:49.331753 django_restit-4.2.90/rest/models/base.py
+-rw-r--r--   0        0        0      578 2024-04-13 20:28:15.661399 django_restit-4.2.90/rest/models/cacher.py
+-rw-r--r--   0        0        0    12904 2024-05-22 18:31:57.736705 django_restit-4.2.90/rest/models/metadata.py
+-rw-r--r--   0        0        0     2974 2024-04-13 20:28:15.661574 django_restit-4.2.90/rest/net.py
+-rw-r--r--   0        0        0   149463 2024-04-13 20:28:15.661780 django_restit-4.2.90/rest/regexes.yaml
+-rw-r--r--   0        0        0    16127 2024-04-13 20:28:15.661904 django_restit-4.2.90/rest/requestex.py
+-rw-r--r--   0        0        0     4200 2024-04-13 20:28:15.661966 django_restit-4.2.90/rest/rpc.py
+-rw-r--r--   0        0        0     8362 2024-04-13 20:28:15.662107 django_restit-4.2.90/rest/search.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.662168 django_restit-4.2.90/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     4646 2024-04-13 20:28:15.662236 django_restit-4.2.90/rest/serializers/collection.py
+-rw-r--r--   0        0        0     3916 2024-04-13 20:28:15.662294 django_restit-4.2.90/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2024-04-13 20:28:15.662347 django_restit-4.2.90/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2024-04-13 20:28:15.662397 django_restit-4.2.90/rest/serializers/json.py
+-rw-r--r--   0        0        0    61981 2024-04-13 20:28:15.662517 django_restit-4.2.90/rest/serializers/legacy.py
+-rw-r--r--   0        0        0      410 2024-04-13 20:28:15.662578 django_restit-4.2.90/rest/serializers/localizers.py
+-rw-r--r--   0        0        0     8598 2024-04-13 20:28:15.662709 django_restit-4.2.90/rest/serializers/model.py
+-rw-r--r--   0        0        0      997 2024-04-13 20:28:15.662760 django_restit-4.2.90/rest/serializers/profiler.py
+-rw-r--r--   0        0        0     7602 2024-05-10 20:20:45.107027 django_restit-4.2.90/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2024-04-13 20:28:15.662937 django_restit-4.2.90/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2024-04-13 20:28:15.662997 django_restit-4.2.90/rest/settings_helper.py
+-rw-r--r--   0        0        0     1419 2024-04-13 20:28:15.663054 django_restit-4.2.90/rest/ssl_check.py
+-rw-r--r--   0        0        0    95786 2024-04-13 20:28:15.663327 django_restit-4.2.90/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.663392 django_restit-4.2.90/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.663422 django_restit-4.2.90/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.663450 django_restit-4.2.90/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.663479 django_restit-4.2.90/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2024-04-13 20:28:15.663592 django_restit-4.2.90/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.663618 django_restit-4.2.90/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2024-04-13 20:28:15.663684 django_restit-4.2.90/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    11048 2024-04-13 20:28:15.663811 django_restit-4.2.90/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185398 2024-04-13 20:28:15.664071 django_restit-4.2.90/rest/ua.py
+-rw-r--r--   0        0        0    17064 2024-04-13 20:28:15.664170 django_restit-4.2.90/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2024-04-13 20:28:15.664320 django_restit-4.2.90/rest/url_docs.py
+-rw-r--r--   0        0        0     1870 2024-04-30 22:59:33.197788 django_restit-4.2.90/rest/urls.py
+-rw-r--r--   0        0        0     1115 2024-04-13 20:28:15.664431 django_restit-4.2.90/rest/views.py
+-rw-r--r--   0        0        0      118 2024-04-13 20:28:15.664508 django_restit-4.2.90/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2024-04-13 20:28:15.664553 django_restit-4.2.90/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.664575 django_restit-4.2.90/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-13 20:28:15.664632 django_restit-4.2.90/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2024-04-13 20:28:15.664704 django_restit-4.2.90/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.664729 django_restit-4.2.90/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3662 2024-04-13 20:28:15.664797 django_restit-4.2.90/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2024-04-13 20:28:15.664849 django_restit-4.2.90/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2024-04-13 20:28:15.664899 django_restit-4.2.90/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2024-04-13 20:28:15.664987 django_restit-4.2.90/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.665015 django_restit-4.2.90/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-13 20:28:15.665073 django_restit-4.2.90/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2024-04-13 20:28:15.665172 django_restit-4.2.90/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.665197 django_restit-4.2.90/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    22407 2024-04-13 20:28:15.665283 django_restit-4.2.90/taskqueue/models.py
+-rw-r--r--   0        0        0     3543 2024-04-13 20:28:15.665348 django_restit-4.2.90/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5793 2024-05-11 15:22:18.077751 django_restit-4.2.90/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2024-04-13 20:28:15.665450 django_restit-4.2.90/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.665504 django_restit-4.2.90/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2024-04-13 20:28:15.665563 django_restit-4.2.90/taskqueue/transports/email.py
+-rw-r--r--   0        0        0      839 2024-04-13 20:28:15.665619 django_restit-4.2.90/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1913 2024-04-13 20:28:15.665676 django_restit-4.2.90/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2024-04-13 20:28:15.665722 django_restit-4.2.90/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2024-04-13 20:28:15.665764 django_restit-4.2.90/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    15822 2024-04-13 20:28:15.665889 django_restit-4.2.90/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.665935 django_restit-4.2.90/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-13 20:28:15.665979 django_restit-4.2.90/telephony/admin.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.665998 django_restit-4.2.90/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2024-04-13 20:28:15.666076 django_restit-4.2.90/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0      424 2024-04-13 20:28:15.666121 django_restit-4.2.90/telephony/migrations/0002_alter_sms_sid.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.666142 django_restit-4.2.90/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     8248 2024-04-13 20:28:15.666266 django_restit-4.2.90/telephony/models.py
+-rw-r--r--   0        0        0     5067 2024-04-13 20:28:15.666315 django_restit-4.2.90/telephony/phone_util.py
+-rw-r--r--   0        0        0     3473 2024-04-13 20:28:15.666362 django_restit-4.2.90/telephony/rpc.py
+-rw-r--r--   0        0        0        1 2024-04-13 20:28:15.666426 django_restit-4.2.90/wiki/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-13 20:28:15.666501 django_restit-4.2.90/wiki/migrations/0001_initial.py
+-rw-r--r--   0        0        0      485 2024-05-13 02:34:55.168648 django_restit-4.2.90/wiki/migrations/0002_alter_pagemedia_entry.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.666521 django_restit-4.2.90/wiki/migrations/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-13 20:28:15.666590 django_restit-4.2.90/wiki/models/__init__.py
+-rw-r--r--   0        0        0     1745 2024-04-13 20:28:15.666635 django_restit-4.2.90/wiki/models/faq.py
+-rw-r--r--   0        0        0     7203 2024-04-13 20:28:15.666696 django_restit-4.2.90/wiki/models/page.py
+-rw-r--r--   0        0        0      729 2024-04-13 20:28:15.666741 django_restit-4.2.90/wiki/models/revision.py
+-rw-r--r--   0        0        0      334 2024-04-13 20:28:15.666791 django_restit-4.2.90/wiki/periodic.py
+-rw-r--r--   0        0        0      461 2024-04-13 20:28:15.666864 django_restit-4.2.90/wiki/renderers/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-04-13 20:28:15.666938 django_restit-4.2.90/wiki/renderers/mistune/__init__.py
+-rwxr-xr-x   0        0        0     1264 2024-04-13 20:28:15.666986 django_restit-4.2.90/wiki/renderers/mistune/highlight.py
+-rwxr-xr-x   0        0        0     1901 2024-04-13 20:28:15.667033 django_restit-4.2.90/wiki/renderers/mistune/math.py
+-rw-r--r--   0        0        0     2610 2024-04-13 20:28:15.667082 django_restit-4.2.90/wiki/renderers/mistune/media.py
+-rwxr-xr-x   0        0        0      805 2024-04-13 20:28:15.667124 django_restit-4.2.90/wiki/renderers/mistune/meta.py
+-rw-r--r--   0        0        0     1889 2024-04-13 20:28:15.667169 django_restit-4.2.90/wiki/renderers/mistune/task_list.py
+-rwxr-xr-x   0        0        0     2302 2024-04-13 20:28:15.667217 django_restit-4.2.90/wiki/renderers/mistune/toc.py
+-rw-r--r--   0        0        0       40 2024-04-13 20:28:15.667294 django_restit-4.2.90/wiki/rpc/__init__.py
+-rw-r--r--   0        0        0     1333 2024-04-13 20:28:15.667341 django_restit-4.2.90/wiki/rpc/wiki.py
+-rw-r--r--   0        0        0      313 2024-04-13 20:28:15.667390 django_restit-4.2.90/wiki/tq.py
+-rw-r--r--   0        0        0     3624 2024-04-13 20:28:15.667476 django_restit-4.2.90/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2024-04-13 20:28:15.667515 django_restit-4.2.90/ws4redis/__init__.py
+-rw-r--r--   0        0        0     7013 2024-04-13 20:28:15.667571 django_restit-4.2.90/ws4redis/client.py
+-rw-r--r--   0        0        0    13431 2024-04-13 20:28:15.667695 django_restit-4.2.90/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2024-04-13 20:28:15.667746 django_restit-4.2.90/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     6093 2024-04-13 20:28:15.667813 django_restit-4.2.90/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2024-04-13 20:28:15.667877 django_restit-4.2.90/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2024-04-13 20:28:15.667948 django_restit-4.2.90/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     5898 2024-04-30 22:59:33.206473 django_restit-4.2.90/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2024-04-13 20:28:15.668065 django_restit-4.2.90/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1536 2024-04-13 20:28:15.668112 django_restit-4.2.90/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2024-04-13 20:28:15.668166 django_restit-4.2.90/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2024-04-25 19:45:04.792690 django_restit-4.2.90/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7645 1970-01-01 00:00:00.000000 django_restit-4.2.90/PKG-INFO
```

### Comparing `django_restit-4.2.9/LICENSE.md` & `django_restit-4.2.90/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/README.md` & `django_restit-4.2.90/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/admin.py` & `django_restit-4.2.90/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/fcm/__init__.py` & `django_restit-4.2.90/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0001_initial.py` & `django_restit-4.2.90/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0003_member_phone_number.py` & `django_restit-4.2.90/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.2.90/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.2.90/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.2.90/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0011_authtoken.py` & `django_restit-4.2.90/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.2.90/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/migrations/0014_alter_notificationmemberrecord_member.py` & `django_restit-4.2.90/account/migrations/0014_alter_notificationmemberrecord_member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/models/device.py` & `django_restit-4.2.90/account/models/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from django.db import models
 from rest import models as rm
+from rest import fields as rf
 from rest import settings
 from objict import objict
 from datetime import datetime
 
 CM_BACKENDS = objict()
 DEVICE_USE_BUID = settings.get("DEVICE_USE_BUID", False)
 
@@ -106,14 +107,53 @@
         return True
 
 
 class MemberDeviceMetaData(rm.MetaDataBase):
     parent = models.ForeignKey(MemberDevice, related_name="properties", on_delete=models.CASCADE)
 
 
+class CloudCredentials(models.Model, rm.RestModel, rm.MetaDataModel):
+    """
+    CloudCredentials is a global setting for a group to store this groups cloud credentials.
+    """
+    class RestMeta:
+        VIEW_PERMS = ["view_cm", "manage_cm"]
+        EDIT_PERMS = ["manage_cm"]
+        GRAPHS = {
+            "default": {
+                "extra": ["metadata"],
+                "graphs": {
+                    "group": "basic"
+                }
+            }
+        }
+
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+    group = models.ForeignKey("account.Group", related_name="cloud_credentials", on_delete=models.CASCADE)
+
+    name = models.CharField(max_length=128, blank=True, null=True, default=None)
+    uuid = models.CharField(db_index=True, max_length=64, blank=True, null=True, default=None)
+    state = models.IntegerField(db_index=True, default=1)
+
+    credentials = rf.JSONField()
+
+    def sendToDevice(self, device, message):
+        pass
+
+    def sendNotification(self, token, title, body):
+        pass
+
+
+class CloudCredentialsMetaData(rm.MetaDataBase):
+    parent = models.ForeignKey(CloudCredentials, related_name="properties", on_delete=models.CASCADE)
+
+
 def getCloudMessanger(name):
+    # creds = CloudCredentials.objects.filter(uuid=name).last()
+    # if creds is not None:
+    #     return creds
     if name not in CM_BACKENDS:
         if name == "fcm":
             from account import fcm
             CM_BACKENDS["fcm"] = fcm
-    return CM_BACKENDS[name]
-
+    return CM_BACKENDS.get(name, None)
```

### Comparing `django_restit-4.2.9/account/models/feeds.py` & `django_restit-4.2.90/incident/models/ticket.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,65 @@
 from django.db import models
+from django.conf import settings
 
+from rest import models as rm
+from rest import helpers as rh
 
-class FeedBase(models.Model):
-    class Meta:
-        abstract = True
 
+class Ticket(models.Model, rm.RestModel, rm.MetaDataModel):
     class RestMeta:
+        SEARCH_FIELDS = ["title", "description"]
+        CAN_DELETE = True
+        VIEW_PERMS = ["view_tickets"]
         GRAPHS = {
             "default": {
-                "recurse_into": ["generic__component"]
-            }
+                "extra": ["metadata"],
+                "graphs": {
+                    "group": "basic",
+                    "created_by": "basic",
+                    "assigned_to": "basic",
+                    "incident": "basic"
+                },
+            },
+            "detailed": {
+                "graphs": {
+                    "group": "basic",
+                    "created_by": "basic",
+                    "assigned_to": "basic",
+                    "incident": "basic",
+                    "generic__component": "basic"
+                },
+            },
         }
 
-    created = models.DateTimeField(auto_now_add=True, editable=True, db_index=True)
-    component = models.SlugField(max_length=124, null=True, blank=True, default=None, db_index=True)
-    component_id = models.IntegerField(null=True, blank=True, default=None, db_index=True)
-
-    kind = models.SlugField(max_length=32, db_index=True)
-    note = models.TextField(null=True, blank=True, default=None)
-
-    @classmethod
-    def log(cls, member, group, kind, component=None, component_id=None, note=None):
-        obj = cls(member=member, group=group, kind=kind, component=component, component_id=component_id, note=note)
-        obj.save()
-        return obj
-
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
 
-class MemberFeed(FeedBase):
-    member = models.ForeignKey("account.Member", default=None, null=True, related_name="feed", on_delete=models.CASCADE)
-    group = models.ForeignKey("account.Group", default=None, null=True, related_name="+", on_delete=models.CASCADE)
-
-
-class GroupFeed(FeedBase):
-    member = models.ForeignKey("account.Member", default=None, null=True, related_name="+", on_delete=models.CASCADE)
-    group = models.ForeignKey("account.Group", default=None, null=True, related_name="feed", on_delete=models.CASCADE)
+    group = models.ForeignKey(
+        "account.Group", on_delete=models.SET_NULL, 
+        related_name="tickets",
+        null=True, default=None)
+    assigned_to = models.ForeignKey(
+        "account.Member", on_delete=models.SET_NULL, 
+        related_name="tickets",
+        null=True, default=None)
+    created_by = models.ForeignKey(
+        "account.Member", on_delete=models.CASCADE,
+        related_name="+",
+        null=True, default=None)
+
+    # if category is null then this will run on all events?
+    category = models.CharField(max_length=200, db_index=True)
+    priority = models.IntegerField(default=10, db_index=True)  # 1-10, 1 being the highest
+
+    title = models.CharField(max_length=200)
+    description = models.TextField()
+
+    status = models.CharField(max_length=32, default=None, null=True, db_index=True)
+    state = models.IntegerField(default=0)  # how many incidents before firing action
+
+    incident = models.ForeignKey(
+        "incident.Incident", null=True, default=None, 
+        related_name="tickets", on_delete=models.SET_NULL)
 
+    component = models.CharField(max_length=200, null=True, default=None, db_index=True)
+    component_id = models.IntegerField(null=True, blank=True, default=None, db_index=True)
```

### Comparing `django_restit-4.2.9/account/models/group.py` & `django_restit-4.2.90/account/models/group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.db import models
 from django.db.models import Q
-from rest import settings
-app_settings = settings.getAppSettings("account")
 import re
 
 from rest.models import RestModel, MetaDataModel, MetaDataBase, RestValidationError, PermissionDeniedException
 from rest import helpers as rh
 from rest import RemoteEvents
 from rest import crypto
 from rest import mail as rest_mail
 from rest.views import restPermissionDenied
 
 from .member import Member
 
-
+from rest import settings
+app_settings = settings.getAppSettings("account")
 MEMBERSHIP_ROLES = settings.get("MEMBERSHIP_ROLES", None)
 TRUE_VALUES = app_settings.get("TRUE_VALUES", [])
 
+
 class Group(models.Model, RestModel, MetaDataModel):
     """
     Group Model allows for the grouping of other models and works with Member throug Membership Model
 
     parent allows for tree based heirachy of groups
     children allows for manytomany relationships with other groups
     kind is heavily used to filter different kinds of groups
@@ -34,23 +34,37 @@
     kind = models.CharField(db_index=True, max_length=80, default="org")
     parent = models.ForeignKey("Group", default=None, null=True, blank=True, related_name="groups", on_delete=models.CASCADE)
 
     is_active = models.BooleanField(default=True, blank=True)
     # this is the new model for groups having multiple parents
     children = models.ManyToManyField("self", related_name="parents", symmetrical=False)
 
+    location = models.ForeignKey(
+        "location.Address", default=None, null=True, blank=True,
+        related_name="+", on_delete=models.SET_NULL)
+
     class RestMeta:
         SEARCH_FIELDS = [
             "name"
         ]
         LIST_DEFAULT_FILTERS = {
             "is_active": True
         }
+        LIST_PARENT_KINDS = ["org", "iso"]
         POST_SAVE_FIELDS = ["child_of"]
-        VIEW_PERMS = ["view_all_groups", "manage_groups", "is_terminal"]
+        GROUP_FIELD = "self"
+        VIEW_PERMS = [
+            "view_all_groups",
+            "manage_groups",
+            "manage_group",
+            "manage_settings"]
+        SAVE_PERMS = [
+            "manage_groups",
+            "manage_group",
+            "manage_settings"]
         CREATE_PERMS = ["manage_groups", "create_groups"]
         GRAPHS = {
             "basic": {
                 "fields": [
                     "id",
                     "parent",
                     "uuid",
@@ -62,25 +76,34 @@
                     "is_active",
                     "timezone"
                 ]
             },
             "default": {
                 "graphs": {
                     "self": "basic",
-                    "parent": "basic"
+                    "parent": "basic",
+                    "location": "basic"
                 },
                 "fields": ["metadata"],
             },
             "detailed": {
                 "graphs": {
                     "self": "basic",
                     "parent": "basic",
-                    "children": "basic"
+                    "children": "basic",
+                    "location": "basic"
                 },
-                "fields": ["metadata"],
+                "extra": ["metadata"],
+            },
+            "location": {
+                "fields": ["name", "kind", "id"],
+                "extra": ["location"],
+                "graphs": {
+                    "location": "basic"
+                }
             },
             "abstract": {
                 "fields": [
                     ('uuid', 'id'),
                     "name",
                     "kind",
                     "timezone"
@@ -92,20 +115,24 @@
                 "created",
                 "id",
                 "name",
                 "kind",
                 ("metadata__timezone", "timezone"),
                 ("metadata__eod", "end_of_day"),
                 ("parent__name", "parent"),
-                ("metadata.location.line1", "address_line1"),
-                ("metadata.location.line2", "address_line2"),
-                ("metadata.location.city", "city"),
-                ("metadata.location.state", "state"),
-                ("metadata.location.country", "country"),
-                ("metadata.location.zip", "zipcode")
+                ("location.line1", "address_line1"),
+                ("location.line2", "address_line2"),
+                ("location.city", "city"),
+                ("location.state", "state"),
+                ("location.county", "county"),
+                ("location.country", "country"),
+                ("location.postalcode", "zipcode"),
+                ("location.postalcode_suffix", "zipcode_ext"),
+                ("location.lat", "lat"),
+                ("location.lng", "lng")
             ]
         }
 
     @property
     def timezone(self):
         return self.getProperty("timezone", "America/Los_Angeles")
 
@@ -114,14 +141,20 @@
         zone = self.getProperty("timezone", "America/Los_Angeles")
         return rh.getShortTZ(zone)
 
     @property
     def file_safe_name(self):
         return re.sub("[^0-9a-zA-Z]+", "_", self.name.lower())
 
+    @property
+    def initials(self):
+        if self.name:
+            return "".join([s[0] for s in self.name.split(' ')]).upper()
+        return None
+
     def thumbnail(self, name="default"):
         lib = self.libraries.filter(name=name).first()
         if lib:
             item = lib.items.all().first()
             if item:
                 return item.thumbnail_url()
         return None
@@ -137,43 +170,57 @@
         parent_id = request.DATA.get(["parent", "parent_id"])
         if parent_id:
             parent = request.member.getGroup(parent_id)
             if not parent:
                 raise PermissionDeniedException("invalid parent")
             qset = qset.filter(parent=parent)
         elif child_of:
-            parent = parent = request.member.getGroup(child_of)
+            parent = request.member.getGroup(child_of)
             if parent:
                 request.group = None
                 return parent.getAllChildren(grand_children=True)
         return qset
 
     def on_rest_get(self, request):
         if (request.member and request.member.isMemberOf(self)) or self.on_rest_can_get(request):
             return self.restGet(request)
         return restPermissionDenied(request)
 
-    def onRestCanSave(self, request=None, data=None, extended=None):
-        if request.member is None:
-            raise PermissionDeniedException("permission denied for save")
-        if request.member.hasPermission(["manage_groups", "create_groups"]):
-            return True
-        if self.checkPermission(request.member, ["manage_settings", "manage_members"]):
-            return True
-        raise PermissionDeniedException("permission denied for save")
+    # def onRestCanSave(self, request=None, data=None, extended=None):
+    #     if request.member is None:
+    #         raise PermissionDeniedException("permission denied for save")
+    #     if request.member.hasPermission(["manage_groups", "create_groups"]):
+    #         return True
+    #     if self.checkPermission(request.member, ["manage_settings", "manage_members", "manage_group"]):
+    #         return True
+    #     raise PermissionDeniedException("permission denied for save")
 
     def on_rest_pre_save(self, request, **kwargs):
         pass
 
     def on_rest_saved(self, request, is_new=False):
         if request.member:
             note = "edited group {}:{}\n{}".format(self.name, self.pk, request.DATA.asDict())
             request.member.log("group_edit", note, method="group")
+            self.auditLog(note, "group_edit", level=21)
             self.logEvent("group_edit", component="account.Member", component_id=request.member.id, note=note)
 
+    def set_name(self, value):
+        if value is not None:
+            self.name = value.strip()
+        else:
+            self.name = None
+
+    def set_parent(self, value):
+        if isinstance(value, (str, int)):
+            if int(value) == self.pk:
+                raise RestValidationError("cannot set self as parent", 1101)
+            value = Group.objects.filter(pk=value).last()
+        self.parent = value
+    
     def set_child_of(self, value):
         # this is a helper to add this group to another group
         parent = Group.objects.filter(pk=value).last()
         if parent and parent.pk != self.pk:
             if not parent.children.filter(pk=self.pk).exists() and not self.hasChild(parent) and self.kind != "org":
                 parent.children.add(self)
 
@@ -189,14 +236,15 @@
 
     def getChildModels(self, Model, grand_children=False, great_grand_children=False):
         q = Q(group=self)
         if grand_children:
             q = q | Q(group__parent=self)
         if great_grand_children:
             q = q | Q(group__parent__parent=self)
+            q = q | Q(group__parent__parent__parent=self)
         if hasattr(Model, "objects"):
             return Model.objects.filter(q)
         return Model.filter(q)
 
     def getChildren(self):
         return Group.objects.filter(parent=self)
 
@@ -204,17 +252,22 @@
         q = Q(parent=self)| Q(parents=self)
         if include_me:
             q = q | Q(pk=self.id)
         if grand_children:
             q = q | Q(parent__parent=self)
         if great_grand_children:
             q = q | Q(parent__parent__parent=self)
+            q = q | Q(parent__parent__parent__parent=self)
         return Group.objects.filter(q)
 
-    def getAllChildrenIds(self, include_me=False, grand_children=False, great_grand_children=False):
+    def getAllChildrenIds(self, include_me=False, grand_children=False, great_grand_children=False, depth=0):
+        if depth > 1:
+            grand_children = True
+        if depth > 2:
+            great_grand_children = True
         qset = self.getAllChildren(include_me, grand_children, great_grand_children)
         return list(qset.values_list("id", flat=True))
 
     def hasChild(self, group):
         if not group:
             return False
         if self.children.filter(pk=group.pk).exists():
@@ -249,20 +302,24 @@
                 return True
             if parent.hasParent(group):
                 return True
         return False
 
     def notifyMembers(self, subject, message=None, template=None, context=None, 
                       email_only=False, sms_msg=None, perms=None, force=False,
-                      from_email=None):
+                      from_email=None, exclude_member=None):
         if perms is not None:
-            members = self.getMembers(perms=perms, as_member=True)
+            members = self.getMembers(perms=perms, as_member=True, exclude_member=exclude_member)
         else:
             Member = RestModel.getModel("account", "Member")
-            members = Member.objects.filter(is_active=True, memberships__group=self, memberships__state__gte=-10)
+            members = Member.objects.filter(
+                is_active=True, memberships__group=self,
+                memberships__state__gte=-10)
+            if exclude_member:
+                members = members.exclude(pk=exclude_member.pk)
         NotificationRecord = RestModel.getModel("account", "NotificationRecord")
         NotificationRecord.notify(
             members, subject, message, template,
             context, email_only, sms_msg, force,
             from_email=from_email)
 
     def hasPerm(self, member, perm, staff_override=True, check_member=False):
@@ -330,54 +387,58 @@
         if self.memberships.filter(member=member, role=role).count():
             return None
         Membership = RestModel.getModel("account", "Membership")
         ms = Membership(group=self, member=member, role=role)
         ms.save()
         return ms
 
-    def getMembers(self, perms=None, role=None, as_member=False):
+    def getMembers(self, perms=None, role=None, as_member=False, exclude_member=None):
         if isinstance(perms, str):
             perms = [perms]
         if isinstance(role, str):
             role = [role]
         notify = None
         if perms:
             notify = [p.split('.')[1] for p in perms if p.startswith("notify.")]
             perms = [p for p in perms if not p.startswith("notify.")]
         if as_member:
             Member = RestModel.getModel("account", "Member")
-            res = Member.objects.filter(is_active=True, memberships__group=self, memberships__state__gte=-10)
+            qset = Member.objects.filter(is_active=True, memberships__group=self, memberships__state__gte=-10)
             if perms:
-                res = res.filter(memberships__group=self, memberships__properties__category="permissions", memberships__properties__key__in=perms, memberships__properties__value__in=TRUE_VALUES)
+                qset = qset.filter(memberships__group=self, memberships__properties__category="permissions", memberships__properties__key__in=perms, memberships__properties__value__in=TRUE_VALUES)
             if notify:
-                res = res.filter(memberships__group=self, memberships__properties__category="notify", memberships__properties__key__in=notify, memberships__properties__value__in=TRUE_VALUES)
+                qset = qset.filter(memberships__group=self, memberships__properties__category="notify", memberships__properties__key__in=notify, memberships__properties__value__in=TRUE_VALUES)
             if role:
-                res = res.filter(memberships__group=self, memberships__role__in=role)
-            return res.distinct()
-        res = self.memberships.filter(state__gte=-10)
+                qset = qset.filter(memberships__group=self, memberships__role__in=role)
+            if exclude_member:
+                qset = qset.exclude(pk=exclude_member.pk)
+            return qset.distinct()
+        qset = self.memberships.filter(state__gte=-10)
         if perms:
-            res = res.filter(
+            qset = qset.filter(
                 Q(properties__category="permissions", 
                   properties__key__in=perms, 
                   properties__value__in=TRUE_VALUES) | 
                 Q(member__properties__category="permissions", 
                   member__properties__key__in=perms, 
                   member__properties__value__in=TRUE_VALUES))
         if notify:
-            res = res.filter(
+            qset = qset.filter(
                 Q(properties__category="notify", 
                   properties__key__in=notify, 
                   properties__value__in=TRUE_VALUES) | 
                 Q(member__properties__category="notify", 
                   member__properties__key__in=notify, 
                   member__properties__value__in=TRUE_VALUES))
 
         if role:
-            res = res.filter(role__in=role)
-        return res.distinct()
+            qset = qset.filter(role__in=role)
+        if exclude_member:
+            qset = qset.exclude(member__pk=exclude_member.pk)
+        return qset.distinct()
 
     def getParentIDs(self):
         ids = []
         group = self
         counter = 0
         while group.parent != None and counter < 6:
             counter += 1
@@ -395,22 +456,22 @@
             counter += 1
             group = group.parent
             ms = group.getMembership(member)
             if ms:
                 return ms
         return ms
 
-
     def invite(self, member, role="guest"):
         # invite a user to this group
         Membership = RestModel.getModel("account", "Membership")
         ms = Membership.objects.filter(group=self, member=member).last()
         if ms is None:
             ms = Membership(member=member, group=self, role=role)
             ms.save()
+            ms.on_rest_created(self.getActiveRequest())
         elif ms.role != role:
             ms.clearPermissions()
         if not ms.is_enabled:
             # enable again?
             ms.set_state(0)
             ms.save()
```

### Comparing `django_restit-4.2.9/account/models/legacy.py` & `django_restit-4.2.90/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/models/member.py` & `django_restit-4.2.90/account/models/member.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             "is_staff",
             ("ip", "auth_sessions__ip"),
             ("notify_via", "properties|notify_via"),
             ("phone", "phone_number"),
             ("perms", "properties|permissions.")]
         QUERY_FIELDS_SPECIAL = {
             "ip": "auth_sessions__ip",
+            "login_country": "auth_sessions__location__country",
+            "not_login_country": "auth_sessions__location__country__ne"
         }
         UNIQUE_LOOKUP = ["username", "email"]
         METADATA_FIELD_PROPERTIES = settings.USER_METADATA_PROPERTIES
         GRAPHS = {
             "basic": {
                 "fields": [
                     'id',
@@ -124,14 +126,15 @@
                     'is_active',
                     'is_blocked',
                     'is_staff',
                     'is_superuser',
                     'requires_totp',
                     'last_login',
                     'last_activity',
+                    'password_changed',
                     ('date_joined', 'created'),
                     ("hasLoggedIn", "has_logged_in"),
                     'avatar',
                     'has_totp',
                     'auth_token'
                 ],
                 "extra": ["metadata", "password_expires_in"],
@@ -156,14 +159,20 @@
 
     def __str__(self):
         return self.username
 
     def getUser(self):
         return self.user_ptr
 
+    def getUUID(self):
+        if not self.uuid and self.pk:
+            self.uuid = Member.generateUUID(self.pk)
+            self.save()
+        return self.uuid
+
     def getGroup(self, group_id, include_parents=True):
         # now we want to verify we are a member of this group or a parent group
         if isinstance(group_id, str) and not group_id.isdigit():
             return None
         Group = RestModel.getModel("account", "Group")
         if self.hasPerm("view_all_groups"):
             return Group.objects.filter(pk=group_id).first()
@@ -210,14 +219,22 @@
     def auth_token(self):
         token = AuthToken.objects.filter(member=self, role="default").last()
         if token:
             return token.secure_token
         return None
 
     @property
+    def force_single_session(self):
+        return self.hasPermission("force_single_session", ignore_su=True)
+
+    @property
+    def email_disabled(self):
+        return self.hasPermission("email_disabled", ignore_su=True)
+
+    @property
     def has_totp(self):
         token = self.getProperty("totp_token", category="secrets", default=None)
         verified = self.getProperty("totp_verified", default=False)
         return token is not None and verified
 
     @property
     def password_expires_in(self):
@@ -272,30 +289,40 @@
 
     def login(self, password=None, request=None, use_jwt=False):
         if not self.is_active or self.is_blocked:
             return False
         # can force login
         if not request:
             request = rh.getActiveRequest()
-        if password:
-            if not self.checkPassword(password):
-                # invalid password
-                self.recordFailedLogin(request)
-                return False
-            else:
-                self.recordSuccessLogin(request)
+        if not self.checkPassword(password):
+            # invalid password
+            self.recordFailedLogin(request)
+            return False
+        else:
+            self.recordSuccessLogin(request)
         if use_jwt:
             self.recordSuccessLogin(request)
             self.locateByIP(request.ip)
             return True
         self.user_ptr.backend = 'django.contrib.auth.backends.ModelBackend'
         auth_login(request, self.user_ptr)
         self.locateByIP(request.ip)
         return True
 
+    def loginNoPassword(self, request=None):
+        if not self.is_active or self.is_blocked:
+            return False
+        # can force login
+        if not request:
+            request = rh.getActiveRequest()
+        self.user_ptr.backend = 'django.contrib.auth.backends.ModelBackend'
+        auth_login(request, self.user_ptr)
+        self.locateByIP(request.ip)
+        return True
+
     def canLogin(self, request=None, throw_exception=True):
         if not self.is_active:
             self.log("login_blocked", F"account is not active {self.username}", request, method="login", level=31)
             if throw_exception:
                 if request is not None:
                     request.member = self
                 raise PermissionDeniedException(
@@ -463,16 +490,17 @@
                 group = Group.objects.get(pk=group)
             return group.getMembership(self, True)
             # now check by children
         return self.memberships.filter(group=group).first()
 
     def disable(self, by="system", reason="", notify=True):
         self.is_active = False
+        self.security_token = None
         self.save()
-        self.memberships.update(state=-100)
+        self.memberships.update(state=-25)
 
         [s.delete() for s in Session.objects.all() if s.get_decoded().get('_auth_user_id') == self.pk]
         # notify account disabled
         subject = f"MEMBER {self.username} DISABLED BY {by}"
         accounts = []
         body = "{}<br>\ndisabled from: ".format(reason)
         for m in self.memberships.all():
@@ -481,42 +509,62 @@
         self.log(
             "disabled",
             f"account({self.username}) disabled by {by}, {reason}",
             method="disabled", level=35)
         if notify:
             Member.notifyWithPermission("user_audit", subject, message=body, email_only=True)
 
-    def enable(self, by, memberships=None):
+    def enable(self, by, memberships=None, notify=True):
         if not self.is_active:
             self.is_active = True
             self.save()
-        # notify account disabled
-        subject = "MEMBER {} RE-ENABLED BY {}".format(self, by)
-        body = "enabled for: "
         if memberships is None:
             memberships = self.memberships.all()
-
         accounts = []
         for m in memberships:
             m.state = 10
             m.save()
             accounts.append(m.group.name)
-        body += "<br>\n".join(accounts)
         self.log("enabled", "account enabled by {}".format(by.username), method="enabled", level=35)
-        Member.notifyWithPermission("user_audit", subject, message=body, email_only=True)
+        if notify:
+            # notify account disabled
+            subject = f"MEMBER {self.username} RE-ENABLED BY {by.username}"
+            body = "enabled for: "
+            body += "<br>\n".join(accounts)
+            Member.notifyWithPermission("user_audit", subject, message=body, email_only=True)
 
-    def locateByIP(self, ip):
+    def locateByIP(self, ip, security_check=True):
         loc = GeoIP.get(ip)
         if loc is not None:
             self.setProperty("last_ip", ip)
             self.setProperty("city", loc.city, "location")
             self.setProperty("state", loc.state, "location")
             self.setProperty("country", loc.country, "location")
             self.setProperty("lat", loc.lat, "location")
             self.setProperty("lng", loc.lng, "location")
+            if security_check:
+                self.checkLocationSecurity(loc)
+
+    def checkLocationSecurity(self, loc=None, ip=None):
+        if loc is None and ip is None:
+            return
+        if loc is None:
+            loc = GeoIP.get(ip)
+        auth_session = self.auth_sessions.last()
+        # check for state or country changes
+        if auth_session is not None and auth_session.location is not None:
+            try:
+                if auth_session.location.country != loc.country:
+                    details = f"user({self.username}) login from new country {loc.country} vs previous {auth_session.location.country}"
+                    self.reportIncident("account", details, details=details, error_code=491)
+                elif auth_session.location.state != loc.state:
+                    details = f"user({self.username}) login from new state {loc.state} vs previous {auth_session.location.state}"
+                    self.reportIncident("account", details, details=details, error_code=491)
+            except Exception:
+                rh.log_exception(self.username)
 
     def sendSMS(self, msg):
         from telephony.models import SMS
         phone = self.phone_number
         if not phone or len(phone) < 7:
             return False
         SMS.send(phone, msg)
@@ -594,15 +642,19 @@
         if not self.is_active and not force:
             return False
         via = self.getProperty("notify_via", "all")
         phone = self.getProperty("phone")
         email = self.email
         valid_email = email is not None and "@" in email and "invalid" not in email
         allow_sms = not email_only and phone and (force or via in ["all", "sms"])
-        allow_email = valid_email and (force or via in ["all", "email"])
+        if not force:
+            allow_email = not self.email_disabled and valid_email and (force or via in ["all", "email"])
+        else:
+            allow_email = valid_email
+        
         if not allow_email and not allow_sms:
             return False
 
         if allow_email:
             ctx = {
                 'to': self.email,
                 'to_token': crypto.hashit(self.email),
@@ -664,20 +716,25 @@
     def canEditMe(self, user):
         return user.canEdit(self)
 
     def refreshSecurityToken(self):
         self.security_token = crypto.randomString(8)
         self.save()
 
+    def forceLogout(self):
+        self.refreshSecurityToken()
+        self.sendEvent("logged_out", "Your user session has been terminated.")
+
     def generateAuthCode(self, length=6, expires=AUTH_CODE_EXPIRES_SECS):
         for i in range(0, 100):
             code = crypto.randomCode(length)
             if Member.objects.filter(auth_code=code).count() == 0:
                 self.auth_code = code
                 self.auth_code_expires = datetime.now() + timedelta(seconds=expires)
+                self.auditLog(f"auth_code generated '{code}'", "auth_code", level=21)
                 self.save()
                 return self.auth_code
         return None
 
     # time based one time passwords / GOOGLE Authenticator
     def totp_getSecret(self, reset=False):
         token = self.getSecretProperty("totp_token", default=None)
@@ -717,25 +774,34 @@
         PersistentLog.log("account blocked, {}".format(reason), 5, request, "account.Member", self.pk, "blocked")
         RemoteEvents.hset("users:blocked:username", self.username, time.time())
         self.reportIncident(
             "account", f"account '{self.username}' blocked: {reason}", level=2,
             request=request,
             error_code=499,
             details=reason)
+        self.sendEmail(
+            subject=settings.EMAIL__ACCOUNT_LOCKED_SUBJECT,
+            body=settings.EMAIL__ACCOUNT_LOCKED_BODY,
+            template="email/plain/base.html")
 
     def unblock(self, request=None):
         if not request:
             request = self.getActiveRequest()
         if request and request.user.is_authenticated:
             who = request.user.username
         else:
             who = "time"
         PersistentLog.log("account unblocked by {}".format(who), 5, request, "account.Member", self.pk, "unblocked")
         RemoteEvents.hdel("users:blocked:username", self.username)
         RemoteEvents.hdel("users:failed:username", self.username)
+        if who != "time":
+            self.sendEmail(
+                subject=settings.EMAIL__ACCOUNT_UNLOCKED_SUBJECT,
+                body=settings.EMAIL__ACCOUNT_UNLOCKED_BODY,
+                template="email/plain/base.html")
 
     def getActiveConnections(self):
         c = RemoteEvents.hget("member:online:connections", self.id)
         if c:
             return int(c)
         return 0
 
@@ -814,14 +880,16 @@
         elif action == "auth_token":
             if not request.member.is_superuser and not self.canEditMe(request.member):
                 raise PermissionDeniedException("Permission Denied: attempting to generate auth_token")
             token = self.default_auth_token
             if token is None:
                 token = AuthToken(member=self, role="default")
             token.generateToken()
+        elif action == "refresh_keys" or action == "force_logout":
+            self.forceLogout()
 
     def set_full_name(self, value):
         self.set_name(value)
 
     def set_name(self, value):
         if not value:
             return
@@ -1009,46 +1077,62 @@
 
     @staticmethod
     def GetMemberByPhone(phone_number):
         phone_number = rh.normalizePhone(phone_number)
         return Member.objects.filter(phone_number=phone_number.lower()).last()
 
     @staticmethod
-    def GetWithPermission(perm, email_list=False):
+    def GetWithPermission(perm, email_list=False, ignore_disabled_email=True):
         if type(perm) is list:
             queries = [Q(properties__category="permissions", properties__key=p, properties__value="1") for p in perm]
             query = queries.pop()
             for item in queries:
                 query |= item
             qset = Member.objects.filter(is_active=True).filter(query).distinct()
         else:
             qset = Member.objects.filter(is_active=True).filter(properties__category="permissions", properties__key=perm, properties__value="1")
 
+        if not ignore_disabled_email:
+            qset = qset.exclude(
+                properties__category="permissions",
+                properties__key="email_disabled",
+                properties__int_value=1)
         if email_list:
             return list(qset.exclude(email__icontains="invalid").values_list('email', flat=True))
         return qset
 
     @staticmethod
-    def GetWithNotification(perm, email_list=False):
+    def GetWithNotification(perm, email_list=False, exclude_member=None, ignore_disabled_email=True):
+        qset = Member.objects.filter(is_active=True)
+        if exclude_member:
+            qset = qset.exclude(pk=exclude_member.pk)
         if isinstance(perm, list):
             perms = []
             for p in perm:
                 if p.startswith("notify."):
                     p = p.split(".")[1]
                 perms.append(p)
             queries = [Q(properties__category="notify", properties__key=p, properties__int_value=1) for p in perms]
             query = queries.pop()
             for item in queries:
                 query |= item
-            qset = Member.objects.filter(is_active=True).filter(query).distinct()
+            qset = qset.filter(query).distinct()
         else:
             if perm.startswith("notify."):
                 perm = perm.split(".")[1]
-            qset = Member.objects.filter(is_active=True).filter(properties__category="notify", properties__key=perm, properties__int_value=1)
-
+            qset = qset.filter(
+                properties__category="notify",
+                properties__key=perm,
+                properties__int_value=1)
+
+        if not ignore_disabled_email:
+            qset = qset.exclude(
+                properties__category="permissions",
+                properties__key="email_disabled",
+                properties__int_value=1)
         if email_list:
             return list(qset.exclude(email__icontains="invalid").values_list('email', flat=True))
         return qset
 
     @staticmethod
     def FilterOnline(is_online, qset):
         ids = list(RemoteEvents.smembers("member:online"))
@@ -1087,24 +1171,26 @@
         return qset
 
     @staticmethod
     def notifyWithPermission(perm, subject, message=None, template=None, context=None,
                              email_only=False, sms_msg=None, force=False, from_email=None):
         NotificationRecord = RestModel.getModel("account", "NotificationRecord")
         NotificationRecord.notify(
-            Member.GetWithPermission(perm), subject, message,
+            Member.GetWithPermission(perm, ignore_disabled_email=True), subject, message,
             template, context, email_only, sms_msg, force,
             from_email=from_email)
 
     @staticmethod
     def notifyWith(setting, subject, message=None, template=None, context=None,
-                   email_only=False, sms_msg=None, force=False, from_email=None):
+                   email_only=False, sms_msg=None, force=False, from_email=None,
+                   exclude_member=None):
         NotificationRecord = RestModel.getModel("account", "NotificationRecord")
         NotificationRecord.notify(
-            Member.GetWithNotification(setting), subject, message,
+            Member.GetWithNotification(setting, exclude_member=exclude_member, ignore_disabled_email=True),
+            subject, message,
             template, context, email_only, sms_msg, force,
             from_email=from_email)
 
     @classmethod
     def authWS4RedisConnection(cls, auth_data):
         """
         This method is used by the async/websocket service to authenticate.
@@ -1131,15 +1217,15 @@
     @classmethod
     def getMemberFromSession(cls, key):
         session = Session.objects.filter(session_key=key).last()
         if session is None:
             rh.log_print("no session for key", key)
             return None
         session_data = session.get_decoded()
-        rh.log_print(session_data)
+        # rh.log_print(session_data)
         uid = session_data.get('_auth_user_id', None)
         if uid is None:
             return None
         return cls.objects.filter(pk=uid).last()
 
 
 class MemberMetaData(MetaDataBase):
@@ -1183,25 +1269,26 @@
     created = models.DateTimeField(auto_now_add=True, editable=False)
     token = models.TextField(db_index=True, unique=True)
     member = models.ForeignKey(Member, related_name="auth_tokens", on_delete=models.CASCADE)
     role = models.CharField(max_length=128, null=True, default=None, blank=True)
     signature = models.CharField(max_length=128, null=True, default=None, blank=True, db_index=True)
 
     def generateToken(self, commit=True):
-        self.token = str(uuid.uuid1())
+        self.token = None
         self.updateSignature()
         if commit:
             self.save()
 
     def updateSignature(self):
+        if not self.token:
+            self.token = uuid.uuid4().hex
         self.signature = crypto.hashSHA256(self.token)
 
     def on_rest_pre_save(self, request, **kwargs):
         if not self.token:
-            self.token = uuid.uuid4().hex
             self.updateSignature()
         if not self.member_id:
             self.member = request.member
         if not request.member.canEdit(self.member):
             raise PermissionDeniedException("user is not allowed to create auth token for user", 469)
 
     @property
```

### Comparing `django_restit-4.2.9/account/models/notify.py` & `django_restit-4.2.90/account/models/notify.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,14 +126,16 @@
                 # TODO handle file inport
                 pass
             else:
                 self.attach(a.name, a.mimetype, a.data)
 
     @classmethod
     def canSend(cls):
+        if not settings.get("THROTTLE_EMAILS", False):
+            return True
         max_emails_per_minute = settings.get("MAX_EMAILS_PER_MINUTE", 30)
         last_email = NotificationRecord.objects.filter(state=1).last()
         now = datetime.now()
         if last_email and (now - last_email.created).total_seconds() < 30:
             # we sent an email less then a minute ago
             # now we can to count the number of message sent in last minute
             when = now - timedelta(seconds=60)
@@ -147,29 +149,109 @@
                          sms_msg=None, force=False,
                          from_email=settings.DEFAULT_FROM_EMAIL,
                          attachments=[]):
         # Member = RestModel.getModel("account", "Member")
         members = Member.objects.filter(email__in=emails)
         cls.notify(members, subject, message, template, context, email_only, sms_msg, force, from_email, attachments)
 
+
     @classmethod
     def notify(cls, notify_users, subject, message=None, 
                template=None, context=None, email_only=False,
                sms_msg=None, force=False,
                from_email=settings.DEFAULT_FROM_EMAIL,
                attachments=[]):
+        dup_list = []
+        email_to = []
+        sms_to = []
+        for member in notify_users:
+            via = member.getProperty("notify_via", "all")
+            phone = member.getProperty("phone")
+            email = member.email
+            valid_email = email is not None and "@" in email and "invalid" not in email
+            allow_sms = not email_only and phone and (force or via in ["all", "sms"])
+            allow_email = not member.email_disabled and valid_email and (force or via in ["all", "email"])
+            if not allow_email and not allow_sms:
+                continue
+            if allow_email and email not in dup_list:
+                dup_list.append(email)
+                email_to.append(member)
+            if not email_only and allow_sms and phone not in dup_list:
+                dup_list.append(phone)
+                sms_to.append(phone)
+
+        if len(dup_list) == 0:
+            return
+
+        if not message and not template and subject:
+            message = subject
+        if not sms_msg and subject:
+            sms_msg = subject
+        if not sms_msg and message:
+            sms_msg = message
+
+        if subject and len(subject) > 80:
+            epos = subject.find('. ') + 1
+            if epos > 10:
+                subject = subject[:epos]
+            if len(subject) > 80:
+                subject = subject[:80]
+                subject = subject[:subject.rfind(' ')] + "..."
+
+        if sms_to:
+            for phone in sms_to:
+                SMS.send(phone, sms_msg)
+
+        if not email_to:
+            return
+        for member in email_to:
+            cls._notifyViaEmail(member, subject, message, template, context, attachments, from_email)
+
+    @classmethod
+    def _notifyViaEmail(cls, member, subject, message, template, context, 
+                        attachments, from_email=settings.DEFAULT_FROM_EMAIL):
+        # lets verify the db is working
+        if template:
+            if context is None:
+                context = {}
+            if message is not None:
+                context["body"] = message
+            context["unsubscribe_token"] = member.getUUID()
+            message = inbox.utils.renderTemplate(template, context)
+        if from_email is None:
+            from_email = settings.DEFAULT_FROM_EMAIL
+
+        nr = NotificationMemberRecord(member=member, to_addr=member.email)
+        email_record = NotificationRecord(
+            method="email",
+            subject=subject,
+            from_addr=from_email,
+            body=message)
+        try:
+            email_record.save()
+            if attachments:
+                email_record.addAttachments(attachments)
+            email_record.send([nr])
+        except Exception as err:
+            rh.log_exception("email send failed", member.username, subject)
+
+    @classmethod
+    def notifyLegacy(cls, notify_users, subject, message=None, 
+               template=None, context=None, email_only=False,
+               sms_msg=None, force=False,
+               from_email=settings.DEFAULT_FROM_EMAIL,
+               attachments=[]):
         # this will create a record for each email address message is sent to
         from telephony.models import SMS
         email_to = []
         email_list = []
         sms_to = []
 
         if not message and not template and subject:
             message = subject
-
         if not sms_msg and subject:
             sms_msg = subject
         if not sms_msg and message:
             sms_msg = message
 
         if subject and len(subject) > 80:
             epos = subject.find('. ') + 1
@@ -193,15 +275,15 @@
         email_record = None
         for member in notify_users:
             via = member.getProperty("notify_via", "all")
             phone = member.getProperty("phone")
             email = member.email
             valid_email = email is not None and "@" in email and "invalid" not in email
             allow_sms = not email_only and phone and (force or via in ["all", "sms"])
-            allow_email = valid_email and (force or via in ["all", "email"])
+            allow_email = not member.email_disabled and valid_email and (force or via in ["all", "email"])
             if not allow_email and not allow_sms:
                 continue
             if allow_email and email not in email_list:
                 email_list.append(email)
                 nr = NotificationMemberRecord(member=member, to_addr=email)
                 email_to.append(nr)
             if not email_only and allow_sms and phone not in sms_to:
@@ -222,15 +304,15 @@
                 from_addr=from_email,
                 body=message)
             try:
                 email_record.save()
                 email_record.addAttachments(attachments)
                 email_record.send(email_to)
             except Exception as err:
-                print(("failed to create record: {}".format(str(err))))
+                rh.log_exception("email send failed", email_to)
                 # we need to send emails the old way
                 addrs = []
                 for to in email_to:
                     addrs.append(to.to_addr)
                 rest_mail.send(
                     addrs,
                     subject,
@@ -298,14 +380,15 @@
             if user:
                 user.log("bounced", "{} bounced to {} from {}".format(kind, address, source_ip), method=kind)
                 since = datetime.now() - timedelta(days=14)
                 bounce_count = BounceHistory.objects.filter(user=user, created__gte=since).count()
                 if bounce_count > 2:
                     # TODO notify support an account has been disabled because of bounce
                     user.setProperty("notify_via", "off")
+                    user.addPermission("email_disabled")
                     user.log("disabled", "notifications disabled because email bounced", method="notify")
         else:
             # TODO notify support of unknown bounce
             pass
         obj.user = user
         obj.save()
```

### Comparing `django_restit-4.2.9/account/models/session.py` & `django_restit-4.2.90/account/models/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,39 @@
 from rest.models import RestModel
 from rest import ua
 
 
 # replacing legacy cookie session system with more robust session info
 class AuthSession(models.Model, RestModel):
     class RestMeta:
-        SEARCH_FIELDS = ["ip", "member__username", "browser", "location__city"]
-        VIEW_PERMS = ["view_members", "manage_members", "manage_users"]
+        SEARCH_FIELDS = ["ip", "member__username", "browser", "location__city", "buid"]
+        VIEW_PERMS = ["view_members", "manage_members", "manage_users", "owner"]
         CAN_SAVE = False
         CAN_DELETE = False
+        VIEW_PERMS_MEMBER_FIELD = "member"
         # note the | will check collection parameter...
         #   trailing "." will check if the collection has the key set to true
         SEARCH_TERMS = [
             "ip", "device", "browser", "os",
             ("username", "member__username"),
             ("email", "member__email"),
             ("first_name", "member__first_name"),
             ("last_name", "member__last_name"),
             "last_activity#datetime"]
         GRAPHS = {
             "default": {
                 "graphs": {
                     "location": "default"
                 }
+            },
+            "location": {
+                "graphs": {
+                    "location": "default",
+                    "member": "basic"
+                }
             }
         }
     # the signature of session
     created = models.DateTimeField(auto_now_add=True, editable=False, db_index=True)
     last_activity = models.DateTimeField(db_index=True)
 
     signature = models.CharField(max_length=127, db_index=True)
```

### Comparing `django_restit-4.2.9/account/models/settings.py` & `django_restit-4.2.90/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/oauth/google.py` & `django_restit-4.2.90/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/periodic.py` & `django_restit-4.2.90/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/rpc/auth.py` & `django_restit-4.2.90/account/rpc/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,25 @@
 from rest import helpers
 from rest import settings
 from account import models as am
 from medialib.qrcode import generateQRCode
 from django.http import HttpResponse
 from datetime import datetime, timedelta
 
+ALLOW_BASIC_LOGIN = settings.get("ALLOW_BASIC_LOGIN", False)
+FORGET_ALWAYS_TRUE = settings.get("FORGET_ALWAYS_TRUE", True)
+JWT_UPDATE_REFRESH_TOKEN = settings.get("JWT_UPDATE_REFRESH_TOKEN", False)
+
 
 @rd.urlPOST(r'^login$')
 @rd.urlPOST(r'^login/$')
 @rd.never_cache
 def member_login(request):
+    if not ALLOW_BASIC_LOGIN:
+        return jwt_login(request)
     username = request.DATA.get('username', None)
     auth_code = request.DATA.get(["auth_code", "code", "invite_token"], None)
     if username and auth_code:
         return member_login_uname_code(request, username, auth_code)
     password = request.DATA.get('password', None)
     if username and password:
         return member_login_uname_pword(request, username, password)
@@ -33,28 +39,31 @@
     # poor mans JWT, carried over
     username = request.DATA.get('username', None)
     if not username:
         return rv.restPermissionDenied(request, "Password and/or Username is incorrect", error_code=422)
     member = getMemberByUsername(username)
     if not member:
         return rv.restPermissionDenied(request, error=f"Password and/or Username is incorrect for {username}", error_code=422)
+    auth_code = request.DATA.get(["auth_code", "code", "invite_token"], None)
+    if username and auth_code:
+        return member_login_uname_code(request, username, auth_code)
     password = request.DATA.get('password', None)
     member.canLogin(request)  # throws exception if cannot login
-    if member.requires_totp:
+    if member.requires_totp or member.has_totp:
         resp = checkForTOTP(request, member)
         if resp is not None:
             return resp
     if not member.login(request=request, password=password, use_jwt=True):
         # we do not want permission denied catcher invoked as it is already handled in login method
         return rv.restStatus(request, False, error=f"Invalid Credentials {username}", error_code=401)
     return on_complete_jwt(request, member)
 
 
 def on_complete_jwt(request, member):
-    if member.security_token is None or member.security_token == JWT_KEY:
+    if member.security_token is None or member.security_token == JWT_KEY or member.force_single_session:
         member.refreshSecurityToken()
 
     member.log(
         "jwt_login", "jwt login succesful", 
         request, method="login", level=7)
 
     device_id = request.DATA.get(["device_id", "deviceID"])
@@ -110,15 +119,17 @@
         request.member = member
         return rv.restPermissionDenied(request, error="invalid token", error_code=-702)
     if member.security_token is None:
         member.refreshSecurityToken()
     member.canLogin(request)
     token.refresh()
     request.jwt_token = token.access_token  # this tells the middleware to store in cookie
-    return rv.restGet(request, dict(access=token.access_token, refresh=token.refresh_token))
+    if JWT_UPDATE_REFRESH_TOKEN:
+        rtoken = token.refresh_token
+    return rv.restGet(request, dict(access=token.access_token, refresh=rtoken))
 
 
 def getMemberByUsername(username):
     member = None
     username = username.lower()
     if username.count('@') == 1:
         member = am.Member.objects.filter(email=username).last()
@@ -154,15 +165,15 @@
 
 
 def member_login_uname_pword(request, username, password):
     member = getMemberByUsername(username)
     if not member:
         return rv.restPermissionDenied(request, error=f"Password or Username is not correct for {username}", error_code=422)
     member.canLogin(request)  # throws exception if cannot login
-    if member.requires_topt:
+    if member.requires_totp or member.has_totp:
         resp = checkForTOTP(request, member)
         if resp is not None:
             return resp
     if not member.login(request=request, password=password, use_jwt=False):
         request.member = member
         member.log("login_failed", "incorrect password", request, method="login", level=31)
         return rv.restPermissionDenied(request, error="Password or Username is incorrect", error_code=401)
@@ -191,25 +202,24 @@
         request.member = member
         member.log("login_blocked", "accessing used or expired token link", request, method="login", level=31)
         return rv.restPermissionDenied(request, f"token already used or expired for {username}", error_code=492)
     if member.auth_code_expires < datetime.now():
         request.member = member
         member.log("login_blocked", "accessing expired token link", request, method="login", level=31)
         return rv.restPermissionDenied(request, "token expired", error_code=493)
-    password = request.DATA.get(['password', 'new_password'], None)
+    password = request.DATA.get('new_password', None)
     if password:
         member.setPassword(password)
     member.auth_code = None
     member.auth_code_expires = None
     member.login(request=request)
     member.save()
     member.log("code_login", "code login", request, method="login", level=8)
     if request.DATA.get("auth_method") == "basic":
         return rv.restGet(request, dict(id=member.pk, session_key=request.session.session_key))
-
     return on_complete_jwt(request, member)
 
 
 @rd.url(r'^logout$')
 @rd.url(r'^logout/$')
 @rd.never_cache
 def member_logout(request):
@@ -237,16 +247,30 @@
     | Check if the current user is logged in
     """
     if request.user:
         return rv.restStatus(request, request.user.is_authenticated)
     return rv.restStatus(request, False)
 
 
+@rd.urlPOST('invite/validate')
+@rd.requires_params(["username"])
+def member_invite_confirm(request):
+    username = request.DATA.get('username', None)
+    auth_code = request.DATA.get(["auth_token", "invite_token"], None)
+    member = getMemberByUsername(username)
+    if not member or not auth_code:
+        return rv.restPermissionDenied(request, error=f"Username or code is incorrect {username}/{auth_code}", error_code=422)
+    auth_code = auth_code.replace('-', '').replace(' ', '')
+    if member.auth_code is None or member.auth_code != auth_code:
+        return rv.restStatus(request, False)
+    return rv.restStatus(request, True)
+
+
 @rd.urlPOST('mfa/request_code')
-@rd.never_cache
+@rd.requires_params(["username"])
 def member_request_code(request):
     member, resp = get_member_from_request(request)
     if resp is not None:
         return resp
     return member_forgot_password_code(request, member)
 
 
@@ -277,22 +301,28 @@
 
     | Return: status + error
 
     | Send fgroupet password reset instructions
     """
     member, resp = get_member_from_request(request)
     if member is None:
+        if FORGET_ALWAYS_TRUE:
+            return rv.restStatus(request, True, msg="Password reset instructions have been sent to your email. (If valid account)")
         return resp
     if resp is not None and not member.is_active:
+        if FORGET_ALWAYS_TRUE:
+            return rv.restStatus(request, True, msg="Password reset instructions have been sent to your email. (If valid account)")
         return resp
 
     if request.DATA.get("use_code", False):
         return member_forgot_password_code(request, member)
 
     if member.auth_code is not None and member.auth_code_expires > datetime.now():
+        if FORGET_ALWAYS_TRUE:
+            return rv.restStatus(request, True, msg="Password reset instructions have been sent to your email. (If valid account)")
         return rv.restPermissionDenied(request, "already sent valid auth code")
 
     member.auth_code = crypto.randomString(16)
     member.auth_code_expires = datetime.now() + timedelta(minutes=10)
     member.save()
     member.log("forgot", "user requested password reset", request, method="password_reset", level=17)
 
@@ -301,15 +331,15 @@
         'user': member,
         'uuid': member.uuid,
         'token': token,
         'subject': 'password reset',
         'to': [member.email],
     })
 
-    return rv.restStatus(request, True, msg="Password reset instructions have been sent to your email.")
+    return rv.restStatus(request, True, msg="Password reset instructions have been sent to your email. (If valid account)")
 
 
 def member_forgot_password_code(request, member):
     member.generateAuthCode(6)
     code = "{} {}".format(member.auth_code[:3], member.auth_code[3:])
 
     context = helpers.getContext(
```

### Comparing `django_restit-4.2.9/account/rpc/device.py` & `django_restit-4.2.90/account/rpc/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from rest import decorators as rd
 from rest import views as rv
 from rest import helpers as rh
 from account import models as am
 from objict import objict
 
 
+@rd.url(r'^group/cloud/credentials$')
+@rd.url(r'^group/cloud/credentials/(?P<pk>\d+)$')
+@rd.login_required
+def rest_on_group_cloud_creds(request, pk=None):
+    return am.CloudCredentials.on_rest_request(request, pk)
+
+
 @rd.url(r'^member/device$')
 @rd.url(r'^member/device/(?P<pk>\d+)$')
 @rd.login_required
 def rest_on_member_device(request, pk=None):
     return am.MemberDevice.on_rest_request(request, pk)
```

### Comparing `django_restit-4.2.9/account/rpc/group.py` & `django_restit-4.2.90/account/rpc/group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rest import decorators as rd
 from rest import views as rv
+from rest import helpers as rh
 from account.models import Group, Membership, Member, GroupFeed, MemberFeed
-from taskqueue import models as tq
 
 
 @rd.url(r'^group$')
 @rd.url(r'^group/$')  # required for legacy support
 @rd.url(r'^group/(?P<pk>\d+)$')
 @rd.login_required
 def rest_on_group(request, pk=None):
@@ -55,14 +55,21 @@
             member = Member.createFromDict(request, data)
         member.auditLog(f"created by {request.member.username}", "created", level=21)
     
     ms = Membership.objects.filter(member=member, group=group).first()
     if ms is None:
         member.auditLog(f"added to {group.name}:{group.id} by {request.member.username}", "group_invite", level=21)
         ms = group.invite(member, request.DATA.get("role", "guest"))
+    elif not ms.is_enabled:
+        # re-enable the member if they are being re-invited after being disabled
+        if not ms.member.is_active:
+            # we need to make sure we only enable the user for this group
+            ms.member.enable(request.member, memberships=[], notify=False)
+        ms.set_state(0)
+        ms.save()
     ms.auditLog(f"invite sent by {request.member.username}", "invite", level=21)
     ms.sendInvite(request)
     return ms.restGet(request)
 
 
 @rd.url(r'^membership$')
 @rd.url(r'^membership/(?P<pk>\d+)$')
@@ -74,22 +81,49 @@
 @rd.url(r'^membership/group/(?P<group_id>\d+)$')
 @rd.url(r'^membership/me-(?P<group_id>\d+)$')
 @rd.login_required
 def rest_on_users_membership(request, group_id=None):
     ms = request.member.getMembershipFor(group_id, include_parents=True)
     if ms is None:
         return rv.restStatus(request, False, error="not found", error_code=404)
+    if not ms.is_enabled:
+        return rv.restPermissionDenied(
+            request,
+            error=f"membership({request.member.username}) has been disabled for this group({group_id})",
+            error_code=410)
     return ms.restGet(request)
 
 
-@rd.urlGET('group/feed')
-@rd.urlGET('group/feed/<int:pk>')
+@rd.url('group/feed')
+@rd.url('group/feed/<int:pk>')
 @rd.login_required
 def rest_on_group_feed(request, pk=None):
     return GroupFeed.on_rest_request(request, pk)
 
 
 @rd.urlGET('member/feed')
 @rd.urlGET('member/feed/<int:pk>')
 @rd.login_required
 def rest_on_member_feed(request, pk=None):
     return MemberFeed.on_rest_request(request, pk)
+
+
+@rd.urlGET('group/stats/kinds')
+@rd.login_required
+def rest_on_group_stats(request):
+    params = request.DATA.asDict()
+    if not params.group:
+        if not request.member.hasPerm(["view_all_groups", "manage_groups"]):
+            return rv.restPermissionDenied()
+        out = rh.countOccurences(Group.objects.filter(is_active=True), "kind")
+        return rv.restResult(request, dict(data=out))
+    # local
+    group = Group.objects.filter(pk=params.group).first()
+    if not group:
+        return rv.restPermissionDenied(request)
+    if not request.member.hasPerm(["view_all_groups", "manage_groups"]):
+        if not request.member.hasGroupPerm(group, ["reports", "reporting"]):
+            return rv.restPermissionDenied(request)
+    qset = group.getAllChildren(True, True, True).filter(is_active=True)
+    out = rh.countOccurences(qset, "kind")
+    return rv.restResult(request, dict(data=out))
+
```

### Comparing `django_restit-4.2.9/account/rpc/member.py` & `django_restit-4.2.90/account/rpc/member.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from rest import decorators as rd
-from rest.views import restPermissionDenied, restStatus
+from rest.views import restPermissionDenied, restStatus, restHTML
+from rest import helpers as rh
 from account import models as am
 
 
 @rd.url(r'^member$')
 @rd.url(r'^member/$')
 @rd.url(r'^member/(?P<pk>\d+)$')
 @rd.login_required
@@ -14,14 +15,16 @@
 @rd.url(r'^member/me$')
 @rd.login_optional
 def member_me_action(request):
     if not request.user.is_authenticated:
         return restPermissionDenied(request, "not authenticated")
     if request.method == "GET":
         # request.session['ws4redis:memberof'] = request.member.getGroupUUIDs()
+        # from rest import helpers as rh
+        # rh.debug("user_platform", request.DATA.getUserAgentPlatform())
         return request.member.on_rest_get(request)
     elif request.method == "POST":
         return request.member.on_rest_post(request)
     return restStatus(request, False, error="not supported")
 
 
 @rd.url(r'^authtoken$')
@@ -33,7 +36,20 @@
 
 @rd.url(r'^session$')
 @rd.url(r'^session/(?P<pk>\d+)$')
 @rd.login_required
 def rest_on_session(request, pk=None):
     return am.AuthSession.on_rest_request(request, pk)
 
+
+@rd.urlGET('unsubscribe')
+@rd.requires_params(["t"])
+def rest_on_member(request):
+    t = request.DATA.get("t")
+    m = am.Member.objects.filter(uuid=t).last()
+    if m is not None:
+        m.addPermission("email_disabled")
+        m.reportIncident("email", f"{m.email} has unsubscribed to all email")
+    context = rh.getContext(request, member=m)
+    if request.DATA.get("format") == "json":
+        return restStatus(request, True)
+    return restHTML(request, template="unsubscribed.html", context=context)
```

### Comparing `django_restit-4.2.9/account/rpc/notify.py` & `django_restit-4.2.90/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/account/rpc/oauth.py` & `django_restit-4.2.90/account/rpc/oauth.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,8 +66,16 @@
 
     member.auth_code = crypto.randomString(16)
     member.auth_code_expires = datetime.now() + timedelta(minutes=5)
     member.save()
     member.auditLog("user succesfully authenticated with google", "google_oauth", level=17)
 
     params = urlencode({'oauth_code': member.auth_code, "username":member.username})
-    return redirect(f"{app_url}?{params}")
+    rurl = None
+    if "?" in app_url:
+        if app_url[-1] == "?":
+            rurl = f"{app_url}{params}"
+        else:
+            rurl = f"{app_url}&{params}"
+    else:
+        rurl = f"{app_url}?{params}"
+    return redirect(rurl)
```

### Comparing `django_restit-4.2.9/account/templates/email/base.html` & `django_restit-4.2.90/account/templates/email/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -277,15 +277,15 @@
                                 <div class="footer">
                                     {% block footer %}
                                     Sent Via 
                                     <div class="links">
                                         <a href="{{settings.BASE_URL}}">{{settings.SITE_LABEL}}</a>
                                     </div>
                                     {% endblock %}
-                                    <p style="text-align: center; font-size: 10px;">Don't want to get notifications? <a href="{{settings.BASE_URL}}rpc/account/member/unsubscribe?email={{to}}&token={{to_token}}">Unsubscribe</a>
+                                    <p style="text-align: center; font-size: 10px;">Don't want to get notifications? <a href="{{UNSUBSCRIBE_URL}}?t={{unsubscribe_token}}">Unsubscribe</a>
                                     </p>
                                     <div>
                                 
                                     </div>
                                 </div>
                             </td>
                         </tr>
```

### Comparing `django_restit-4.2.9/account/templates/email/invite.html` & `django_restit-4.2.90/account/templates/email/reset_code.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load humanize %}
 <!doctype html>
 <html>
   <head>
     <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
     <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
-    <title>INVITE EMAIL</title>
+    <title>RESET PASSWORD</title>
     <style>
       /* -------------------------------------
           GLOBAL RESETS
       ------------------------------------- */
       
       /*All the styling goes here*/
       
@@ -348,55 +348,40 @@
 
               <!-- START MAIN CONTENT AREA -->
               <tr>
                 <td class="wrapper">
                   <table role="presentation" border="0" cellpadding="0" cellspacing="0">
                     <tr>
                       <td>
-                        <h3 style="color: white;">
-                          You have been granted access to "{{group.name}}"!
-                        </h3>
+                      	<h3 style="color: white;">Your one-time code:</h3 style="color: white;">
+                      	<h1 style="color: #FCC431;padding:4px 20px; font-weight: bold; text-align: left;">{{code}}</h1>
                         {% if msg %}
                         <h5 style="color: white;">{{msg}}</h5>
-                        <p>&nbsp;</p>
+                        {% else %}
+                        <h5 style="color: white;">If you did not request this code, please contact customer support.</h5>
                         {% endif %}
+                        <p>&nbsp;</p>
 
                         <div style="text-align: center;">
                           <img src="{{SITE_LOGO}}" height=40>
                         </div>
-
-                        <p>&nbsp;</p>
-                        <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
-                          <tbody>
-                            <tr>
-                              <td>
-                                <a style="display: block; text-align: center;" href="{{url}}" target="_blank">{{btn_label}}</a>
-                              </td>
-                            </tr>
-                          </tbody>
-                        </table>
                       </td>
                     </tr>
                   </table>
                 </td>
               </tr>
 
             <!-- END MAIN CONTENT AREA -->
             </table>
             <!-- END CENTERED WHITE CONTAINER -->
 
             <!-- START FOOTER -->
             <div class="footer">
               <table role="presentation" border="0" cellpadding="0" cellspacing="0">
                 <tr>
-                  <td class="content-block">
-                    <br> Don't like these emails? <a href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                  </td>
-                </tr>
-                <tr>
                   <td class="content-block powered-by">
                     <div>Powered by {{SITE_LABEL}}</div>
                     <div>{{SERVER_NAME}}</div>
                   </td>
                 </tr>
               </table>
             </div>
@@ -404,8 +389,10 @@
 
           </div>
         </td>
         <td>&nbsp;</td>
       </tr>
     </table>
   </body>
-</html>
+</html>
+
+
```

#### html2text {}

 * *error from `html2text {}` (b):*

 * *File "/tmp/diffoscope_bg_ta322_/tmpxy124ltd_TarContainer/0/58.html", line 356, column 118: Levels of opening and closing headings don't match*

```diff
@@ -1,14 +1,12 @@
 {% load humanize %}
 {{reason}}
-  ******** YYoouu hhaavvee bbeeeenn ggrraanntteedd aacccceessss ttoo ""{{{{ggrroouupp..nnaammee}}}}""!! ********
+  ******** YYoouurr oonnee--ttiimmee ccooddee::ttyyllee==""ccoolloorr:: wwhhiittee;;"">>{{{{ccooddee}}}} ********
   {% if msg %}
   **** {{{{mmssgg}}}} ****
-   
+  {% else %}
+  **** IIff yyoouu ddiidd nnoott rreeqquueesstt tthhiiss ccooddee,, pplleeaassee ccoonnttaacctt ccuussttoommeerr ssuuppppoorrtt.. ****  
   {% endif %}
-  [{{SITE_LOGO}}]                                              
    
-  _{_{_b_t_n___l_a_b_e_l_}_}
-
-  Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
+  [{{SITE_LOGO}}]
   Powered by {{SITE_LABEL}}
   {{SERVER_NAME}}
```

### Comparing `django_restit-4.2.9/account/templates/email/plain/base.html` & `django_restit-4.2.90/account/templates/email/plain/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
                     </td>
                   </tr>
                   {% endif %}
                   <tr>
                     <td align="center" style="font-size:0px;padding:8px 0;word-break:break-word;">
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:30px;font-weight:300;line-height:30px;text-align:center;color:#000000;">
-                      {{settings.COMPANY_NAME}}</div>
+                      {{COMPANY_NAME}}</div>
 
                     </td>
                   </tr>
                   <tr>
                     <td style="font-size:0px;padding:10px 25px;word-break:break-word;">
                       <p style="border-top:dashed 1px lightgrey;font-size:1px;margin:0px auto;width:100%;">
                       </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% block preview %}{{preview}}{% endblock %}
                                         
                         {% if SITE_LOGO %} [{{SITE_LOGO}}]{% endif %}
-                                       {{settings.COMPANY_NAME}}
+                                              {{COMPANY_NAME}}
 {% block body %} {% autoescape off %}{{ body }}{% endautoescape %} {% endblock
 %}
                            Powered by {{SITE_LABEL}}
                        © 2023 {{settings.COMPANY_LABEL}}
                     Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
                                       ->
```

### Comparing `django_restit-4.2.9/account/templates/email/plain/invite.html` & `django_restit-4.2.90/account/templates/email/plain/invite.html`

 * *Files 2% similar despite different names*

```diff
@@ -291,21 +291,14 @@
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   {% endif %}
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
-                      <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                      </div>
-                    </td>
-                  </tr>
-                  <tr>
-                    <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
          align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600"
       >
         <tr>
           <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
       <![endif]-->
```

#### html2text {}

```diff
@@ -5,12 +5,11 @@
 You have been invited to join "_{_{_g_r_o_u_p_._n_a_m_e_}_}" on the {{COMPANY_NAME}} portal.
 {{msg}}
  
 Please click the button below to _a_c_c_e_p_t_ _t_h_e_ _i_n_v_i_t_a_t_i_o_n.
                                                 _{_{_b_t_n___l_a_b_e_l_}_}
 If you have any questions simply reply to this email and we would be more than
 happy to reply. :)
-                           Powered by {{SITE_LABEL}}
-                       © 2023 {{settings.COMPANY_LABEL}}
-                    Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
-                                      ->
-                                                
+                            Powered by {{SITE_LABEL}}
+                        © 2023 {{settings.COMPANY_LABEL}}
+                                        ->
+
```

### Comparing `django_restit-4.2.9/account/templates/email/plain/reset_code.html` & `django_restit-4.2.90/account/templates/email/plain/reset_code.html`

 * *Files 1% similar despite different names*

```diff
@@ -280,21 +280,14 @@
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
                         <!-- <a href="#" style="color:#000000">Privacy Policy</a> | <a href="#" style="color:#000000">Contact Support</a> | <a href="#" style="color:#000000">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
-                      <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                      </div>
-                    </td>
-                  </tr>
-                  <tr>
-                    <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
          align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600"
       >
         <tr>
           <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
       <![endif]-->
```

#### html2text {}

```diff
@@ -5,12 +5,11 @@
 You have requested to reset your password on the {{settings.COMPANY_NAME}}
 portal.
 Your one-time reset code:
 {{code}}
  
 If you have any questions simply reply to this email and we would be more than
 happy to reply. :)
-                           Powered by {{SITE_LABEL}}
-                       © 2023 {{settings.COMPANY_LABEL}}
-                    Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
-                                      ->
-                                                
+                            Powered by {{SITE_LABEL}}
+                        © 2023 {{settings.COMPANY_LABEL}}
+                                        ->
+
```

### Comparing `django_restit-4.2.9/account/templates/email/reset_code.html` & `django_restit-4.2.90/account/templates/email/invite.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load humanize %}
 <!doctype html>
 <html>
   <head>
     <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
     <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
-    <title>RESET PASSWORD</title>
+    <title>INVITE EMAIL</title>
     <style>
       /* -------------------------------------
           GLOBAL RESETS
       ------------------------------------- */
       
       /*All the styling goes here*/
       
@@ -348,45 +348,50 @@
 
               <!-- START MAIN CONTENT AREA -->
               <tr>
                 <td class="wrapper">
                   <table role="presentation" border="0" cellpadding="0" cellspacing="0">
                     <tr>
                       <td>
-                      	<h3 style="color: white;">Your one-time code:</h3 style="color: white;">
-                      	<h1 style="color: #FCC431;padding:4px 20px; font-weight: bold; text-align: left;">{{code}}</h1>
+                        <h3 style="color: white;">
+                          You have been granted access to "{{group.name}}"!
+                        </h3>
                         {% if msg %}
                         <h5 style="color: white;">{{msg}}</h5>
-                        {% else %}
-                        <h5 style="color: white;">If you did not request this code, please contact customer support.</h5>
-                        {% endif %}
                         <p>&nbsp;</p>
+                        {% endif %}
 
                         <div style="text-align: center;">
                           <img src="{{SITE_LOGO}}" height=40>
                         </div>
+
+                        <p>&nbsp;</p>
+                        <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
+                          <tbody>
+                            <tr>
+                              <td>
+                                <a style="display: block; text-align: center;" href="{{url}}" target="_blank">{{btn_label}}</a>
+                              </td>
+                            </tr>
+                          </tbody>
+                        </table>
                       </td>
                     </tr>
                   </table>
                 </td>
               </tr>
 
             <!-- END MAIN CONTENT AREA -->
             </table>
             <!-- END CENTERED WHITE CONTAINER -->
 
             <!-- START FOOTER -->
             <div class="footer">
               <table role="presentation" border="0" cellpadding="0" cellspacing="0">
                 <tr>
-                  <td class="content-block">
-                    <br> Don't like these emails? <a href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                  </td>
-                </tr>
-                <tr>
                   <td class="content-block powered-by">
                     <div>Powered by {{SITE_LABEL}}</div>
                     <div>{{SERVER_NAME}}</div>
                   </td>
                 </tr>
               </table>
             </div>
@@ -394,10 +399,8 @@
 
           </div>
         </td>
         <td>&nbsp;</td>
       </tr>
     </table>
   </body>
-</html>
-
-
+</html>
```

#### html2text {}

 * *error from `html2text {}` (a):*

 * *File "/tmp/diffoscope_bg_ta322_/tmpsw1sorp4_TarContainer/0/49.html", line 356, column 118: Levels of opening and closing headings don't match*

```diff
@@ -1,14 +1,12 @@
 {% load humanize %}
 {{reason}}
-  ******** YYoouurr oonnee--ttiimmee ccooddee::ttyyllee==""ccoolloorr:: wwhhiittee;;"">>{{{{ccooddee}}}} ********
+  ******** YYoouu hhaavvee bbeeeenn ggrraanntteedd aacccceessss ttoo ""{{{{ggrroouupp..nnaammee}}}}""!! ********
   {% if msg %}
   **** {{{{mmssgg}}}} ****
-  {% else %}
-  **** IIff yyoouu ddiidd nnoott rreeqquueesstt tthhiiss ccooddee,, pplleeaassee ccoonnttaacctt ccuussttoommeerr ssuuppppoorrtt.. ****
-  {% endif %}                                                               
    
+  {% endif %}                                                  
   [{{SITE_LOGO}}]
-
-  Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
+   
+  _{_{_b_t_n___l_a_b_e_l_}_}
   Powered by {{SITE_LABEL}}
   {{SERVER_NAME}}
```

### Comparing `django_restit-4.2.9/account/templates/email/simple/invite.html` & `django_restit-4.2.90/account/templates/email/simple/invite.html`

 * *Files 2% similar despite different names*

```diff
@@ -289,21 +289,14 @@
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#fafafa;">
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
-                      <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#fafafa;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                      </div>
-                    </td>
-                  </tr>
-                  <tr>
-                    <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
          align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600"
       >
         <tr>
           <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
       <![endif]-->
```

#### html2text {}

```diff
@@ -5,12 +5,11 @@
 You have been invited to join "_{_{_g_r_o_u_p_._n_a_m_e_}_}" on the {{COMPANY_NAME}} portal.
 {{msg}}
  
 Please click the button below to _a_c_c_e_p_t_ _t_h_e_ _i_n_v_i_t_a_t_i_o_n.
                                                 _{_{_b_t_n___l_a_b_e_l_}_}
 If you have any questions simply reply to this email and we would be more than
 happy to reply. :)
-                           Powered by {{SITE_LABEL}}
-                       © 2023 {{settings.COMPANY_LABEL}}
-                    Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
-                                      ->
-                                                
+                            Powered by {{SITE_LABEL}}
+                        © 2023 {{settings.COMPANY_LABEL}}
+                                        ->
+
```

### Comparing `django_restit-4.2.9/account/templates/email/simple/reset_code.html` & `django_restit-4.2.90/account/templates/email/simple/reset_code.html`

 * *Files 2% similar despite different names*

```diff
@@ -280,21 +280,14 @@
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#fafafa;">
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
-                      <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#fafafa;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
-                      </div>
-                    </td>
-                  </tr>
-                  <tr>
-                    <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
          align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600"
       >
         <tr>
           <td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;">
       <![endif]-->
```

#### html2text {}

```diff
@@ -5,12 +5,11 @@
 You have requested to reset your password on the {{settings.COMPANY_NAME}}
 portal.
 Your one-time reset code:
 {{code}}
  
 If you have any questions simply reply to this email and we would be more than
 happy to reply. :)
-                           Powered by {{SITE_LABEL}}
-                       © 2023 {{settings.COMPANY_LABEL}}
-                    Don't like these emails? _U_n_s_u_b_s_c_r_i_b_e.
-                                      ->
-                                                
+                            Powered by {{SITE_LABEL}}
+                        © 2023 {{settings.COMPANY_LABEL}}
+                                        ->
+
```

### Comparing `django_restit-4.2.9/auditlog/README` & `django_restit-4.2.90/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/auditlog/admin.py` & `django_restit-4.2.90/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/auditlog/decorators.py` & `django_restit-4.2.90/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/auditlog/middleware.py` & `django_restit-4.2.90/auditlog/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from rest import settings
-from .models import PersistentLog
 
 DEBUG_REST_ALL = settings.get("DEBUG_REST_ALL", False)
 DEBUG_REST_END_POINTS = settings.get("DEBUG_REST_END_POINTS", [])
 IGNORE_REST_END_POINTS = settings.get("IGNORE_REST_END_POINTS", [])
 LOG_REST_PREFIX = settings.get("REST_PREFIX", "api/")
 if not LOG_REST_PREFIX.startswith("/"):
     LOG_REST_PREFIX = f"/{LOG_REST_PREFIX}"
 
 
 def checkRestDebug(request):
+    if checkRestIgnore(request):
+        return False
     if DEBUG_REST_ALL:
         return True
     for ep in DEBUG_REST_END_POINTS:
         if request.path.startswith(ep):
-            return not checkRestIgnore(request)
+            return True
     return False
 
 
 def checkRestIgnore(request):
     for ep in IGNORE_REST_END_POINTS:
         if isinstance(ep, tuple):
-            method, ep = ep
-            return request.method == method and request.path.startswith(ep)
+            method, epath = ep
+            if request.method == method and request.path.startswith(epath):
+                return True
         if request.path.startswith(ep):
             return True
     return False
 
 
 class LogRequest(object):
     last_request = None
@@ -42,8 +44,7 @@
         request.rest_debug = False
         if request.path.startswith(LOG_REST_PREFIX) or request.path.startswith("/rpc/"):
             request.rest_debug = checkRestDebug(request)
             if request.rest_debug:
                 request.DATA.log()
         response = self.get_response(request)
         return response
-
```

### Comparing `django_restit-4.2.9/auditlog/migrations/0001_initial.py` & `django_restit-4.2.90/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/auditlog/models.py` & `django_restit-4.2.90/auditlog/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from django.conf import settings
 
 import copy
 
 from rest.models import RestModel
 from rest import helpers
 from rest.log import getLogger
+from auditlog import cloudwatch
 
 import traceback
 
 AUDIT_LOGGER = getLogger("auditlog", filename="auditlog.log")
 AUDITLOG_LOGGER_BY_USER = getattr(settings, "AUDITLOG_LOGGER_BY_USER", False)
 AUDITLOG_LOGGERS = getattr(settings, "AUDITLOG_LOGGERS", {})
 
@@ -277,23 +278,27 @@
                 sobj[key] = sobj[key][:MAX_AUDIT_LINE_LENGTH] + '...<truncated linelen>'
             if isinstance(sobj[key], dict):
                 sobj[key] = PersistentLog.sanatize(sobj[key])
         return sobj
 
     @staticmethod
     def log(message, level=0, request=None, component=None,
-            pkey=None, action=None, group=None, path=None, method=None, tid=None, no_truncate=False):
+            pkey=None, action=None, group=None, path=None,
+            method=None, tid=None, no_truncate=False,
+            aws_log_group=None, aws_log_stream=None):
         plog = PersistentLog.createLogFromRequest(
             request, component=component, tid=tid, pkey=pkey, action=action, group=group,
             path=path, method=method, level=level)
 
         plog.setMessage(message, truncate=not no_truncate)
 
         try:
             plog.save()
+            if aws_log_group and aws_log_stream:
+                cloudwatch.log(plog.toDict(), aws_log_group, aws_log_stream)
         except Exception:
             helpers.log_exception(plog.message)
 
         if PERSISTENT_LOG_PRINT:
             plog.printToLog()
         return plog
```

### Comparing `django_restit-4.2.9/auditlog/rpc.py` & `django_restit-4.2.90/account/passkeys/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,123 @@
-from . import models as auditlog
+import json
+from base64 import urlsafe_b64encode
 
-from rest import views as rv
-from rest import decorators as rd
+try:
+    from fido2 import webauthn
+    import fido2
+    from fido2.server import Fido2Server
+    from fido2.utils import websafe_decode, websafe_encode
+    from fido2 import cbor
+    fido2.features.webauthn_json_mapping.enabled = True
+except Exception:
+    pass
 
+from rest import settings
+from rest import helpers as rh
+from account.models import UserPassKey
 
-@rd.url(r'^plog$')
-@rd.url(r'^plog/(?P<plog_id>\d+)$')
-@rd.perm_required('view_logs')
-def plog_handler(request, plog_id=None):
-    if not plog_id:
-        min_pk = getattr(auditlog.settings, "PLOG_STALE_ID", 0)
-        return auditlog.PersistentLog.on_rest_list(request, qset=auditlog.PersistentLog.objects.filter(pk__gte=min_pk))
-    return auditlog.PersistentLog.on_rest_request(request, plog_id)
-
-
-@rd.urlGET(r'^plog_old$')
-@rd.perm_required('view_logs')
-def plogList(request):
-    auditlog.PersistentLog.on_request_handle()
-
-    graph = request.DATA.get("graph", "default")
-    qset = auditlog.PersistentLog.objects.all()
-    if request.group:
-        qset = qset.filter(group=request.group)
-
-    ip = request.DATA.get("ip")
-    if ip:
-        qset = qset.filter(session__ip=ip)
-
-    path = request.DATA.get("path")
-    if path:
-        qset = qset.filter(remote_path__icontains=path)
-    
-    method = request.DATA.get("method")
-    if method:
-        qset = qset.filter(method=method)
-
-    action = request.DATA.get("action")
-    if action:
-        qset = qset.filter(action=action)
-    
-    component = request.DATA.get("component")
-    if component:
-        qset = qset.filter(component=component)
-    
-    pkey = request.DATA.get("pkey")
-    if pkey:
-        qset = qset.filter(pkey=pkey)
-
-    username = request.DATA.get("username")
-    if username:
-        qset = qset.filter(user__username=username)
-    
-    term = request.DATA.get("term")
-    if term:
-        qset = qset.filter(message__icontains=term)
-    
-    return rv.restList(request, qset.order_by('-when'), **auditlog.PersistentLog.getGraph(graph))
 
+from objict import objict
+# platform == fires apple keychain
+# cross-platform = tries for bluetooh
+FIDO_KEY_ATTACHMENT = settings.get("FIDO_KEY_ATTACHMENT", "cross-platform")
 
-@rd.urlGET (r'^list$')
-def auditList(request):
+FIDO_SERVER_ID = settings.get("FIDO_SERVER_ID", settings.SERVER_NAME)
+FIDO_SERVER_NAME = settings.get("FIDO_SERVER_NAME", settings.SITE_LABEL)
+
+
+def verify_origin(id):
+    return True
+
+
+def getServer(request=None, rp_id=FIDO_SERVER_ID, rp_name=FIDO_SERVER_NAME):
+    if request is not None:
+        rp_id = request.DATA.get(["rp_id", "fido_server_id"], rp_id)
+        rp_name = request.DATA.get(["rp_name", "fido_server_name"], rp_name)
+    rp = webauthn.PublicKeyCredentialRpEntity(id=rp_id, name=rp_name)
+    return Fido2Server(rp, verify_origin=verify_origin)
+
+
+def registerBegin(member, request, attachment=FIDO_KEY_ATTACHMENT):
     """
-    | Parameter: model=<string> (default=all)
-    | Parameter: id=<int> (default=all)
-    | Parameter: attributes=<string> (default=all)
-    | Parameter: user=<id|username> (default=all)
-    |
-    | Return: audit log entries
+    data = CredentialCreationOptions
+    state = {'challenge': '4yZmyZmnWP11t7g1S151oVgL0Vw0AU9GegTYJM2_928', 'user_verification': None}
     """
-    ret = auditlog.AuditLog.objects.all()
-    
-    model = request.DATA.get('model')
-    if model:
-        ret = ret.filter(model=model)
-
-    id = request.DATA.get('id')
-    if id:
-        ret = ret.filter(pkey=int(id))
-
-    attributes = request.DATA.get('attributes')
-    if attributes:
-        attributes = attributes.split(',')
-        print(attributes)
-        ret = ret.filter(attribute__in=attributes)
-
-    user = request.DATA.get('user')
-    if user:
-        ret = ret.filter(user=user)
-
-    return rv.restList(
-        request, ret, sort='-when',
-        fields=(
-            'when',
-            'model',
-            'pkey',
-            'attribute',
-            'user.id',
-            'user.username',
-            'reference',
-            'how',
-            'referer',
-            'stack',
-            'oldval',
-            'newval',
-        ), recurse_into=(
-            'user',
-        ), require_perms=(
-            'auditlog.can_read',
-        ),
-    )
 
+    server = getServer(request)
+    reg_data = dict(
+        id=rh.toBase64(member.getUUID()),
+        name=member.username,
+        displayName=member.display_name)
+    data, state = server.register_begin(
+        reg_data,
+        authenticator_attachment=attachment,
+        resident_key_requirement=webauthn.ResidentKeyRequirement.PREFERRED)
+    rp = objict(server.rp)
+    data = objict.fromdict(dict(data))
+    data.excludeCredentials = getUserCredentials(member, websafe=True)
+    rh.debug("data", data)
+    # rh.debug("registerBegin", rp, server.rp.id_hash)
+    return data, state, rp
+
+
+def registerComplete(request, fido2_state, rp_id):
+    credentials = request.DATA.get("credentials")
+    # rh.debug("registerComplete", fido2_state, rp_id)
+    server = getServer(request, rp_id)
+    rp = objict(server.rp)
+    # rh.debug("registerBegin", rp, server.rp.id_hash)
+
+    auth_data = server.register_complete(
+        fido2_state,
+        response=credentials
+    )
 
-@rd.url(r'^nuke$')
-@rd.perm_required("nuke_logs")
-def nuke_log_data(request):
-    # nuclear option used for testing system to clear out all wallet data
-    # make sure this is enabled for this setup
-    confirm_nuke = request.DATA.get("nuke_code", None)
-    if confirm_nuke != "launch" or not getattr(auditlog.settings, "CAN_NUKE_DATABASE", False):
-        return rv.restPermissionDenied(request)
-
-    # first nuke all transactions
-    auditlog.PersistentLog.objects.all().delete()
-    auditlog.AuditLog.objects.all().delete()
-    auditlog.SessionLog.objects.all().delete()
-    return rv.restStatus(request, True)
+    user_key = UserPassKey(
+        uuid=credentials.id,
+        name=request.DATA.get("key_name", ""),
+        rp_id=rp_id,
+        member=request.member,
+        platform=request.DATA.getUserAgentPlatform(),
+        token=websafe_encode(auth_data.credential_data))
+    # Store `auth_data.credential_data` in your database associated with the user
+    user_key.save()
+    return user_key
+
+
+def getUserCredentials(member, websafe=False):
+    if member is None:
+        return []
+    creds = [webauthn.AttestedCredentialData(websafe_decode(uk.token)) for uk in member.passkeys.all()]
+    if websafe:
+        return [dict(
+            type="public-key",
+            id=rh.toBase64(acd.credential_id)) for acd in creds]
+    return creds
+
+
+def authBegin(request):
+    server = getServer(request)
+    stored_credentials = getUserCredentials(request.member)
+    auth_data, state = server.authenticate_begin(stored_credentials)
+    return auth_data, state, objict(server.rp)
+
+
+def authComplete(request, fido2_state, rp_id):
+    credential = request.DATA.get("credential")
+    upk = UserPassKey.objects.filter(uuid=credential.id, is_enabled=1).last()
+    if upk is None:
+        raise Exception("PassKey not found on host.")
+    stored_credentials = [webauthn.AttestedCredentialData(websafe_decode(upk.token))]
+    server = getServer(request, rp_id)
+    cred = server.authenticate_complete(
+        fido2_state,
+        credentials=stored_credentials,
+        response=credential)
+    request.member = upk.member
+    request.member.canLogin(request)  # throws exception if cannot login
+    request.member.loginNoPassword(request=request)
+    request.member.log(
+        "passkey_login", "passkey login succesful", 
+        request, method="login", level=7)
+    upk.touch()
+    return upk
```

### Comparing `django_restit-4.2.9/auditlog/tq.py` & `django_restit-4.2.90/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/README.md` & `django_restit-4.2.90/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/handlers.py` & `django_restit-4.2.90/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/migrations/0001_initial.py` & `django_restit-4.2.90/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.2.90/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/models/bounce.py` & `django_restit-4.2.90/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/models/complaint.py` & `django_restit-4.2.90/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/models/message.py` & `django_restit-4.2.90/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/models/template.py` & `django_restit-4.2.90/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/rpc.py` & `django_restit-4.2.90/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/utils/parsing.py` & `django_restit-4.2.90/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/inbox/utils/render.py` & `django_restit-4.2.90/inbox/utils/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,18 @@
 
 
 def renderTemplate(template, context, group=None):
     context["SITE_LABEL"] = settings.SITE_LABEL
     context["BASE_URL"] = settings.BASE_URL
     context["SITE_LOGO"] = settings.SITE_LOGO
     context["SERVER_NAME"] = settings.SERVER_NAME
+    context["UNSUBSCRIBE_URL"] = settings.get("UNSUBSCRIBE_URL", f"{settings.BASE_URL}/api/account/unsubscribe")
     context["version"] = settings.VERSION
+    if "COMPANY_NAME" not in context and settings.COMPANY_NAME:
+        context["COMPANY_NAME"] = settings.COMPANY_NAME
 
     if template[-4:] in ["html", ".txt"]:
         # this is a django template
         return render_to_string(template, context)
     qset = MailTemplate.objects.filter(name=template)
     if group is not None:
         gqset = qset.filter(group=group)
```

### Comparing `django_restit-4.2.9/inbox/utils/sending.py` & `django_restit-4.2.90/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/README.md` & `django_restit-4.2.90/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/__init__.py` & `django_restit-4.2.90/incident/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from objict import objict
 
 META_KEYS = ["SERVER_PROTOCOL", "REQUEST_METHOD", "QUERY_STRING", "HTTP_USER_AGENT"]
 
 
-def event(category, description, level=10, request=None, **kwargs):
+def _request_to_meta(request, metadata):
+    metadata.ip = request.ip
+    if "path" not in metadata:
+        metadata.path = request.path
+    for key in META_KEYS:
+        value = request.META.get(key, None)
+        if value is not None and isinstance(value, str) and "." not in key:
+            metadata[key.lower()] = str(value)
+    if hasattr(request, "buid"):
+        metadata["buid"] = request.buid
+    if "username" not in metadata and hasattr(request, "member") and request.member is not None:
+        metadata["username"] = request.member.username
+    return metadata
+
+
+def event(category, description, level=10, request=None, group=None, **kwargs):
     from taskqueue.models import Task
-    data = objict(category=category, description=description, level=level)
+    data = objict(category=category, description=description, level=level, group=group)
     data.metadata = objict.fromdict(kwargs)
+    if request is not None:
+        _request_to_meta(request, data.metadata)
     Task.Publish("incident", "new_event", channel="tq_app_handler", data=data)
 
 
-def event_now(category, description, level=10, request=None, **kwargs):
+def event_now(category, description, level=10, request=None, group=None, **kwargs):
     from .models.event import Event
-    data = objict(category=category, description=description, level=level)
+    data = objict(category=category, description=description, level=level, group=group)
     data.metadata = objict.fromdict(kwargs)
     if request is not None:
-        data.metadata.ip = request.ip
-        if "path" not in data.metadata:
-            data.metadata.path = request.path
-        for key in META_KEYS:
-            value = request.META.get(key, None)
-            if value is not None and isinstance(value, str) and "." not in key:
-                data.metadata[key.lower()] = str(value)
-        if hasattr(request, "buid"):
-            data.metadata["buid"] = request.buid
-        if "username" not in data.metadata and hasattr(request, "member") and request.member is not None:
-            data.metadata["username"] = request.member.username
+        _request_to_meta(request, data.metadata)
     if "hostname" in data.metadata:
         data.hostname = data.metadata.hostname
     if "details" in data.metadata:
         data.details = data.metadata.details
     if "component" in data.metadata:
         data.component = data.metadata.component
     if "component_id" in data.metadata:
@@ -70,18 +77,19 @@
 
     for k, v in kwargs.items():
         metadata[k] = v
 
     if request.auth_model is not None:
         metadata['auth_model'] = str(request.auth_model)
     if request.group is not None:
-        metadata['group'] = request.group.name
+        metadata['group_name'] = request.group.name
+        metadata['group_id'] = request.group.id
     if hasattr(request, "buid"):
         metadata["buid"] = request.buid
     if hasattr(request, "_log_component"):
         metadata["component"] = request._log_component
         metadata["pkey"] = request._log_pk
 
     event_now(
         category, description=subject, level=level, hostname=host,
         details=stack, reporter_ip=request.ip, request=request,
-        metadata=metadata)
+        **metadata)
```

### Comparing `django_restit-4.2.9/incident/migrations/0001_initial.py` & `django_restit-4.2.90/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.2.90/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.2.90/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.2.90/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.2.90/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0010_incident_category_incident_component_id.py` & `django_restit-4.2.90/incident/migrations/0010_incident_category_incident_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/migrations/0011_ticket.py` & `django_restit-4.2.90/incident/migrations/0011_ticket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/incident/models/event.py` & `django_restit-4.2.90/incident/models/event.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rest import log
 from rest import settings
 from objict import objict
 
 import metrics
 
 from datetime import datetime, timedelta
-from .incident import Incident
+from .incident import Incident, INCIDENT_STATE_PENDING
 from .rules import Rule
 
 INCIDENT_METRICS = settings.get("INCIDENT_METRICS", False)
 INCIDENT_EVENT_METRICS = settings.get("INCIDENT_EVENT_METRICS", False)
 EVENT_TO_INCIDENT_LEVEL = settings.get("EVENT_TO_INCIDENT_LEVEL", 4)
 EVENT_DETAIL_TEMPLATES = settings.get("EVENT_DETAIL_TEMPLATES", None)
 EVENT_META_KEYWORDS = settings.get("EVENT_META_KEYWORDS", [
@@ -42,15 +42,15 @@
 """
 
 
 class Event(JSONMetaData, rm.RestModel):
     class RestMeta:
         POST_SAVE_FIELDS = ["level", "catagory"]
         SEARCH_FIELDS = ["description", "hostname"]
-        VIEW_PERMS = ["view_incidents"]
+        VIEW_PERMS = ["view_incidents", "view_logs"]
         CREATE_PERMS = None  # allow anyone to create an event
         GRAPHS = {
             "default": {
                 "graphs": {
                     "group": "basic",
                     "created_by": "basic"
                 },
@@ -69,15 +69,20 @@
 
     hostname = models.CharField(max_length=255, blank=True, null=True, default=None, db_index=True)
     description = models.CharField(max_length=84)
     details = models.TextField(default=None, null=True)
 
     level = models.IntegerField(default=0, db_index=True)
     category = models.CharField(max_length=124, db_index=True)
-    
+    # code = models.IntegerField(default=0, db_index=True)
+
+    group = models.ForeignKey(
+        "account.Group", on_delete=models.SET_NULL, 
+        related_name="+", null=True, default=None)
+ 
     component = models.SlugField(max_length=250, null=True, blank=True, default=None)
     component_id = models.IntegerField(null=True, blank=True, default=None)
 
     # this allows us to bundle multiple events to an incident
     incident = models.ForeignKey(
         Incident, null=True, default=None, 
         related_name="events", on_delete=models.SET_NULL)
@@ -113,14 +118,16 @@
             self.setProperty("country", gip.country)
             self.setProperty("state", gip.state)
             self.setProperty("city", gip.city)
             self.setProperty("isp", gip.isp)
 
     def set_description(self, value):
         # trun desc to 84
+        if value is None:
+            value = ""
         if len(value) > 84:
             value = value[:80] + "..."
         self.description = value
 
     def on_rest_pre_save(self, request):
         if self.hostname is None:
             self.hostname = settings.HOSTNAME
@@ -128,57 +135,71 @@
             self.setProperty("hostname", self.hostname)
         self.setProperty("category", self.category)
         if request and request.DATA.get("ip_lookup", field_type=bool):
             self.reporter_ip = request.ip
             self.lookupIP(request.ip)
 
     def on_rest_saved(self, request, is_new=False):
+        if not is_new:
+            return
         if INCIDENT_EVENT_METRICS:
             if self.hostname:
                 metrics.metric(f"incident_evt_{self.hostname}", category="incident_events", min_granularity="hourly")
             metrics.metric("incident_evt", category="incident_events", min_granularity="hourly")
 
         self.setProperty("level", self.level)
         if request is not None:
             self.reporter_ip = request.ip
         # run through rules for the category
         hit_rule = self.runRules()
         priority = 10
         incident = None
+        action_count = 0
         if hit_rule is not None:
-            logger.error(f"RULE HIT: {hit_rule.name}")
+            # logger.error(f"RULE HIT: {hit_rule.name}")
             priority = hit_rule.priority
             if hit_rule.action == "ignore":
                 self.save()
                 return
             if hit_rule.bundle > 0:
                 incident = Incident.getBundled(rule=hit_rule, event=self)
+
         elif self.level >= EVENT_TO_INCIDENT_LEVEL:
             # we ignore levels 4 and higher if they did not create a rule
             self.save()
             # logger.info(f"ignore event {self.pk} {self.description}")
             return
 
         # always create an incident 
         if incident is None:
             incident = Incident(
                 rule=hit_rule, priority=priority,
                 reporter_ip=self.reporter_ip,
                 category=self.category,
+                group=self.group,
                 component=self.component, 
                 component_id=self.component_id,
                 hostname=self.hostname)
-            if hit_rule is not None:
+            if self.group is None and hit_rule is not None:
                 incident.group = hit_rule.group
+            if hit_rule is not None and hit_rule.action_after != 0:
+                incident.state = INCIDENT_STATE_PENDING
             # TODO possibly make this smarter?
-            if self.category == "ossec":
+            if hit_rule and hit_rule.title_template and "{" in hit_rule.title_template:
+                try:
+                    incident.description = hit_rule.title_template.format(event=self)
+                except Exception:
+                    logger.exception(hit_rule.title_template)
+                    incident.description = self.description
+            elif self.category == "ossec":
                 incident.description = f"{self.hostname}: {self.description}"
             else:
                 incident.description = self.description
             incident.save()
+            incident.updateMeta(self)
         self.incident = incident
         self.save()
         if INCIDENT_METRICS:
             if self.hostname:
                 metrics.metric(f"incidents_{self.hostname}", category="incidents", min_granularity="hourly")
             metrics.metric("incidents", category="incidents", min_granularity="hourly")
```

### Comparing `django_restit-4.2.9/incident/models/incident.py` & `django_restit-4.2.90/incident/models/incident.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 from django.db import models
 from rest import settings
 
 from rest import models as rm
 from rest import helpers as rh
 from taskqueue.models import Task
-from account.models import Member
+from account.models import Member, Group
 from objict import objict
 from datetime import datetime, timedelta
 from rest import log
 from ws4redis import client as ws4redis
 import time
 
 logger = log.getLogger("incident", filename="incident.log")
 
+EVENT_META_TO_INCIDENT = [
+    "username",
+    "email",
+    "phone",
+    "group_name",
+    "group_id",
+    ("http_user_agent", "user_agent"),
+    "user_agent",
+    "http_url",
+    "error",
+    "error_code",
+    "rule_id",
+    "path"
+]
+
 INCIDENT_STATE_NEW = 0
 INCIDENT_STATE_OPENED = 1
 INCIDENT_STATE_PAUSED = 2
 INCIDENT_STATE_IGNORE = 3
 INCIDENT_STATE_RESOLVED = 4
+INCIDENT_STATE_PENDING = 5
 
 INCIDENT_STATES = [
     (INCIDENT_STATE_NEW, "new"),
     (INCIDENT_STATE_OPENED, "opened"),
     (INCIDENT_STATE_PAUSED, "paused"),
     (INCIDENT_STATE_IGNORE, "ignored"),
     (INCIDENT_STATE_RESOLVED, "resolved"),
+    (INCIDENT_STATE_PENDING, "pending"),
 ]
 
 INCIDENT_EMAIL_FROM = settings.get("INCIDENT_EMAIL_FROM", None)
 if INCIDENT_EMAIL_FROM is None:
     INCIDENT_EMAIL_FROM = f"{settings.SITE_LABEL} INCIDENT <incident@{settings.EMAIL_DEFAULT_DOMAIN}>"
 
 
 class Incident(models.Model, rm.RestModel, rm.MetaDataModel):
     class RestMeta:
         POST_SAVE_FIELDS = ["level", "catagory", "action"]
         SEARCH_FIELDS = ["description", "hostname"]
-        VIEW_PERMS = ["view_incidents"]
+        VIEW_PERMS = ["view_incidents", "view_issues"]
+        LIST_PARENT_KINDS = ["org", "iso"]
+        LIST_CHILD_DEPTH = 3
         GRAPHS = {
             "default": {
                 "extra": ["metadata", ("get_state_display", "state_display")],
                 "graphs": {
                     "group": "basic",
                     "rule": "basic",
                     "assigned_to": "basic"
@@ -61,23 +80,46 @@
     hostname = models.CharField(max_length=200, null=True, default=None, db_index=True)
     reporter_ip = models.CharField(max_length=16, blank=True, null=True, default=None, db_index=True)
 
     group = models.ForeignKey("account.Group", on_delete=models.SET_NULL, null=True, default=None)
     assigned_to = models.ForeignKey("account.Member", on_delete=models.SET_NULL, null=True, default=None)
     
     priority = models.IntegerField(default=0)  # 1-10, 1 being the highest
-    state = models.IntegerField(default=0, choices=INCIDENT_STATES)  # 0=new, 1=opened, 2=paused, 3=ignore, 4=resolved
+    # 0=new, 1=opened, 2=paused, 3=ignore, 4=resolved, 5=pending
+    state = models.IntegerField(default=0, choices=INCIDENT_STATES)
     action_sent = models.DateTimeField(default=None, null=True)
 
     rule = models.ForeignKey("incident.Rule", on_delete=models.SET_NULL, null=True, default=None)
 
     @property
     def first_event(self):
         return self.events.first()
 
+    @property
+    def action_triggered(self):
+        if self.rule is None or self.rule.action_after == 0:
+            return True
+        return self.events.all().count() >= abs(self.rule.action_after)
+
+    @property
+    def bundle_expired(self):
+        if self.rule is not None:
+            return self.created < (datetime.now() - timedelta(minutes=self.rule.bundle))
+        return True
+
+    @property
+    def email_subject(self):
+        # normalize subject
+        return f"Incident #{self.pk} - {self.category}"
+
+    def get_action_perm(self):
+        if self.rule and ":" in self.rule.action:
+            return self.rule.action.split(":")
+        return None, None
+
     def set_action(self, value):
         if value == "merge":
             request = self.getActiveRequest()
             ids = request.DATA.getList("merge_ids")
             if ids and len(ids) > 0:
                 self.mergeWith(ids, request)
                 self._changed__ = objict()
@@ -92,14 +134,32 @@
             for h in self.history.all():
                 h.parent = self
                 h.save()
         qset.delete()
         count = self.events.all().count()
         self.setProperty("event_count", count)
 
+    def updateMeta(self, event):
+        for key in EVENT_META_TO_INCIDENT:
+            new_key = key
+            if isinstance(key, tuple):
+                key, new_key = key
+            if key in event.metadata:
+                self.setProperty(new_key, event.metadata[key])
+        self.setProperty("details", event.details)
+        if event.metadata.geoip and event.metadata.geoip.city:
+            self.setProperty("city", event.metadata.geoip.city)
+            self.setProperty("state", event.metadata.geoip.state)
+            self.setProperty("country", event.metadata.geoip.country)
+            self.setProperty("isp", event.metadata.geoip.isp)
+        else:
+            for key in ["city", "state", "country", "isp"]:
+                if key in event.metadata:
+                    self.setProperty(new_key, event.metadata[key])
+
     def shouldTriggerAction(self):
         count = self.events.all().count()
         self.setProperty("event_count", count)
         aa = self.rule.action_after
         if aa >= 0:
             return aa == count-1
         aa = abs(self.rule.action_after)
@@ -113,23 +173,31 @@
             return
         # if self.rule.bundle == 0:
         #     return
         # only do query if not 0
         logger.info("triggerAction", self.rule.action)
         if force or self.shouldTriggerAction():
             logger.info(f"triggering incident action: {self.rule.action}")
+            if self.state == INCIDENT_STATE_PENDING:
+                self.state = INCIDENT_STATE_NEW
+                self.save()
             self.triggerAsyncNotify()
             if self.rule.action is None or self.rule.action == "notify":
                 self.triggerNotify()
             elif self.rule.action.startswith("email:") or self.rule.action.startswith("notify:"):
                 self.triggerEmail()
             elif self.rule.action.startswith("sms:"):
                 self.triggerSMS()
             elif self.rule.action.startswith("task:"):
                 self.triggerTask()
+            elif self.rule.action.startswith("group:"):
+                self.triggerGroup()
+            elif self.rule.action == "resolved":
+                self.state = INCIDENT_STATE_RESOLVED
+                self.save()
             elif self.rule.action.startswith("firewall_block"):
                 if settings.FIREWALL_GLOBAL_BLOCK:
                     Task.Publish("incident", "firewall_block", 
                                  dict(ip=self.reporter_ip),
                                  channel="tq_broadcast")
 
     def triggerAsyncNotify(self):
@@ -151,14 +219,16 @@
             msg["catagory"] = event.category
             msg["details"] = event.getProperty("details")
             msg["hostname"] = event.hostname
             msg["username"] = event.getProperty("username")
             msg["server"] = event.getProperty("server")
             msg["ip"] = event.getProperty("ip")
             msg["method"] = event.getProperty("method")
+        if self.group is not None:
+            msg["group_id"] = self.group.id
         try:
             ws4redis.sendMessageToPK("incident", "all", msg)
         except Exception:
             rh.log_exception("triggerAsyncNotify")
 
     def triggerTask(self):
         # task:APP_NAME:FNAME:CHANNEL
@@ -193,24 +263,75 @@
             url = F"{settings.INCIDENT_PORTAL_URL}?incident={self.pk}"
             msg = f"Incident #{self.pk}\n{self.description}\n{url}"
             for m in members:
                 m.sendSMS(msg)
         except Exception:
             rh.log_exception("triggerSMS")
 
-    def notifyWith(self, perm):
-        # logger.info("notifyWith", perm)
-        count = self.getProperty("event_count", default=1, field_type=int)
-        events = None
-        if count > 1:
-            subject = F"Incident #{self.pk} {self.category}@{self.hostname} had {count} events"
-            events = self.events.all()
+    def triggerGroup(self):
+        if self.rule.action.count(":") == 2:
+            action, gid, perm = self.rule.action.split(":")
+            self.group = Group.objects.filter(pk=int(gid)).last()
+            self.save()
         else:
-            subject = F"New Incident #{self.pk} {self.category}@{self.hostname}"
+            action, perm = self.rule.action.split(":")
 
+        if not self.group:
+            self.notifyWith("notify.unknown_incidents")
+            return
+        self.action_sent = datetime.now()
+        self.save()
+
+        subject = f"New Issue @ {self.group.name} - {self.description}"
+        details = self.getProperty("details", self.description)
+        username = self.getProperty("username", None)
+        email = self.getProperty("email", None)
+        phone = self.getProperty("phone", None)
+        if self.category == "support":
+            sms_msg = f"{settings.SITE_LABEL}\n{self.description}\n{details}"
+        else:
+            sms_msg = f"{settings.SITE_LABEL}\nIssue @ {self.group.name}\n{details}"
+
+        body = []
+
+        if username is not None:
+            body.append(f"Reported by: {username}")
+        if phone is not None:
+            body.append(f"Requesting Callback: {phone}")
+        elif email is not None:
+            body.append(f"Respond to: {email}")
+        body.append(f"Location: {self.group.name}")
+        body.append("<hr>")
+        body.append(f"<pre>{details}</pre>")
+        if username is not None:
+            body.append(f"- {username}")
+        body = "<br>\n".join(body)
+        # now we loop up through our groups parents
+        count = 0
+        group = self.group
+        if perm.startswith("notify."):
+            perm = perm.split(".")[1]
+        sms_perms = f"notify.sms_{perm}"
+        email_perms = f"notify.email_{perm}"
+        while group is not None or count > 4:
+            self.notifyMembers(group, subject, body, sms_msg, sms_perms, email_perms)
+            group = group.parent
+
+    def notifyMembers(self, group, subject, body, sms_msg, sms_perms, email_perms):
+        members = group.getMembers(perms=sms_perms, as_member=True)
+        for member in members:
+            member.sendSMS(sms_msg)
+        members = group.getMembers(perms=email_perms, as_member=True)
+        for member in members:
+            member.sendEmail(subject, body)       
+
+    def notifyWith(self, perm):
+        # logger.info("notifyWith", perm)
+        # count = self.getProperty("event_count", default=1, field_type=int)
+        subject = self.email_subject
         Member.notifyWith(
             perm,
             subject=subject,
             template=settings.get("INCIDENT_TEMPLATE", "email/incident_plain.html"),
             context=dict(incident=self, portal_url=settings.INCIDENT_PORTAL_URL),
             email_only=True, from_email=INCIDENT_EMAIL_FROM)
 
@@ -221,24 +342,15 @@
         return int((datetime.now() - self.action_sent).total_seconds())
 
     def triggerNotify(self):
         if self.lastSentAge() < 300:
             return
         self.action_sent = datetime.now()
         self.save()
-        if self.group is not None:
-            # all member of the group are notified because it is an incident group
-            self.group.notifyMembers(
-                subject=F"Incident #{self.pk} {self.category}@{self.hostname}",
-                template=settings.get("INCIDENT_TEMPLATE", "email/incident_plain.html"),
-                context=dict(incident=self, portal_url=settings.INCIDENT_PORTAL_URL),
-                perms=["notify.incident_alerts"],
-                email_only=True, from_email=INCIDENT_EMAIL_FROM)
-        else:
-            self.notifyWith("notify.unknown_incidents")
+        self.notifyWith("notify.unknown_incidents")
 
     def on_rest_saved(self, request, is_new=False):
         if not is_new:
             if self._changed__:
                 self.logHistory(request=request)
             if request != None and len(request.FILES):
                 for name, value in request.FILES.items():
@@ -272,17 +384,36 @@
                 self.assigned_to = member
                 self.save()
         if media is not None:
             h.saveMediaFile(media, "media", media.name)
         h.save()
         if notify and h.state != INCIDENT_STATE_IGNORE:
             self.notifyWatchers(
-                subject=F"Updated Incident #{self.id}",
+                subject=self.email_subject,
                 history=h)
 
+    def notifyMessage(self, message, by):
+        action, perm = self.get_action_perm()
+        if perm is None:
+            perm = "notify.incident_alerts"
+        subject = self.email_subject
+        context = dict(
+                    incident=self,
+                    portal_url=settings.INCIDENT_PORTAL_URL,
+                    message=message,
+                    by=by)
+        template = "email/incident_msg.html"
+        Member.notifyWith(
+            perm,
+            subject,
+            template=template,
+            context=context,
+            email_only=True,
+            from_email=INCIDENT_EMAIL_FROM)
+
     def notifyWatchers(self, subject, history=None):
         action = None
         perm = "notify.incident_alerts"
         if self.rule is not None and (self.rule.action.startswith("email:") or self.rule.action.startswith("notify:")):
             action, perm = self.rule.action.split(":")
         context = dict(
                     incident=self,
@@ -308,15 +439,15 @@
                 template=template,
                 context=context,
                 email_only=True,
                 from_email=INCIDENT_EMAIL_FROM)
         else:
             # notitfy everyone but the sender          
             if history.by is None:
-                members = Member.GetWithPermission(perm).exclude(pk=history.by.pk)
+                members = Member.GetWithPermission(perm, ignore_disabled_email=True).exclude(pk=history.by.pk)
                 if members.count() == 0:
                     return
                 NotificationRecord = Incident.getModel("account", "NotificationRecord")
                 NotificationRecord.notify(
                     members,
                     subject,
                     template=template,
@@ -331,17 +462,17 @@
         q = objict(rule=rule, created__gte=when)
         if rule.bundle_by in [2, 3, 5]:
             if event.component_id:
                 q.component = event.component
                 q.component_id = event.component_id
         if rule.bundle_by in [1, 3, 7]:
             q.hostname = event.hostname
-        elif rule.bundle_by in [4, 5, 8]:
+        if rule.bundle_by in [4, 5, 8]:
             q.reporter_ip = event.reporter_ip
-        elif rule.bundle_by in [6, 7, 8]:
+        if rule.bundle_by in [6, 7, 8]:
             q.category = event.category
         return Incident.objects.filter(**q).last()
 
     @classmethod
     def canPublishTo(cls, credentials, msg):
         if credentials:
             return True
@@ -356,21 +487,21 @@
     class Meta:
         ordering = ['-created']
 
     class RestMeta:
         SEARCH_FIELDS = ["to__username", "note"]
         GRAPHS = {
             "default": {
-                "extra":[
+                "extra": [
                     ("get_state_display", "state_display"),
                     ("get_priority_display", "priority_display"),
                 ],
-                "graphs":{
-                    "by":"basic",
-                    "to":"basic",
+                "graphs": {
+                    "by": "basic",
+                    "to": "basic",
                     "media": "basic"
                 }
             },
         }
     parent = models.ForeignKey(Incident, related_name="history", on_delete=models.CASCADE)
     created = models.DateTimeField(auto_now_add=True, editable=False)
 
@@ -383,7 +514,11 @@
 
     state = models.IntegerField(default=0)
     priority = models.IntegerField(default=0)
 
     note = models.TextField(blank=True, null=True, default=None)
     media = models.ForeignKey("medialib.MediaItem", related_name="+", null=True, default=None, on_delete=models.CASCADE)
 
+    def on_rest_created(self, request):
+        # self.group.sendEvent("chat_message", None, custom=dict(pk=self.pk, by=request.member.id, kind=self.kind))
+        if self.kind in ["note", "message"]:
+            self.parent.notifyMessage(self.note, self.by)
```

### Comparing `django_restit-4.2.9/incident/models/ossec.py` & `django_restit-4.2.90/incident/models/ossec.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,9 +43,11 @@
     username2   = models.CharField(max_length=64, blank=False, null=True, default=None)
     ssh_sig     = models.TextField(blank=False, null=True, default=None)
 
     level       = models.IntegerField(default=0)
     title       = models.CharField(max_length=200, blank=True, null=True, default=None)
     geoip       = models.ForeignKey("location.GeoIP", blank=True, null=True, default=None, on_delete=models.DO_NOTHING)
     
+    metadata = None
+    
     def __str__(self):
         return f'{self.hostname}: {self.title}'
```

### Comparing `django_restit-4.2.9/incident/models/rules.py` & `django_restit-4.2.90/incident/models/rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 """
 
 
 class Rule(models.Model, rm.RestModel):
     class RestMeta:
         SEARCH_FIELDS = ["name", "group__name"]
+        POST_SAVE_FIELDS = ["checks"]
         CAN_DELETE = True
         VIEW_PERMS = ["view_incidents"]
         # VIEW_PERMS = ["example_permission"]
         GRAPHS = {
             "default": {
                 "graphs": {
                     "group": "basic",
@@ -38,29 +39,36 @@
             },
             "basic": {
                 "fields": [
                     "id",
                     "created",
                     "priority",
                     "name",
+                    "title_template",
                     "category",
                     "priority",
                     "action",
                     "action_after",
                     "bundle",
                     "bundle_by",
                     "match_by"
                 ]
+            },
+            "download": {
+                "graphs": {
+                    "checks": "basic"
+                }
             }
         }
 
     created = models.DateTimeField(auto_now_add=True)
     modified = models.DateTimeField(auto_now=True)
 
     name = models.CharField(max_length=200)
+    title_template = models.CharField(max_length=200, default=None, null=True)
     # the group the rule gets assigned to when triggered
     group = models.ForeignKey("account.Group", on_delete=models.CASCADE, null=True, default=None)
     # category allows us to limit running rules to only those with a category
     # if category is null then this will run on all events?
     category = models.CharField(max_length=200, db_index=True)
     created_by = models.ForeignKey("account.Member", on_delete=models.CASCADE, null=True, default=None)
     # this specifies the order the rule runs in and will assign the priority to the created incident
@@ -85,21 +93,38 @@
         for check in checks:
             if not check.run(event):
                 return False
         return True
 
     def check_any_match(self, event):
         checks = self.checks.all().order_by("index")
+        # first we must check all required checks
+        for check in checks:
+            if check.is_required:
+                if not check.run(event):
+                    return False
+        # next we can match on any non required checks
         for check in checks:
+            if check.is_required:
+                continue
             if check.run(event):
                 return True
-            elif check.is_required:
-                return False
         return False
 
+    def set_checks(self, value):
+        if not isinstance(value, list):
+            return
+        exclude = ["id", "pk", "created", "modified", "parent"]
+        for item in value:
+            nval = {key: item[key] for key in item if key not in exclude and RuleCheck.hasField(key)}
+            nval["parent"] = self.id
+            rh.debug(nval)
+            obj = RuleCheck.createFromDict(self.getActiveRequest(), nval)
+            rh.debug("created", obj)
+
 
 class RuleCheck(models.Model, rm.RestModel):
     class RestMeta:
         SEARCH_FIELDS = ["name"]
         CAN_DELETE = True
         # VIEW_PERMS = ["example_permission"]
         GRAPHS = {
```

### Comparing `django_restit-4.2.9/incident/models/ticket.py` & `django_restit-4.2.90/location/models/legacy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,56 @@
 from django.db import models
-from django.conf import settings
-
 from rest import models as rm
-from rest import helpers as rh
-
+from location import geolocate
 
-class Ticket(models.Model, rm.RestModel, rm.MetaDataModel):
-    class RestMeta:
-        SEARCH_FIELDS = ["title", "description"]
-        CAN_DELETE = True
-        VIEW_PERMS = ["view_tickets"]
-        GRAPHS = {
-            "default": {
-                "extra": ["metadata"],
-                "graphs": {
-                    "group": "basic",
-                    "created_by": "basic",
-                    "assigned_to": "basic",
-                    "incident": "basic"
-                },
-            },
-            "detailed": {
-                "graphs": {
-                    "group": "basic",
-                    "created_by": "basic",
-                    "assigned_to": "basic",
-                    "incident": "basic",
-                    "generic__component": "basic"
-                },
-            },
-        }
 
-    created = models.DateTimeField(auto_now_add=True)
-    modified = models.DateTimeField(auto_now=True)
+class GeoIPLocation(models.Model, rm.RestModel):
+    # assocate with a user if possible
+    owner = models.ForeignKey("account.User", blank=True, null=True, default=None, related_name="locations", on_delete=models.CASCADE)
 
-    group = models.ForeignKey(
-        "account.Group", on_delete=models.SET_NULL, 
-        related_name="tickets",
-        null=True, default=None)
-    assigned_to = models.ForeignKey(
-        "account.Member", on_delete=models.SET_NULL, 
-        related_name="tickets",
-        null=True, default=None)
-    created_by = models.ForeignKey(
-        "account.Member", on_delete=models.CASCADE,
-        related_name="+",
-        null=True, default=None)
-
-    # if category is null then this will run on all events?
-    category = models.CharField(max_length=200, db_index=True)
-    priority = models.IntegerField(default=10, db_index=True)  # 1-10, 1 being the highest
-
-    title = models.CharField(max_length=200)
-    description = models.TextField()
-
-    status = models.CharField(max_length=32, default=None, null=True, db_index=True)
-    state = models.IntegerField(default=0)  # how many incidents before firing action
-
-    incident = models.ForeignKey(
-        "incident.Incident", null=True, default=None, 
-        related_name="tickets", on_delete=models.SET_NULL)
+    # use this to reference a Model
+    obj_id = models.IntegerField(blank=True, default=0)
+    obj_kind = models.CharField(max_length=64, blank=True, null=True, default="")
 
-    component = models.CharField(max_length=200, null=True, default=None, db_index=True)
-    component_id = models.IntegerField(null=True, blank=True, default=None, db_index=True)
+    ip = models.CharField(max_length=32)
+    created = models.DateTimeField(auto_now_add=True)
+    city = models.CharField(max_length=64, blank=True, null=True)
+    region = models.CharField(max_length=64)
+    country = models.CharField(max_length=64)
+    area_codes = models.CharField(max_length=64)
+    timezone = models.CharField(max_length=32)
+    kind = models.CharField(max_length=32)
+
+    lat = models.FloatField(default=0.0, blank=True)
+    lng = models.FloatField(default=0.0, blank=True)
+
+    @staticmethod
+    def cloneForOwner(obj, owner):
+        clone = obj
+        clone.pk = None
+        clone.id = None
+        clone.owner = owner
+        clone.save()
+        return clone
+
+    @staticmethod
+    def createByIP(ip, owner=None):
+        # first check if we have already seen this ip
+        locs = GeoIPLocation.objects.filter(ip=ip)
+        if locs.count():
+            if locs.filter(owner=owner).count():
+                return locs.filter(owner=owner).first()
+            # clone the first obj
+            return GeoIPLocation.cloneForOwner(locs.first(), owner)
+
+        res = geolocate.locateIP(ip)
+        obj = None
+        if res:
+            obj = GeoIPLocation(owner=owner, ip=ip, lat=res["lat"], lng=res["lng"])
+            if "city" in res:
+                obj.city = res["city"]
+            if "country" in res:
+                obj.country = res["country"]
+            if "region" in res:
+                obj.region = res["region"]
+            obj.save()
+        return obj
```

### Comparing `django_restit-4.2.9/incident/rpc.py` & `django_restit-4.2.90/incident/rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,42 @@
 from .parsers import ossec
 from taskqueue.models import Task
 import incident
 
 LOG_REST_PREFIX = settings.get("REST_PREFIX", "api/")
 if not LOG_REST_PREFIX.startswith("/"):
     LOG_REST_PREFIX = f"/{LOG_REST_PREFIX}"
+STATUS_ON_PERM_DENIED = settings.get("STATUS_ON_PERM_DENIED", 403)
 
 
 def patched_restPermissionDenied(request, error="permission denied", 
-                                 error_code=403, status=200,
+                                 error_code=403, status=STATUS_ON_PERM_DENIED,
                                  component=None, component_id=None):
+    
+    description = f"permission denied: {error_code} '{error}' for {request.user} {request.method}:{request.path}"
+    # rh.log_error(description)
     if error_code == 404:
-        if not request.path.startswith("/rpc/") and not request.path.startswith(LOG_REST_PREFIX):
+        if not request.path.startswith(LOG_REST_PREFIX) and not request.path.startswith("/rpc"):
             # just ignore these
             return rv.restResult(request, dict(status=False, error=error, error_code=error_code), status=status)
 
-    description = f"permission denied: {error_code} '{error}' for {request.user} {request.method}:{request.path}"
-    rh.log_error(description)
     metadata = dict(error=error, error_code=error_code, details=description)
     if component is not None:
         metadata["component"] = component
         metadata["component_id"] = component_id
     if hasattr(request, "member") and request.member is not None:
+        request.DATA.log()
         request.member.log("rest_denied", error, request, level=10)
         if component is None:
             metadata["component"] = "account.Member"
             metadata["component_id"] = request.member.pk
 
     if getattr(request, "token_bearer", None) is not None:
         metadata["token_bearer"] = request.token_bearer
-        metadata["token"] = request.token
+        metadata["token"] = f"***{request.token[-6:]}"
     incident.event_now(
         "rest_denied",
         description,
         level=10,
         request=request,
         **metadata)
     return rv.restResult(request, dict(status=False, error=error, error_code=error_code), status=status)
@@ -54,14 +57,15 @@
 
 @rd.urlPOST(r'^ossec/alert$')
 def ossec_alert_creat_from_request(request):
     payload = request.DATA.get("payload")
     if payload:
         try:
             # TODO make this a task (background it)
+            # rh.log_error("parsing payload", payload)
             od = ossec.parseAlert(request, payload)
             # lets now create a local event
             if od is not None:
                 level = 10
                 if od.level > 10:
                     level = 1
                 elif od.level > 7:
@@ -71,46 +75,54 @@
                 elif od.level == 5:
                     level = 4
                 elif od.level == 4:
                     level = 6
                 elif od.level <= 3:
                     level = 8
                 metadata = od.toDict(graph="default")
-                ssh_sig = metadata.get("ssh_sig", None)
-                if ssh_sig is not None and ssh_sig.startswith("http"):    
-                    metadata.url = ssh_sig
-                    metadata.pop("ssh_sig")
+                metadata.update(od.metadata)
+                # we reuse the ssh_sig because it is a text field to store urls
+                # ssh_sig = metadata.get("ssh_sig", None)
+                # if ssh_sig is not None and ssh_sig.startswith("http"):    
+                #     metadata["url"] = ssh_sig
+                #     metadata["domain"] = ossec.extractDomain(ssh_sig)
+                #     metadata["path"] = ossec.extractUrlPath(ssh_sig)
+                #     metadata.pop("ssh_sig")
                 if od.geoip:
                     metadata["country"] = od.geoip.country
                     metadata["city"] = od.geoip.city
                     metadata["province"] = od.geoip.state
                     metadata["isp"] = od.geoip.isp
+
                 am.Event.createFromDict(None, {
                     "hostname": od.hostname,
                     "description": od.title,
                     "details": od.text,
                     "level": level,
                     "category": "ossec",
                     "component": "incident.ServerOssecAlert",
                     "component_id": od.id,
                     "reporter_ip": od.src_ip,
                     "metadata": metadata
                 })
+                return rv.restStatus(request, True)
         except Exception as err:
+            rh.log_exception()
             stack = rh.getStackString()
             # rh.log_exception("during ossec alert", payload)
             metadata = dict(ip=request.ip, payload=payload)
             am.Event.createFromDict(None, {
                 "hostname": request.get_host(),
                 "description": f"error parseing alert: {err}",
                 "details": stack,
                 "level": 8,
                 "category": "ossec_error",
                 "metadata": metadata
             })
+    # rh.log_error("ossec alert", request.DATA.asDict())
     return rv.restStatus(request, False, error="no alert data")
 
 
 @rd.urlGET(r'^ossec$')
 @rd.urlGET(r'^ossec/(?P<pk>\d+)$')
 @rd.login_required
 def on_ossec(request, pk=None):
@@ -122,14 +134,15 @@
     # TODO check for key?
     resp = am.Event.on_rest_request(request)
     return rv.restStatus(request, True)
 
 
 @rd.urlGET(r'^event$')
 @rd.urlGET(r'^event/(?P<pk>\d+)$')
+@rd.urlPOST(r'^event/(?P<pk>\d+)$')
 @rd.login_required
 def rest_on_event(request, pk=None):
     return am.Event.on_rest_request(request, pk)
 
 
 @rd.url(r'^incident$')
 @rd.url(r'^incident/(?P<pk>\d+)$')
@@ -209,15 +222,15 @@
     ip = request.DATA.get("ip")
     action = request.DATA.get("action")
     if action not in ["block", "unblock"]:
         return rv.restPermissionDenied(request)
     metadata = request.DATA.asDict()
     metadata.username = request.member.username
     record_block(ip, action, "all", metadata)
-    Task.Publish("incident", f"firewall_{action}", dict(ip=ip), channel="tq_broadcast")
+    Task.Publish("incident", f"firewall_{action}", dict(ip=ip), channel="tq_firewall")
     return rv.restStatus(request, True)
 
 
 @rd.url('ticket')
 @rd.url('ticket/<int:pk>')
 def rest_on_ticket(request, pk=None):
     return am.Ticket.on_rest_request(request, pk)
```

### Comparing `django_restit-4.2.9/incident/templates/email/incident_change.html` & `django_restit-4.2.90/incident/templates/email/incident_change.html`

 * *Files 2% similar despite different names*

```diff
@@ -189,20 +189,14 @@
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;text-align: center;background: #e4e4e4; background-color: #e4e4e4;">
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:20px;font-weight:300;font-style:italic;line-height:30px;text-align:center;color:#000000;">
                         {{incident.description}}
                       </div>
                     </td>
                   </tr>
-                  <tr>
-                    <td>
-                      <pre style="font-size: 16px; overflow-x: scroll; word-wrap: normal; max-width: 980px; padding: 8px;">{{incident.first_event.details_by_category}}
-                      </pre>
-                    </td>
-                  </tr>
                   {% if history %}
                   <tr>
                     <td>
                       <pre style="font-size: 16px; overflow-x: scroll; word-wrap: normal; max-width: 980px; padding: 8px;">
 updated by: {% if history %}{{history.by.username}}{% else %}system{% endif %}
 
 {{history.note}}
@@ -281,15 +275,15 @@
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
+                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{UNSUBSCRIBE_URL}}?t={{unsubscribe_token}}">Unsubscribe</a>.
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {{incident.description}}
                                         
               Incident #{{incident.pk}} on {{incident.hostname}}
                                         {{incident.description}}
-{{incident.first_event.details_by_category}}
 updated by: {% if history %}{{history.by.username}}{% else %}system{% endif %}
 
 {{history.note}}
 You can respond to this email with notes or actions. Make sure to leave to
 blank lines at the end of your email. For actions just include one of these
 words on its own line: "open", "close", "pause", "ignore".
                                                 _V_I_E_W_ _O_N_ _P_O_R_T_A_L
```

### Comparing `django_restit-4.2.9/incident/templates/email/incident_new.html` & `django_restit-4.2.90/incident/templates/email/incident_new.html`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
+                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{UNSUBSCRIBE_URL}}?t={{unsubscribe_token}}">Unsubscribe</a>.
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
```

### Comparing `django_restit-4.2.9/incident/templates/email/incident_plain.html` & `django_restit-4.2.90/incident/templates/email/incident_plain.html`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
                         <!-- <a href="#" style="color:#fafafa">Privacy Policy</a> | <a href="#" style="color:#fafafa">Contact Support</a> | <a href="#" style="color:#fafafa">Unsubscribe</a><br /> --> Powered by {{SITE_LABEL}}<br> © 2023 {{settings.COMPANY_LABEL}}
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
                       <div style="font-family:Roboto, Helvetica, Arial, sans-serif;font-size:14px;font-weight:300;line-height:20px;text-align:center;color:#000000;">
-                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{BASE_URL}}member/unsubscribe/">Unsubscribe</a>.
+                        Don't like these emails? <a style="color: #c0c1ff;font-weight: bold;text-decoration: none;" href="{{UNSUBSCRIBE_URL}}?t={{unsubscribe_token}}">Unsubscribe</a>.
                       </div>
                     </td>
                   </tr>
                   <tr>
                     <td align="center" style="font-size:0px;padding:10px 25px;word-break:break-word;">
       
       <table
```

### Comparing `django_restit-4.2.9/incident/tq.py` & `django_restit-4.2.90/incident/tq.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         data.reporter_ip = data.metadata.ip
     ia.Event.createFromDict(None, task.data)
     task.completed()
 
 
 def firewall_block(task):
     # Task.Publish("incident", "firewall_block", {ip:"x.x.x.x"}, channel="tq_broadcast")
-    helpers.blockIP(task.data.ip)
+    helpers.local_block_ip(task.data.ip, metadata=task.data.metadata)
     task.log(f"{settings.HOSTNAME} - {task.data.ip} BLOCKED")
     task.completed()
 
 
 def firewall_unblock(task):
     # Task.Publish("incident", "firewall_unblock", {ip:"x.x.x.x"}, channel="tq_broadcast")
-    helpers.unblockIP(task.data.ip)
+    helpers.local_unblock_ip(task.data.ip, metadata=task.data.metadata)
     task.log(f"{settings.HOSTNAME} - {task.data.ip} UNBLOCKED")
     task.completed()
 
 
 def on_incoming_email(task):
     # dict(pk=msg.pk, to_email=msg.to_email, from_email=msg.from_email)
     msg = inbox.Message.objects.filter(pk=task.data.pk).last()
@@ -119,15 +119,29 @@
     stale = datetime.now() - timedelta(days=90)
     # delete all ossec alerts older then 90 days
     count = ia.ServerOssecAlert.objects.filter(created__lte=stale).delete()
     if count:
         task.log(f"deleted {count} old ServerOssecAlert")
     # delete all events older then 90 days
     count = ia.Event.objects.filter(created__lte=stale).filter(
-        Q(incident__state=ia.INCIDENT_STATE_IGNORE)|Q(incident__isnull=True)).delete()
+        Q(incident__state=ia.INCIDENT_STATE_IGNORE) | Q(incident__isnull=True)).delete()
     if count:
         task.log(f"deleted {count} old Events")
+    
+    count = ia.Incident.objects.filter(created__lte=stale).filter(state=ia.INCIDENT_STATE_IGNORE).delete()
+    if count:
+        task.log(f"deleted {count} old Incidents")
 
     count = GeoIP.removeDuplicates()
     if count:
         task.log(f"deleted {count} duplicate IPs")
 
+
+def run_auto_close(task):
+    # lets check any incidents that haven't reached action threshold and older then bundle time
+    qset = ia.Incident.objects.filter(state=ia.INCIDENT_STATE_PENDING)
+    for inc in qset:
+        if inc.bundle_expired:
+            inc.state = ia.INCIDENT_STATE_IGNORE
+            inc.save()
+            inc.logHistory("history", "auto ignore", notify=False)
+
```

### Comparing `django_restit-4.2.9/location/geolocate.py` & `django_restit-4.2.90/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/migrations/0001_initial.py` & `django_restit-4.2.90/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.2.90/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/models/address.py` & `django_restit-4.2.90/location/models/address.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,51 +2,80 @@
 from rest import models as rm
 from rest import helpers as rh
 from .. import geolocate
 
 
 class Address(models.Model, rm.RestModel):
     class RestMeta:
+        VIEW_PERMS = [
+            "view_all_groups",
+            "manage_groups",
+            "manage_group",
+            "manage_settings"]
+        CREATE_PERMS = None  # allow anyone to create
+        SAVE_PERMS = None  # allow anyone to edit
         GRAPHS = {
             "abstract": {
                 "fields":[
                     ('line1', 'street1'),
                     ('line2', 'street2'),
                     'city',
                     'state',
                     ('postalcode', 'zip'),
                     'country',
                 ]
             }
         }
-    modified_by = models.ForeignKey("account.User", null=True, blank=True, default=None, on_delete=models.CASCADE)
+    label = models.CharField(
+        max_length=250, null=True, blank=True,
+        default=None, db_index=True)
+    member = models.ForeignKey(
+        "account.User", null=True, blank=True,
+        default=None, on_delete=models.SET_NULL, related_name="addresses")
+    group = models.ForeignKey(
+        "account.Group", null=True, blank=True,
+        default=None, on_delete=models.SET_NULL, related_name="addresses")
     modified = models.DateTimeField(auto_now=True)
     line1 = models.CharField(max_length=255, blank=True, null=True, default=None)
     line2 = models.CharField(max_length=255, blank=True, null=True, default=None)
     city = models.CharField(max_length=127, blank=True, null=True, default=None)
     state = models.CharField(max_length=127, blank=True, null=True, default=None)
     county = models.CharField(max_length=127, blank=True, null=True, default=None)
     country = models.CharField(max_length=16, blank=True, null=True, default=None)
     postalcode = models.CharField(max_length=32, blank=True, null=True, default=None)
+    postalcode_suffix = models.CharField(max_length=32, blank=True, null=True, default=None)
     lat = models.FloatField(default=0.0, blank=True)
     lng = models.FloatField(default=0.0, blank=True)
 
     def getTimezone(self):
         if self.lat:
             return geolocate.getTimeZone(self.lat, self.lng)
         return None
 
+    def lookup(self):
+        res = geolocate.search("{}, {}, {}".format(self.line1, self.city, self.state))
+        if isinstance(res, list) and len(res):
+            return res[0]
+        return None
+
     def refresh(self):
         try:
-            res = geolocate.search("{}, {}, {}".format(self.line1, self.city, self.state))
-            self.county = res.county
-            self.country = res.short_country
-            self.lat = res.latitude
-            self.lng = res.longitude
-            super(Address, self).save()
+            addr = self.lookup()
+            if addr:
+                if addr.county:
+                    self.county = addr.county
+                self.country = addr.country
+                if addr.lat:
+                    self.lat = addr.lat
+                    self.lng = addr.lng
+                if not self.postalcode and addr.postal_code:
+                    self.postalcode = addr.postal_code
+                if addr.postal_code_suffix:
+                    self.postalcode_suffix = addr.postal_code_suffix
+                super(Address, self).save()
         except Exception:
             rh.log_exception("address.refresh")
 
     def save(self, *args, **kwargs):
         if not self.lat:
             self.refresh()
         super(Address, self).save(*args, **kwargs)
```

### Comparing `django_restit-4.2.9/location/models/ip.py` & `django_restit-4.2.90/location/models/ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 
     @classmethod
     def lookup(cls, ip, force_refresh=False, stale_after=300, using=None):
         if isinstance(ip, str):
             ip = ip.strip()
         if not geolocate.isIP(ip):
             ip = geolocate.dnsToIP(ip)
+            if ip is None:
+                return None
         subnet = ip[:ip.rfind(".")]
         gip = GeoIP.objects.filter(ip=ip).first()
         if gip is None:
             gip = GeoIP(ip=ip, subnet=subnet)
             if GEOIP_LOOKUP_BY_SUBNET:
                 subgip = GeoIP.objects.filter(subnet=subnet).last()
                 if subgip:
```

### Comparing `django_restit-4.2.9/location/models/location.py` & `django_restit-4.2.90/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/models/track.py` & `django_restit-4.2.90/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/__init__.py` & `django_restit-4.2.90/location/providers/iplookup/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,12 @@
         return True
     except Exception:
         pass
     return False
 
 
 def dnsToIP(name):
-    return socket.gethostbyname(name)
+    try:
+        return socket.gethostbyname(name)
+    except Exception:
+        pass
+    return None
```

### Comparing `django_restit-4.2.9/location/providers/iplookup/abstractapi.py` & `django_restit-4.2.90/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/extremeip.py` & `django_restit-4.2.90/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/geoplugin.py` & `django_restit-4.2.90/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/ipapi.py` & `django_restit-4.2.90/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/ipinfo.py` & `django_restit-4.2.90/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/iplookup/restit.py` & `django_restit-4.2.90/location/providers/iplookup/restit.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
         "lat": 33.6409,
         "lng": -117.6031
     }
     """
     if GEOIP_RESTIT_HOST is None:
         return None
     params = {"ip": ip}
-    url = f"https://{GEOIP_RESTIT_HOST}/rpc/location/ip/lookup"
+    url = f"https://{GEOIP_RESTIT_HOST}/api/location/ip/lookup"
     res = requests.get(url, params=params)
     if res.status_code != 200:
         return None
     data = objict.fromdict(res.json())
     data.provider = GEOIP_RESTIT_HOST
     return data.data
```

### Comparing `django_restit-4.2.9/location/providers/location/google.py` & `django_restit-4.2.90/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/timezones/google.py` & `django_restit-4.2.90/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/providers/zillow.py` & `django_restit-4.2.90/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/rpc/ip.py` & `django_restit-4.2.90/location/rpc/ip.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,19 +23,24 @@
         stale_after=request.DATA.get("stale_after", 90, field_type=int))
     graph = request.DATA.get("graph", "default")
     return gip.restGet(request, graph)
 
 
 @rd.urlGET('geo/ip')
 @rd.urlGET('geo/ip/<int:pk>')
-@rd.login_required
 def rest_on_geoip(request, pk=None):
     return location.GeoIP.on_rest_request(request, pk)
 
 
+@rd.urlPOST('geo/ip/<int:pk>')
+@rd.perm_required(["manage_location"])
+def rest_save_geoip(request, pk=None):
+    return location.GeoIP.on_rest_request(request, pk)
+
+
 @rd.urlPOST('geo/ip')
 @rd.login_required
 @rd.requires_params(["ip"])
 def rest_on_geoip_lookup(request, pk=None):
     ip = request.DATA.get("ip", request.ip)
     gip = location.GeoIP.get(
         ip,
```

### Comparing `django_restit-4.2.9/location/rpc/location.py` & `django_restit-4.2.90/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/location/rpc/track.py` & `django_restit-4.2.90/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/admin.py` & `django_restit-4.2.90/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/cvutil/contours.py` & `django_restit-4.2.90/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/cvutil/images.py` & `django_restit-4.2.90/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/cvutil/misc.py` & `django_restit-4.2.90/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/cvutil/text.py` & `django_restit-4.2.90/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/fixtures/initial_data.json` & `django_restit-4.2.90/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/fixtures/medialib.json` & `django_restit-4.2.90/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.2.90/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/forms.py` & `django_restit-4.2.90/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/migrations/0001_initial.py` & `django_restit-4.2.90/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/models.py` & `django_restit-4.2.90/medialib/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,19 +320,21 @@
 
     def default_store(self):
         try:
             return settings.MEDIALIB_STORE[self.id]
         except (KeyError, AttributeError):
             return settings.MEDIALIB_DEFAULT_STORE
 
+
 class MediaItem(models.Model, RestModel, MetaDataModel):
     """
     Media Item (a video or image)
     """
     class RestMeta:
+        SEARCH_FIELDS = ["name", "description"]
         VIEW_PERMS = ["view_media", "manage_users", "manage_media"]
         SAVE_PERMS = ["manage_media", "manage_users"]
         OWNER_FIELD = "owner"
         GRAPHS = {
             "simple": {
                 "fields": [
                     'id',
```

### Comparing `django_restit-4.2.9/medialib/ocr.py` & `django_restit-4.2.90/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/pdf.py` & `django_restit-4.2.90/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/qrcode.py` & `django_restit-4.2.90/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/__init__.py` & `django_restit-4.2.90/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/anigif.py` & `django_restit-4.2.90/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/ffmpeg.py` & `django_restit-4.2.90/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/gifsicle.py` & `django_restit-4.2.90/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/hls.py` & `django_restit-4.2.90/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/mp4box.py` & `django_restit-4.2.90/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.2.90/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/rtmpdump.py` & `django_restit-4.2.90/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/rtmpsink.py` & `django_restit-4.2.90/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/video_getinfo.py` & `django_restit-4.2.90/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/engines/websnap.py` & `django_restit-4.2.90/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/exceptions.py` & `django_restit-4.2.90/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/akamai.py` & `django_restit-4.2.90/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.2.90/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/ffmpeg.py` & `django_restit-4.2.90/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/flv.py` & `django_restit-4.2.90/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/hls.py` & `django_restit-4.2.90/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/image_transcode.py` & `django_restit-4.2.90/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/image_validate.py` & `django_restit-4.2.90/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/mp4.py` & `django_restit-4.2.90/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/video_still.py` & `django_restit-4.2.90/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/video_validate.py` & `django_restit-4.2.90/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/websnap.py` & `django_restit-4.2.90/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/presets/youtube.py` & `django_restit-4.2.90/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/render/render_utils.py` & `django_restit-4.2.90/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/rpc/legacy.py` & `django_restit-4.2.90/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/rpc/media.py` & `django_restit-4.2.90/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/rpc/tools.py` & `django_restit-4.2.90/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/scripts/init_config` & `django_restit-4.2.90/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/css/base_medialibui.css` & `django_restit-4.2.90/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/css/base_widgets.css` & `django_restit-4.2.90/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/css/jquery.jcrop.css` & `django_restit-4.2.90/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/bg-body.gif` & `django_restit-4.2.90/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/loading.gif` & `django_restit-4.2.90/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/noimage.gif` & `django_restit-4.2.90/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/render_err.gif` & `django_restit-4.2.90/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/rendering.gif` & `django_restit-4.2.90/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/img/unknown.gif` & `django_restit-4.2.90/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/caman.full.js` & `django_restit-4.2.90/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/hammer.min.js` & `django_restit-4.2.90/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.2.90/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/jquery.hammer.js` & `django_restit-4.2.90/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/load-image.min.js` & `django_restit-4.2.90/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/swiper.js` & `django_restit-4.2.90/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.2.90/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/__init__.py` & `django_restit-4.2.90/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/__init__.py` & `django_restit-4.2.90/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/channel.py` & `django_restit-4.2.90/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/discovery.py` & `django_restit-4.2.90/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/errors.py` & `django_restit-4.2.90/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/http.py` & `django_restit-4.2.90/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.2.90/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/model.py` & `django_restit-4.2.90/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.2.90/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/apiclient/schema.py` & `django_restit-4.2.90/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/filestore.py` & `django_restit-4.2.90/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/httplib2/__init__.py` & `django_restit-4.2.90/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.2.90/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.2.90/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/httplib2/socks.py` & `django_restit-4.2.90/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/httpstore.py` & `django_restit-4.2.90/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.2.90/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/appengine.py` & `django_restit-4.2.90/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/client.py` & `django_restit-4.2.90/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.2.90/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/crypt.py` & `django_restit-4.2.90/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.2.90/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/file.py` & `django_restit-4.2.90/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/gce.py` & `django_restit-4.2.90/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.2.90/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.2.90/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.2.90/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/old_run.py` & `django_restit-4.2.90/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/tools.py` & `django_restit-4.2.90/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/util.py` & `django_restit-4.2.90/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.2.90/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/s3store.py` & `django_restit-4.2.90/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/stores/uritemplate/__init__.py` & `django_restit-4.2.90/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/base.html` & `django_restit-4.2.90/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/instances.html` & `django_restit-4.2.90/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/items.html` & `django_restit-4.2.90/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/library.html` & `django_restit-4.2.90/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/test.html` & `django_restit-4.2.90/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/templates/medialib/testpicker.html` & `django_restit-4.2.90/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/tests.py` & `django_restit-4.2.90/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/tq.py` & `django_restit-4.2.90/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/utils.py` & `django_restit-4.2.90/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/views.py` & `django_restit-4.2.90/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/__init__.py` & `django_restit-4.2.90/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/__init__.py` & `django_restit-4.2.90/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/channel.py` & `django_restit-4.2.90/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/discovery.py` & `django_restit-4.2.90/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/errors.py` & `django_restit-4.2.90/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/http.py` & `django_restit-4.2.90/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.2.90/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/model.py` & `django_restit-4.2.90/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.2.90/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/apiclient/schema.py` & `django_restit-4.2.90/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/httplib2/__init__.py` & `django_restit-4.2.90/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.2.90/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.2.90/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/httplib2/socks.py` & `django_restit-4.2.90/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/client.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/file.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/gce.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/tools.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/util.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.2.90/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/upload.py` & `django_restit-4.2.90/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.2.90/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/README.md` & `django_restit-4.2.90/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/client.py` & `django_restit-4.2.90/metrics/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,38 +34,42 @@
 
 
 def set_metric(slug, value, category=None, expire=None, date=None):
     """Create/Increment a metric."""
     get_r().set_metric(slug, value, category=category, expire=expire, date=date)
 
 
-def get_metric(slug, min_granularity=None, max_granularity=None):
+def get_metric(slug, min_granularity=None, max_granularity=None, category=None):
     """get a metric."""
+    if category is not None:
+        return get_r().get_metric_by_category(category, min_granularity, max_granularity)
     return get_r().get_metric(slug, min_granularity, max_granularity)
 
 
 def get_metrics(slugs, since=None, granularity="daily", group=None, samples=None):
     """Create/Increment a metric."""
     return get_r().get_metric_history_chart_data(
         slugs, since, granularity, group=group, samples=samples)
 
 
 def get_category_metrics(category, since=None, granularity="daily", samples=None):
     """Create/Increment a metric."""
     r = get_r()
-    slugs = [utils.to_string(s) for s in list(r.category_slugs(category))]
+    slugs = r.category_slugs(category, True)
     return r.get_metric_history_chart_data(
         slugs, since, granularity, samples=samples)
 
 
 def get_slugs(category=None):
     """get slug list"""
     if category:
-        return list(get_r().category_slugs(category))
-    return list(get_r().metric_slugs())
+        slugs = list(get_r().category_slugs(category))
+    else:
+        slugs = list(get_r().metric_slugs())
+    return [utils.to_string(s) for s in list(slugs)]
 
 
 def get_gauge(slug):
     """get a gauge."""
     return get_r().get_gauge(slug)
 
 
@@ -169,18 +173,20 @@
         """Returns a set of Categories under which metrics may have been
         organized."""
         return self.r.smembers(self._categories_key)
 
     def _category_key(self, category):
         return u"c:{0}".format(category)
 
-    def category_slugs(self, category):
+    def category_slugs(self, category, as_string=False):
         """Returns a set of the metric slugs for the given category"""
         key = self._category_key(category)
         slugs = self.r.smembers(key)
+        if as_string:
+            return [utils.to_string(s) for s in slugs]
         return slugs
 
     def _categorize(self, slug, category):
         """Add the ``slug`` to the ``category``. We store category data as
         as set, with a key of the form::
 
             c:<category name>
@@ -206,15 +212,15 @@
 
             {<category_name>: set(<slug1>, <slug2>, ...)}
 
         """
         result = utils.OrderedDict()
         categories = sorted(self.r.smembers(self._categories_key))
         for category in categories:
-            result[category] = self.category_slugs(category)
+            result[category] = self.category_slugs(category, True)
 
         # We also need to see the uncategorized metric slugs, so need some way
         # to check which slugs are not already stored.
         categorized_metrics = set([  # Flatten the list of metrics
             slug for sublist in result.values() for slug in sublist
         ])
         f = lambda slug: slug not in categorized_metrics
@@ -350,29 +356,40 @@
                     pipe.expireat(key, m_expireat)
                 elif ":m:" in key or ":y:" in key:
                     continue
                 else:
                     pipe.expireat(key, d_expireat)
         pipe.execute()
 
+    def get_metric_by_category(self, category, min_granularity=None, max_granularity=None):
+        results = UberDict()
+        for slug in self.category_slugs(category, True):
+            results[slug] = self.get_metric(slug, min_granularity, max_granularity)
+        return results
+
     def get_metric(self, slug, min_granularity=None, max_granularity=None):
         """Get the current values for a metric.
 
         Returns a dictionary with metric values accumulated for the seconds,
         minutes, hours, day, week, month, and year.
 
         """
         results = UberDict()
         granularities = utils.granularities(min_granularity, max_granularity)
-        keys = utils.build_keys(slug)
+        keys = utils.build_keys(slug, min_granularity=min_granularity, max_granularity=max_granularity)
+
         for granularity, key in zip(granularities, keys):
+            rh.debug("-- get_metric --", granularity, key)
             try:
                 results[granularity] = int(self.r.get(key))
             except Exception:
-                pass
+                results[granularity] = 0
+                rh.log_exception("get_metric", granularity, key)
+        if min_granularity and min_granularity == max_granularity:
+            return results[min_granularity]
         return results
 
     def get_metrics(self, slug_list):
         """Get the metrics for multiple slugs.
 
         Returns a list of two-tuples containing the metric slug and a
         dictionary like the one returned by ``get_metric``::
@@ -397,16 +414,17 @@
             metrics = self.r.mget(*utils.build_keys(slug))
             if any(metrics):  # Only if we have data.
                 results.append((slug, dict(zip(keys, metrics))))
         return results
 
     def get_category_metrics(self, category):
         """Get metrics belonging to the given category"""
-        slug_list = self.category_slugs(category)
-        return self.get_metrics(slug_list)
+        slug_list = self.category_slugs(category, True)
+        res = self.get_metrics(slug_list)
+        return res
 
     def delete_category(self, category):
         """Removes the category from Redis. This doesn't touch the metrics;
         they simply become uncategorized."""
         # Remove mapping of metrics-to-category
         category_key = self._category_key(category)
         self.r.delete(category_key)
@@ -567,15 +585,15 @@
             since = utils.start_by_granularity(granularity, samples=samples)
         elif group:
             since = group.getLocalTime(since)
         elif settings.METRICS_TIMEZONE:
             since = date_util.convertToLocalTime(settings.METRICS_TIMEZONE, since)
 
         slugs = sorted(slugs)
-        rh.debug(f"get_metric_history {since}")
+        # rh.debug(f"get_metric_history {since}", slugs)
         history = self.get_metric_history(slugs, since, granularity=granularity)
 
         # Convert the history into an intermediate data structure organized
         # by periods. Since the history is sorted by key (which includes both
         # the slug and the date, the values should be ordered correctly.
         data = utils.OrderedDict()
         for k, v in history:
```

### Comparing `django_restit-4.2.9/metrics/eod.py` & `django_restit-4.2.90/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/examples/eod_example.py` & `django_restit-4.2.90/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.2.90/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.2.90/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.2.90/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.2.90/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/management/commands/system_metric.py` & `django_restit-4.2.90/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/migrations/0001_initial.py` & `django_restit-4.2.90/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.2.90/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.2.90/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.2.90/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/models.py` & `django_restit-4.2.90/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/periodic.py` & `django_restit-4.2.90/metrics/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/providers/aws.py` & `django_restit-4.2.90/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/metrics/rpc.py` & `django_restit-4.2.90/metrics/rpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
 from rest import decorators as rd
 from rest import views as rv
 from rest import settings
 from rest import helpers as rh
 from rest import net
 from rest import ssl_check
+from rest import helpers as rh
 from location.models import GeoIP
 from . import client as metrics
 from . import models as mm
 from . import models as em
 from .providers import aws
-from objict import nobjict
+from objict import nobjict, objict
 import time
+import re
 
 """
 Capture simple analytics counters.
 """
 LOCATION_METRICS = settings.LOCATION_METRICS
 REST_PREFIX = settings.get("REST_PREFIX", "api/")
 
@@ -42,41 +44,61 @@
 
 
 @rd.urlGET('metric')
 @rd.login_required
 def rest_on_get_metric(request):
     # slug, num=1, category=None, expire=None, date=None
     data = request.DATA.toObject()
-    if data.slug is None:
+    if data.slug is None and data.category is None:
         return rv.restStatus(request, False)
-    result = metrics.get_metric(data.slug)
+    if data.granularity:
+        data.min_granularity = data.granularity
+        data.max_granularity = data.granularity
+    result = metrics.get_metric(
+        data.slug, category=data.category,
+        min_granularity=data.min_granularity,
+        max_granularity=data.max_granularity)
     if result is None:
         return rv.restStatus(request, False)
+    if data.prefix:
+        result = {key[len(data.prefix):]:value for key, value in result.items()}
     return rv.restReturn(request, dict(data=result))
 
 
+def truncatePrefix(prefix, data):
+    # rh.debug("prefix", prefix, data)
+    for values in data["data"]:
+        if values["slug"].startswith(prefix):
+            values["slug"] = values["slug"][len(prefix):]
+
+
 @rd.urlGET('metrics')
 @rd.login_required
 def rest_on_get_metrics(request, pk=None):
     # slug, since, granularity
     since = request.DATA.get("since", field_type=datetime)
     granularity = request.DATA.get(["granularity", "period"], default="daily")
     samples = request.DATA.get("samples", field_type=int)
     category = request.DATA.get("category")
-    rh.debug(f"rest_on_get_metrics: {since}, {granularity}, {samples}, {category}")
+    prefix = request.DATA.get("prefix")
+    # rh.debug(f"rest_on_get_metrics: {since}, {granularity}, {samples}, {category}")
     if category:
         result = metrics.get_category_metrics(category, since, granularity, samples=samples)
+        if prefix:
+            truncatePrefix(prefix, result)
         return rv.restReturn(request, dict(data=result))
     slugs = request.DATA.getlist(["slugs", "slug"])
     if slugs is None:
         return rv.restStatus(request, False)
 
     result = metrics.get_metrics(slugs, since, granularity, samples=samples)
     if result is None:
         return rv.restStatus(request, False)
+    if prefix:
+        truncatePrefix(prefix, result)
     return rv.restReturn(request, dict(data=result))
 
 
 @rd.urlGET('slugs')
 @rd.login_required
 def rest_on_get_metrics_slugs(request, pk=None):
     category = request.DATA.get("category", None)
@@ -290,19 +312,25 @@
     for name in hosts:
         if settings.SERVER_NAME_MAP and name in settings.SERVER_NAME_MAP:
             host = settings.SERVER_NAME_MAP[name]
             if "." not in host:
                 host = f"{name}.{hostname}"
         else:
             host = f"{name}.{hostname}"
-        resp = net.REQUEST("GET", host, f"/{REST_PREFIX}versions", params=dict(detailed=1))
+        resp = net.REQUEST(
+            "GET", host, 
+            f"/{REST_PREFIX}versions", 
+            params=dict(detailed=1),
+            timeout=5.0)
         if resp.status:
             resp.data.id = host
             resp.data.hostname = host
             data.append(resp.data)
+        else:
+            data.append(dict(id=host, hostname=host))
     return rv.restReturn(request, dict(data=data))
 
 
 @rd.urlGET('aws/ec2/list/details')
 @rd.login_required
 def rest_on_ec2_list(request, pk=None):
     return rv.restReturn(request, dict(data=aws.getAllEC2()))
@@ -514,7 +542,86 @@
 
 @rd.urlGET('aws/rds/list/ids')
 @rd.login_required
 def rest_on_rds_list_ids(request, pk=None):
     return rv.restReturn(request, dict(data=aws.getAllRDS(True)))
 
 
+@rd.urlGET('logs/nginx')
+@rd.perm_required("view_logs")
+def rest_on_get_logs(request):
+    ip = request.DATA.get("ip", None)
+    gz = request.DATA.get("gz", None)
+    if ip is None:
+        return rv.restPermissionDenied(request)
+    return rv.restReturn(request, dict(data=search_logs(ip, gz)))
+
+
+def search_logs(ip, gz, custom=None):
+    cmd = ["/opt/api/bin/logsearch.sh", ip]
+    if gz:
+        cmd.append(gz)
+    out, err = rh.sudoCMD(cmd, return_output=True)
+    output = []
+    index = 0
+    for line in out.decode().split("\n"):
+        jline = nginx_line_to_json(line)
+        if jline is not None:
+            index += 1
+            jline["id"] = f"{settings.SERVER_NAME}{index}"
+            output.append(jline)
+    return output
+
+
+NGINX_PATTERN = r'(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}) (.*) (.*) \[(.*?)\] "(.*?)" (\d{3}) (\d*) "(.*?)" "(.*?)"'
+def nginx_line_to_json(line):
+    prog = re.compile(NGINX_PATTERN)
+    match = prog.match(line)
+    if match is None:
+        return None
+    return {
+        'server': settings.SERVER_NAME,
+        'remote_addr': match.group(1),
+        'sent_http_x_sessionid': match.group(2),
+        'sent_http_x_uid': match.group(3),
+        'time_local': match.group(4),
+        'request': match.group(5),
+        'status': int(match.group(6)),
+        'body_bytes_sent': int(match.group(7)),
+        'referrer': match.group(8),
+        'http_user_agent': match.group(9)
+    }
+
+
+@rd.urlGET('servers/logs')
+@rd.perm_required("view_logs")
+def rest_on_ec2_logs(request, pk=None):
+    hostname = settings.SERVER_ROOT
+    if hostname is None:
+        hostname = settings.SERVER_NAME
+    if hostname.count(".") == 2:
+        hostname = hostname[hostname.find(".")]
+    instances = aws.getAllEC2()
+    hosts = [inst.name for inst in instances]
+    ip = request.DATA.get("ip", "headless")
+    gz = request.DATA.get("gz", None)
+    params = dict(ip=ip, gz=gz)
+    logs = []
+    auth = request.META.get("HTTP_AUTHORIZATION", None)
+    if not auth or not ip:
+        return rv.restPermissionDenied(request)
+    headers = dict(Authorization=auth, referer=settings.BASE_URL)
+    for name in hosts:
+        if settings.SERVER_NAME_MAP and name in settings.SERVER_NAME_MAP:
+            host = settings.SERVER_NAME_MAP[name]
+            if "." not in host:
+                host = f"{name}.{hostname}"
+        else:
+            host = f"{name}.{hostname}"
+        resp = net.REQUEST(
+            "GET", host,
+            f"/{REST_PREFIX}metrics/logs/nginx",
+            headers=headers, params=params, timeout=30.0)
+        if resp.status and resp.data:
+            logs.extend(resp.data)
+    return rv.restReturn(request, dict(data=logs, size=len(logs), count=len(logs)))
+
```

### Comparing `django_restit-4.2.9/metrics/tq.py` & `django_restit-4.2.90/metrics/tq.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if not settings.DOMAIN_WATCH:
         task.log("no domains to check")
         return False
     now = datetime.utcnow()
     alarm_date = now + timedelta(days=30)
     result = ssl_check.check(*settings.DOMAIN_WATCH)
     for key, value in result.items():
-        if value is None:
+        if value is None or isinstance(value, str):
             continue
         if value < alarm_date:
             task.log(f"{key} is expiring soon")
             notifyDomainExpiring(key, value)
 
 
 def notifyDomainExpiring(domain, expires):
```

### Comparing `django_restit-4.2.9/metrics/utils.py` & `django_restit-4.2.90/metrics/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,29 +86,44 @@
     """
     return value.split(":")[1]
 
 
 def granularities(min_granularity=None, max_granularity=None):
     """Returns a generator of all possible granularities based on the
     MIN_GRANULARITY and MAX_GRANULARITY settings.
+    
+    Args:
+        min_granularity (str): Optional; the minimum granularity to include.
+        max_granularity (str): Optional; the maximum granularity to include.
+        
+    Yields:
+        str: A granularity level from the predefined list of granularities.
     """
+    # Use default settings if no values are provided
     if min_granularity is None:
         min_granularity = app_settings.MIN_GRANULARITY
     if max_granularity is None:
         max_granularity = app_settings.MAX_GRANULARITY
-    keep = False
+
+    # Initialize a flag to determine when to start yielding granularities
+    start_yielding = False
+
+    # Loop through each granularity in the list of all granularities
     for g in GRANULARITIES:
-        if g == min_granularity and not keep:
-            keep = True
-        elif g == max_granularity and keep:
-            keep = False
-        if keep:
-            if g == max_granularity:
-                keep = False
+        # Start yielding when the minimum granularity is reached
+        if g == min_granularity:
+            start_yielding = True
+        
+        # Yield the current granularity if the flag is true
+        if start_yielding:
             yield g
+        
+        # Stop yielding after the maximum granularity has been yielded
+        if g == max_granularity:
+            break
 
 
 def get_metric_key_pattern(granularity, slug, date):
     """ The Redis metric key and date formatting patterns for each key, by granularity"""
     patterns_by_granularity = {
         "seconds": {"key": "m:{0}:s:{1}", "date_format": "%Y-%m-%d-%H-%M-%S"},
         "minutes": {"key": "m:{0}:i:{1}", "date_format": "%Y-%m-%d-%H-%M"},
```

### Comparing `django_restit-4.2.9/pushit/migrations/0001_initial.py` & `django_restit-4.2.90/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/pushit/models.py` & `django_restit-4.2.90/pushit/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/pushit/rpc/githooks.py` & `django_restit-4.2.90/pushit/rpc/githooks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/pushit/rpc/legacy.py` & `django_restit-4.2.90/pushit/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/pushit/utils.py` & `django_restit-4.2.90/pushit/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/pyproject.toml` & `django_restit-4.2.90/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.2.9"
+version = "4.2.90"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
@@ -38,14 +38,15 @@
 pycountry = "*"
 psutil = "*"
 pillow = "*"
 pypng = "*"
 pygments = "*"
 mistune = "*"
 inlinestyler = "*"
+fido2 = "*"
 python-dateutil = "^2.8.2"
 hashids = "^1.3.1"
 boto3 = "^1.26.160"
 pyotp = "^2.8.0"
 pyqrcode = "^1.2.1"
 redis = "^3.0.1"
 django-redis-cache = "^3.0.1"
```

### Comparing `django_restit-4.2.9/rest/README.md` & `django_restit-4.2.90/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/arc4.py` & `django_restit-4.2.90/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/crypto/aes.py` & `django_restit-4.2.90/rest/crypto/aes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 from Crypto.Cipher import AES
 from Crypto import Random
-from hashlib import md5
+import hashlib
+from hashlib import md5, sha256
 
 import json
 from . import util
 
 
 DEFAULT_SALT = b"Salted__"
 MD5V_SALT = b"__MD5V__"
 SDKV_SALT = b"__SDKV__"
 SDKV16_SALT = b"__SDKV16"
+SHA256_SALT = b"SALTY__"
 
-KNOWN_SALTS = [DEFAULT_SALT, SDKV_SALT, MD5V_SALT, SDKV16_SALT]
+KNOWN_SALTS = [DEFAULT_SALT, SDKV_SALT, MD5V_SALT, SDKV16_SALT, SHA256_SALT]
 
 DEFAULT_IV_GENERATOR = "md5"
 
-# THIS USES AES/CBC/PKCS7Padding
 
-def encrypt(key, data, random_size=128, ivgen=DEFAULT_IV_GENERATOR):
+def encrypt(key, data, random_size=128, ivgen=DEFAULT_IV_GENERATOR, base64=True):
     """
     encrypts @data with @key using AES
     will pad data with random string of @random_size
         this will keep it so the same data is never producing the same encryption
     returns bytes as base64 string
+
+    HIS USES AES/CBC/PKCS7Padding
     """
     if random_size > 0:
         rdata = util.toBytes(data) + util.toBytes(util.randomString(random_size))
     else:
         rdata = data
+    if not base64:
+        return cbc_encrypt(key, rdata, ivgen, base64)
     return util.toString(cbc_encrypt(key, rdata, ivgen))
 
 
-def decrypt(key, edata, random_size=128, as_string=True):
-    encrypted = util.fromBase64(edata, False)
+def decrypt(key, edata, random_size=128, as_string=True, base64=True):
+    if base64:
+        encrypted = util.fromBase64(edata, False)
+    else:
+        encrypted = edata
     data = cbc_decrypt(key, encrypted)
     if random_size > 0:
         data = data[:-1 * random_size]
     if as_string:
         return util.toString(data)
     return data
 
 
-def cbc_encrypt(key, data, ivgen=DEFAULT_IV_GENERATOR):
+def cbc_encrypt(key, data, ivgen=DEFAULT_IV_GENERATOR, base64=True):
     if isinstance(data, dict) or isinstance(data, list):
         data = json.dumps(data)
     salt_prefix = getSaltPrefix(ivgen)
     data = util.toBytes(data)
     key = util.toBytes(key)
     salt = Random.new().read(8)
     if ivgen == "simple": 
@@ -53,14 +61,16 @@
         key = key_iv[:16]
         iv = key_iv[16:]
     else:
         key_iv = deterministric_key_iv(ivgen, key, salt, 32 + 16)
         key = key_iv[:32]
         iv = key_iv[32:]
     aes = AES.new(key, AES.MODE_CBC, iv)
+    if not base64:
+        return salt_prefix + salt + aes.encrypt(util.pad(data))
     return util.toBase64(salt_prefix + salt + aes.encrypt(util.pad(data)))
 
 
 def cbc_decrypt(key, encrypted):
     salt_prefix = encrypted[0:8]
     if salt_prefix not in KNOWN_SALTS:
         print("unknown salt: {}".format(str(salt_prefix)))
@@ -78,14 +88,16 @@
     decrypted = aes.decrypt(encrypted[16:])
     return util.unpad(decrypted)
 
 
 def deterministric_key_iv(generator, data, salt, length=48):
     if generator in [DEFAULT_SALT, MD5V_SALT, "md5"]:
         return md5_deterministic_key_iv(data, salt, length)
+    elif generator == SHA256_SALT:
+        return sha256_deterministic_key_iv(data, salt, length)
     return simple_deterministic_key_iv(data, salt, length)
 
 
 def getSaltPrefix(generator):
     if generator == "md5":
         return DEFAULT_SALT
     elif generator == "simple":
@@ -101,14 +113,26 @@
     final_key = key
     while len(final_key) < length:
         key = md5(key + data).digest()
         final_key += key
     return final_key[:length]
 
 
+def sha256_deterministic_key_iv(data, salt, length=48):
+    # extended from https://gist.github.com/gsakkis/4546068
+    assert len(salt) == 8, len(salt)
+    data += salt
+    key = sha256(data).digest()
+    final_key = key
+    while len(final_key) < length:
+        key = sha256(key + data).digest()
+        final_key += key
+    return final_key[:length]
+
+
 def simple_deterministic_key_iv(data, salt, length=48):
     src = data + salt
     src_len = len(src)
     dst = bytearray(length)
     p = salt[2] >> 4
     while p >= src_len:
         p = int(p / 2)
```

### Comparing `django_restit-4.2.9/rest/crypto/privpub.py` & `django_restit-4.2.90/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/crypto/util.py` & `django_restit-4.2.90/rest/crypto/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/datem.py` & `django_restit-4.2.90/rest/datem.py`

 * *Files 21% similar despite different names*

```diff
@@ -91,15 +91,16 @@
 
     offset = getTimeZoneOffset(zone, when)
     if offset >= 0:
         when = when - timedelta(hours=offset)
     else:
         when = when + timedelta(hours=offset)
     if tz_aware:
-        return when.replace(tzinfo=pytz.timezone(zone))
+        return pytz.timezone(zone).localize(when)
+        # return when.replace(tzinfo=pytz.timezone(zone))
     return when
 
 
 def convertToUTC(zone, when=None):
     # this works because it gets around the issue with naive vs aware
     offset = getTimeZoneOffset(zone, when)
     if offset >= 0:
@@ -200,37 +201,37 @@
     res = parseDateTime(date_str, is_future, is_past, month_end)
     if as_date and res:
         return date(res.year, res.month, res.day)
     return res
 
 
 def parseDateTime(date_str, is_future=False, is_past=False, month_end=True):
-    if type(date_str) in [str, str]:
+    if isinstance(date_str, str):
         dt = None
         if len(date_str) > 6 and date_str.count('.') <= 1 and date_str.split('.')[0].isdigit():
             try:
                 f = float(date_str)
                 return datetime.utcfromtimestamp(f)
             except Exception as err:
                 print(err)
         else:
             fix_month = False
             if date_str.count('-') or date_str.count('/') or date_str.count(' ') or date_str.count('.'):
-                dts = re.split('/|-| |\.',date_str)
+                dts = re.split('/|-| |\.', date_str)
                 if len(dts) == 2:
                     date_str = "{0}-{1}-01".format(dts[0], dts[1])
                 else:
                     "-".join(dts)
             elif len(date_str) == 4:
                 fix_month = month_end
                 date_str = date_str[:2] + "-01-" + date_str[2:4]
             elif len(date_str) == 3:
                 date_str = date_str[0] + "/1/" + date_str[-2:]
             elif len(date_str) == 6:
-                date_str = date_str[:2] + "-" + date_str[2:4] +  "-" + date_str[4:6]
+                date_str = date_str[:2] + "-" + date_str[2:4] + "-" + date_str[4:6]
         try:
             # print "parse date: {}".format(date_str)
             dt = date_parser(date_str)
             if is_future and dt.year < 2000:
                 dt = dt.replace(year=dt.year+100)
             elif is_past and dt.year >= 2000:
                 dt = dt.replace(year=dt.year-100)
@@ -238,17 +239,17 @@
             if fix_month:
                 dt = dt.replace(day=calendar.monthrange(dt.year, dt.month)[1])
             # print dt
             return dt
         except BaseException:
             pass
 
-    elif type(date_str) in [date, datetime]:
+    elif isinstance(date_str, (date, datetime)):
         return date_str
-    elif type(date_str) in [float, int]:
+    elif isinstance(date_str, (float, int)):
         return datetime.utcfromtimestamp(date_str)
     return None
 
 
 def getDateRangeZ(start, end=None, kind=None, zone=None, hour=0, eod=None, end_eod=None):
     return getDateRange(start, end, kind, zone, hour, eod, end_eod)
 
@@ -260,14 +261,16 @@
         zone = "UTC"
     if start == end:
         end = None
     if eod is not None:
         hour = eod
 
     start = parseDate(start)
+    if start is None:
+        raise Exception(f"invalid date format {start}")
     if end:
         end = parseDate(end)
         if start == end:
             end = None
 
     if kind and kind != "second":
         start = start.replace(minute=0, second=0, microsecond=0)
@@ -281,15 +284,15 @@
             start, end = getWeek(start)
         elif kind == "month":
             start = start.replace(hour=0, day=1)
             end = getEndOfMonth(start)
         elif kind == "year":
             start = start.replace(hour=0, day=1, month=1)
             end = getEndOfMonth(start.replace(month=12))
-        elif type(kind) is int or (isinstance(kind, str) and kind.isdigit()):
+        elif isinstance(kind, int) or (isinstance(kind, str) and kind.isdigit()):
             end = start + timedelta(days=1)
             start = end - timedelta(days=int(kind))
     
     if end is None:
         end = start + timedelta(hours=24)
 
     if zone and zone.lower() == "utc":
@@ -305,7 +308,81 @@
             start = start + timedelta(hours=offset)
         if end_eod:
             hour = end_eod
         offset = getTimeZoneOffset(zone, end, hour=hour)
         if offset:
             end = end + timedelta(hours=offset)
     return start, end
+
+
+def convert_to_epoch_range(start, end=None):
+    """
+    Convert start and end times to epoch timestamps in milliseconds.
+
+    Parameters:
+    start (int, datetime, or str): The start time, which can be:
+        - An int representing the epoch time in milliseconds.
+        - A datetime object representing the start time.
+        - A string representing a timedelta relative to the end time. The string can end with:
+            - 'm' for minutes (e.g., '30m' for 30 minutes ago)
+            - 'h' for hours (e.g., '5h' for 5 hours ago)
+            - 'd' for days (e.g., '2d' for 2 days ago)
+    end (datetime or None): The end time, which can be:
+        - A datetime object representing the end time.
+        - None, in which case the current time (UTC) is used.
+
+    Returns:
+    tuple: A tuple containing two integers:
+        - start_epoch: The epoch time of the start parameter in milliseconds.
+        - end_epoch: The epoch time of the end parameter in milliseconds.
+
+    Raises:
+    ValueError: If the end parameter is not a datetime object or None.
+    ValueError: If the start parameter is not an int, datetime object, or a valid timedelta string.
+    ValueError: If the start string does not end with 'm', 'h', or 'd'.
+
+    Examples:
+    >>> start = "30m"
+    >>> end = datetime(2024, 5, 13, 12, 30, tzinfo=timezone.utc)
+    >>> convert_to_epoch(start, end)
+    (1715676600000, 1715681400000)
+
+    >>> start = "1d"
+    >>> end = None
+    >>> convert_to_epoch(start, end)
+    (1715595000000, 1715681400000)
+
+    >>> start = "5h"
+    >>> end = datetime(2024, 5, 13, 12, 30, tzinfo=timezone.utc)
+    >>> convert_to_epoch(start, end)
+    (1715661000000, 1715681400000)
+    """
+    if end is None:
+        end = datetime.utcnow()
+
+    if isinstance(end, datetime):
+        end_epoch = int(end.timestamp() * 1000)
+    else:
+        raise ValueError("End parameter must be a datetime object or None.")
+
+    if isinstance(start, int):
+        start_epoch = start
+    elif isinstance(start, datetime):
+        start_epoch = int(start.timestamp() * 1000)
+    elif isinstance(start, str):
+        if start.endswith('m'):
+            delta_minutes = int(start[:-1])
+            start_datetime = end - timedelta(minutes=delta_minutes)
+        elif start.endswith('h'):
+            delta_hours = int(start[:-1])
+            start_datetime = end - timedelta(hours=delta_hours)
+        elif start.endswith('d'):
+            delta_days = int(start[:-1])
+            start_datetime = end - timedelta(days=delta_days)
+        else:
+            raise ValueError("Start string must end with 'm' for minutes, 'h' for hours, or 'd' for days.")
+        
+        start_epoch = int(start_datetime.timestamp() * 1000)
+    else:
+        raise ValueError("Start parameter must be an int, datetime object, or a string representing a timedelta.")
+
+    return start_epoch, end_epoch
```

### Comparing `django_restit-4.2.9/rest/decorators.py` & `django_restit-4.2.90/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/encryption.py` & `django_restit-4.2.90/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/errors.py` & `django_restit-4.2.90/rest/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/extra/json_metadata.py` & `django_restit-4.2.90/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/fields.py` & `django_restit-4.2.90/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/forms.py` & `django_restit-4.2.90/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/helpers.py` & `django_restit-4.2.90/rest/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import re
 import time
 from datetime import date, datetime, timedelta
 from .settings_helper import settings
 import importlib
 from django.db.models import Count, Q, Avg, Sum, Max, Min
 from django.db.models.query import QuerySet
+# from django.db.models.functions import TruncWeek, TruncMonth, TruncYear
 from io import StringIO
 import base64
-import binascii
 
 from objict import objict
 from .datem import *
 from .log import getLogger
 import getpass
 
 from urllib.parse import urlparse
@@ -467,15 +467,17 @@
 
     c = {
         "version":version,
         "SITE_LABEL":settings.SITE_LABEL,
         "SITE_LOGO":settings.SITE_LOGO,
         "SERVER_NAME":settings.SERVER_NAME,
         "BASE_URL":settings.BASE_URL,
-        "DISCLAIMER": settings.REST_DISCLAIMER
+        "DISCLAIMER": settings.REST_DISCLAIMER,
+        "COMPANY_LABEL": settings.COMPANY_LABEL,
+        "UNSUBSCRIBE_URL": settings.get("UNSUBSCRIBE_URL", f"{settings.BASE_URL}api/account/unsubscribe")
     }
 
     if request:
         c["protocol"] = getProtocol(request)
         c["request"] = request
 
     for k, v in kwargs.items():
@@ -512,32 +514,36 @@
 
     if end:
         q["{}__lte".format(date_field)] = end
     if q:
         return qset.filter(**q)
     return qset
 
+
 def getAverage(qset, field_name):
     res = qset.aggregate(avg_result=Avg(field_name))
     if "avg_result" in res and res["avg_result"] != None:
         return res["avg_result"]
     return 0.0
 
+
 def getMin(qset, field_name):
     res = qset.aggregate(min_result=Min(field_name))
     if "min_result" in res and res["min_result"] != None:
         return res["min_result"]
     return 0.0
 
+
 def getMax(qset, field_name):
     res = qset.aggregate(max_result=Max(field_name))
     if "max_result" in res and res["max_result"] != None:
         return res["max_result"]
     return 0.0
 
+
 def getSum(qset, *args):
     params = {}
     for field_name in args:
         key = "sum_{}".format(field_name)
         params[key] = Sum(field_name)
     # print params
     res = qset.aggregate(**params)
@@ -549,14 +555,41 @@
             value = 0
         results[field_name] = value
     if len(args) == 1:
         return list(results.values())[0]
     return results
 
 
+def getGroupLeaders(Model, timeframe="week", date_field="created", 
+                    size=10, field="id", action="count", out_field="value"):
+    today = datetime.now()
+    # FIXME: yes timerange to deal with timezone issues
+    q = {f"{date_field}__year": today.year}
+    if timeframe == "week":
+        q[f"{date_field}__week"] = today.isocalendar()[1]
+    elif timeframe == "month":
+        q[f"{date_field}__month"] = today.month
+    elif timeframe == "day":
+        q[f"{date_field}__day"] = today.day
+    qset = Model.objects.filter(**q).values('group__name', 'group')
+    if field == "id":
+        return list(qset.annotate(value=Count('id')).order_by('-value')[:size])
+    field_key = f"{field}_{action}"
+    if out_field:
+        field_key = out_field
+    aq = {}
+    if action == "sum":
+        aq[field_key] = Sum(field)
+    elif action == "average":
+        aq[field_key] = Avg(field)
+    else:
+        aq[field_key] = Count(field)
+    return list(qset.annotate(**aq).order_by(f"-{field_key}")[:size])
+
+
 def countOccurences(qset, field_name):
     output = objict()
     for item in list(qset.values(field_name).annotate(count=Count(field_name))):
         output[item[field_name]] = item["count"]
     return output
 
 
@@ -761,15 +794,15 @@
         with open(pid_file, "r") as f:
             pid = f.read()
             if pid.isdigit():
                 pid = int(pid)
     return pid
 
 
-def sudoCMD(cmd, as_user=None, test_first=True):
+def sudoCMD(cmd, as_user=None, test_first=False, return_output=False):
     if as_user and as_user == getUsername():
         sudo_cmd = []
         if isinstance(cmd, list):
             sudo_cmd.extend(cmd)
         else:
             sudo_cmd.append(cmd)
         return subprocess.Popen(sudo_cmd, close_fds=True)
@@ -786,33 +819,71 @@
     if isinstance(cmd, list):
         test_sudo_cmd.extend(cmd)
         sudo_cmd.extend(cmd)
     else:
         test_sudo_cmd.append(cmd)
         sudo_cmd.append(cmd)
     if test_first:
-        print(test_sudo_cmd)
         process = subprocess.Popen(test_sudo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         out, err = process.communicate()
         if err.strip():
             raise Exception("WARNING: cannot run {}, we don't have sudo rights".format(test_sudo_cmd))
+    if return_output:
+        proc = subprocess.Popen(sudo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        return proc.communicate()
     return subprocess.Popen(sudo_cmd, close_fds=True)
 
 
-def blockIP(ip):
-    # for global Task.Publish("incident", "global_block", {ip:"x.x.x.x"}, channel="tq_broadcast")
-    log_error(f"blocking {ip}")
+def local_block_ip(ip, **kwargs):
+    record_firewall_action(ip, "add", settings.hostname, kwargs.get("metadata", None))
+    if settings.LOCAL:
+        return True
     return sudoCMD([settings.BLOCK_IP_CMD, "add", ip])
 
 
-def unblockIP(ip):
-    # for global Task.Publish("incident", "global_unblock", {ip:"x.x.x.x"}, channel="tq_broadcast")
+def local_unblock_ip(ip, **kwargs):
+    record_firewall_action(ip, "delete", settings.hostname, kwargs.get("metadata", None))
+    if settings.LOCAL:
+        return True
     return sudoCMD([settings.BLOCK_IP_CMD, "delete", ip])
 
 
+def blockIP(ip, **kwargs):
+    if settings.FIREWALL_GLOBAL_BLOCK:
+        from taskqueue.models import Task
+        Task.Publish("incident", "firewall_block", dict(ip=ip), channel="tq_broadcast")
+        # record_firewall_action(ip, "add", "all", kwargs.get("metadata", None))
+        return True
+    return local_block_ip(ip, **kwargs)
+
+
+def unblockIP(ip, **kwargs):
+    # for global Task.Publish("incident", "global_unblock", {ip:"x.x.x.x"}, channel="tq_broadcast")
+    if settings.FIREWALL_GLOBAL_BLOCK:
+        from taskqueue.models import Task
+        Task.Publish("incident", "firewall_unblock", dict(ip=ip), channel="tq_broadcast")
+        # record_firewall_action(ip, "delete", "all", kwargs.get("metadata", None))
+        return True
+    return local_unblock_ip(ip, **kwargs)
+
+
+def record_firewall_action(ip, action, hostname, metadata):
+    from incident.models import Event
+    title = f"FIREWALL: {ip} {action} on {hostname}"
+    Event.createFromDict(None, dict(
+        hostname=hostname,
+        reporter_ip=ip,
+        description=title,
+        details=title,
+        category="firewall",
+        level=6,
+        metadata=metadata
+    ))
+
+
 def getBlockedIPs():
     return sudoCMD([settings.BLOCK_IP_CMD, "list"])
 
 
 def getBlockedHosts():
     blocked = []
     if not os.path.exists("/etc/hosts.deny"):
@@ -823,14 +894,23 @@
                 continue
             if line.startswith("ALL:"):
                 line = line.split("L:")[1]
             blocked.append(line.strip())
     return blocked
 
 
+def toInteger(value):
+    if isinstance(value, str):
+        if "." in value:
+            return int(float(value))
+    if isinstance(value, list):
+        return value
+    return int(value)
+
+
 def toString(value):
     if isinstance(value, bytes):
         value = value.decode()
     elif isinstance(value, bytearray):
         value = value.decode("utf-8")
     elif isinstance(value, (int, float)):
         value = str(value)
@@ -857,16 +937,18 @@
 
 def hexToByteArray(value):
     return bytearray.fromhex(value)
 
 def hexToString(value):
     return bytes.fromhex(value).decode('utf-8')
 
-def toBase64(value):
-    return base64.b64encode(value)
+def toBase64(value, as_str=True):
+    if as_str:
+        return toString(base64.b64encode(toBytes(value)))
+    return base64.b64encode(toBytes(value))
 
 def fromBase64(value):
     return toString(base64.b64decode(value))
 
 def removeNonAscii(input_str):
     """Remove all non-ASCII characters from the input string."""
     return ''.join(char for char in input_str if 0 <= ord(char) < 128)
```

### Comparing `django_restit-4.2.9/rest/jwtoken.py` & `django_restit-4.2.90/rest/jwtoken.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 from objict import objict
 import time
 import uuid
 from rest import settings
 
 
 JWT_EXP_1_DAY = 86400
+JWT_EXP_2_DAY = 172800
 JWT_EXP_7_DAY = 604800
 JWT_EXP_30_MIN = 1800
+JWT_EXP_15_MIN = 900
 JWT_KEY = settings.SECRET_KEY
-JWT_EXP_DEFAULT = settings.get("JWT_EXP_DEFAULT", JWT_EXP_30_MIN)
+JWT_EXPIRES = settings.get("JWT_EXPIRES", JWT_EXP_30_MIN)
+JWT_REFRESH_EXPIRES = settings.get("JWT_REFRESH_EXPIRES", JWT_EXP_2_DAY)
 
 
 class JWToken():
-    def __init__(self, token=None, user_id=None, key=JWT_KEY, device_id=None, alg="HS256", access_expires_in=JWT_EXP_DEFAULT, refresh_expires_in=JWT_EXP_7_DAY):
+    def __init__(self, token=None, user_id=None, key=JWT_KEY, 
+                 device_id=None, alg="HS256", access_expires_in=JWT_EXPIRES,
+                 refresh_expires_in=JWT_REFRESH_EXPIRES):
         # takes full JWT token header.payload.signature
         self.token = token
         self.key = key
         self.alg = alg
         self.access_expires_in = access_expires_in
         self.refresh_expires_in = refresh_expires_in
         self._is_valid = None
```

### Comparing `django_restit-4.2.9/rest/log.py` & `django_restit-4.2.90/rest/log.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/mail.py` & `django_restit-4.2.90/rest/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from email.mime.application import MIMEApplication
 
 try:
     from inlinestyler.utils import inline_css
 except Exception:
     inline_css = None
 
+try:
+    from premailer import transform as premailer
+except Exception:
+    premailer = None
+
 from django.template.loader import render_to_string
 from django.template import TemplateDoesNotExist
 
 import metrics
 from rest import settings
 from rest.uberdict import UberDict
 from rest.middleware import get_request
@@ -71,15 +76,17 @@
 
     if template and context:
         if isinstance(context, dict):
             context['settings'] = settings
         if template[-4:] not in ["html", ".txt"]:
             template += ".html"
         body = render_to_string(template, context)
-        if inline_css:
+        if premailer:
+            body = premailer(body)
+        elif inline_css:
             body = inline_css(body)
     return body
 
 
 def createMultiPartMessage(sender, recipients, subject, text, html, attachments, replyto):
     """
     Creates a MIME multipart message object.
@@ -199,15 +206,17 @@
         pass
     if len(toaddrs) == 0:
         EMAIL_LOGGER.error("Sending email to no one: {}".format(name), context)
         return
 
     try:
         html_content = render_to_string(name + ".html", context)
-        if inline_css:
+        if premailer:
+            html_content = premailer(html_content)
+        elif inline_css:
             html_content = inline_css(html_content)
     except TemplateDoesNotExist:
         html_content = None
         pass
 
     text_content = ""
     try:
```

### Comparing `django_restit-4.2.9/rest/mailman.py` & `django_restit-4.2.90/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/cors.py` & `django_restit-4.2.90/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/db_router.py` & `django_restit-4.2.90/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/jwt.py` & `django_restit-4.2.90/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/request.py` & `django_restit-4.2.90/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/session.py` & `django_restit-4.2.90/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/middleware/session_store.py` & `django_restit-4.2.90/rest/middleware/session_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     def __init__(self, session_key=None):
         super(SessionStore, self).__init__(session_key)
         self._exists = None
 
     def load(self):
         try:
             sk = self._get_or_create_session_key()
-            session_data = redis.get(self.get_stored_key(sk))
+            session_data = redis.get(self.get_stored_key(sk)).decode()
             return self.decode(session_data)
         except Exception:
             pass
-        self._session_key = None
+        # self._session_key = None
         return {}
 
     def exists(self, session_key=None):
         if session_key is None:
             session_key = self.session_key
         if session_key is None:
             return False
@@ -33,16 +33,17 @@
         self.modified = True
         return
 
     def save(self, must_create=False):
         if self.session_key is None:
             return self.create()
         data = self.encode(self._get_session(no_load=must_create))
+        sk = self._get_or_create_session_key()
         redis.set(
-            self.get_stored_key(self._get_or_create_session_key()),
+            self.get_stored_key(sk),
             data,
             self.get_expiry_age())
         return True
 
     def delete(self, session_key=None):
         if session_key is None:
             session_key = self.session_key
```

### Comparing `django_restit-4.2.9/rest/models/base.py` & `django_restit-4.2.90/rest/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,24 @@
     def restGetModel(app_name, model_name):
         return apps.get_model(app_name, model_name)
 
     @staticmethod
     def getModel(app_name, model_name):
         return apps.get_model(app_name, model_name)
 
+    @staticmethod
+    def getModelInstance(app_name, model_name, **kwargs):
+        Model = apps.get_model(app_name, model_name)
+        return Model.objects.filter(**kwargs).last()
+
+    @staticmethod
+    def createModelInstance(app_name, model_name, **kwargs):
+        Model = apps.get_model(app_name, model_name)
+        return Model(**kwargs)
+
     def restGetGenericModel(self, field):
         # called by the rest module to magically parse
         # a component that is marked genericr elation in a graph
         if not hasattr(self, field):
             rh.log_print("model has no field: {0}".format(field))
             return None
 
@@ -380,14 +390,16 @@
         if not hasattr(self, "_changed__"):
             self._changed__ = objict()
 
         if fieldname.startswith("_"):
             return
         if not hasattr(self, "_field_names__"):
             self._field_names__ = [f.name for f in self._meta.get_fields()]
+        # if not hasattr(self, "_related_field_names__"):
+        #     self._related_field_names__ = self.get_related_name_fields()
         # print "saving field: {0} = {1}".format(fieldname, value)
         if fieldname in RestModel.__RestMeta__.NO_SAVE_FIELDS:
             return
         if has_no_fields and fieldname in self.RestMeta.NO_SAVE_FIELDS:
             return
         if has_fields and fieldname not in self.RestMeta.SAVE_FIELDS:
             return
@@ -465,16 +477,14 @@
                             else:
                                 value = False
                 except Exception:
                     return
             if hasattr(self, fieldname) and getattr(self, fieldname) != value:
                 self._changed__[fieldname] = getattr(self, fieldname)
             setattr(self, fieldname, value)
-        # else:
-        #   print "does not have field: {0}".format(fieldname)
 
     def saveFromRequest(self, request, **kwargs):
         if "files" not in kwargs:
             kwargs["files"] = request.FILES
         return self.checkPermsAndSave(request, request.DATA, **kwargs)
 
     def hasFieldChanged(self, fieldname):
@@ -709,40 +719,46 @@
             return
         if not self.id:
             self.save()
         request.setLogModel(model, self.id)
 
     def checkIsOwner(self, member):
         owner_field = getattr(self.RestMeta, "OWNER_FIELD", None)
+        if owner_field is None:
+            owner_field = getattr(self.RestMeta, "VIEW_PERMS_MEMBER_FIELD", None)
         if owner_field is not None:
-            return member is getattr(self, owner_field, None)
+            owner = getattr(self, owner_field, None)
+            return member == owner
         return False
 
     def on_rest_pre_get(self, request):
         pass
 
     def on_rest_can_get(self, request):
         perms = getattr(self.RestMeta, "VIEW_PERMS", None)
         if perms:
             if "owner" in perms and self.checkIsOwner(request.member):
                 return True
             # we need to check if this user has permission
             group_field = getattr(self.RestMeta, "GROUP_FIELD", "group")
             status, error, code = rh.requestHasPerms(request, perms, getattr(self, group_field, None))
             if not status:
-                raise re.PermissionDeniedException(error, code)
+                raise re.PermissionDeniedException(error + " getting", code)
         return True
 
     def on_rest_get(self, request):
         # check view permissions
         if not self.on_rest_can_get(request):
             return self.restStatus(request, False, error="permission denied", error_code=402)
         self.on_rest_pre_get(request)
         return self.restGet(request)
 
+    def onRestCanDelete(self, request=None, data=None, extended=None):
+        self.onRestCheckSavePerms(request, data, extended)
+
     def onRestCanSave(self, request=None, data=None, extended=None):
         self.onRestCheckSavePerms(request, data, extended)
 
     def onRestCheckSavePerms(self, request=None, data=None, extended=None):
         if request is None:
             request = self.getActiveRequest()
             if request is None:
@@ -754,15 +770,17 @@
             perms = getattr(self.RestMeta, "CREATE_PERMS", perms)
         if perms:
             if "owner" in perms and self.checkIsOwner(request.member):
                 return True
             # we need to check if this user has permission
             group_field = getattr(self.RestMeta, "GROUP_FIELD", "group")
             # rh.log_error(F"group field={group_field}")
-            if self.id is None:
+            if group_field == "self" and self.pk:
+                group = self
+            elif self.id is None:
                 group = None
                 if extended is not None:
                     group = extended.get(group_field, None)
                 if group is None:
                     if data is not None:
                         group = data.get(group_field, None)
                 if group is None:
@@ -779,16 +797,16 @@
                         break
             else:
                 group = getattr(self, group_field, None)
             status, error, code = rh.requestHasPerms(request, perms, group)
             if not status:
                 if self.id is None and code == 402:
                     code = 435
-                    rh.log_error(F"onRestCheckSavePerms: {self.__class__.__name__} {request.member} {group} permission denied: status={status}, error={error}, code={code}", perms)
-                raise re.PermissionDeniedException(error, code)
+                    rh.log_error(F"permission denied onRestCheckSavePerms: {self.__class__.__name__}\ngroup: {group}\nstatus={status}, error={error}, code={code}\nperms:", perms)
+                raise re.PermissionDeniedException(error + " saving", code)
 
     def on_rest_post(self, request):
         self.checkPermsAndSave(request, request.DATA)
         status_only = request.DATA.get("status_only", False, field_type=bool)
         if status_only:
             return self.restStatus(request, True)
         graph = request.DATA.get("graph", "default")
@@ -802,28 +820,30 @@
 
     def on_rest_saved(self, request, is_new=False):
         pass
 
     def on_rest_delete(self, request, force=False):
         can_delete = getattr(self.RestMeta, "CAN_DELETE", False)
         if not can_delete:
-            return self.restStatus(request, False, error="deletion not allowed via rest for this model.")
+            raise re.PermissionDeniedException(f"deletion not allowed for {self.get_class_name()}", 438)
         if not force:
-            self.onRestCanSave(request)
+            self.onRestCanDelete(request)
         self.on_rest_deleted(request)
         self.delete()
         RestModel._setupGraphHelpers()
         return self.restStatus(request, True)
 
     def on_rest_deleted(self, request):
         self.auditLog(F"deleted {self.pk}", "deleted", level=8)
         if request and request.member:
             request.member.auditLog(F"deleted {self.get_class_name(True)}:{self.pk}", "deleted", level=8)
 
     def auditLog(self, message, action="log", path=None, level=0, group=None, method=None):
+        if group is None and hasattr(self, "group"):
+            group = self.group
         PLOG = self.getModel("auditlog", "PersistentLog")
         component = self.get_class_name(True)
         PLOG.log(message=message, action=action, path=path, level=level, method=method, component=component, pkey=self.id, group=group)
 
     @classmethod
     def restList(cls, request, qset, graph=None, totals=None, return_httpresponse=True):
         RestModel._setupGraphHelpers()
@@ -868,31 +888,35 @@
         if not graph and request:
             graph = request.DATA.get("graph", "default")
         elif not graph:
             graph = "default"
         return_response = not as_dict
         return GRAPH_HELPERS.restGet(request, self, return_httpresponse=return_response, **self.getGraph(graph))
 
-    def toDict(self, graph=None):
+    def toDict(self, graph=None, schema=None):
         RestModel._setupGraphHelpers()
-        return self.restGet(None, graph=graph, as_dict=True)
+        if schema is None:
+            return self.restGet(None, graph=graph, as_dict=True)
+        return GRAPH_HELPERS.restGet(None, self, return_httpresponse=False, **schema)
 
     def __str__(self):
         return f"<{self.get_class_name(True)}>"
 
     @classmethod
     def on_rest_list_filter(cls, request, qset=None):
         # override on do any pre filters
         return cls.on_rest_list_perms(request, qset)
 
     @classmethod
     def on_rest_filter_member_field(cls, request, qset):
         member_field = getattr(cls.RestMeta, "VIEW_PERMS_MEMBER_FIELD", None)
         if member_field is None:
             # this would be permission denied
+            member_field = getattr(cls.RestMeta, "OWNER_FIELD", None)
+        if member_field is None:
             if EXCEPTION_ON_LIST_PERM_DENIED:
                 raise re.PermissionDeniedException(f"user does not have permission to access {cls.get_class_name()}")
             return cls.objects.none()
         # rh.log_error(dict(**{member_field: request.member}))
         return qset.filter(**{member_field: request.member})
 
     @classmethod
@@ -927,15 +951,16 @@
     def on_rest_filter_children(cls, request, qset=None):
         # rh.log_error("filter by group?")
         group_field = getattr(cls.RestMeta, "GROUP_FIELD", "group")
         if group_field is None or ("__" not in group_field and not cls.has_model_field_name(group_field)):
             return qset
         parent_kinds = getattr(cls.RestMeta, "LIST_PARENT_KINDS", ["org"])
         if request.DATA.get("child_groups") or request.group.kind in parent_kinds:
-            ids = request.group.getAllChildrenIds()
+            list_depth = getattr(cls.RestMeta, "LIST_CHILD_DEPTH", 0)
+            ids = request.group.getAllChildrenIds(depth=list_depth)
             ids.append(request.group.id)
             # to avoid future filtering issues remove group
             request.group = None
             request.DATA.remove(group_field)
             if group_field != "group":
                 # rh.debug("removing group field!!")
                 request.DATA.remove("group")
@@ -1035,50 +1060,72 @@
 
     @classmethod
     def getRestFormatFields(cls, format, graph=None):
         fields = []
         if hasattr(cls.RestMeta, "FORMATS"):
             fields = cls.RestMeta.FORMATS.get(format, fields)
         if len(fields) == 0:
+            if format == "json":
+                g = cls.getGraph("default")
+                if "fields" in g:
+                    return g["fields"]
             no_show_fields = RestModel.__RestMeta__.NO_SHOW_FIELDS
             if hasattr(cls.RestMeta, "NO_SHOW_FIELDS"):
                 no_show_fields = cls.RestMeta.NO_SHOW_FIELDS
             for f in cls._meta.fields:
                 if not f.name.endswith("_ptr"):
                     if f.name not in no_show_fields:
                         fields.append(f.name)
         return fields
 
     @classmethod
     def on_rest_list_format(cls, request, format, qset):
         if format in ["summary", "summary_only"]:
             return cls.on_rest_list_summary(request, qset)
-        fields = cls.getRestFormatFields(format)
+        fields = None
+        if format == "json":
+            g = cls.getGraph(request.DATA.get("graph", "download"))
+            if g and "fields" in g:
+                fields = g["fields"]
+        if fields is None:
+            fields = cls.getRestFormatFields(format)
         if fields or format == "json":
             name = request.DATA.get("format_filename", None)
             format_size = request.DATA.get("format_size", 10000)
+            localize = request.DATA.get("localize", None, field_type=dict)
             if name is None:
-                name = "{}.{}".format(cls.get_class_name(), format)
+                ext = format
+                if "_" in ext:
+                    ext = ext[:ext.find("_")]
+                name = "{}.{}".format(cls.get_class_name(), ext)
             # print "csv size: {}".format(qset.count())
             sort = request.DATA.get("sort", getattr(cls.RestMeta, "DEFAULT_SORT", "-id"))
             sort_args = cls.getSortArgs(sort)
             if sort_args:
                 try:
                     qset = qset.order_by(*sort_args)
                 except Exception:
                     pass
             cls._boundRest()
-            if format == "json":
-                return GRAPH_HELPERS.views.restJSON(request, qset, fields, name, format_size)
-            elif format == "csv":
-                return GRAPH_HELPERS.views.restCSV(request, qset, fields, name, format_size)
+            if format.startswith("json"):
+                return GRAPH_HELPERS.views.restJSON(
+                    request, qset, fields, 
+                    name, format_size, localize=localize)
+            elif format.startswith("csv"):
+                return GRAPH_HELPERS.views.restCSV(
+                    request, qset, fields,
+                    name, format_size, localize=localize)
             elif format == "xlsx":
-                return GRAPH_HELPERS.views.restExcel(request, qset, fields, name, format_size)
+                return GRAPH_HELPERS.views.restExcel(
+                    request, qset, fields,
+                    name, format_size, localize=localize)
             elif format == "flat":
-                return GRAPH_HELPERS.views.restFlat(request, qset, fields, name, format_size)
+                return GRAPH_HELPERS.views.restFlat(
+                    request, qset, fields,
+                    name, format_size, localize=localize)
     
     @classmethod
     def on_rest_list_summary(cls, request, qset):
         cls._boundRest()
         summary_info = getattr(cls.RestMeta, "SUMMARY_FIELDS", {})
         output = objict()
         output.count = qset.count()
@@ -1116,14 +1163,22 @@
                 elif action == "avg":
                     output[lbl] = rh.getAverage(act_qset, field)
                 elif action == "max":
                     output[lbl] = rh.getMax(act_qset, field)
         return GRAPH_HELPERS.restGet(request, output)
 
     @classmethod
+    def getRestBatchCreateFilter(cls, item, exclude=["id", "pk", "created", "modified"], include=None):
+        if isinstance(include, list):
+            return {key: item[key] for key in include if key in item}
+        # ignore related fields
+        rfs = cls.get_related_name_fields()
+        return {key: item[key] for key in item if key not in exclude and cls.hasField(key) and key not in rfs}
+
+    @classmethod
     def on_rest_batch(cls, request, action):
         # this method is called when rest_batch='somme action'
         cls._boundRest()
         batch_ids = request.DATA.getlist("batch_ids", [])
         batch_id_field = request.DATA.get("batch_id_field", "pk")
         q = {}
         if batch_ids:
@@ -1143,28 +1198,47 @@
             qset = cls.rw_objects().filter(**q)
             update_fields = request.DATA.get(["batch_data", "batch_update"])
             if not isinstance(update_fields, dict):
                 return GRAPH_HELPERS.restStatus(request, False, error="batch_update should be key/values")
             count = qset.update(**update_fields)
             return GRAPH_HELPERS.restStatus(request, True, error="updated {} items".format(count))
         elif action == "create":
-            batch_data = request.DATA.getlist("batch_data", [])
-            items = []
-            for item in batch_data:
-                try:
-                    obj = cls.ro_objects().filter(**item).last()
-                    if not obj:
-                        obj.checkPermsAndSave(request, item)
-                    items.append(obj)
-                except Exception:
-                    pass
-            return GRAPH_HELPERS.restList(request, items)
+            cls.on_rest_batch_create(request)
         return GRAPH_HELPERS.restStatus(request, False, error="not implemented")
 
     @classmethod
+    def on_rest_batch_create(cls, request):
+        batch_data = request.DATA.get("batch_data")
+        if isinstance(batch_data, str):
+            batch_data = objict.fromJSON(batch_data)
+        if isinstance(batch_data, dict):
+            if "data" in batch_data:
+                batch_data = batch_data["data"]
+        items = []
+        for item in batch_data:
+            obj = cls.createFromBatch(item)
+            if obj:
+                items.append(obj)
+        return GRAPH_HELPERS.restList(request, items)
+
+    @classmethod
+    def createFromBatch(cls, item, request=None):
+        obj = None
+        try:
+            rh.debug("batch item", item)
+            item_filter = cls.getRestBatchCreateFilter(item)
+            rh.debug("batch filters", item_filter)
+            obj = cls.ro_objects().filter(**item_filter).last()
+            if obj is None:
+                obj = cls.createFromDict(request, item)
+        except Exception:
+            rh.log_exception(item)
+        return obj
+
+    @classmethod
     def on_rest_create(cls, request, pk=None):
         # permissions are checked in the save routine
         can_create = getattr(cls.RestMeta, "CAN_CREATE", True)
         if not can_create:
             return GRAPH_HELPERS.restStatus(request, False, error="creation not allowed via rest for this model.")
 
         if hasattr(cls.RestMeta, "KEY_TO_FIELD_MAP"):
@@ -1445,15 +1519,15 @@
                 value = getattr(request, fn, None)
                 if value is not None:
                     q[rfields[fn]] = value
             if bool(q):
                 qset = qset.filter(**q)
         return qset
 
-    ALLOWED_QUERY_OPERATORS = ["gt", "gte", "lt", "lte", "contains", "icontains", "in", "startswith", "endswith"]
+    ALLOWED_QUERY_OPERATORS = ["isnull", "gt", "gte", "lt", "lte", "contains", "icontains", "in", "startswith", "endswith"]
 
     @classmethod
     def queryFromRequest(cls, request, qset):
         """
         This will look at the query request and allow for basic filtering.
 
         QUERY_FIELDS_SPECIAL can be used to allow mappings of certain queries:
@@ -1484,14 +1558,15 @@
             __icontains
             __in
 
         values can also be prefixed with special operators
             <field_name>=<operator>:value
         """
         q = {}
+        exq = {}
         field_names = cls.rest_getQueryFields()
         query_keys = request.DATA.keys()
         special_keys = getattr(cls.RestMeta, "QUERY_FIELDS_SPECIAL", {})
         cls.on_rest_set_query_defaults(request)
         # rh.debug("queryFromRequest.key", query_keys, special_keys, field_names)
         for key in query_keys:
             # remove the key from defaults
@@ -1555,24 +1630,32 @@
                 oper, value = value[2:].split(':')
                 if oper not in RestModel.ALLOWED_QUERY_OPERATORS:
                     continue
                 key = "{}__{}".format(key, oper)
             if oper == "in":
                 if isinstance(value, str) and ',' in value:
                     value = [a.strip() for a in value.split(',')]
+            elif oper == "isnull":
+                value = value in [True, "true", 1, "1"]
             elif oper is None and value in ["null", "None"]:
                 key = "{}__isnull".format(key)
                 value = True
             ft = cls.get_field_type(fn)
             if ft == "DateTimeField":
                 value = rh.parseDateTime(value)
+            elif ft == "IntegerField":
+                value = rh.toInteger(value)
             q[key] = value
         if bool(q):
-            # rh.debug("queryFromRequest", q, "default_filters:", request.default_rest_filters)
-            qset = qset.filter(**q)
+            exq = {key[:-4]: q[key] for key in q if key.endswith("__ne")}
+            q = {key: q[key] for key in q if not key.endswith("__ne")}
+            if bool(exq):
+                qset = qset.exclude(**exq)
+            if bool(q):
+                qset = qset.filter(**q)
         return qset
 
     @classmethod
     def createFromRequest(cls, request, **kwargs):
         obj = cls()
         return obj.saveFromRequest(request, files=request.FILES, __is_new=True, **kwargs)
 
@@ -1628,14 +1711,22 @@
 
     @classmethod
     def get_foreign_fields(cls):
         '''returns the internal field type'''
         return [field.name for field in cls._meta.fields if field.get_internal_type() == "ForeignKey"]
 
     @classmethod
+    def get_related_name_fields(cls):
+        return [f.related_name for f in cls._meta.related_objects]
+
+    @classmethod
+    def get_model_field_names(cls):
+        return [f.name for f in cls._meta.get_fields()]
+
+    @classmethod
     def get_fk_model(cls, fieldname):
         '''returns None if not foreignkey, otherswise the relevant model'''
         try:
             field = cls._meta.get_field(fieldname)
             return field.related_model
         except Exception:
             return None
```

### Comparing `django_restit-4.2.9/rest/models/cacher.py` & `django_restit-4.2.90/rest/models/cacher.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/models/metadata.py` & `django_restit-4.2.90/rest/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 if isinstance(item, dict):
                     output.update(item)
             values = output
 
         if not isinstance(values, dict):
             raise Exception("invalid metadata: {}".format(values))
 
-        for key, value in list(values.items()):
+        for key, value in values.items():
             cat = None
             if "." in key:
                 cat, key = key.split('.')
             self.setProperty(key, value, cat, request=request)
 
     def metadata(self):
         return self.getProperties()
@@ -226,32 +226,37 @@
         on_change = None
         if not using:
             using = getattr(self.RestMeta, "DATABASE", using)
         if not request:
             request = rh.getActiveRequest()
         self.__initFieldProps()
 
+        if "." in key:
+            category, key = key.split('.')
+            
         if isinstance(value, dict):
-            return self.setProperties(value, key)
+            if category is None:
+                return self.setProperties(value, key)
         username = "root"
         if request and request.member:
             username = request.member.username
         prop = None
 
-        if "." in key:
-            category, key = key.split('.')
         if category:
             # delete any keys with this category name
             full_key = "{}.{}".format(category, key)
             # this deletes anything with the key that matches the category
             # this works because the category is stored not in key but category field
             # rh.log_print("deleting key={}".format(category))
             self.properties.filter(key=category).delete()
             if category == "secrets":
                 encrypted = True
+            elif category == "permissions":
+                if value == 0:
+                    value = None
         else:
             full_key = key
 
         value_len = 0
         if encrypted:
             value_len = len(value)
             value = ENCRYPTER.encrypt(value)
@@ -264,15 +269,16 @@
         has_changed = False
         prop = self.properties.filter(category=category, key=key).last()
         old_value = None
         if prop:
             # existing property we need to make sure we delete
             old_value = prop.getValue()
             if value is None or value == "":
-                prop.delete()
+                # we need to delete all, if there was dups for some reason
+                self.properties.filter(category=category, key=key).delete()
                 has_changed = True
             else:
                 has_changed = check_value != prop.value
                 if not has_changed:
                     return
                 prop.setValue(value)
                 if encrypted and value_len:
```

### Comparing `django_restit-4.2.9/rest/regexes.yaml` & `django_restit-4.2.90/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/requestex.py` & `django_restit-4.2.90/rest/requestex.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             request.DATA.parse()
 
     def __init__(self, request=None, data=None):
         self.__data = data
         self.is_logged = False
         self.request = request
         self.ua_info = None
+        self.url_params = None
         if not self.request:
             return
         self.request.is_sns = False
         self.parsePARAMS()
         self.request.is_json = self.isJSON()
 
     def parse(self):
@@ -74,18 +75,23 @@
         except Exception:
             pass
         return data
 
     def parsePARAMS(self):
         if self.request.method == "POST":
             data = self.request.POST
+            if self.request.GET:
+                self.url_params = UberDict.fromdict(self.normalizeData(self.request.GET))
         elif self.request.method == "GET":
             data = self.request.GET
         elif self.request.method == "DELETE":
-            data = dict()
+            if self.request.body:
+                data = QueryDict(self.request.body)
+            else:
+                data = objict()
         elif self.request.method == "PUT":
             if self.request.content_type == "application/json":
                 data = UberDict.fromJSON(self.request.body, ignore_errors=True)
             else:
                 if hasattr(self.request, '_post'):
                     del self.request._post
                     del self.request._files
@@ -97,14 +103,16 @@
                     self.request.META['REQUEST_METHOD'] = 'POST'
                     self.request._load_post_and_files()
                     self.request.META['REQUEST_METHOD'] = 'PUT'
                 data = self.request.POST
         else:
             data = dict()
         self.params = UberDict.fromdict(self.normalizeData(data))
+        if self.url_params:
+            self.params.extend(self.url_params)
 
     def parseJSON(self):
         try:
             self.__data = UberDict.fromJSON(self.request.body, ignore_errors=False)
             if isinstance(self.__data, list):
                 self.__data = UberDict(data=self.__data)
             self.__data.update(self.params)
@@ -248,17 +256,14 @@
         if self.__data:
             return str(self.__data)
         return ""
 
     def log(self, include_headers=True):
         if not self.is_logged:
             self.is_logged = True
-            track = self.get("track", None)
-            cardnumber = self.get(["cardnumber", "pan"], None)
-            password = self.get("password", None)
             sanitized = UberDict.fromdict(self.toDict())
             if include_headers:
                 headers = {}
                 for key in self.request.META:
                     if key in ["HTTP_AUTHORIZATION"]:
                         value = self.request.META.get(key)
                         if value and len(value) > 6:
@@ -292,14 +297,16 @@
                 if value and value != NOTFOUND:
                     if type(value) in [dict, list]:
                         return value
                     elif "," in value:
                         return value.split(',')
                     return [value]
                 return []
+            elif field_type is dict and isinstance(value, str):
+                return objict.fromJSON(value)
         except Exception:
             return default
         return value
 
     def getList(self, key, default=None, split_spaces=False):
         return self.getlist(key, default, split_spaces)
 
@@ -478,11 +485,15 @@
                 return default
             return self.getStrictType(data, field_type, default)
         return data
 
     def getUserAgent(self):
         return self.request.META.get('HTTP_USER_AGENT', '')
 
+    def getUserAgentPlatform(self):
+        ua = self.getUserAgentInfo()
+        return f"{ua.user_agent.family} on {ua.os.family}"
+
     def getUserAgentInfo(self):
         if self.ua_info is None:
             self.ua_info = ua.parse(self.request.META.get('HTTP_USER_AGENT', ''))
         return self.ua_info
```

### Comparing `django_restit-4.2.9/rest/rpc.py` & `django_restit-4.2.90/rest/rpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,33 +19,42 @@
 except Exception:
     print("no psutil")
 
 
 URL_PREFIX = ""
 
 SOFTWARE_VERSIONS = getattr(settings, 'SOFTWARE_VERSIONS', None)
+ALLOW_PUBLIC_SYS_INFO = getattr(settings, 'ALLOW_PUBLIC_SYS_INFO', False)
 # SOFTWARE_VERSIONS_ACTUAL = {}
 
 
 @url(r'^version$')
 def on_get_version(request):
-    return views.restStatus(request, True, {"data": version.VERSION})
+    return views.restStatus(request, True, {"data": version.VERSION, "ip": request.ip})
 
 
 @url(r'^versions$')
 def on_get_version(request):
     from rest import __version__ as restit_version
     versions = dict(
         project=version.VERSION,
         restit=restit_version)
     if request.DATA.get("detailed") and SOFTWARE_VERSIONS:
         getVersions(versions)
     return views.restStatus(request, True, {"data": versions})
 
 
+@url('test/session')
+def on_get_my_session(request):
+    echo = request.DATA.get("echo", None)
+    if echo:
+        request.session["echo"] = echo
+    return views.restReturn(request, dict(echo=request.session.get("echo", "not set")))
+
+
 @url(r'^joke$')
 def on_get_joke(request):
     return views.restGet(request, {"joke": joke.getRandomJoke()})
 
 
 def getTcpEstablishedCount():
     return len(getTcpEstablished())
@@ -58,14 +67,16 @@
         if c.status == "ESTABLISHED":
             established.append(c)
     return established
 
 
 @url(r'^system/info$')
 def on_get_system_info(request):
+    if not ALLOW_PUBLIC_SYS_INFO and not request.user.is_authenticated:
+        return views.restPermissionDenied(request, "system info is not public", 565)
     mem = psutil.virtual_memory()
     disk = psutil.disk_usage('/')
     net = psutil.net_io_counters()
 
     out = {
         "time": time.time(),
         "datetime": str(datetime.now()),
@@ -74,46 +85,55 @@
             "system": platform.system(),
             "version": platform.version(),
             "hostname": platform.node(),
             "release": platform.release(),
             "processor": platform.processor(),
             "machine": platform.machine()
         },
-        "cpu": {
-            "count": psutil.cpu_count(),
-            "freq": psutil.cpu_freq(),
-        },
         "boot_time": psutil.boot_time(),
         "cpu_load": psutil.cpu_percent(),
         "cpus_load": psutil.cpu_percent(percpu=True),
         "memory": {
             "total": mem.total,
             "used": mem.used,
             "available": mem.available,
             "percent": mem.percent
         },
         "disk": {
             "total": disk.total,
             "used": disk.used,
             "free": disk.free,
             "percent": disk.percent
-        },
-        "network": {
+        }, 
+        "users": psutil.users()
+    }
+
+    try:
+        out["cpu"] = {
+            "count": psutil.cpu_count(),
+            "freq": psutil.cpu_freq(),
+        }
+    except Exception:
+        pass
+
+    try:
+        out["network"] = {
             "tcp_cons": getTcpEstablishedCount(),
             "bytes_sent": net.bytes_sent,
             "bytes_recv": net.bytes_recv,
             "packets_sent": net.packets_sent,
             "packets_recv": net.packets_recv,
             "errin": net.errin,
             "errout": net.errout,
             "dropin": net.dropin,
             "dropout": net.dropout
-        },
-        "users": psutil.users()
-    }
+        }
+    except Exception:
+        pass
+
     if request.DATA.get("versions") and SOFTWARE_VERSIONS:
         out["versions"] = getVersions()
     if request.DATA.get("blocked"):
         out["blocked"] = helpers.getBlockedHosts()
     return views.restGet(request, out)
```

### Comparing `django_restit-4.2.9/rest/search.py` & `django_restit-4.2.90/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/serializers/collection.py` & `django_restit-4.2.90/rest/serializers/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     if cache is None and isinstance(qset, QuerySet):
         cache = dict()
     output = {"size": size, "start": start}
     if sort and isinstance(qset, QuerySet):
         qset, sort_args = sort_list(qset, sort)
         output["sort"] = sort_args
 
-    qset = qset[start:start+size+1]
+    qset = qset[start:start+size]
     if not fields:
         fields = ms.get_fields(qset)
     if settings.REST_SELECT_RELATED:
         # this should improve speed greatly for lookups
         foreign_fields = ms.get_select_related_fields(qset.model, fields)
         if foreign_fields:
             qset = qset.select_related(*foreign_fields)
```

### Comparing `django_restit-4.2.9/rest/serializers/csv.py` & `django_restit-4.2.90/rest/serializers/csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from objict import objict
 from io import StringIO
 from django.http import StreamingHttpResponse
 import csv
+from rest import helpers as rh
+from . import localizers
 
 
-def flattenObject(obj, field_names):
+def flattenObject(obj, field_names, localize=None):
     row = []
     for f in field_names:
         d = ""
         if "__" in f:
             f = f.replace("__", ".")
         if "." in f:
             # we could use obj.getFieldValue
@@ -28,41 +30,56 @@
                 d1 = getattr(obj, f1, None)
                 if d1 is not None:
                     if not hasattr(d1, f2):
                         if hasattr(d1, "first"):
                             d1 = d1.first()
                     d = getattr(d1, f2, "")
                     if callable(d):
-                        d = d()                
+                        d = d()               
         else:
             d = getattr(obj, f, "n/a")
             if callable(d):
                 d = d()
         if d is None:
             d = "n/a"
         elif hasattr(d, "pk"):
             d = d.pk
-        row.append(str(d))
+        if localize and f in localize:
+            rh.debug("localize....", localize[f])
+            d = localizeValue(d, localize[f])
+        else:
+            d = str(d)
+        row.append(d)
     return row
 
 
+def localizeValue(value, localizer_name, extra=None):
+    if "|" in localizer_name:
+        localizer_name, extra = localizer_name.split("|")
+    localizer = getattr(localizers, localizer_name, None)
+    if localizer is not None:
+        return localizer(value, extra)
+    return value
+
+
 def extractFieldNames(fields):
     header = []
     field_names = []
     for f in fields:
         if type(f) is tuple:
             r, f = f
             field_names.append(r)
         else:
             field_names.append(f)
         header.append(f)
     return header, field_names
 
 
-def generateCSV(qset, fields, name, header_cols=None, values_list=False, output=None, stream=False):
+def generateCSV(qset, fields, name, header_cols=None,
+                values_list=False, output=None, stream=False, localize=None):
     a = objict()
     a.name = name
     a.file = StringIO()
     if output:
         a.file = output
     csvwriter = csv.writer(a.file)
     header, field_names = extractFieldNames(fields)
@@ -70,37 +87,38 @@
         header = header_cols
     csvwriter.writerow(header)
     if values_list:
         for row in qset.values_list(*field_names):
             row = [str(x) for x in row]
             csvwriter.writerow(row)
     else:
+        rh.debug("localize.", localize)
         for obj in qset:
-            csvwriter.writerow(flattenObject(obj, field_names))
+            csvwriter.writerow(flattenObject(obj, field_names, localize))
     if hasattr(a.file, "getvalue"):
         a.data = a.file.getvalue()
     a.mimetype = "text/csv"
     return a
 
 
-def iterCsvObject(items, writer, header, field_names):
+def iterCsvObject(items, writer, header, field_names, localize=None):
     yield writer.writerow(header)
     for item in items:
-        yield writer.writerow(flattenObject(item, field_names))
+        yield writer.writerow(flattenObject(item, field_names, localize))
 
 
-def generateCSVStream(qset, fields, name):
+def generateCSVStream(qset, fields, name, localize=None):
     import csv
     # check if we support stream mode
     header, field_names = extractFieldNames(fields)
     # rows = qset.values_list(*fields)
     pseudo_buffer = EchoWriter()
     writer = csv.writer(pseudo_buffer)
     return StreamingHttpResponse(
-        iterCsvObject(qset, writer, header, field_names))
+        iterCsvObject(qset, writer, header, field_names, localize=localize))
 
 
 class EchoWriter(object):
     """An object that implements just the write method of the file-like
     interface.
     """
     def writeline(self, value):
```

### Comparing `django_restit-4.2.9/rest/serializers/excel.py` & `django_restit-4.2.90/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/serializers/json.py` & `django_restit-4.2.90/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/serializers/legacy.py` & `django_restit-4.2.90/rest/serializers/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1533,15 +1533,15 @@
     try:
         oldid = obj.pk
         obj.delete()
         return restResult(request, {'status': True, 'id': oldid}, accept_list=accept_list)
     except:
         return restResult(request, {'status': False, 'error': 'Cannot delete'}, accept_list=accept_list)
 
-def restPermissionDenied(request, error="permission denied", error_code=403, status=200,
+def restPermissionDenied(request, error="permission denied", error_code=403, status=403,
                          component=None, component_id=None):
     return restResult(request, dict(status=False, error=error, error_code=error_code), status=status)
 
 def restNotFound(request):
     return restStatus(request, False, error="resource not found", error_code=404)
 
 def restOK(request):
```

### Comparing `django_restit-4.2.9/rest/serializers/model.py` & `django_restit-4.2.90/rest/serializers/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/serializers/profiler.py` & `django_restit-4.2.90/rest/serializers/profiler.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/serializers/response.py` & `django_restit-4.2.90/rest/serializers/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from auditlog.models import PersistentLog
 from . import model as ms
 from . import collection as cs
 from . import json as js
 from . import csv
 from . import excel
 # from . import profiler
+STATUS_ON_PERM_DENIED = settings.get("STATUS_ON_PERM_DENIED", 403)
 
 
 def restStatus(request, status, data={}, **kwargs):
     if isinstance(data, str):
         if status:
             data = dict(message=data)
         else:
@@ -90,15 +91,15 @@
                 PersistentLog.log(sanatized, 0, request, "rest", action="response")
             else:
                 PersistentLog.log(resp, 0, request, "rest", action="response")
         else:
             PersistentLog.log(resp, 0, request, "rest", action="response")
 
 
-def restPermissionDenied(request, error="permission denied", error_code=403, status=200,
+def restPermissionDenied(request, error="permission denied", error_code=403, status=STATUS_ON_PERM_DENIED,
                          component=None, component_id=None):
     # from rest import helpers as rh
     # rh.log_error(error)
     return restResult(request, dict(status=False, error=error, error_code=error_code), status=status)
 
 
 def restNotFound(request):
@@ -109,47 +110,55 @@
     return restStatus(request, True)
 
 
 def restError(request, error, error_code=None):
     return restStatus(request, False, error=error, error_code=error_code)
 
 
-def restJSON(request, qset, fields, name, size=10000):
+def restJSON(request, qset, fields, name, size=10000, localize=None):
     if fields:
         data = cs.to_list(qset, fields=fields, size=size)
     else:
         data = cs.serialize(qset, request.DATA.get("graph"), size=size)
     response = HttpResponse(js.prettyJSON(data), content_type="application/json")
     response['Content-Disposition'] = 'attachment; filename="{0}"'.format(name)
     return response
 
 
-def restFlat(request, qset, fields, name, size=10000, header_cols=None):
+def restFlat(request, qset, fields, name, size=10000, header_cols=None, localize=None):
     return HttpResponse(js.prettyJSON(list(qset.values_list(*fields))), content_type="application/json", status=200)
 
 
-def restCSV(request, qset, fields, name, size=10000, header_cols=None):
+def restCSV(request, qset, fields, name, size=10000, header_cols=None, localize=None):
     if size > 1200 and qset.count() > 1200:
         # large data set lets stream
         qset = qset[:size]
-        response = csv.generateCSVStream(qset, fields, name)
+        response = csv.generateCSVStream(qset, fields, name, localize=localize)
         response['Cache-Control'] = 'no-cache'
         response['Content-Disposition'] = f'attachment; filename="{name}"'
     else:
         response = HttpResponse(content_type='text/csv')
         response['Content-Disposition'] = f'attachment; filename="{name}"'
         qset = qset[:size]
-        csv.generateCSV(qset, fields, name, output=response, header_cols=header_cols)
+        csv.generateCSV(qset, fields, name, output=response, header_cols=header_cols, localize=localize)
     return response
 
 
-def restExcel(request, qset, fields, name, size=10000, **kwargs):
+def restExcel(request, qset, fields, name, size=10000, localize=None, **kwargs):
     return excel.qsetToExcel(request, qset[:size], fields, name)
 
 
+def restHTML(request, html_content=None, template=None, context=None, status=200):
+    if not html_content and not template:
+        return HttpResponse("<html><body><h1>Hello, World!</h1><p>Welcome to my site.</p></body></html>")
+    if template:
+        return render(request, template, context, status=status)
+    return HttpResponse(html_content, status=status)
+
+
 def parse_accept_list(request):
     if request and hasattr(request, "DATA") and request.DATA.get('_type', None) is not None:
         accept_list = [request.DATA.get('_type')]
     elif request and 'HTTP_ACCEPT' in request.META:
         accept_list = request.META["HTTP_ACCEPT"].split(',')
     elif request and 'HTTP_ACCEPT_ENCODING' in request.META:
         accept_list = request.META["HTTP_ACCEPT_ENCODING"].split(',')
```

### Comparing `django_restit-4.2.9/rest/serializers/util.py` & `django_restit-4.2.90/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/settings_helper.py` & `django_restit-4.2.90/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/ssl_check.py` & `django_restit-4.2.90/rest/ssl_check.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/static/lib/jquery.js` & `django_restit-4.2.90/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/templates/email/error.html` & `django_restit-4.2.90/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/templates/rest_docs.html` & `django_restit-4.2.90/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/templates/rest_html.html` & `django_restit-4.2.90/rest/templates/rest_html.html`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 		font-family: arial;
 		color: white;
 		box-shadow: 0 0 4px rgb(0, 0, 0);
 		padding: 10px;
 		font-size: 18px;
 		height: 100%;
 		background: #333333;
+		background: linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(50,43,56,1) 35%, rgba(56,54,85,1) 100%);
+
 	}
 
 	footer {
 		font-size:  12px;
 		position: absolute;
 /*		width:  20em;*/
 		padding:  15px;
@@ -247,15 +249,14 @@
 		    </select>
 		    <button type="submit" class="btn btn-submit">SUBMIT</button>
 		    </form>
 		    {% else %}
 		    <div class="path">
 		        {{path}}
 		    </div>
-		    <h4 class='subtitle'>request:</h4>
 		    <div class="request">
 		        <pre>{{req_out}}</pre>
 		    </div>
 		    {% endif %}
 
 		    <footer>
 		    	<div class="disclaimer">
```

#### html2text {}

```diff
@@ -5,14 +5,13 @@
 PK    [{{pk}}              ]
 {{k}} [{{v}}               ] X
       + ADD NEW PARAM
 ===============================================================================
 [One of: GET/POST/DELETE]SUBMIT
 {% else %}
 {{path}}
-****** rreeqquueesstt:: ******
 {{req_out}}
 {% endif %}
 {% autoescape off %} {{disclaimer}} {% endautoescape %}
 {{version}}
 ****** rreessppoonnssee:: ******
 {{ output }}
```

### Comparing `django_restit-4.2.9/rest/ua.py` & `django_restit-4.2.90/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/uberdict.py` & `django_restit-4.2.90/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/url_docs.py` & `django_restit-4.2.90/rest/url_docs.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/rest/urls.py` & `django_restit-4.2.90/rest/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def load_app(app, root_module=None):
     module = None
     try:
         module = loadModule(f"{app}.rpc")
         if module is None:
-            module = loadModule(f"{app}.rurl")
+            module = loadModule(f"{app}.rurls")
             if module is None:
                 module = loadModule(f"{app}.rapi")
     except ImportError as err:
         print("**** failed to load {0}.rpc! ****".format(app))
         print("**** missing dependencies ****")
         print("**** {0} ****".format(err))
     except SyntaxError:
```

### Comparing `django_restit-4.2.9/rest/views.py` & `django_restit-4.2.90/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/sessionlog/migrations/0001_initial.py` & `django_restit-4.2.90/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/sessionlog/models.py` & `django_restit-4.2.90/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/README.md` & `django_restit-4.2.90/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/migrations/0001_initial.py` & `django_restit-4.2.90/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/models.py` & `django_restit-4.2.90/taskqueue/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     (TASK_STATE_STARTED, 'started'),
     (TASK_STATE_RETRY, 'retry_later'),
     (TASK_STATE_COMPLETED, 'completed'),
     (TASK_STATE_FAILED, 'failed'),
     (TASK_STATE_CANCELED, 'canceled')
 ]
 
+TQ_RETRY_BACKOFF_FACTOR = settings.get("TQ_RETRY_BACKOFF_FACTOR", 2)
+TQ_RETRY_ATTEMPTS = settings.get("TQ_RETRY_ATTEMPTS", 5)
+TQ_RETRY_DELAY = settings.get("TQ_RETRY_DELAY", 60)
+
 def getAppHandler(app_name, fname):
     try:
         # module = __import__(app_name + '.tq', globals(), locals(), ['*'], 0)
         module = importlib.import_module(app_name + '.tq')
 
     except ImportError as err:
         return None
@@ -139,14 +143,20 @@
     def current_runtime(self):
         if self.state in [10, -1]:
             return self.runtime
         if not self.started_at:
             return self.runtime
         return (datetime.now() - self.started_at).total_seconds()
 
+    @property
+    def max_attempts(self):
+        if self.data:
+            return self.data.get("retry_max_attempts", TQ_RETRY_ATTEMPTS)
+        return TQ_RETRY_ATTEMPTS
+
     def set_action(self, value):
         if value == "retry_now":
             self.retry_now()
         elif value == "cancel":
             request = self.getActiveRequest()
             self.reason = "cancel request by {}".format(request.member.username)
             self.cancel(request.DATA.get("reason", "canceled by {}".format(request.member.username)))
@@ -154,14 +164,28 @@
     # def auditlog(self, action, message, request=None, path=None, component="taskqueue.Task"):
     #     # message, level=0, request=None, component=None, pkey=None, action=None, group=None, path=None, method=None
     #     # PersistentLog.log(message=message, level=1, action=action, request=request, component=component, pkey=self.pk, path=path, method=self.fname)
     #     raise Exception("auditlog called but is not supported")
 
     def log(self, text, kind="info"):
         TaskLog.Log(self, text, kind=kind)
+        if self.data and ((self.data.log_component and self.data.log_pk) or self.data.log_tid):
+            PLOG = self.getModel("auditlog", "PersistentLog")
+            level = 0
+            if kind == "exception":
+                level = 21
+            elif kind == "error":
+                level = 17
+            PLOG.log(message=text, action=f"taskqueue_{kind}", 
+                     level=level,
+                     method=self.fname, path=self.model,
+                     tid=self.data.log_tid,
+                     component=self.data.log_component,
+                     pkey=self.data.log_pk,
+                     group=self.data.group_id)
 
     def log_exception(self, text, kind="exception"):
         self.log(str(text), kind=kind)
         self.log(traceback.format_exc(), "exception")
 
     def started(self):
         self.state = TASK_STATE_STARTED
@@ -169,15 +193,25 @@
         self._started = time.time()
         self.attempts += 1
         self.save()
 
     def retry_later(self, reason=None, from_now_secs=None):
         if reason:
             self.reason = reason
-        if from_now_secs:
+        if from_now_secs == -1:
+            # allow backoff retry
+            if self.data:
+                bof = self.data.get("retry_bof", TQ_RETRY_BACKOFF_FACTOR)
+                delay = self.data.get("retry_delay", TQ_RETRY_DELAY)
+            else:
+                bof = TQ_RETRY_BACKOFF_FACTOR
+                delay = TQ_RETRY_DELAY
+            attempts = self.attempts - 1
+            from_now_secs = delay * (bof ** attempts)
+        if from_now_secs is not None:
             # this will not run the task again until after this time has been hit
             self.scheduled_for = datetime.now() + timedelta(seconds=from_now_secs)
         self.state = TASK_STATE_RETRY
         self.cancel_requested = False
         self.save()
 
     def retry_now(self):
@@ -188,44 +222,55 @@
 
     def completed(self):
         self.completed_at = datetime.now()
         self.runtime = int(time.time() - self._started)
         self.state = TASK_STATE_COMPLETED
         self.save()
 
-    def failed(self, reason=None):
+    def failed(self, reason=None, category="taskqueue_errors"):
         if reason and len(reason) > 250:
             reason = reason[:250]
         self.reason = reason
         self.state = TASK_STATE_FAILED
-        self.notifyError()
+        self.notifyError(category=category, reason=reason)
         self.save()
 
-    def notifyError(self, kind="Failure"):
-        subject = "TaskQueue - {}".format(kind)
-        handler = "unknown bg_handler"
-        if self.data:
-            handler = self.data.get("bg_handler")
-        msg = "{}:{}<br>\n{}".format(self.model, handler, self.reason)
-        # sms_msg = "{}\n{}".format(subject, msg)
-        # Member.notifyWithPermission("taskqueue_alerts", subject, msg, sms_msg=sms_msg)
+    def notifyError(self, category="taskqueue_errors", reason=None):
+        handler = f"{self.model}.{self.fname}"
+        subject = f"TaskQueue - {handler}"
+        if reason is None:
+            reason = self.reason
+
+        msg = f"{handler}<br>\n{reason}"
         metadata = {
             "server": settings.get("HOSTNAME", "unknown"),
             "task": self.pk,
-            "reason": self.reason,
-            "kind": kind,
+            "reason": reason,
             "app": self.model,
             "fname": self.fname,
             "channel": self.channel,
+            "attempts": self.attempts,
             "handler": handler
         }
+
+        if self.data:
+            if self.data.url:
+                metadata["url"] = self.data.url
+                from urllib.parse import urlparse
+                purl = urlparse(self.data.url)
+                metadata["host"] = purl.netloc
+                msg = f"{msg}<br>\n{self.data.url}"
+            if self.data.log_component:
+                metadata["component"] = self.data.log_component
+            if self.data.log_pk:
+                metadata["component_id"] = self.data.log_pk
         try:
             import incident
             incident.event_now(
-                "taskqueue_errors", description=subject, details=msg, 
+                category, description=subject, details=msg, 
                 level=3, metadata=metadata)
         except Exception as err:
             self.log(str(err), kind="error")
 
     def cancel(self, reason=None):
         self.cancel_requested = True
         self.save()
@@ -250,72 +295,101 @@
         app, mname = self.model.split('.')
         model = self.restGetModel(app, mname)
         if not model:
             return None
         return getattr(model, self.fname, None)
 
     @classmethod
-    def WebRequest(cls, url, data, fname="POST", stale_after_seconds=0):
+    def WebRequest(cls, url, data, fname="POST", stale_after_seconds=0,
+                   log_component=None, log_pk=None, log_tid=None):
         tdata = nobjict()
         tdata.url = url
         tdata.data = data
+        if log_component is not None:
+            tdata.log_component = log_component
+            tdata.log_pk = log_pk
+        if log_tid is not None:
+            tdata.log_tid = log_tid
         task = cls(channel="tq_hook", model="tq_web_request", fname=fname, data=tdata)
         if stale_after_seconds:
             task.stale_after = datetime.now() + timedelta(seconds=stale_after_seconds)
         task.save()
         task.publish()
         return task
 
     @classmethod
-    def EmailRequest(cls, address, data, filename=None, subject=None):
+    def EmailRequest(cls, address, data, filename=None, subject=None,
+                     log_component=None, log_pk=None, log_tid=None):
         tdata = nobjict()
         tdata.address = address
         tdata.filename = filename
         tdata.subject = subject
         tdata.data = data
+        if log_component is not None:
+            tdata.log_component = log_component
+            tdata.log_pk = log_pk
+        if log_tid is not None:
+            tdata.log_tid = log_tid
         task = cls(channel="tq_hook", model="tq_email_request", data=tdata)
         task.save()
         task.publish()
         return task
 
     @classmethod
-    def SMSRequest(cls, phone, data):
+    def SMSRequest(cls, phone, data, log_component=None, log_pk=None, log_tid=None):
         tdata = nobjict()
         tdata.phone = phone
         tdata.data = data
+        if log_component is not None:
+            tdata.log_component = log_component
+            tdata.log_pk = log_pk
+        if log_tid is not None:
+            tdata.log_tid = log_tid
         task = cls(channel="tq_hook", model="tq_sms_request", data=tdata)
         task.save()
         task.publish()
         return task
 
     @classmethod
-    def SFTPRequest(cls, host, data, filename, username, password):
+    def SFTPRequest(cls, host, data, filename, username, password,
+                    log_component=None, log_pk=None, log_tid=None):
         tdata = nobjict()
         tdata.host = host
         tdata.filename = filename
         # TODO this should be more secure!
         # TODO support ssh keys?
         tdata.username = username
         tdata.password = password
         tdata.data = data
+        if log_component is not None:
+            tdata.log_component = log_component
+            tdata.log_pk = log_pk
+        if log_tid is not None:
+            tdata.log_tid = log_tid
         task = cls(channel="tq_hook", model="tq_sftp_request", data=tdata)
         task.save()
         task.publish()
         return task
     
     @classmethod
-    def S3Request(cls, bucket, data, folder, aws, secret, filename, when):
+    def S3Request(cls, bucket, data, folder, aws, secret, filename, when,
+                  log_component=None, log_pk=None, log_tid=None):
         tdata = nobjict()
         tdata.bucket = bucket
         tdata.filename = filename
         tdata.data = data
         tdata.folder = folder
         tdata.aws = aws
         tdata.secret = secret
         tdata.when = str(when)
+        if log_component is not None:
+            tdata.log_component = log_component
+            tdata.log_pk = log_pk
+        if log_tid is not None:
+            tdata.log_tid = log_tid
         task = cls(channel="tq_hook", model="tq_s3_request", data=tdata)
         task.save()
         task.publish()
         return task
 
     @classmethod
     def PublishModelTask(cls, model_name, fname, data, stale_after_seconds=0, channel="tq_model_handler", scheduled_for=scheduled_for):
```

### Comparing `django_restit-4.2.9/taskqueue/periodic.py` & `django_restit-4.2.90/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/rpc.py` & `django_restit-4.2.90/taskqueue/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 @rd.perm_required("manage_staff")
 def rest_on_test(request):
     tq.Task.PublishTest(request.DATA.get("test_count", 1, field_type=int), request.DATA.get("sleep_time", 10.0, field_type=float))
     return rv.restStatus(request, True)
 
 
 @rd.url(r'^task/status$')
+@rd.login_required
 def rest_on_task_status(request):
     out = UberDict()
     last_completed = tq.Task.objects.filter(state=tq.TASK_STATE_COMPLETED).last()
     if last_completed:
         out.last_completed = last_completed.completed_at
     last_scheduled = tq.Task.objects.all().last()
     if last_scheduled:
@@ -105,14 +106,15 @@
         backlog=Count('state', filter=Q(state=tq.TASK_STATE_SCHEDULED)))
     status["total"] = qset.count()
     out.update(status)
     return rv.restGet(request, out)
 
 
 @rd.urlGET('workers')
+@rd.login_required
 def rest_on_runners(request):
     workers = tq.TaskWorkerClient.GET_ONLINE()
     if request.DATA.get("graph") == "detailed":
         output = []
         for r in workers:
             stats = tq.TaskWorkerClient.GET_STATS(r)
             stats.id = r
@@ -120,14 +122,15 @@
         workers = output
     return rv.restReturn(request, dict(data=workers))
 
 
 # write a django query to 
 
 @rd.url(r'^task/stats$')
+@rd.login_required
 def rest_on_stats(request):
     now = datetime.now() 
     when = now - timedelta(days=request.DATA.get("days", 7, field_type=int))
     qset = tq.Task.objects.filter(
         created__gte=when)
     reports = list(
         qset
```

### Comparing `django_restit-4.2.9/taskqueue/tq.py` & `django_restit-4.2.90/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/transports/email.py` & `django_restit-4.2.90/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/transports/s3.py` & `django_restit-4.2.90/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/transports/sftp.py` & `django_restit-4.2.90/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/taskqueue/worker.py` & `django_restit-4.2.90/taskqueue/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                 del self._scheduled_tasks[task.id]
                 self._pending_count -= 1
                 self.updateCounts()
         except Exception:
             pass
 
     def processBacklog(self):
-        tasks = Task.objects.filter(state__in=[0,1,2])
+        tasks = Task.objects.filter(state__in=[0, 1, 2])
         for task in tasks:
             if task.channel in self.subscribe_to:
                 if task.cancel_requested:
                     self.logger.info("task has cancel request {}".format(task.id))
                     task.state = -2
                     if not task.reason:
                         task.reason = "task canceled"
@@ -190,42 +190,37 @@
                     continue
                 self.logger.debug("resubmitting job {}".format(task.id))
                 self.addTask(task)
             else:
                 self.logger.warning("ignore job {}:{}".format(task.id, task.channel))
 
     def _on_webrequest(self, task):
-        # self.logger.debug("starting web request to: {}".format(task.data.url))
-        # we need to copy the data and remove the url
-        if task.fname.upper() == "GET":
-            resp = http.GET(task)
-        else:
-            resp = http.POST(task)
-        if resp:
+        if http.REQUEST(task):
             task.completed()
-        elif task.state == 1:
-            # slowly backoff retries
-            if task.attempts >= 5:
-                task.failed("max attempts")
-            task.retry_later(from_now_secs=task.attempts * task.attempts * 60)
+        elif task.attempts < task.max_attempts:
+            # -1 will auto calculate retry with back off
+            # lets report the issue
+            task.notifyError(reason=task.reason)
+            task.retry_later(from_now_secs=-1)
+        else:
+            task.failed("max attempts")
 
     def _on_hookrequest(self, task):
-        # we need to copy the data and remove the url
         if task.model == "tq_email_request":
             resp = email.SEND(task)
         elif task.model == "tq_sms_request":
             resp = sms.SEND(task)
         elif task.model == "tq_sftp_request":
             resp = sftp.SEND(task)
         elif task.model == "tq_s3_request":
             resp = s3.UPLOAD(task)
         if resp:
             task.completed()
-        elif task.state == 1:
-            task.retry_later(from_now_secs=task.attempts * 60)
+        elif task.attempts < task.max_attempts:
+            task.retry_later(from_now_secs=-1)
         else:
             task.failed()
 
     def on_host_event(self, event):
         action = event.data.action
         if action == "ping":
             redis.publish(
```

### Comparing `django_restit-4.2.9/telephony/migrations/0001_initial.py` & `django_restit-4.2.90/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/telephony/models.py` & `django_restit-4.2.90/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/telephony/rpc.py` & `django_restit-4.2.90/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/migrations/0001_initial.py` & `django_restit-4.2.90/wiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/models/faq.py` & `django_restit-4.2.90/wiki/models/faq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/models/page.py` & `django_restit-4.2.90/wiki/models/page.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/models/revision.py` & `django_restit-4.2.90/wiki/models/revision.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/highlight.py` & `django_restit-4.2.90/wiki/renderers/mistune/highlight.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/math.py` & `django_restit-4.2.90/wiki/renderers/mistune/math.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/media.py` & `django_restit-4.2.90/wiki/renderers/mistune/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/meta.py` & `django_restit-4.2.90/wiki/renderers/mistune/meta.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/task_list.py` & `django_restit-4.2.90/wiki/renderers/mistune/task_list.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/renderers/mistune/toc.py` & `django_restit-4.2.90/wiki/renderers/mistune/toc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/wiki/rpc/wiki.py` & `django_restit-4.2.90/wiki/rpc/wiki.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/README.md` & `django_restit-4.2.90/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/connection.py` & `django_restit-4.2.90/ws4redis/connection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/exceptions.py` & `django_restit-4.2.90/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/redis.py` & `django_restit-4.2.90/ws4redis/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from redis import ConnectionPool, StrictRedis
 
 from ws4redis import settings
+import time
 
 from rest import UberDict
 from rest.log import getLogger
 logger = getLogger("async", filename="async.log")
 
 REDIS_CON_POOL = None
 
@@ -21,15 +22,15 @@
         if isinstance(value, str):
             if value != settings.WS4REDIS_HEARTBEAT:
                 return bytes(value, 'utf-8')
         elif isinstance(value, list):
             if len(value) >= 2 and value[0] == b'message':
                 return value[2]
         elif isinstance(value, dict):
-            if not isinstance(value, UberDict):
+            if not hasattr(value, "toJSON"):
                 value = UberDict(value)
             return bytes(value.toJSON(as_string=True), 'utf-8')
         elif isinstance(value, bytes):
             return value
         return None
 
 
@@ -80,15 +81,15 @@
     def channelToKey(self, channel, facility="events", pk=None, prefix=settings.WS4REDIS_PREFIX):
         if not pk:
             key = F'{prefix}:{channel}:{facility}'
         else:
             key = F'{prefix}:{channel}:{pk}:{facility}'
         return key
 
-    def subscribe(self, channel, facility, pk=None, prefix=settings.WS4REDIS_PREFIX):
+    def subscribe(self, channel, facility="events", pk=None, prefix=settings.WS4REDIS_PREFIX):
         if self.pubsub is None:
             self.pubsub = self.connection.pubsub()
         key = self.channelToKey(channel, facility, pk, prefix)
         if key not in self.subscriptions:
             if settings.WS4REDIS_LOG_DEBUG:
                 logger.info(F"subscribing to: {key}")
             self.subscriptions.append(key)
@@ -124,14 +125,23 @@
             if self.only_one:
                 self.connection.srem(F"{name}:online", pk)
             else:
                 count = self.connection.hincrby(F"{name}:online:connections", pk, -1)
                 if count == 0:
                     self.connection.srem(F"{name}:online", pk)
 
+    def waitForMessage(self, muid=None, timeout=55):
+        timeout_at = time.time() + timeout
+        while time.time() < timeout_at:
+            message = self.pubsub.get_message()
+            if message is not None and message.get("type") == "message":
+                return UberDict.fromJSON(message.get("data"))
+            time.sleep(1.0)
+        return None
+
     def get_file_descriptor(self):
         """
         Returns the file descriptor used for passing to the select call when listening
         on the message queue.
         """
         if self.pubsub.connection:
             return self.pubsub.connection._sock.fileno()
@@ -143,7 +153,13 @@
         memory sap when Redis Output Buffer and Output Lists build when websockets are abandoned.
         """
         self.unpublishModelOnline()
         if self.pubsub and self.pubsub.subscribed:
             self.pubsub.unsubscribe()
             self.pubsub.reset()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.release()
+        return False
```

### Comparing `django_restit-4.2.9/ws4redis/servers/base.py` & `django_restit-4.2.90/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/servers/django.py` & `django_restit-4.2.90/ws4redis/servers/django.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,79 @@
 #-*- coding: utf-8 -*-
 import six
 import base64
 import select
 from hashlib import sha1
 from wsgiref import util
+from django.core.handlers import wsgi as django_wsgi
 from django.core.wsgi import get_wsgi_application
 from django.core.servers.basehttp import WSGIServer, WSGIRequestHandler, ServerHandler
 
 from django.conf import settings
 from django.core.management.commands import runserver
 import socketserver
 from django.utils.encoding import force_str
 from ws4redis.websocket import WebSocket
 from ws4redis.servers.base import WebsocketServerBase, HandshakeError, UpgradeRequiredError
 
+from io import IOBase
+
+
 from rest.log import getLogger
 logger = getLogger("async", filename="async.log")
 
 util._hoppish = {}.__contains__
 
 
+class LimitedStreamPatched(IOBase):
+    """
+    Wrap another stream to disallow reading it past a number of bytes.
+
+    Based on the implementation from werkzeug.wsgi.LimitedStream
+    See https://github.com/pallets/werkzeug/blob/dbf78f67/src/werkzeug/wsgi.py#L828
+    """
+
+    def __init__(self, stream, limit):
+        self.stream = stream
+        self._read = stream.read
+        self._readline = stream.readline
+        self._pos = 0
+        self.limit = limit
+
+    def read(self, size=-1, /):
+        _pos = self._pos
+        limit = self.limit
+        if _pos >= limit:
+            return b""
+        if size == -1 or size is None:
+            size = limit - _pos
+        else:
+            size = min(size, limit - _pos)
+        data = self._read(size)
+        self._pos += len(data)
+        return data
+
+    def readline(self, size=-1, /):
+        _pos = self._pos
+        limit = self.limit
+        if _pos >= limit:
+            return b""
+        if size == -1 or size is None:
+            size = limit - _pos
+        else:
+            size = min(size, limit - _pos)
+        line = self._readline(size)
+        self._pos += len(line)
+        return line
+
+
+def patchLimitedStream():
+    django_wsgi.LimitedStream = LimitedStreamPatched
+
+
 class WSGIRequestHandlerRunServer(WSGIRequestHandler):
     def handle(self):
         self.raw_requestline = self.rfile.readline(65537)
         if len(self.raw_requestline) > 65536:
             self.requestline = ''
             self.request_version = ''
             self.command = ''
@@ -77,40 +127,47 @@
         ]
         if environ.get('HTTP_SEC_WEBSOCKET_PROTOCOL') is not None:
             headers.append(('Sec-WebSocket-Protocol', environ.get('HTTP_SEC_WEBSOCKET_PROTOCOL')))
 
         logger.debug('WebSocket request accepted, switching protocols')
         start_response(force_str('101 Switching Protocols'), headers)
         six.get_method_self(start_response).finish_content()
-        return WebSocket(environ['wsgi.input'].stream)
+        winput = environ['wsgi.input']
+        if not hasattr(winput, "stream"):
+            # hack to get the stream back in later DJANGO
+            winput.stream = winput._read.__self__
+        return WebSocket(winput.stream)
 
     def select(self, rlist, wlist, xlist, timeout=None):
         return select.select(rlist, wlist, xlist, timeout)
 
 
-def run(addr, port, wsgi_handler, ipv6=False, threading=False, server_cls=None):
+def run(addr, port, wsgi_handler, ipv6=False, threading=False, server_cls=None, **kwargs):
     """
     Function to monkey patch the internal Django command: manage.py runserver
     """
     server_address = (addr, port)
     logger.info('Websocket support is enabled', server_address)
     if not threading:
         raise Exception("Django's Websocket server must run with threading enabled")
     httpd_cls = type('WSGIServer', (socketserver.ThreadingMixIn, WSGIServer), {'daemon_threads': True})
     httpd = httpd_cls(server_address, WSGIRequestHandlerRunServer, ipv6=ipv6)
     httpd.set_app(wsgi_handler)
     httpd.serve_forever()
 
 
+patchLimitedStream()
+
 runserver.run = run
 
 _django_app = get_wsgi_application()
 _websocket_app = WebsocketRunServer()
 _websocket_url = getattr(settings, 'WEBSOCKET_URL')
 
 
 def application(environ, start_response):
     if _websocket_url and environ.get('PATH_INFO').startswith(_websocket_url):
+        logger.info("environ", environ)
         return _websocket_app(environ, start_response)
     return _django_app(environ, start_response)
```

### Comparing `django_restit-4.2.9/ws4redis/servers/uwsgi.py` & `django_restit-4.2.90/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/settings.py` & `django_restit-4.2.90/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/utf8validator.py` & `django_restit-4.2.90/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/ws4redis/websocket.py` & `django_restit-4.2.90/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.2.9/PKG-INFO` & `django_restit-4.2.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.2.9
+Version: 4.2.90
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.26.160,<2.0.0)
 Requires-Dist: django
 Requires-Dist: django-redis-cache (>=3.0.1,<4.0.0)
 Requires-Dist: django-redis-sessions (>=0.6.2,<0.7.0)
+Requires-Dist: fido2
 Requires-Dist: gevent (>=23.7.0,<24.0.0)
 Requires-Dist: hashids (>=1.3.1,<2.0.0)
 Requires-Dist: inlinestyler
 Requires-Dist: mistune
 Requires-Dist: phonenumbers
 Requires-Dist: pillow
 Requires-Dist: psutil
```

