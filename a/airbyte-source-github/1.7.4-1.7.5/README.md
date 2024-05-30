# Comparing `tmp/airbyte_source_github-1.7.4.tar.gz` & `tmp/airbyte_source_github-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_github-1.7.4.tar", max compression
+gzip compressed data, was "airbyte_source_github-1.7.5.tar", max compression
```

## Comparing `airbyte_source_github-1.7.4.tar` & `airbyte_source_github-1.7.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     4506 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/README.md
--rw-r--r--   0        0        0      801 2024-05-22 15:28:59.754833 airbyte_source_github-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/__init__.py
--rw-r--r--   0        0        0     3849 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/config_migrations.py
--rw-r--r--   0        0        0      238 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/constants.py
--rw-r--r--   0        0        0  1600314 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/github_schema.py
--rw-r--r--   0        0        0    11625 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/graphql.py
--rw-r--r--   0        0        0      407 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/run.py
--rw-r--r--   0        0        0     2335 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/assignees.json
--rw-r--r--   0        0        0     2734 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/branches.json
--rw-r--r--   0        0        0     3505 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/collaborators.json
--rw-r--r--   0        0        0     4193 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/comments.json
--rw-r--r--   0        0        0       87 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/commit_comment_reactions.json
--rw-r--r--   0        0        0     2164 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/commit_comments.json
--rw-r--r--   0        0        0     5122 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/commits.json
--rw-r--r--   0        0        0     3957 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/contributor_activity.json
--rw-r--r--   0        0        0     2893 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/deployments.json
--rw-r--r--   0        0        0     2299 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/events.json
--rw-r--r--   0        0        0       87 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_comment_reactions.json
--rw-r--r--   0        0        0    13840 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_events.json
--rw-r--r--   0        0        0     1200 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_labels.json
--rw-r--r--   0        0        0     2309 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_milestones.json
--rw-r--r--   0        0        0      998 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_reactions.json
--rw-r--r--   0        0        0    30392 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issue_timeline_events.json
--rw-r--r--   0        0        0    11962 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/issues.json
--rw-r--r--   0        0        0     9349 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/organizations.json
--rw-r--r--   0        0        0     2016 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/project_cards.json
--rw-r--r--   0        0        0     1489 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/project_columns.json
--rw-r--r--   0        0        0     1848 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/projects.json
--rw-r--r--   0        0        0     3162 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/projects_v2.json
--rw-r--r--   0        0        0     1038 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/pull_request_comment_reactions.json
--rw-r--r--   0        0        0     4800 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/pull_request_commits.json
--rw-r--r--   0        0        0     3497 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/pull_request_stats.json
--rw-r--r--   0        0        0    12196 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/pull_requests.json
--rw-r--r--   0        0        0     5140 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/releases.json
--rw-r--r--   0        0        0    13319 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/repositories.json
--rw-r--r--   0        0        0     4905 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/review_comments.json
--rw-r--r--   0        0        0     2731 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/reviews.json
--rw-r--r--   0        0        0     7387 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/events/comment.json
--rw-r--r--   0        0        0     4197 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/events/commented.json
--rw-r--r--   0        0        0     1443 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/events/committed.json
--rw-r--r--   0        0        0    36914 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/events/cross_referenced.json
--rw-r--r--   0        0        0     2764 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/events/reviewed.json
--rw-r--r--   0        0        0      449 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/reaction.json
--rw-r--r--   0        0        0      616 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/reactions.json
--rw-r--r--   0        0        0     1135 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/user.json
--rw-r--r--   0        0        0      453 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/shared/user_graphql.json
--rw-r--r--   0        0        0      630 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/stargazers.json
--rw-r--r--   0        0        0     1133 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/tags.json
--rw-r--r--   0        0        0     2518 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/team_members.json
--rw-r--r--   0        0        0      911 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/team_memberships.json
--rw-r--r--   0        0        0     1796 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/teams.json
--rw-r--r--   0        0        0     2530 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/users.json
--rw-r--r--   0        0        0     3934 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/workflow_jobs.json
--rw-r--r--   0        0        0    19453 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/workflow_runs.json
--rw-r--r--   0        0        0     1470 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/schemas/workflows.json
--rw-r--r--   0        0        0    13895 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/source.py
--rw-r--r--   0        0        0     7073 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/spec.json
--rw-r--r--   0        0        0    77006 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/streams.py
--rw-r--r--   0        0        0     5462 2024-05-22 14:54:39.000000 airbyte_source_github-1.7.4/source_github/utils.py
--rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     4506 2024-05-30 17:55:29.078817 airbyte_source_github-1.7.5/README.md
+-rw-r--r--   0        0        0      801 2024-05-30 18:00:22.341224 airbyte_source_github-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-05-30 17:55:29.078817 airbyte_source_github-1.7.5/source_github/__init__.py
+-rw-r--r--   0        0        0     3849 2024-05-30 17:55:29.078817 airbyte_source_github-1.7.5/source_github/config_migrations.py
+-rw-r--r--   0        0        0      238 2024-05-30 17:55:29.078817 airbyte_source_github-1.7.5/source_github/constants.py
+-rw-r--r--   0        0        0  1600314 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/github_schema.py
+-rw-r--r--   0        0        0    11625 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/graphql.py
+-rw-r--r--   0        0        0      407 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/run.py
+-rw-r--r--   0        0        0     2335 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/assignees.json
+-rw-r--r--   0        0        0     2734 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/branches.json
+-rw-r--r--   0        0        0     3505 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/collaborators.json
+-rw-r--r--   0        0        0     4193 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/comments.json
+-rw-r--r--   0        0        0       87 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/commit_comment_reactions.json
+-rw-r--r--   0        0        0     2164 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/commit_comments.json
+-rw-r--r--   0        0        0     5122 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/commits.json
+-rw-r--r--   0        0        0     3957 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/contributor_activity.json
+-rw-r--r--   0        0        0     2893 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/deployments.json
+-rw-r--r--   0        0        0     2299 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/events.json
+-rw-r--r--   0        0        0       87 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_comment_reactions.json
+-rw-r--r--   0        0        0    13840 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_events.json
+-rw-r--r--   0        0        0     1200 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_labels.json
+-rw-r--r--   0        0        0     2309 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_milestones.json
+-rw-r--r--   0        0        0      998 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_reactions.json
+-rw-r--r--   0        0        0    30392 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issue_timeline_events.json
+-rw-r--r--   0        0        0    11962 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/issues.json
+-rw-r--r--   0        0        0     9349 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/organizations.json
+-rw-r--r--   0        0        0     2016 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/project_cards.json
+-rw-r--r--   0        0        0     1489 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/project_columns.json
+-rw-r--r--   0        0        0     1848 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/projects.json
+-rw-r--r--   0        0        0     3162 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/projects_v2.json
+-rw-r--r--   0        0        0     1038 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/pull_request_comment_reactions.json
+-rw-r--r--   0        0        0     4800 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/pull_request_commits.json
+-rw-r--r--   0        0        0     3497 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/pull_request_stats.json
+-rw-r--r--   0        0        0    12196 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/pull_requests.json
+-rw-r--r--   0        0        0     5140 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/releases.json
+-rw-r--r--   0        0        0    13319 2024-05-30 17:55:29.082817 airbyte_source_github-1.7.5/source_github/schemas/repositories.json
+-rw-r--r--   0        0        0     4905 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/review_comments.json
+-rw-r--r--   0        0        0     2731 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/reviews.json
+-rw-r--r--   0        0        0     7387 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/events/comment.json
+-rw-r--r--   0        0        0     4197 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/events/commented.json
+-rw-r--r--   0        0        0     1443 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/events/committed.json
+-rw-r--r--   0        0        0    36914 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/events/cross_referenced.json
+-rw-r--r--   0        0        0     2764 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/events/reviewed.json
+-rw-r--r--   0        0        0      449 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/reaction.json
+-rw-r--r--   0        0        0      616 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/reactions.json
+-rw-r--r--   0        0        0     1135 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/user.json
+-rw-r--r--   0        0        0      453 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/shared/user_graphql.json
+-rw-r--r--   0        0        0      630 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/stargazers.json
+-rw-r--r--   0        0        0     1133 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/tags.json
+-rw-r--r--   0        0        0     2518 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/team_members.json
+-rw-r--r--   0        0        0      911 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/team_memberships.json
+-rw-r--r--   0        0        0     1796 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/teams.json
+-rw-r--r--   0        0        0     2530 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/users.json
+-rw-r--r--   0        0        0     3934 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/workflow_jobs.json
+-rw-r--r--   0        0        0    19453 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/workflow_runs.json
+-rw-r--r--   0        0        0     1470 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/schemas/workflows.json
+-rw-r--r--   0        0        0    14028 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/source.py
+-rw-r--r--   0        0        0     7443 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/spec.json
+-rw-r--r--   0        0        0    77038 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/streams.py
+-rw-r--r--   0        0        0     5462 2024-05-30 17:55:29.086817 airbyte_source_github-1.7.5/source_github/utils.py
+-rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.5/PKG-INFO
```

### Comparing `airbyte_source_github-1.7.4/README.md` & `airbyte_source_github-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/pyproject.toml` & `airbyte_source_github-1.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.7.4"
+version = "1.7.5"
 name = "airbyte-source-github"
 description = "Source implementation for GitHub."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_github-1.7.4/source_github/__init__.py` & `airbyte_source_github-1.7.5/source_github/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/config_migrations.py` & `airbyte_source_github-1.7.5/source_github/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/github_schema.py` & `airbyte_source_github-1.7.5/source_github/github_schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/graphql.py` & `airbyte_source_github-1.7.5/source_github/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/assignees.json` & `airbyte_source_github-1.7.5/source_github/schemas/assignees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/branches.json` & `airbyte_source_github-1.7.5/source_github/schemas/branches.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/collaborators.json` & `airbyte_source_github-1.7.5/source_github/schemas/collaborators.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/comments.json` & `airbyte_source_github-1.7.5/source_github/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/commit_comments.json` & `airbyte_source_github-1.7.5/source_github/schemas/commit_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/commits.json` & `airbyte_source_github-1.7.5/source_github/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/contributor_activity.json` & `airbyte_source_github-1.7.5/source_github/schemas/contributor_activity.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/deployments.json` & `airbyte_source_github-1.7.5/source_github/schemas/deployments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/events.json` & `airbyte_source_github-1.7.5/source_github/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issue_events.json` & `airbyte_source_github-1.7.5/source_github/schemas/issue_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issue_labels.json` & `airbyte_source_github-1.7.5/source_github/schemas/issue_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issue_milestones.json` & `airbyte_source_github-1.7.5/source_github/schemas/issue_milestones.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issue_reactions.json` & `airbyte_source_github-1.7.5/source_github/schemas/issue_reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issue_timeline_events.json` & `airbyte_source_github-1.7.5/source_github/schemas/issue_timeline_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/issues.json` & `airbyte_source_github-1.7.5/source_github/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/organizations.json` & `airbyte_source_github-1.7.5/source_github/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/project_cards.json` & `airbyte_source_github-1.7.5/source_github/schemas/project_cards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/project_columns.json` & `airbyte_source_github-1.7.5/source_github/schemas/project_columns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/projects.json` & `airbyte_source_github-1.7.5/source_github/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/projects_v2.json` & `airbyte_source_github-1.7.5/source_github/schemas/projects_v2.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/pull_request_comment_reactions.json` & `airbyte_source_github-1.7.5/source_github/schemas/pull_request_comment_reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/pull_request_commits.json` & `airbyte_source_github-1.7.5/source_github/schemas/pull_request_commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/pull_request_stats.json` & `airbyte_source_github-1.7.5/source_github/schemas/pull_request_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/pull_requests.json` & `airbyte_source_github-1.7.5/source_github/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/releases.json` & `airbyte_source_github-1.7.5/source_github/schemas/releases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/repositories.json` & `airbyte_source_github-1.7.5/source_github/schemas/repositories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/review_comments.json` & `airbyte_source_github-1.7.5/source_github/schemas/review_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/reviews.json` & `airbyte_source_github-1.7.5/source_github/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/events/comment.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/events/comment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/events/commented.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/events/commented.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/events/committed.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/events/committed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/events/cross_referenced.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/events/cross_referenced.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/events/reviewed.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/events/reviewed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/reactions.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/shared/user.json` & `airbyte_source_github-1.7.5/source_github/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/stargazers.json` & `airbyte_source_github-1.7.5/source_github/schemas/stargazers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/tags.json` & `airbyte_source_github-1.7.5/source_github/schemas/tags.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/team_members.json` & `airbyte_source_github-1.7.5/source_github/schemas/team_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/team_memberships.json` & `airbyte_source_github-1.7.5/source_github/schemas/team_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/teams.json` & `airbyte_source_github-1.7.5/source_github/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/users.json` & `airbyte_source_github-1.7.5/source_github/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/workflow_jobs.json` & `airbyte_source_github-1.7.5/source_github/schemas/workflow_jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/workflow_runs.json` & `airbyte_source_github-1.7.5/source_github/schemas/workflow_runs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/schemas/workflows.json` & `airbyte_source_github-1.7.5/source_github/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/source_github/source.py` & `airbyte_source_github-1.7.5/source_github/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
