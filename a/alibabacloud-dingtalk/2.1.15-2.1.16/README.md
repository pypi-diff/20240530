# Comparing `tmp/alibabacloud_dingtalk-2.1.15.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.15.tar", last modified: Fri May 24 10:50:54 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.16.tar", last modified: Wed May 29 09:36:02 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.1.15.tar` & `alibabacloud_dingtalk-2.1.16.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/
--rw-r--r--   0 root         (0) root         (0)   135727 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2660 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10220 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15463 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24694 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    36448 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25446 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24061 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51732 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    55896 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23886 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69836 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171793 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19974 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25370 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30918 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47170 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31278 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27481 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114212 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   145728 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248134 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413198 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53158 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    64382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306758 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   657929 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98018 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   115937 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11616 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9944 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   192336 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   407651 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34906 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42901 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89960 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   237978 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10504 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88282 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124205 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185660 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   224275 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71002 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   126248 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408970 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   425714 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25686 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43876 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40206 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44858 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21312 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30666 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23500 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10844 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14576 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10302 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315868 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   638801 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5774 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37328 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46524 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494304 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515207 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134392 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   150282 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15793 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70120 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56029 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79025 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81667 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   313048 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322887 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260012 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385294 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23366 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168538 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   200479 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672294 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   877133 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89270 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113792 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104118 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121491 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22157 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20888 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   482712 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   556456 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191008 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   320947 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21190 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28705 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42854 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53610 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5681 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12390 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98153 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137888 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18299 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84750 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124476 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   199981 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   276424 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   396886 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413672 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28815 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33507 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107508 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91958 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   824822 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   952300 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75114 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157606 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78582 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108065 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110044 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133326 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18311 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23610 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181489 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173547 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62895 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53887 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71486 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63136 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42982 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44105 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107234 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167406 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93818 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123438 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    59069 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35028 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68771 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   319400 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   411401 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21787 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44394 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164608 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172757 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115490 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105876 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129210 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167086 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47742 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46647 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   460426 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   551312 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38532 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26120 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54274 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95239 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226462 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   350226 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70068 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95695 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16918 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28519 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84018 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152968 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16445 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22383 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16528 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17427 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91210 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135827 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92596 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111817 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40437 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40791 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10216 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79864 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129013 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6226 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8459 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50430 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43338 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   262706 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   457246 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3678 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   590500 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   761218 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4472 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14334 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/
+-rw-r--r--   0 root         (0) root         (0)   137273 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15463 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24694 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    36448 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25446 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24061 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51732 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    55896 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23886 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69836 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171793 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25370 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30918 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47170 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31278 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27481 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114212 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   145728 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248134 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413198 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53158 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    64382 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306758 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   657929 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98018 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   115937 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   192336 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   407651 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34906 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42901 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89960 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   237978 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93622 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133896 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185660 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   226061 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71002 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   126248 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   408970 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   425714 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43876 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40206 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44858 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21312 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30666 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23500 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   324430 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   646132 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37328 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46524 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494304 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515207 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134392 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   150282 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15793 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70120 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56029 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79025 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81667 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   313048 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322887 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260012 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385294 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23366 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168538 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   200479 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672294 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   877133 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89270 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113792 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104118 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121491 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22157 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20888 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   482712 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   556456 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191008 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   320947 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21190 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28705 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42854 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53610 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98153 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137888 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18299 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84750 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124476 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   199981 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   276424 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   396886 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413672 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28815 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33507 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107508 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91958 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   824822 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   952300 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75114 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157606 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78582 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108065 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   110044 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133326 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18311 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23610 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181489 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173547 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62895 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53887 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71486 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63136 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42982 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44105 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107234 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167406 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93818 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123438 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69184 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    59069 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35028 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68771 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319400 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   411401 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21787 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44394 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164608 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172757 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115490 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105876 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129210 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167086 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47742 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46647 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460426 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   551312 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38532 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26120 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54274 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95239 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226462 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   350226 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70068 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95695 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16918 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28519 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84018 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152968 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22383 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91210 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   136189 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92596 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111817 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40437 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40791 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10216 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79864 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129013 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8459 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50430 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43338 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   262706 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   457246 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   590492 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   761218 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14334 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-29 09:36:02.000000 alibabacloud_dingtalk-2.1.16/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-29 09:36:01.000000 alibabacloud_dingtalk-2.1.16/setup.py
```

### Comparing `alibabacloud_dingtalk-2.1.15/ChangeLog.md` & `alibabacloud_dingtalk-2.1.16/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-24 Version: 2.1.15
+- Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-05-23 Version: 2.1.14
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-22 Version: 2.1.13
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-18 Version: 2.1.12
```

### Comparing `alibabacloud_dingtalk-2.1.15/LICENSE` & `alibabacloud_dingtalk-2.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/PKG-INFO` & `alibabacloud_dingtalk-2.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.1.15
+Version: 2.1.16
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.15/README-CN.md` & `alibabacloud_dingtalk-2.1.16/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/README.md` & `alibabacloud_dingtalk-2.1.16/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/agoal_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1897,14 +1897,144 @@
         @param request: ListProgressByIdsRequest
         @return: ListProgressByIdsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkchengfeng__1__0_models.ListProgressByIdsHeaders()
         return await self.list_progress_by_ids_with_options_async(request, headers, runtime)
 
