# Comparing `tmp/annoworkcli-3.7.1.tar.gz` & `tmp/annoworkcli-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkcli-3.7.1.tar", max compression
+gzip compressed data, was "annoworkcli-3.7.2.tar", max compression
```

## Comparing `annoworkcli-3.7.1.tar` & `annoworkcli-3.7.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     2107 2024-02-07 02:06:19.174617 annoworkcli-3.7.1/README.md
--rw-r--r--   0        0        0       71 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/__init__.py
--rw-r--r--   0        0        0     3608 2024-04-24 02:10:19.836885 annoworkcli-3.7.1/annoworkcli/__main__.py
--rw-r--r--   0        0        0      131 2024-04-24 03:15:55.410866 annoworkcli-3.7.1/annoworkcli/__version__.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/account/__init__.py
--rw-r--r--   0        0        0     2922 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/account/list_external_linkage_info.py
--rw-r--r--   0        0        0     2406 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/account/put_external_linkage_info.py
--rw-r--r--   0        0        0      881 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/account/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/actual_working_time/__init__.py
--rw-r--r--   0        0        0     7666 2024-03-15 05:00:41.781340 annoworkcli-3.7.1/annoworkcli/actual_working_time/delete_actual_working_time.py
--rw-r--r--   0        0        0    14647 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
--rw-r--r--   0        0        0    13329 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    15180 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_time.py
--rw-r--r--   0        0        0     1410 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/actual_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/annofab/__init__.py
--rw-r--r--   0        0        0     9042 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/list_job_with_annofab_project.py
--rw-r--r--   0        0        0    24006 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/list_working_hours.py
--rw-r--r--   0        0        0     5763 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/put_account_external_linkage_info.py
--rw-r--r--   0        0        0     4507 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/put_job_from_annofab_project.py
--rw-r--r--   0        0        0    51925 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/reshape_working_hours.py
--rw-r--r--   0        0        0     1517 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/subcommand.py
--rw-r--r--   0        0        0     2256 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/utils.py
--rw-r--r--   0        0        0    12048 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/annofab/visualize_statistics.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/common/__init__.py
--rw-r--r--   0        0        0      827 2024-04-24 03:10:16.182721 annoworkcli-3.7.1/annoworkcli/common/annofab.py
--rw-r--r--   0        0        0    11712 2024-04-24 03:10:16.182721 annoworkcli-3.7.1/annoworkcli/common/cli.py
--rw-r--r--   0        0        0      222 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/common/exeptions.py
--rw-r--r--   0        0        0       43 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/common/job.py
--rw-r--r--   0        0        0     4488 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/common/utils.py
--rw-r--r--   0        0        0      888 2024-04-24 03:10:16.182721 annoworkcli-3.7.1/annoworkcli/common/workspace_tag.py
--rw-r--r--   0        0        0      829 2024-02-07 02:06:19.184617 annoworkcli-3.7.1/annoworkcli/data/logging.yaml
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/expected_working_time/__init__.py
--rw-r--r--   0        0        0     3851 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/expected_working_time/delete_expected_working_time.py
--rw-r--r--   0        0        0     6724 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time.py
--rw-r--r--   0        0        0     8795 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
--rw-r--r--   0        0        0     5840 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
--rw-r--r--   0        0        0     1298 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/expected_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/job/__init__.py
--rw-r--r--   0        0        0     4030 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/job/change_job_properties.py
--rw-r--r--   0        0        0     3348 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/job/delete_job.py
--rw-r--r--   0        0        0     6283 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/job/list_job.py
--rw-r--r--   0        0        0      887 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/job/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/my/__init__.py
--rw-r--r--   0        0        0     1426 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/my/get_my_account.py
--rw-r--r--   0        0        0     2404 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/my/list_my_workspace_member.py
--rw-r--r--   0        0        0      818 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/my/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/schedule/__init__.py
--rw-r--r--   0        0        0     5800 2024-03-15 05:00:41.781340 annoworkcli-3.7.1/annoworkcli/schedule/delete_schedule.py
--rw-r--r--   0        0        0     9074 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/schedule/list_assigned_hours_daily.py
--rw-r--r--   0        0        0     9244 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    10998 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/schedule/list_schedule.py
--rw-r--r--   0        0        0     1105 2024-03-15 05:00:41.781340 annoworkcli-3.7.1/annoworkcli/schedule/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/workspace/__init__.py
--rw-r--r--   0        0        0     3297 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/workspace/list_workspace.py
--rw-r--r--   0        0        0     2163 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/workspace/put_workspace.py
--rw-r--r--   0        0        0      849 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/workspace/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/workspace_member/__init__.py
--rw-r--r--   0        0        0     5015 2024-03-14 07:54:38.928497 annoworkcli-3.7.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py
--rw-r--r--   0        0        0     4530 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_member/change_workspace_member_properties.py
--rw-r--r--   0        0        0     2881 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_member/delete_workspace_member.py
--rw-r--r--   0        0        0     7940 2024-04-24 03:10:16.182721 annoworkcli-3.7.1/annoworkcli/workspace_member/list_workspace_member.py
--rw-r--r--   0        0        0     4746 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_member/put_workspace_member.py
--rw-r--r--   0        0        0     5046 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
--rw-r--r--   0        0        0     1520 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_member/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-14 07:37:50.012331 annoworkcli-3.7.1/annoworkcli/workspace_tag/__init__.py
--rw-r--r--   0        0        0     2702 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_tag/list_workspace_tag.py
--rw-r--r--   0        0        0     2576 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_tag/put_workspace_tag.py
--rw-r--r--   0        0        0      879 2024-03-14 07:54:38.938497 annoworkcli-3.7.1/annoworkcli/workspace_tag/subcommand.py
--rw-r--r--   0        0        0     4474 2024-04-24 03:15:55.410866 annoworkcli-3.7.1/pyproject.toml
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 annoworkcli-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2107 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/README.md
+-rw-r--r--   0        0        0       71 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/__init__.py
+-rw-r--r--   0        0        0     3608 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/__main__.py
+-rw-r--r--   0        0        0      131 2024-05-30 04:06:02.844863 annoworkcli-3.7.2/annoworkcli/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/account/__init__.py
+-rw-r--r--   0        0        0     2922 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/account/list_external_linkage_info.py
+-rw-r--r--   0        0        0     2406 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/account/put_external_linkage_info.py
+-rw-r--r--   0        0        0      881 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/account/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/__init__.py
+-rw-r--r--   0        0        0     7666 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/delete_actual_working_time.py
+-rw-r--r--   0        0        0    14647 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
+-rw-r--r--   0        0        0    13329 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    15180 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_time.py
+-rw-r--r--   0        0        0     1410 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/actual_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/__init__.py
+-rw-r--r--   0        0        0     9042 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/list_job_with_annofab_project.py
+-rw-r--r--   0        0        0    24006 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/list_working_hours.py
+-rw-r--r--   0        0        0     5763 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/put_account_external_linkage_info.py
+-rw-r--r--   0        0        0     4507 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/put_job_from_annofab_project.py
+-rw-r--r--   0        0        0    51925 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/reshape_working_hours.py
+-rw-r--r--   0        0        0     1517 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/subcommand.py
+-rw-r--r--   0        0        0     2256 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/utils.py
+-rw-r--r--   0        0        0    12795 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/annofab/visualize_statistics.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/annofab.py
+-rw-r--r--   0        0        0    11712 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/cli.py
+-rw-r--r--   0        0        0      222 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/exeptions.py
+-rw-r--r--   0        0        0       43 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/job.py
+-rw-r--r--   0        0        0     4488 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/utils.py
+-rw-r--r--   0        0        0      888 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/common/workspace_tag.py
+-rw-r--r--   0        0        0      829 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/data/logging.yaml
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/__init__.py
+-rw-r--r--   0        0        0     3851 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/delete_expected_working_time.py
+-rw-r--r--   0        0        0     6724 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time.py
+-rw-r--r--   0        0        0     8795 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
+-rw-r--r--   0        0        0     5840 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
+-rw-r--r--   0        0        0     1298 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/expected_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/job/__init__.py
+-rw-r--r--   0        0        0     4030 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/job/change_job_properties.py
+-rw-r--r--   0        0        0     3348 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/job/delete_job.py
+-rw-r--r--   0        0        0     6283 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/job/list_job.py
+-rw-r--r--   0        0        0      887 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/job/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/my/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/my/get_my_account.py
+-rw-r--r--   0        0        0     2404 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/my/list_my_workspace_member.py
+-rw-r--r--   0        0        0      818 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/my/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/__init__.py
+-rw-r--r--   0        0        0     5783 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     9074 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/list_assigned_hours_daily.py
+-rw-r--r--   0        0        0     9244 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    10998 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/list_schedule.py
+-rw-r--r--   0        0        0     1105 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/schedule/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace/__init__.py
+-rw-r--r--   0        0        0     3297 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace/list_workspace.py
+-rw-r--r--   0        0        0     2163 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace/put_workspace.py
+-rw-r--r--   0        0        0      849 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/__init__.py
+-rw-r--r--   0        0        0     5015 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     4530 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/change_workspace_member_properties.py
+-rw-r--r--   0        0        0     2881 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/delete_workspace_member.py
+-rw-r--r--   0        0        0     7940 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/list_workspace_member.py
+-rw-r--r--   0        0        0     4746 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/put_workspace_member.py
+-rw-r--r--   0        0        0     5046 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     1520 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_member/subcommand.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_tag/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-30 04:05:50.928749 annoworkcli-3.7.2/annoworkcli/workspace_tag/list_workspace_tag.py
+-rw-r--r--   0        0        0     2576 2024-05-30 04:05:50.932749 annoworkcli-3.7.2/annoworkcli/workspace_tag/put_workspace_tag.py
+-rw-r--r--   0        0        0      879 2024-05-30 04:05:50.932749 annoworkcli-3.7.2/annoworkcli/workspace_tag/subcommand.py
+-rw-r--r--   0        0        0     4715 2024-05-30 04:06:02.844863 annoworkcli-3.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 annoworkcli-3.7.2/PKG-INFO
```

### Comparing `annoworkcli-3.7.1/README.md` & `annoworkcli-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/__main__.py` & `annoworkcli-3.7.2/annoworkcli/__main__.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/account/list_external_linkage_info.py` & `annoworkcli-3.7.2/annoworkcli/account/list_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/account/put_external_linkage_info.py` & `annoworkcli-3.7.2/annoworkcli/account/put_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/account/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/account/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/actual_working_time/delete_actual_working_time.py` & `annoworkcli-3.7.2/annoworkcli/actual_working_time/delete_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py` & `annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py` & `annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/actual_working_time/list_actual_working_time.py` & `annoworkcli-3.7.2/annoworkcli/actual_working_time/list_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/actual_working_time/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/actual_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/list_job_with_annofab_project.py` & `annoworkcli-3.7.2/annoworkcli/annofab/list_job_with_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/list_working_hours.py` & `annoworkcli-3.7.2/annoworkcli/annofab/list_working_hours.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/put_account_external_linkage_info.py` & `annoworkcli-3.7.2/annoworkcli/annofab/put_account_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/put_job_from_annofab_project.py` & `annoworkcli-3.7.2/annoworkcli/annofab/put_job_from_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/reshape_working_hours.py` & `annoworkcli-3.7.2/annoworkcli/annofab/reshape_working_hours.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/annofab/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/utils.py` & `annoworkcli-3.7.2/annoworkcli/annofab/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/annofab/visualize_statistics.py` & `annoworkcli-3.7.2/annoworkcli/annofab/visualize_statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import copy
 import datetime
 import logging
 import subprocess
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
@@ -125,14 +126,16 @@
             job_id_annofab_project_id_dict = self.get_job_id_annofab_project_id_dict_from_annofab_project_id(annofab_project_id_list)
             actual_working_time_list = self.list_actual_working_time_obj.get_actual_working_times(
                 job_ids=job_id_annofab_project_id_dict.keys(),
                 start_date=start_date,
                 end_date=end_date,
                 is_set_additional_info=True,
             )