-
+import logging
 from os import getenv
 from typing import Any, List, Mapping, MutableMapping, Optional, Tuple
 from urllib.parse import urlparse
 
-from airbyte_cdk import AirbyteLogger
-from airbyte_cdk.models import FailureType, SyncMode
+from airbyte_cdk.models import FailureType
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http.requests_native_auth import MultipleTokenAuthenticator
 from airbyte_cdk.utils.traced_exception import AirbyteTracedException
 from source_github.utils import MultipleTokenAuthenticatorWithRateLimiter
 
 from . import constants
@@ -187,15 +186,15 @@
         elif "401 Client Error: Unauthorized for url" in message:
             # 401 Client Error: Unauthorized for url: https://api.github.com/orgs/datarootsio/repos?per_page=100&sort=updated&direction=desc
             user_message = (
                 "Github credentials have expired or changed, please review your credentials and re-authenticate or renew your access token."
             )
         return user_message
 
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         config = self._validate_and_transform_config(config)
         try:
             authenticator = self._get_authenticator(config)
             _, repositories, _ = self._get_org_repositories(config=config, authenticator=authenticator)
             if not repositories:
                 return (
                     False,
@@ -234,30 +233,32 @@
                 message=user_message,
                 failure_type=FailureType.config_error,
             )
 
         # This parameter is deprecated and in future will be used sane default, page_size: 10
         page_size = config.get("page_size_for_large_streams", constants.DEFAULT_PAGE_SIZE_FOR_LARGE_STREAM)
         access_token_type, _ = self.get_access_token(config)