+    def list_sls_log_with_options(
+        self,
+        request: dingtalkchengfeng__1__0_models.ListSlsLogRequest,
+        headers: dingtalkchengfeng__1__0_models.ListSlsLogHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkchengfeng__1__0_models.ListSlsLogResponse:
+        """
+        @summary 获取组织下的日志数据
+        
+        @param request: ListSlsLogRequest
+        @param headers: ListSlsLogHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSlsLogResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.app_code):
+            query['appCode'] = request.app_code
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListSlsLog',
+            version='chengfeng_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/chengfeng/organizations/slsLogDatas',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkchengfeng__1__0_models.ListSlsLogResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def list_sls_log_with_options_async(
+        self,
+        request: dingtalkchengfeng__1__0_models.ListSlsLogRequest,
+        headers: dingtalkchengfeng__1__0_models.ListSlsLogHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkchengfeng__1__0_models.ListSlsLogResponse:
+        """
+        @summary 获取组织下的日志数据
+        
+        @param request: ListSlsLogRequest
+        @param headers: ListSlsLogHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSlsLogResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.app_code):
+            query['appCode'] = request.app_code
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListSlsLog',
+            version='chengfeng_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/chengfeng/organizations/slsLogDatas',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkchengfeng__1__0_models.ListSlsLogResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def list_sls_log(
+        self,
+        request: dingtalkchengfeng__1__0_models.ListSlsLogRequest,
+    ) -> dingtalkchengfeng__1__0_models.ListSlsLogResponse:
+        """
+        @summary 获取组织下的日志数据
+        
+        @param request: ListSlsLogRequest
+        @return: ListSlsLogResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkchengfeng__1__0_models.ListSlsLogHeaders()
+        return self.list_sls_log_with_options(request, headers, runtime)
+
+    async def list_sls_log_async(
+        self,
+        request: dingtalkchengfeng__1__0_models.ListSlsLogRequest,
+    ) -> dingtalkchengfeng__1__0_models.ListSlsLogResponse:
+        """
+        @summary 获取组织下的日志数据
+        
+        @param request: ListSlsLogRequest
+        @return: ListSlsLogResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkchengfeng__1__0_models.ListSlsLogHeaders()
+        return await self.list_sls_log_with_options_async(request, headers, runtime)
+
     def page_list_objective_progress_with_options(
         self,
         request: dingtalkchengfeng__1__0_models.PageListObjectiveProgressRequest,
         headers: dingtalkchengfeng__1__0_models.PageListObjectiveProgressHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkchengfeng__1__0_models.PageListObjectiveProgressResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -899,14 +899,98 @@
             temp_model = OpenUserDTO()
             self.modifier = temp_model.from_map(m['modifier'])
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         return self
 
 
+class SlsLogResp(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        entity: str = None,
+        header: str = None,
+        id: str = None,
+        info: str = None,
+        operator: str = None,
+        tenant: str = None,
+        tenant_id: str = None,
+        time: int = None,
+    ):
+        # This parameter is required.
+        self.action = action
+        # This parameter is required.
+        self.entity = entity
+        # This parameter is required.
+        self.header = header
+        # This parameter is required.
+        self.id = id
+        # This parameter is required.
+        self.info = info
+        # This parameter is required.
+        self.operator = operator
+        # This parameter is required.
+        self.tenant = tenant
+        # This parameter is required.
+        self.tenant_id = tenant_id
+        # This parameter is required.
+        self.time = time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['action'] = self.action
+        if self.entity is not None:
+            result['entity'] = self.entity
+        if self.header is not None:
+            result['header'] = self.header
+        if self.id is not None:
+            result['id'] = self.id
+        if self.info is not None:
+            result['info'] = self.info
+        if self.operator is not None:
+            result['operator'] = self.operator
+        if self.tenant is not None:
+            result['tenant'] = self.tenant
+        if self.tenant_id is not None:
+            result['tenantId'] = self.tenant_id
+        if self.time is not None:
+            result['time'] = self.time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        if m.get('entity') is not None:
+            self.entity = m.get('entity')
+        if m.get('header') is not None:
+            self.header = m.get('header')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('info') is not None:
+            self.info = m.get('info')
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        if m.get('tenant') is not None:
+            self.tenant = m.get('tenant')
+        if m.get('tenantId') is not None:
+            self.tenant_id = m.get('tenantId')
+        if m.get('time') is not None:
+            self.time = m.get('time')
+        return self
+
+
 class GetAllJobLevelHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -3663,14 +3747,242 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListProgressByIdsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListSlsLogHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ListSlsLogRequest(TeaModel):
+    def __init__(
+        self,
+        app_code: str = None,
+        end_time: int = None,
+        page_number: int = None,
+        page_size: int = None,
+        start_time: int = None,
+    ):
+        # This parameter is required.
+        self.app_code = app_code
+        self.end_time = end_time
+        # This parameter is required.
+        self.page_number = page_number
+        # This parameter is required.
+        self.page_size = page_size
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_code is not None:
+            result['appCode'] = self.app_code
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appCode') is not None:
+            self.app_code = m.get('appCode')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        return self
+
+
+class ListSlsLogResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        current_page_size: int = None,
+        data: List[SlsLogResp] = None,
+        page_number: int = None,
+        page_size: int = None,
+        pages: int = None,
+        total_count: int = None,
+    ):
+        self.current_page_size = current_page_size
+        self.data = data
+        self.page_number = page_number
+        self.page_size = page_size
+        self.pages = pages
+        self.total_count = total_count
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_page_size is not None:
+            result['currentPageSize'] = self.current_page_size
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.pages is not None:
+            result['pages'] = self.pages
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('currentPageSize') is not None:
+            self.current_page_size = m.get('currentPageSize')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = SlsLogResp()
+                self.data.append(temp_model.from_map(k))
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('pages') is not None:
+            self.pages = m.get('pages')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class ListSlsLogResponseBody(TeaModel):
+    def __init__(
+        self,
+        content: ListSlsLogResponseBodyContent = None,
+        success: bool = None,
+    ):
+        self.content = content
+        self.success = success
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['content'] = self.content.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            temp_model = ListSlsLogResponseBodyContent()
+            self.content = temp_model.from_map(m['content'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ListSlsLogResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListSlsLogResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListSlsLogResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PageListObjectiveProgressHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6300,77 +6300,107 @@
             self.extension_app_biz_data = m.get('extensionAppBizData')
         return self
 
 
 class UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSetting(TeaModel):
     def __init__(
         self,
+        cloud_record_owner_union_id: str = None,
         enable_chat: int = None,
         enable_web_anonymous_join: bool = None,
         join_before_host: int = None,
         lock_media_status_mic_mute: int = None,
         lock_nick: int = None,
+        minutes_owner_union_id: str = None,
         mozi_conf_extension_app_settings: List[UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings] = None,
+        push_all_meeting_records: bool = None,
+        push_cloud_record_card: bool = None,
+        push_minutes_card: bool = None,
         waiting_room: int = None,
     ):
+        self.cloud_record_owner_union_id = cloud_record_owner_union_id
         self.enable_chat = enable_chat
         self.enable_web_anonymous_join = enable_web_anonymous_join
         self.join_before_host = join_before_host
         self.lock_media_status_mic_mute = lock_media_status_mic_mute
         self.lock_nick = lock_nick
+        self.minutes_owner_union_id = minutes_owner_union_id
         self.mozi_conf_extension_app_settings = mozi_conf_extension_app_settings
+        self.push_all_meeting_records = push_all_meeting_records
+        self.push_cloud_record_card = push_cloud_record_card
+        self.push_minutes_card = push_minutes_card
         self.waiting_room = waiting_room
 
     def validate(self):
         if self.mozi_conf_extension_app_settings:
             for k in self.mozi_conf_extension_app_settings:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.cloud_record_owner_union_id is not None:
+            result['cloudRecordOwnerUnionId'] = self.cloud_record_owner_union_id
         if self.enable_chat is not None:
             result['enableChat'] = self.enable_chat
         if self.enable_web_anonymous_join is not None:
             result['enableWebAnonymousJoin'] = self.enable_web_anonymous_join
         if self.join_before_host is not None:
             result['joinBeforeHost'] = self.join_before_host
         if self.lock_media_status_mic_mute is not None:
             result['lockMediaStatusMicMute'] = self.lock_media_status_mic_mute
         if self.lock_nick is not None:
             result['lockNick'] = self.lock_nick
+        if self.minutes_owner_union_id is not None:
+            result['minutesOwnerUnionId'] = self.minutes_owner_union_id
         result['moziConfExtensionAppSettings'] = []
         if self.mozi_conf_extension_app_settings is not None:
             for k in self.mozi_conf_extension_app_settings:
                 result['moziConfExtensionAppSettings'].append(k.to_map() if k else None)
+        if self.push_all_meeting_records is not None:
+            result['pushAllMeetingRecords'] = self.push_all_meeting_records
+        if self.push_cloud_record_card is not None:
+            result['pushCloudRecordCard'] = self.push_cloud_record_card
+        if self.push_minutes_card is not None:
+            result['pushMinutesCard'] = self.push_minutes_card
         if self.waiting_room is not None:
             result['waitingRoom'] = self.waiting_room
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('cloudRecordOwnerUnionId') is not None:
+            self.cloud_record_owner_union_id = m.get('cloudRecordOwnerUnionId')
         if m.get('enableChat') is not None:
             self.enable_chat = m.get('enableChat')
         if m.get('enableWebAnonymousJoin') is not None:
             self.enable_web_anonymous_join = m.get('enableWebAnonymousJoin')
         if m.get('joinBeforeHost') is not None:
             self.join_before_host = m.get('joinBeforeHost')
         if m.get('lockMediaStatusMicMute') is not None:
             self.lock_media_status_mic_mute = m.get('lockMediaStatusMicMute')
         if m.get('lockNick') is not None:
             self.lock_nick = m.get('lockNick')
+        if m.get('minutesOwnerUnionId') is not None:
+            self.minutes_owner_union_id = m.get('minutesOwnerUnionId')
         self.mozi_conf_extension_app_settings = []
         if m.get('moziConfExtensionAppSettings') is not None:
             for k in m.get('moziConfExtensionAppSettings'):
                 temp_model = UpdateScheduleConfSettingsRequestScheduleConfSettingModelMoziConfVirtualExtraSettingMoziConfExtensionAppSettings()
                 self.mozi_conf_extension_app_settings.append(temp_model.from_map(k))
+        if m.get('pushAllMeetingRecords') is not None:
+            self.push_all_meeting_records = m.get('pushAllMeetingRecords')
+        if m.get('pushCloudRecordCard') is not None:
+            self.push_cloud_record_card = m.get('pushCloudRecordCard')
+        if m.get('pushMinutesCard') is not None:
+            self.push_minutes_card = m.get('pushMinutesCard')
         if m.get('waitingRoom') is not None:
             self.waiting_room = m.get('waitingRoom')
         return self
 
 
 class UpdateScheduleConfSettingsRequestScheduleConfSettingModel(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6007,14 +6007,106 @@
         @param request: QueryCrmPersonalCustomerRequest
         @return: QueryCrmPersonalCustomerResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcrm__1__0_models.QueryCrmPersonalCustomerHeaders()
         return await self.query_crm_personal_customer_with_options_async(request, headers, runtime)
 
+    def query_customer_biz_type_with_options(
+        self,
+        headers: dingtalkcrm__1__0_models.QueryCustomerBizTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse:
+        """
+        @summary 查询客户模板启用类型
+        
+        @param headers: QueryCustomerBizTypeHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryCustomerBizTypeResponse
+        """
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers
+        )
+        params = open_api_models.Params(
+            action='QueryCustomerBizType',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/orgSettings/templates/customerBizTypes',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_customer_biz_type_with_options_async(
+        self,
+        headers: dingtalkcrm__1__0_models.QueryCustomerBizTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse:
+        """
+        @summary 查询客户模板启用类型
+        
+        @param headers: QueryCustomerBizTypeHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryCustomerBizTypeResponse
+        """
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers
+        )
+        params = open_api_models.Params(
+            action='QueryCustomerBizType',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/orgSettings/templates/customerBizTypes',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_customer_biz_type(self) -> dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse:
+        """
+        @summary 查询客户模板启用类型
+        
+        @return: QueryCustomerBizTypeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.QueryCustomerBizTypeHeaders()
+        return self.query_customer_biz_type_with_options(headers, runtime)
+
+    async def query_customer_biz_type_async(self) -> dingtalkcrm__1__0_models.QueryCustomerBizTypeResponse:
+        """
+        @summary 查询客户模板启用类型
+        
+        @return: QueryCustomerBizTypeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.QueryCustomerBizTypeHeaders()
+        return await self.query_customer_biz_type_with_options_async(headers, runtime)
+
     def query_global_info_with_options(
         self,
         request: dingtalkcrm__1__0_models.QueryGlobalInfoRequest,
         headers: dingtalkcrm__1__0_models.QueryGlobalInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcrm__1__0_models.QueryGlobalInfoResponse:
         """
@@ -6983,14 +7075,128 @@
         @param request: UpdateCrmPersonalCustomerRequest
         @return: UpdateCrmPersonalCustomerResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcrm__1__0_models.UpdateCrmPersonalCustomerHeaders()
         return await self.update_crm_personal_customer_with_options_async(request, headers, runtime)
 
+    def update_customer_biz_type_with_options(
+        self,
+        request: dingtalkcrm__1__0_models.UpdateCustomerBizTypeRequest,
+        headers: dingtalkcrm__1__0_models.UpdateCustomerBizTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse:
+        """
+        @summary 更新客户模板类型
+        
+        @param request: UpdateCustomerBizTypeRequest
+        @param headers: UpdateCustomerBizTypeHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateCustomerBizTypeResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.customer_biz_type):
+            body['customerBizType'] = request.customer_biz_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateCustomerBizType',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/orgSettings/templates/customerBizTypes',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_customer_biz_type_with_options_async(
+        self,
+        request: dingtalkcrm__1__0_models.UpdateCustomerBizTypeRequest,
+        headers: dingtalkcrm__1__0_models.UpdateCustomerBizTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse:
+        """
+        @summary 更新客户模板类型
+        
+        @param request: UpdateCustomerBizTypeRequest
+        @param headers: UpdateCustomerBizTypeHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateCustomerBizTypeResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.customer_biz_type):
+            body['customerBizType'] = request.customer_biz_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateCustomerBizType',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/orgSettings/templates/customerBizTypes',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_customer_biz_type(
+        self,
+        request: dingtalkcrm__1__0_models.UpdateCustomerBizTypeRequest,
+    ) -> dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse:
+        """
+        @summary 更新客户模板类型
+        
+        @param request: UpdateCustomerBizTypeRequest
+        @return: UpdateCustomerBizTypeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.UpdateCustomerBizTypeHeaders()
+        return self.update_customer_biz_type_with_options(request, headers, runtime)
+
+    async def update_customer_biz_type_async(
+        self,
+        request: dingtalkcrm__1__0_models.UpdateCustomerBizTypeRequest,
+    ) -> dingtalkcrm__1__0_models.UpdateCustomerBizTypeResponse:
+        """
+        @summary 更新客户模板类型
+        
+        @param request: UpdateCustomerBizTypeRequest
+        @return: UpdateCustomerBizTypeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.UpdateCustomerBizTypeHeaders()
+        return await self.update_customer_biz_type_with_options_async(request, headers, runtime)
+
     def update_group_set_with_options(
         self,
         request: dingtalkcrm__1__0_models.UpdateGroupSetRequest,
         headers: dingtalkcrm__1__0_models.UpdateGroupSetHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcrm__1__0_models.UpdateGroupSetResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -16265,14 +16265,144 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryCrmPersonalCustomerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryCustomerBizTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryCustomerBizTypeResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        customer_biz_type: str = None,
+    ):
+        self.customer_biz_type = customer_biz_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.customer_biz_type is not None:
+            result['customerBizType'] = self.customer_biz_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customerBizType') is not None:
+            self.customer_biz_type = m.get('customerBizType')
+        return self
+
+
+class QueryCustomerBizTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: QueryCustomerBizTypeResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = QueryCustomerBizTypeResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class QueryCustomerBizTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryCustomerBizTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryCustomerBizTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryGlobalInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -18708,14 +18838,143 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateCrmPersonalCustomerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateCustomerBizTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateCustomerBizTypeRequest(TeaModel):
+    def __init__(
+        self,
+        customer_biz_type: str = None,
+    ):
+        # This parameter is required.
+        self.customer_biz_type = customer_biz_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.customer_biz_type is not None:
+            result['customerBizType'] = self.customer_biz_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customerBizType') is not None:
+            self.customer_biz_type = m.get('customerBizType')
+        return self
+
+
+class UpdateCustomerBizTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class UpdateCustomerBizTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateCustomerBizTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateCustomerBizTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateGroupSetHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
         invoice_title_third_party_id: str = None,
         itinerary_project: str = None,
         itinerary_project_third_party_id: str = None,
         journeys: List[GetTravelProcessDetailResponseBodyResultJourneys] = None,
         main_process_instance_id: str = None,
         memo: str = None,
         originator_id: str = None,
+        originator_id_on_behalf: str = None,
         process_instance_id: str = None,
         process_result: str = None,
         process_status: str = None,
         remark: str = None,
         travel_category: str = None,
         travelers: List[str] = None,
     ):
@@ -412,14 +413,15 @@
         self.invoice_title_third_party_id = invoice_title_third_party_id
         self.itinerary_project = itinerary_project
         self.itinerary_project_third_party_id = itinerary_project_third_party_id
         self.journeys = journeys
         self.main_process_instance_id = main_process_instance_id
         self.memo = memo
         self.originator_id = originator_id
+        self.originator_id_on_behalf = originator_id_on_behalf
         self.process_instance_id = process_instance_id
         self.process_result = process_result
         self.process_status = process_status
         self.remark = remark
         self.travel_category = travel_category
         self.travelers = travelers
 
@@ -475,14 +477,16 @@
                 result['journeys'].append(k.to_map() if k else None)
         if self.main_process_instance_id is not None:
             result['mainProcessInstanceId'] = self.main_process_instance_id
         if self.memo is not None:
             result['memo'] = self.memo
         if self.originator_id is not None:
             result['originatorId'] = self.originator_id
+        if self.originator_id_on_behalf is not None:
+            result['originatorIdOnBehalf'] = self.originator_id_on_behalf
         if self.process_instance_id is not None:
             result['processInstanceId'] = self.process_instance_id
         if self.process_result is not None:
             result['processResult'] = self.process_result
         if self.process_status is not None:
             result['processStatus'] = self.process_status
         if self.remark is not None:
@@ -533,14 +537,16 @@
                 self.journeys.append(temp_model.from_map(k))
         if m.get('mainProcessInstanceId') is not None:
             self.main_process_instance_id = m.get('mainProcessInstanceId')
         if m.get('memo') is not None:
             self.memo = m.get('memo')
         if m.get('originatorId') is not None:
             self.originator_id = m.get('originatorId')
+        if m.get('originatorIdOnBehalf') is not None:
+            self.originator_id_on_behalf = m.get('originatorIdOnBehalf')
         if m.get('processInstanceId') is not None:
             self.process_instance_id = m.get('processInstanceId')
         if m.get('processResult') is not None:
             self.process_result = m.get('processResult')
         if m.get('processStatus') is not None:
             self.process_status = m.get('processStatus')
         if m.get('remark') is not None:
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5169,15 +5169,15 @@
             action='GetMeCorpSubmission',
             version='yida_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/yida/tasks/myCorpSubmission/{user_id}',
             method='GET',
             auth_type='AK',
             style='ROA',
-            req_body_type='formData',
+            req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
             dingtalkyida__1__0_models.GetMeCorpSubmissionResponse(),
             self.execute(params, req, runtime)
         )
 
@@ -5231,15 +5231,15 @@
             action='GetMeCorpSubmission',
             version='yida_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/yida/tasks/myCorpSubmission/{user_id}',
             method='GET',
             auth_type='AK',
             style='ROA',
-            req_body_type='formData',
+            req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
             dingtalkyida__1__0_models.GetMeCorpSubmissionResponse(),
             await self.execute_async(params, req, runtime)
         )
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.1.15
+Version: 2.1.16
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.16/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.15/setup.py` & `alibabacloud_dingtalk-2.1.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 24/05/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