+        else:
+            raise RuntimeError("`job_id_list`と`annofab_project_id_list`の両方がNoneです。")
 
         if len(actual_working_time_list) == 0:
             return []
 
         # annofabのデータは日本時間に固定されているので、日本時間を指定する
         daily_list = create_actual_working_hours_daily_list(actual_working_time_list, timezone_offset_hours=TIMEZONE_OFFSET_HOURS)
 
@@ -156,14 +159,31 @@
                     project_id=annofab_project_id,
                     actual_worktime_hour=elm.actual_working_hours,
                 )
             )
         return result
 
 
+def mask_credential_in_command(command: list[str]) -> list[str]:
+    """
+    コマンドのリストに含まれている認証情報を、`***`に置き換えてマスクします。
+
+    Args:
+        command: 実行するコマンドのリスト（変更されません）
+    """
+    tmp_command = copy.deepcopy(command)
+    for masked_option in ["--annofab_user_id", "--annofab_password", "--mfa_code"]:
+        try:
+            index = tmp_command.index(masked_option)
+            tmp_command[index + 1] = "***"
+        except ValueError:
+            continue
+    return tmp_command
+
+
 def visualize_statistics(temp_dir: Path, args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     annofab_project_id_list = get_list_from_args(args.annofab_project_id)
     main_obj = ListLabor(annowork_service, args.workspace_id)
     annofab_labor_list = main_obj.get_annofab_labor_list(
         job_id_list=job_id_list,
@@ -213,15 +233,15 @@
 
     if args.annofab_password is not None:
         command.extend(["--annofab_password", str(args.annofab_password)])
 
     if args.annofabcli_options is not None:
         command.extend(args.annofabcli_options)
 
-    str_command = " ".join(command)
+    str_command = " ".join(mask_credential_in_command(command))
     logger.debug(f"run command: {str_command}")
     subprocess.run(command, check=True)
 
 
 def main(args):  # noqa: ANN001, ANN201
     if args.temp_dir is not None:
         visualize_statistics(args.temp_dir, args)
```

### Comparing `annoworkcli-3.7.1/annoworkcli/common/annofab.py` & `annoworkcli-3.7.2/annoworkcli/common/annofab.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/common/cli.py` & `annoworkcli-3.7.2/annoworkcli/common/cli.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/common/utils.py` & `annoworkcli-3.7.2/annoworkcli/common/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/common/workspace_tag.py` & `annoworkcli-3.7.2/annoworkcli/common/workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/data/logging.yaml` & `annoworkcli-3.7.2/annoworkcli/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/expected_working_time/delete_expected_working_time.py` & `annoworkcli-3.7.2/annoworkcli/expected_working_time/delete_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time.py` & `annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py` & `annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py` & `annoworkcli-3.7.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/expected_working_time/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/expected_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/job/change_job_properties.py` & `annoworkcli-3.7.2/annoworkcli/job/change_job_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/job/delete_job.py` & `annoworkcli-3.7.2/annoworkcli/job/delete_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/job/list_job.py` & `annoworkcli-3.7.2/annoworkcli/job/list_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/job/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/job/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/my/get_my_account.py` & `annoworkcli-3.7.2/annoworkcli/my/get_my_account.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/my/list_my_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/my/list_my_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/my/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/my/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/schedule/delete_schedule.py` & `annoworkcli-3.7.2/annoworkcli/schedule/delete_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         all_yes: bool,
     ) -> None:
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
         self.all_yes = all_yes
 
-    def delete_schedule(  # noqa: PLR0912
+    def delete_schedule(
         self, schedule_ids: Collection[str], *, target_user_ids: Optional[Collection[str]] = None, target_job_ids: Optional[Collection[str]] = None
     ) -> None:
         all_jobs = self.annowork_service.api.get_jobs(self.workspace_id)
         all_job_dict = {e["job_id"]: e for e in all_jobs}
         all_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         all_member_dict = {e["workspace_member_id"]: e for e in all_members}
```

### Comparing `annoworkcli-3.7.1/annoworkcli/schedule/list_assigned_hours_daily.py` & `annoworkcli-3.7.2/annoworkcli/schedule/list_assigned_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py` & `annoworkcli-3.7.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/schedule/list_schedule.py` & `annoworkcli-3.7.2/annoworkcli/schedule/list_schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/schedule/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/schedule/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace/list_workspace.py` & `annoworkcli-3.7.2/annoworkcli/workspace/list_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace/put_workspace.py` & `annoworkcli-3.7.2/annoworkcli/workspace/put_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/workspace/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/change_workspace_member_properties.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/change_workspace_member_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/delete_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/delete_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/list_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/list_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/put_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/put_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_member/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/workspace_member/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_tag/list_workspace_tag.py` & `annoworkcli-3.7.2/annoworkcli/workspace_tag/list_workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_tag/put_workspace_tag.py` & `annoworkcli-3.7.2/annoworkcli/workspace_tag/put_workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/annoworkcli/workspace_tag/subcommand.py` & `annoworkcli-3.7.2/annoworkcli/workspace_tag/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.7.1/pyproject.toml` & `annoworkcli-3.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "annoworkcli"
-version = "3.7.1"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+version = "3.7.2"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "AnnoworkのCLI(Command Line Interface)"
 authors = ["Kurusugawa Computer Inc."]
 license = "MIT"
 keywords=["annowork", "cli"]
 readme="README.md"
 repository="https://github.com/kurusugawa-computer/annowork-cli"
 classifiers = [
@@ -87,15 +87,15 @@
     "PERF203", # try-except-in-loop: ループ内でtry-exceptを使うこともあるため無視する。またPython3.11以降ｈ
     "FIX", # TODOやFIXMEを使うため無視する
     "TD", # TODOコメントの書き方に気にしていないので無視する
 
     # いずれ無視しないようにする
     "FA100", # future-rewritable-type-annotation
 
-    # 以下のルールはannofabcliのコードに合っていないので無効化した
+    # 以下のルールはコードに合っていないので無効化した
     "RSE", # flake8-raise
     "D", # pydocstyle, Docstringを中途半端にしか書いていないので、除外する
     "C90", # mccabe
     "T20", # flake8-print
     "SLF", #  flake8-self
     "BLE", # flake8-blind-except
     "FBT", # flake8-boolean-trap
@@ -122,14 +122,24 @@
 convention = "google"
 
 
 [tool.ruff.lint.pylint]
 max-args = 10
 
 
+[tool.ruff.lint.per-file-ignores]
+# テストコードはチェックを緩和する
+"tests/**.py" = [
+    "PGH",  # pygrep-hooks
+    "DTZ",  # flake8-datetimez
+    "ANN",  # flake8-annotations
+    "E501",  # line-too-long
+    "RUF100"  # unused-noqa
+]
+
 
 [tool.poetry-dynamic-versioning]
 enable = false
 format = "{base}"
 
 
 [build-system]
```

### Comparing `annoworkcli-3.7.1/PKG-INFO` & `annoworkcli-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoworkcli
-Version: 3.7.1
+Version: 3.7.2
 Summary: AnnoworkのCLI(Command Line Interface)
 Home-page: https://github.com/kurusugawa-computer/annowork-cli
 License: MIT
 Keywords: annowork,cli
 Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