-
+        max_waiting_time = config.get("max_waiting_time", 10) * 60
         organization_args = {
             "authenticator": authenticator,
             "organizations": organizations,
             "api_url": config.get("api_url"),
             "access_token_type": access_token_type,
+            "max_waiting_time": max_waiting_time,
         }
         start_date = config.get("start_date")
         organization_args_with_start_date = {**organization_args, "start_date": start_date}
 
         repository_args = {
             "authenticator": authenticator,
             "api_url": config.get("api_url"),
             "repositories": repositories,
             "page_size_for_large_streams": page_size,
             "access_token_type": access_token_type,
+            "max_waiting_time": max_waiting_time,
         }
         repository_args_with_start_date = {**repository_args, "start_date": start_date}
 
         pull_requests_stream = PullRequests(**repository_args_with_start_date)
         projects_stream = Projects(**repository_args_with_start_date)
         project_columns_stream = ProjectColumns(projects_stream, **repository_args_with_start_date)
         teams_stream = Teams(**organization_args)
```

### Comparing `airbyte_source_github-1.7.4/source_github/spec.json` & `airbyte_source_github-1.7.5/source_github/spec.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998263888888889%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'max_waiting_time': OrderedDict([('type', "*

 * *                              "'integer'), ('title', 'Max Waiting Time (in minutes)'), "*

 * *                              "('examples', [10, 30, 60]), ('default', 10), ('minimum', 1), "*

 * *                              "('maximum', 60), ('description', 'Max Waiting Time for rate limit. "*

 * *                              'Set higher value to wait till rate limits will be resetted to '*

 * *                              "continue syn […]*

```diff
@@ -150,14 +150,28 @@
                         "type": "object"
                     }
                 ],
                 "order": 0,
                 "title": "Authentication",
                 "type": "object"
             },
+            "max_waiting_time": {
+                "default": 10,
+                "description": "Max Waiting Time for rate limit. Set higher value to wait till rate limits will be resetted to continue sync",
+                "examples": [
+                    10,
+                    30,
+                    60
+                ],
+                "maximum": 60,
+                "minimum": 1,
+                "order": 5,
+                "title": "Max Waiting Time (in minutes)",
+                "type": "integer"
+            },
             "repositories": {
                 "description": "List of GitHub organizations/repositories, e.g. `airbytehq/airbyte` for single repository, `airbytehq/*` for get all repositories from organization and `airbytehq/a* for matching multiple repositories by pattern.",
                 "examples": [
                     "airbytehq/airbyte",
                     "airbytehq/another-repo",
                     "airbytehq/*",
                     "airbytehq/a*"
```

### Comparing `airbyte_source_github-1.7.4/source_github/streams.py` & `airbyte_source_github-1.7.5/source_github/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # Detect streams with high API load
     large_stream = False
 
     stream_base_params = {}
 
     def __init__(self, api_url: str = "https://api.github.com", access_token_type: str = "", **kwargs):
         if kwargs.get("authenticator"):
-            kwargs["authenticator"].max_time = self.max_time
+            kwargs["authenticator"].max_time = kwargs.pop("max_waiting_time", self.max_time)
         super().__init__(**kwargs)
 
         self.access_token_type = access_token_type
         self.api_url = api_url
 
     @property
     def url_base(self) -> str:
```

### Comparing `airbyte_source_github-1.7.4/source_github/utils.py` & `airbyte_source_github-1.7.5/source_github/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.4/PKG-INFO` & `airbyte_source_github-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-github
-Version: 1.7.4
+Version: 1.7.5
 Summary: Source implementation for GitHub.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

