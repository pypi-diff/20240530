# Comparing `tmp/gitty-1.7.0.tar.gz` & `tmp/gitty-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitty-1.7.0.tar", last modified: Sun Jan  2 14:04:48 2022, max compression
+gzip compressed data, was "gitty-1.8.0.tar", last modified: Thu May 30 21:05:11 2024, max compression
```

## Comparing `gitty-1.7.0.tar` & `gitty-1.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.712378 gitty-1.7.0/
--rw-r--r--   0 lmeadors   (501) staff       (20)    10442 2022-01-02 14:04:48.712041 gitty-1.7.0/PKG-INFO
--rw-r--r--   0 lmeadors   (501) staff       (20)     8039 2021-06-16 14:57:03.000000 gitty-1.7.0/README.md
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.694036 gitty-1.7.0/bin/
--rwxr-xr-x   0 lmeadors   (501) staff       (20)      199 2021-06-16 14:45:45.000000 gitty-1.7.0/bin/_gitty_completion.zsh
--rwxr-xr-x   0 lmeadors   (501) staff       (20)      187 2020-11-27 14:00:28.000000 gitty-1.7.0/bin/gitty
--rw-r--r--   0 lmeadors   (501) staff       (20)      113 2021-06-16 14:51:37.000000 gitty-1.7.0/bin/gitty_completion.zsh
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.703724 gitty-1.7.0/gitty/
--rw-r--r--   0 lmeadors   (501) staff       (20)       29 2020-05-30 14:03:12.000000 gitty-1.7.0/gitty/__init__.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     2724 2020-08-25 22:53:29.000000 gitty-1.7.0/gitty/gitty_color.py
--rw-r--r--   0 lmeadors   (501) staff       (20)    19822 2022-01-01 16:01:35.000000 gitty-1.7.0/gitty/gitty_command.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1131 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_clean.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      536 2021-05-30 13:00:12.000000 gitty-1.7.0/gitty/gitty_command_head.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      511 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_help.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      800 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_parent.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1668 2021-06-03 20:27:26.000000 gitty-1.7.0/gitty/gitty_command_plugins.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     3019 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_release.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1159 2020-11-23 15:40:36.000000 gitty-1.7.0/gitty/gitty_command_show.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1471 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_task.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      478 2021-06-13 13:19:38.000000 gitty-1.7.0/gitty/gitty_command_version.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1904 2021-06-03 19:24:23.000000 gitty-1.7.0/gitty/gitty_executor.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     3987 2021-06-09 19:38:41.000000 gitty-1.7.0/gitty/gitty_git_api.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1537 2020-08-26 22:02:40.000000 gitty-1.7.0/gitty/gitty_project_type.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     4700 2022-01-02 13:58:26.000000 gitty-1.7.0/gitty/gitty_project_type_gradle_kotlin.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     5756 2021-08-08 18:38:51.000000 gitty-1.7.0/gitty/gitty_project_type_maven.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     3224 2021-08-08 18:38:51.000000 gitty-1.7.0/gitty/gitty_project_type_node.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     3593 2021-08-08 18:38:51.000000 gitty-1.7.0/gitty/gitty_project_type_pip.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     2770 2022-01-01 15:55:03.000000 gitty-1.7.0/gitty/gitty_project_type_xcode.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     4041 2021-08-08 18:31:54.000000 gitty-1.7.0/gitty/gitty_support.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      223 2020-08-25 22:53:29.000000 gitty-1.7.0/gitty/gitty_xml_tree_builder.py
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.704856 gitty-1.7.0/gitty.egg-info/
--rw-r--r--   0 lmeadors   (501) staff       (20)    10442 2022-01-02 14:04:48.000000 gitty-1.7.0/gitty.egg-info/PKG-INFO
--rw-r--r--   0 lmeadors   (501) staff       (20)     1307 2022-01-02 14:04:48.000000 gitty-1.7.0/gitty.egg-info/SOURCES.txt
--rw-r--r--   0 lmeadors   (501) staff       (20)        1 2022-01-02 14:04:48.000000 gitty-1.7.0/gitty.egg-info/dependency_links.txt
--rw-r--r--   0 lmeadors   (501) staff       (20)       21 2022-01-02 14:04:48.000000 gitty-1.7.0/gitty.egg-info/top_level.txt
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.706563 gitty-1.7.0/plugin_samples/
--rw-r--r--   0 lmeadors   (501) staff       (20)     1211 2021-06-06 14:11:26.000000 gitty-1.7.0/plugin_samples/finish_task.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     2569 2021-06-07 02:04:13.000000 gitty-1.7.0/plugin_samples/merge_check.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     2118 2021-06-13 13:24:03.000000 gitty-1.7.0/plugin_samples/pull_request.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      790 2021-06-12 19:15:59.000000 gitty-1.7.0/plugin_samples/zsh_complete.py
--rw-r--r--   0 lmeadors   (501) staff       (20)       38 2022-01-02 14:04:48.712479 gitty-1.7.0/setup.cfg
--rw-r--r--   0 lmeadors   (501) staff       (20)      884 2022-01-02 14:04:32.000000 gitty-1.7.0/setup.py
-drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2022-01-02 14:04:48.711394 gitty-1.7.0/tests/
--rw-r--r--   0 lmeadors   (501) staff       (20)        0 2020-08-25 22:53:29.000000 gitty-1.7.0/tests/__init__.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      420 2020-08-25 22:53:29.000000 gitty-1.7.0/tests/test_gitty_color.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1227 2021-05-30 12:45:19.000000 gitty-1.7.0/tests/test_gitty_command.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     1860 2020-11-22 16:05:57.000000 gitty-1.7.0/tests/test_gitty_command_task.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      599 2020-08-25 22:53:29.000000 gitty-1.7.0/tests/test_gitty_command_version.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     5342 2020-11-21 11:49:05.000000 gitty-1.7.0/tests/test_gitty_git_api.py
--rw-r--r--   0 lmeadors   (501) staff       (20)      896 2020-08-25 22:53:29.000000 gitty-1.7.0/tests/test_gitty_project_type.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     2079 2021-05-30 12:46:20.000000 gitty-1.7.0/tests/test_gitty_project_type_base_test.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     9775 2021-05-30 12:50:40.000000 gitty-1.7.0/tests/test_gitty_project_type_maven.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     9462 2021-05-30 12:49:38.000000 gitty-1.7.0/tests/test_gitty_project_type_node.py
--rw-r--r--   0 lmeadors   (501) staff       (20)     7511 2021-05-30 12:48:27.000000 gitty-1.7.0/tests/test_gitty_project_type_pip.py
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.305732 gitty-1.8.0/
+-rw-r--r--   0 lmeadors   (501) staff       (20)     9799 2024-05-30 21:05:11.304658 gitty-1.8.0/PKG-INFO
+-rw-r--r--   0 lmeadors   (501) staff       (20)     9388 2024-05-30 21:01:31.000000 gitty-1.8.0/README.md
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.269906 gitty-1.8.0/bin/
+-rwxr-xr-x   0 lmeadors   (501) staff       (20)      199 2021-06-16 14:45:45.000000 gitty-1.8.0/bin/_gitty_completion.zsh
+-rwxr-xr-x   0 lmeadors   (501) staff       (20)      187 2020-11-27 14:00:28.000000 gitty-1.8.0/bin/gitty
+-rw-r--r--   0 lmeadors   (501) staff       (20)      113 2021-06-16 14:51:37.000000 gitty-1.8.0/bin/gitty_completion.zsh
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.285630 gitty-1.8.0/gitty/
+-rw-r--r--   0 lmeadors   (501) staff       (20)       29 2020-05-30 14:03:12.000000 gitty-1.8.0/gitty/__init__.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     2724 2020-08-25 22:53:29.000000 gitty-1.8.0/gitty/gitty_color.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)    19919 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_command.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1131 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_clean.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      536 2021-05-30 13:00:12.000000 gitty-1.8.0/gitty/gitty_command_head.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      511 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_help.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      800 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_parent.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1670 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_command_plugins.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     3019 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_release.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1159 2020-11-23 15:40:36.000000 gitty-1.8.0/gitty/gitty_command_show.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1471 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_task.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      478 2021-06-13 13:19:38.000000 gitty-1.8.0/gitty/gitty_command_version.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1904 2021-06-03 19:24:23.000000 gitty-1.8.0/gitty/gitty_executor.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     4237 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_git_api.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1539 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_project_type.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     4822 2022-03-16 12:26:49.000000 gitty-1.8.0/gitty/gitty_project_type_gradle_kotlin.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     5756 2021-08-08 18:38:51.000000 gitty-1.8.0/gitty/gitty_project_type_maven.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     3224 2021-08-08 18:38:51.000000 gitty-1.8.0/gitty/gitty_project_type_node.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     3714 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_project_type_pip.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     2770 2022-01-01 15:55:03.000000 gitty-1.8.0/gitty/gitty_project_type_xcode.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     4298 2024-05-30 21:01:31.000000 gitty-1.8.0/gitty/gitty_support.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      223 2020-08-25 22:53:29.000000 gitty-1.8.0/gitty/gitty_xml_tree_builder.py
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.288421 gitty-1.8.0/gitty.egg-info/
+-rw-r--r--   0 lmeadors   (501) staff       (20)     9799 2024-05-30 21:05:11.000000 gitty-1.8.0/gitty.egg-info/PKG-INFO
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1307 2024-05-30 21:05:11.000000 gitty-1.8.0/gitty.egg-info/SOURCES.txt
+-rw-r--r--   0 lmeadors   (501) staff       (20)        1 2024-05-30 21:05:11.000000 gitty-1.8.0/gitty.egg-info/dependency_links.txt
+-rw-r--r--   0 lmeadors   (501) staff       (20)       21 2024-05-30 21:05:11.000000 gitty-1.8.0/gitty.egg-info/top_level.txt
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.291658 gitty-1.8.0/plugin_samples/
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1211 2021-06-06 14:11:26.000000 gitty-1.8.0/plugin_samples/finish_task.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     2585 2022-03-16 12:21:44.000000 gitty-1.8.0/plugin_samples/merge_check.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     2118 2021-06-13 13:24:03.000000 gitty-1.8.0/plugin_samples/pull_request.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      790 2021-06-12 19:15:59.000000 gitty-1.8.0/plugin_samples/zsh_complete.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)       38 2024-05-30 21:05:11.306130 gitty-1.8.0/setup.cfg
+-rw-r--r--   0 lmeadors   (501) staff       (20)      884 2024-05-30 21:01:43.000000 gitty-1.8.0/setup.py
+drwxr-xr-x   0 lmeadors   (501) staff       (20)        0 2024-05-30 21:05:11.303126 gitty-1.8.0/tests/
+-rw-r--r--   0 lmeadors   (501) staff       (20)        0 2020-08-25 22:53:29.000000 gitty-1.8.0/tests/__init__.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      420 2020-08-25 22:53:29.000000 gitty-1.8.0/tests/test_gitty_color.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1227 2021-05-30 12:45:19.000000 gitty-1.8.0/tests/test_gitty_command.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     1860 2020-11-22 16:05:57.000000 gitty-1.8.0/tests/test_gitty_command_task.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      599 2020-08-25 22:53:29.000000 gitty-1.8.0/tests/test_gitty_command_version.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     5342 2020-11-21 11:49:05.000000 gitty-1.8.0/tests/test_gitty_git_api.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)      896 2020-08-25 22:53:29.000000 gitty-1.8.0/tests/test_gitty_project_type.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     2079 2021-05-30 12:46:20.000000 gitty-1.8.0/tests/test_gitty_project_type_base_test.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     9775 2021-05-30 12:50:40.000000 gitty-1.8.0/tests/test_gitty_project_type_maven.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     9462 2021-05-30 12:49:38.000000 gitty-1.8.0/tests/test_gitty_project_type_node.py
+-rw-r--r--   0 lmeadors   (501) staff       (20)     7511 2021-05-30 12:48:27.000000 gitty-1.8.0/tests/test_gitty_project_type_pip.py
```

### Comparing `gitty-1.7.0/PKG-INFO` & `gitty-1.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,277 @@
-Metadata-Version: 2.1
-Name: gitty
-Version: 1.7.0
-Summary: An alternate git workflow tool
-Home-page: https://github.com/lmeadors/gitty
-Author: Larry Meadors
-Author-email: larry.meadors@elm-software.com
-License: UNKNOWN
-Description: # gitty - a simple alternative to git flow with less rigidity
-        
-        
-        This project provides an easy way to deal with git branches in an environment with multiple parallel development streams.
-        
-        View download stats here: https://pypistats.org/packages/gitty
-        
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/gitty">
-        
-        ### Some assumptions:
-        
-        - the `master` branch is the cutting edge of new development
-        - release stabilization branches are created for each major and minor release
-        - semantic versioning will be used to track where we are
-        - projects are using either maven, python, or nodejs 
-        
-        # Some sample work flows...
-        
-        To get started, we'll make a new empty project using node. 
-        
-        Next, we'll walk through some common scenarios and see how to use this thing.
-        
-        ```shell script
-        % mkdir test-project
-        % cd test-project
-        % npm init --yes
-        % git init
-        % git add package.json
-        % git commit -m "initial commit"
-        ```
-        
-        Now, we have a blank project with a package.json file in it and nothing else.
-        
-        # current state of affairs (and some help)
-        
-        To see some useful info about your project, you can just run the gitty command.
-        
-        > I'm assuming that you installed gitty using pip from [https://pypi.org/project/gitty/](https://pypi.org/project/gitty/)
-        
-        ```shell script
-        -> % gitty
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.0.0
-        command name:    help
-        available commands on branch "master" are:
-        
-        cleanup: ['c', 'clean']
-          # tidy up the local repository - remove obsolete branches
-          # make sure the git repo has no outstanding changes
-          $ git fetch --all --prune
-          $ git pull --rebase
-          # remove select local branches that have been merged to master
-        ...and a LOT more output here...
-        ```
-        
-        This is telling you what gitty thinks the state of your project is, and what you can do.
-        
-        # new release stabilization branch
-        
-        Let's say that we're ready to snap a 1.0.0 release of our project. From the output above, you can see the "release" 
-        command and it can be run using either `gitty release` or just `gitty r`:
-        
-        ```shell script
-        -> % gitty r
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.0.0
-        command name:    r
-        $ git checkout -b 1.0/master
-        Switched to a new branch '1.0/master'
-        $ git checkout -b 1.0/releases
-        Switched to a new branch '1.0/releases'
-        bump version to 1.0.0
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.0"
-        b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
-        $ git tag 1.0.0
-        $ git checkout 1.0/master
-        Switched to branch '1.0/master'
-        $ git merge --strategy=ours 1.0/releases
-        bump version to 1.0.1
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.1"
-        $ git checkout master
-        Switched to branch 'master'
-        $ git merge --strategy=ours 1.0/master
-        bump version to 1.1.0
-        $ git add package.json
-        $ git commit -m "bumped version to 1.1.0"
-        ```
-        
-        Wow, that's a lot of crap.
-        
-        That's showing you what's happening when you create a release - why all that stuff? I'll fill in more details later, but for now: Because.
-        
-        At the end of that, you'll be back on `master` and there will be 2 new branches:
-        
-        ```shell script
-        -> % git branch
-          1.0/master
-          1.0/releases
-        * master
-        ```
-        
-        Those branches have purpose.
-        
-        The `1.0/master` branch is used to stabilize the 1.0 release; The `1.0/releases` branch is used to give us a stable 
-        point of reference in the future for things like hot fixes, etc.
-        
-        There's also a new tag:
-        
-        ```shell script
-        -> % git tag
-        1.0.0
-        ```
-        
-        That is on the releases branch, and specifically, on the commit where the release candidate should be built from.
-        
-        # new task for forward development
-        
-        This is a common thing - so it's pretty simple:
-        
-        ```shell script
-        -> % gitty t some_new_thing_here
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.1.0
-        command name:    t
-        $ git checkout -b tasks/some_new_thing_here
-        Switched to a new branch 'tasks/some_new_thing_here'
-        ```
-        
-        Chuck some code here and commit it and push it - eventually, you'll merge it back to `master` and it'll be real code. Yay.
-        
-        # new task for release stabilization branch
-        
-        Yeah, this doesn't sound like a great idea, but sometimes, it's needed.
-        
-        ```shell script
-        -> % gco 1.0/master
-        Switched to branch '1.0/master'
-        -> % gitty t some_new_task_for_10
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  1.0/master
-        project type:    node
-        current version: 1.0.1
-        command name:    t
-        $ git checkout -b 1.0/tasks/some_new_task_for_10
-        Switched to a new branch '1.0/tasks/some_new_task_for_10'
-        ```
-        
-        Now, you've created a branch from the `1.0/master` branch named `1.0/tasks/some_new_task_for_10` - the naming indicates 
-        where it will end up (although eventually, you'll most likely want to merge it to `master` too, for now, we'll just work on 1.0).
-        
-        # new release candidate for 1.0
-        
-        To make a new RC for the stabilization branch, do this:
-        
-        ```shell script
-        % gco 1.0/master
-        -> % gitty r
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  1.0/master
-        project type:    node
-        current version: 1.0.1
-        command name:    r
-        $ git checkout 1.0/releases
-        Switched to branch '1.0/releases'
-        $ git merge 1.0/master
-        bump version to 1.0.1
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.1"
-        b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
-        $ git tag 1.0.1
-        $ git checkout 1.0/master
-        Switched to branch '1.0/master'
-        $ git merge 1.0/releases
-        bump version to 1.0.2
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.2"
-        ```
-        
-        Again, that's a lot of output...but it's what's happening.
-        
-        Now, the `1.0/master` branch got merged to `1.0/release`, we have a new tag for the release candidate (`1.0.1`), and 
-        the `1.0/master` project file reflects that we're now working toward `1.0.2` for the next release candidate.
-        
-        > NOTE: Because we merge back to `1.0/master`, we have a single place to look for changes to be merged to version 1.1 (on `master`).
-        
-        # wrapping up a release to prepare for the next one
-        
-        Once release 1.0 has been released and we're ready to start on the road to 1.1 (and 1.2), we'll want to get all of the 1.0 changes merged back to `master` (where 1.1 lives). There's not much to do there, so we just use git:
-        
-        ```shell script
-        % git merge 1.0/master
-        Auto-merging package.json
-        CONFLICT (content): Merge conflict in package.json
-        Automatic merge failed; fix conflicts and then commit the result.
-        % (do what you need to do to merge the conflicts here)
-        % git add package.json
-        % git commit
-        ```
-        
-        Creating the next release is exactly the same as before:
-        
-        ```shell script
-        % gcm
-        % gitty r
-        ```
-        
-        You'll see a pile of output again, and at the end, there will be `1.1/master` and `1.1/release` branches and a new `1.1.0` tag for the release candidate.
-        
-        # Versioning for python projects (i.e., eating my own dog food)
-        
-        I'm using this tool to manage the git repository for this tool, so its versioning approach is the one that it supports.
-        
-        The versioning scheme is based on [semver 2.0.0](https://semver.org/spec/v2.0.0.html), and will use a suffix of "dev0" 
-        to indicate that a version is not a release (and partly because of how setuptools behaves).
-        
-        For this project, non-release builds will not be deployed to pypi - only actual releases will be deployed.
-        
-        This versioning will start as of version 1.2.0.dev0 (currently master).
-        
-        # plugins
-        
-        You can now make plugins for gitty - there are samples in the oh so cleverly named "plugin_samples" directory.
-        
-        I'll be documenting them more in the future, unless I die or win the lottery or get busy with other things.
-        
-        # tab completion plugin (zsh - experimental)
-        
-        I'm working on making this easier, but for now, to enable tab completion:
-        
-        1. install gitty 1.5 or later 
-        1. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
-        2. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
-        
-        This is a new feature starting with the 1.4 release. It seems to be working for me, but your mileage may vary - if 
-        it's broken, let me know, and I'll try to make it better.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# gitty - a simple alternative to git flow with less rigidity
+
+This project provides an easy way to deal with git branches in an environment with multiple parallel development streams.
+
+View download stats here: https://pypistats.org/packages/gitty
+
+<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/gitty">
+
+> It is worth noting that (like git flow), this is a tool to simplify the implementation of a workflow - you can do 
+> everything manually if you want to, so don't get too hung up on the tooling.
+
+# Some sample work flows...
+
+To get started, we'll make a new empty project using node. 
+
+### But first, some assumptions!
+
+- the `master` branch is the cutting edge of new development (we will see how to change that later)
+- release stabilization branches are created for each major and minor release
+- semantic versioning will be used to track where we are
+- projects are using a supported project type:
+  - maven - solid support
+  - python - I use it for this project, so it is probably adequate
+  - nodejs - experimental - try it and let me know
+  - gradle - expreimental - I am using it, but still with dev builds
+
+Next, we'll walk through some common scenarios and see how to use this thing.
+
+```shell script
+% mkdir test-project
+% cd test-project
+% npm init --yes
+% git init
+% git add package.json
+% git commit -m "initial commit"
+```
+
+Now, we have a blank project with a package.json file in it and nothing else.
+
+# current state of affairs (and some help)
+
+To see some useful info about your project, you can just run the gitty command.
+
+> I'm assuming that you installed gitty using pip from [https://pypi.org/project/gitty/](https://pypi.org/project/gitty/)
+
+```shell script
+-> % gitty
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.0.0
+command name:              head
+for help, try "gitty help"
+```
+
+This is telling you what gitty thinks the state of your project is, if you want more information, try `gitty help`.
+
+# new release stabilization branch
+
+Let's say that we're ready to snap a 1.0.0 release of our project. From the output above, you can see the "release" 
+command and it can be run using either `gitty release` or just `gitty r`:
+
+```shell script
+-> % gitty r
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.0.0
+command name:    r
+$ git checkout -b 1.0/master
+Switched to a new branch '1.0/master'
+$ git checkout -b 1.0/releases
+Switched to a new branch '1.0/releases'
+bump version to 1.0.0
+$ git add package.json
+$ git commit -m "bumped version to 1.0.0"
+b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
+$ git tag 1.0.0
+$ git checkout 1.0/master
+Switched to branch '1.0/master'
+$ git merge --strategy=ours 1.0/releases
+bump version to 1.0.1
+$ git add package.json
+$ git commit -m "bumped version to 1.0.1"
+$ git checkout master
+Switched to branch 'master'
+$ git merge --strategy=ours 1.0/master
+bump version to 1.1.0
+$ git add package.json
+$ git commit -m "bumped version to 1.1.0"
+```
+
+Wow, that's a lot of crap.
+
+That's showing you what's happening when you create a release - why all that stuff? I'll fill in more details later, but for now: Because.
+
+At the end of that, you'll be back on `master` and there will be 2 new branches:
+
+```shell script
+-> % git branch
+  1.0/master
+  1.0/releases
+* master
+```
+
+Those branches have purpose.
+
+The `1.0/master` branch is used to stabilize the 1.0 release; The `1.0/releases` branch is used to give us a stable 
+point of reference in the future for things like hot fixes, etc.
+
+There's also a new tag:
+
+```shell script
+-> % git tag
+1.0.0
+```
+
+That is on the releases branch, and specifically, on the commit where the release candidate should be built from.
+
+# new task for forward development
+
+This is a common thing - so it's pretty simple:
+
+```shell script
+-> % gitty t some_new_thing_here
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.1.0
+command name:    t
+$ git checkout -b tasks/some_new_thing_here
+Switched to a new branch 'tasks/some_new_thing_here'
+```
+
+Chuck some code here and commit it and push it - eventually, you'll merge it back to `master` and it'll be real code. Yay.
+
+# new task for release stabilization branch
+
+Yeah, this doesn't sound like a great idea, but sometimes, it's needed.
+
+```shell script
+-> % gco 1.0/master
+Switched to branch '1.0/master'
+-> % gitty t some_new_task_for_10
+$ git rev-parse --abbrev-ref HEAD
+current branch:  1.0/master
+project type:    node
+current version: 1.0.1
+command name:    t
+$ git checkout -b 1.0/tasks/some_new_task_for_10
+Switched to a new branch '1.0/tasks/some_new_task_for_10'
+```
+
+Now, you've created a branch from the `1.0/master` branch named `1.0/tasks/some_new_task_for_10` - the naming indicates 
+where it will end up (although eventually, you'll most likely want to merge it to `master` too, for now, we'll just work on 1.0).
+
+# new release candidate for 1.0
+
+To make a new RC for the stabilization branch, do this:
+
+```shell script
+% gco 1.0/master
+-> % gitty r
+$ git rev-parse --abbrev-ref HEAD
+current branch:  1.0/master
+project type:    node
+current version: 1.0.1
+command name:    r
+$ git checkout 1.0/releases
+Switched to branch '1.0/releases'
+$ git merge 1.0/master
+bump version to 1.0.1
+$ git add package.json
+$ git commit -m "bumped version to 1.0.1"
+b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
+$ git tag 1.0.1
+$ git checkout 1.0/master
+Switched to branch '1.0/master'
+$ git merge 1.0/releases
+bump version to 1.0.2
+$ git add package.json
+$ git commit -m "bumped version to 1.0.2"
+```
+
+Again, that's a lot of output...but it's what's happening.
+
+Now, the `1.0/master` branch got merged to `1.0/release`, we have a new tag for the release candidate (`1.0.1`), and 
+the `1.0/master` project file reflects that we're now working toward `1.0.2` for the next release candidate.
+
+> NOTE: Because we merge back to `1.0/master`, we have a single place to look for changes to be merged to version 1.1 (on `master`).
+
+# wrapping up a release to prepare for the next one
+
+Once release 1.0 has been released and we're ready to start on the road to 1.1 (and 1.2), we'll want to get all of the 1.0 changes merged back to `master` (where 1.1 lives). There's not much to do there, so we just use git:
+
+```shell script
+% git merge 1.0/master
+Auto-merging package.json
+CONFLICT (content): Merge conflict in package.json
+Automatic merge failed; fix conflicts and then commit the result.
+% (do what you need to do to merge the conflicts here)
+% git add package.json
+% git commit
+```
+
+Creating the next release is exactly the same as before:
+
+```shell script
+% gcm
+% gitty r
+```
+
+You'll see a pile of output again, and at the end, there will be `1.1/master` and `1.1/release` branches and a new `1.1.0` tag for the release candidate.
+
+# Versioning for python projects (i.e., eating my own dog food)
+
+I'm using this tool to manage the git repository for this tool, so its versioning approach is the one that it supports.
+
+The versioning scheme is based on [semver 2.0.0](https://semver.org/spec/v2.0.0.html), and will use a suffix of "dev0" 
+to indicate that a version is not a release (and partly because of how setuptools behaves).
+
+For this project, non-release builds will not be deployed to pypi - only actual releases will be deployed.
+
+This versioning will start as of version 1.2.0.dev0 (currently master).
+
+# plugins
+
+You can now make plugins for gitty - there are samples in the oh so cleverly named "plugin_samples" directory.
+
+I'll be documenting them more in the future, unless I die or win the lottery or get busy with other things.
+
+# EXPERIMENTAL: tab completion plugin (zsh)
+
+I'm working on making this easier, but for now, to enable tab completion:
+
+1. install gitty 1.5 or later 
+2. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
+3. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
+
+This is a new feature starting with the 1.4 release. It seems to be working for me, but your mileage may vary - if 
+it's broken, let me know, and I'll try to make it better.
+
+> UPDATE: I have been using this for a few months - it seems to work fine.
+
+# EXPERIMENTAL: How can I use different branch names? I do not have a "master" branch...
+
+I have a few projects like this, too - 
+
+This should work, but I may have missed a few spots.
+ 
+Create a file named `.gittyrc` in your project directory (or your home directory if you want this to be a global 
+default) - you can override some settings with it. For example, if you just want to call your `master` 
+branch `main` instead:
+
+```
+trunk=main
+```
+
+Your working (trunk) branch(es) would be named "main"; tasks would be named "tasks/...", and releases would live 
+on "release" branches.
+
+If you really miss git flow, you can even do this:
+
+```
+trunk=develop
+tasks=features
+release=master
+```
+
+This will give you a hybrid of gitflow and gitty:
+
+- your "working branches" will be either `develop` or `x.y/develop`
+- releases will live on `x.y/master`
+- task branches will live on either `features/...` or `x.y/features/...`
+
+Because the gitty process has no concept of a "hotfix" (every release can be a hotfix; every version can be patched), 
+there is no need for those extra branch names.
```

### Comparing `gitty-1.7.0/README.md` & `gitty-1.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,46 @@
-# gitty - a simple alternative to git flow with less rigidity
+Metadata-Version: 2.1
+Name: gitty
+Version: 1.8.0
+Summary: An alternate git workflow tool
+Home-page: https://github.com/lmeadors/gitty
+Author: Larry Meadors
+Author-email: larry.meadors@elm-software.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 
+# gitty - a simple alternative to git flow with less rigidity
 
 This project provides an easy way to deal with git branches in an environment with multiple parallel development streams.
 
 View download stats here: https://pypistats.org/packages/gitty
 
 <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/gitty">
 
-### Some assumptions:
-
-- the `master` branch is the cutting edge of new development
-- release stabilization branches are created for each major and minor release
-- semantic versioning will be used to track where we are
-- projects are using either maven, python, or nodejs 
+> It is worth noting that (like git flow), this is a tool to simplify the implementation of a workflow - you can do 
+> everything manually if you want to, so don't get too hung up on the tooling.
 
 # Some sample work flows...
 
 To get started, we'll make a new empty project using node. 
 
+### But first, some assumptions!
+
+- the `master` branch is the cutting edge of new development (we will see how to change that later)
+- release stabilization branches are created for each major and minor release
+- semantic versioning will be used to track where we are
+- projects are using a supported project type:
+  - maven - solid support
+  - python - I use it for this project, so it is probably adequate
+  - nodejs - experimental - try it and let me know
+  - gradle - expreimental - I am using it, but still with dev builds
+
 Next, we'll walk through some common scenarios and see how to use this thing.
 
 ```shell script
 % mkdir test-project
 % cd test-project
 % npm init --yes
 % git init
@@ -39,27 +58,19 @@
 
 ```shell script
 -> % gitty
 $ git rev-parse --abbrev-ref HEAD
 current branch:  master
 project type:    node
 current version: 1.0.0
-command name:    help
-available commands on branch "master" are:
-
-cleanup: ['c', 'clean']
-  # tidy up the local repository - remove obsolete branches
-  # make sure the git repo has no outstanding changes
-  $ git fetch --all --prune
-  $ git pull --rebase
-  # remove select local branches that have been merged to master
-...and a LOT more output here...
+command name:              head
+for help, try "gitty help"
 ```
 
-This is telling you what gitty thinks the state of your project is, and what you can do.
+This is telling you what gitty thinks the state of your project is, if you want more information, try `gitty help`.
 
 # new release stabilization branch
 
 Let's say that we're ready to snap a 1.0.0 release of our project. From the output above, you can see the "release" 
 command and it can be run using either `gitty release` or just `gitty r`:
 
 ```shell script
@@ -227,17 +238,53 @@
 
 # plugins
 
 You can now make plugins for gitty - there are samples in the oh so cleverly named "plugin_samples" directory.
 
 I'll be documenting them more in the future, unless I die or win the lottery or get busy with other things.
 
-# tab completion plugin (zsh - experimental)
+# EXPERIMENTAL: tab completion plugin (zsh)
 
 I'm working on making this easier, but for now, to enable tab completion:
 
 1. install gitty 1.5 or later 
-1. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
-2. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
+2. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
+3. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
 
 This is a new feature starting with the 1.4 release. It seems to be working for me, but your mileage may vary - if 
 it's broken, let me know, and I'll try to make it better.
+
+> UPDATE: I have been using this for a few months - it seems to work fine.
+
+# EXPERIMENTAL: How can I use different branch names? I do not have a "master" branch...
+
+I have a few projects like this, too - 
+
+This should work, but I may have missed a few spots.
+ 
+Create a file named `.gittyrc` in your project directory (or your home directory if you want this to be a global 
+default) - you can override some settings with it. For example, if you just want to call your `master` 
+branch `main` instead:
+
+```
+trunk=main
+```
+
+Your working (trunk) branch(es) would be named "main"; tasks would be named "tasks/...", and releases would live 
+on "release" branches.
+
+If you really miss git flow, you can even do this:
+
+```
+trunk=develop
+tasks=features
+release=master
+```
+
+This will give you a hybrid of gitflow and gitty:
+
+- your "working branches" will be either `develop` or `x.y/develop`
+- releases will live on `x.y/master`
+- task branches will live on either `features/...` or `x.y/features/...`
+
+Because the gitty process has no concept of a "hotfix" (every release can be a hotfix; every version can be patched), 
+there is no need for those extra branch names.
```

### Comparing `gitty-1.7.0/gitty/gitty_color.py` & `gitty-1.8.0/gitty/gitty_color.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command.py` & `gitty-1.8.0/gitty/gitty_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pkg_resources  # part of setuptools
+# import importlib.metadata
 import subprocess
 from .gitty_color import Color
 from .gitty_executor import DescribeExecutor, CommandExecutor
 
 from .gitty_project_type import *
 
 
@@ -94,14 +95,15 @@
             context[key] = None
 
     # now that we know what kind of project we have, get the version info from it
     GittyCommand.get_version_info(context)
 
     # add the current gitty version to the context
     context['gitty_version'] = pkg_resources.require("gitty")[0].version
+    # context['gitty_version'] = importlib.metadata.version("gitty")
 
 
 class GittyCommand:
 
     # the title of the command
     _title = 'base'
```

### Comparing `gitty-1.7.0/gitty/gitty_command_clean.py` & `gitty-1.8.0/gitty/gitty_command_clean.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command_head.py` & `gitty-1.8.0/gitty/gitty_command_head.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command_parent.py` & `gitty-1.8.0/gitty/gitty_command_parent.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command_plugins.py` & `gitty-1.8.0/gitty/gitty_command_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import importlib
+# import importlib
 from pathlib import Path
 from gitty import GittyCommand, Color
 
 
 class GittyPlugins(GittyCommand):
     _title = 'plugins'
     _name = 'list installed plugins'
```

### Comparing `gitty-1.7.0/gitty/gitty_command_release.py` & `gitty-1.8.0/gitty/gitty_command_release.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command_show.py` & `gitty-1.8.0/gitty/gitty_command_show.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_command_task.py` & `gitty-1.8.0/gitty/gitty_command_task.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_executor.py` & `gitty-1.8.0/gitty/gitty_executor.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_git_api.py` & `gitty-1.8.0/gitty/gitty_git_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,22 @@
             context,
             'git rev-parse --abbrev-ref HEAD'.split(),
             quiet,
             raise_error=True
         )
         return current_branch
 
+    def get_root_path(self, context):
+        # git rev-parse --show-toplevel
+        return self.command_executor.execute_immutable_command(
+            context,
+            'git rev-parse --show-toplevel'.split(),
+            quiet=True
+        )
+
     def git_remote(self, context, quiet=False):
         return self.command_executor.execute_immutable_command(
             context,
             'git remote'.split(),
             quiet=quiet
         )
```

### Comparing `gitty-1.7.0/gitty/gitty_project_type.py` & `gitty-1.8.0/gitty/gitty_project_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xml.etree import ElementTree
 # noinspection PyUnresolvedReferences
 # this is so distutils doesn't complain about being imported before setuptools...apparently that's frowned upon.
-import setuptools
+# import setuptools
 
 
 class GittyProjectType:
 
     def get_name(self):
         return 'None'
```

### Comparing `gitty-1.7.0/gitty/gitty_project_type_gradle_kotlin.py` & `gitty-1.8.0/gitty/gitty_project_type_gradle_kotlin.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,37 +10,41 @@
         return 'gradle (w/ kotlin)'
 
     def is_in_use(self, context):
         is_gradle = path.exists('settings.gradle.kts')
         if is_gradle:
             context['project_type_name'] = self.get_name()
             context['project_file'] = 'settings.gradle.kts'
+        # print("**** GRADLE ****")
         return is_gradle
 
     def get_version_info(self, context):
         # start at the project file
         main_project_file = context['project_file']
         # print("starting at {}".format(main_project_file))
         # find the "include" line
         include_line = ''
         with open(main_project_file) as file:
             for line in file:
                 line = line.strip()
                 if line.strip().startswith('include'):
                     include_line = line
-        app_path = ''
+                    app_path = include_line.split('"')[1]
+                elif line.strip().startswith('rootProject.name'):
+                    include_line = line
+                    app_path = '.'
+
         # TODO: this will need some attention for multi-build projects; we
         #  will want to make it possible to deal with more than one build
         #  file - that will be a nice feature - i think we just want a list
         #  of project files and would only support keeping the version
         #  numbers in lockstep (initially, at least). (I suspect xcode
         #  support would benefit from this as well).
-        if len(include_line) > 0:
-            # print('include line: {}'.format(include_line))
-            app_path = include_line.split('"')[1]
+        # print('app path is: {}'.format(app_path))
+
         if len(app_path) > 0:
             # now we have our actual config file and can
             # start setting things up...
             app_file_name = path.join(app_path, 'build.gradle.kts')
             context['project_file'] = app_file_name
             # print('app file: {}'.format(app_file_name))
             with open(app_file_name) as app_file:
```

### Comparing `gitty-1.7.0/gitty/gitty_project_type_maven.py` & `gitty-1.8.0/gitty/gitty_project_type_maven.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_project_type_node.py` & `gitty-1.8.0/gitty/gitty_project_type_node.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_project_type_pip.py` & `gitty-1.8.0/gitty/gitty_project_type_pip.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 class GittyPip(GittyProjectType):
 
     def get_name(self):
         return 'pip'
 
     def is_in_use(self, context):
-        is_pip = path.exists('setup.py')
+        git_api = context['git_api']
+        project_file = '/'.join([(git_api.get_root_path(context)), 'setup.py'])
+        is_pip = path.exists(project_file)
         if is_pip:
             context['project_type_name'] = self.get_name()
-            context['project_file'] = 'setup.py'
+            context['project_file'] = project_file
         return is_pip
 
     def get_version_info(self, context):
 
         # load what we know from the setup file
         setup = run_setup(context['project_file'], stop_after='config')
         current_version = setup.metadata.version
```

### Comparing `gitty-1.7.0/gitty/gitty_project_type_xcode.py` & `gitty-1.8.0/gitty/gitty_project_type_xcode.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/gitty/gitty_support.py` & `gitty-1.8.0/gitty/gitty_support.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import os
 from pathlib import Path
 
 from gitty.gitty_command import *
 import sys
 
+from gitty.gitty_git_api import GitAPI
+
 
 def setup(context):
 
     # look for .gittyrc files - they can live in 2 places:
     # - the user's home directory
     # - the current working directory (CWD)
     # if both exist and define overlapping values, the one in the CWD is used
     # these are the global defaults
+    if 'git_api' not in context:
+        context['executor'] = CommandExecutor()
+        context['git_api'] = GitAPI(context["executor"])
     grc_config = {
         'trunk': 'master',
         'task_prefix': 'tasks',
         'release_prefix': 'releases'
     }
     home_config_location = os.path.join(Path.home(), ".gittyrc")
-    local_config_location = ".gittyrc"
+    git_api = context['git_api']
+    local_config_location = '/'.join([(git_api.get_root_path(context)), ".gittyrc"])
     if os.path.exists(home_config_location):
         with open(home_config_location) as f:
             for line in f:
                 (key, val) = line.split("=")
                 grc_config[key] = val.strip()
 
     if os.path.exists(local_config_location):
```

### Comparing `gitty-1.7.0/gitty.egg-info/PKG-INFO` & `gitty-1.8.0/gitty.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,258 +1,290 @@
 Metadata-Version: 2.1
 Name: gitty
-Version: 1.7.0
+Version: 1.8.0
 Summary: An alternate git workflow tool
 Home-page: https://github.com/lmeadors/gitty
 Author: Larry Meadors
 Author-email: larry.meadors@elm-software.com
-License: UNKNOWN
-Description: # gitty - a simple alternative to git flow with less rigidity
-        
-        
-        This project provides an easy way to deal with git branches in an environment with multiple parallel development streams.
-        
-        View download stats here: https://pypistats.org/packages/gitty
-        
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/gitty">
-        
-        ### Some assumptions:
-        
-        - the `master` branch is the cutting edge of new development
-        - release stabilization branches are created for each major and minor release
-        - semantic versioning will be used to track where we are
-        - projects are using either maven, python, or nodejs 
-        
-        # Some sample work flows...
-        
-        To get started, we'll make a new empty project using node. 
-        
-        Next, we'll walk through some common scenarios and see how to use this thing.
-        
-        ```shell script
-        % mkdir test-project
-        % cd test-project
-        % npm init --yes
-        % git init
-        % git add package.json
-        % git commit -m "initial commit"
-        ```
-        
-        Now, we have a blank project with a package.json file in it and nothing else.
-        
-        # current state of affairs (and some help)
-        
-        To see some useful info about your project, you can just run the gitty command.
-        
-        > I'm assuming that you installed gitty using pip from [https://pypi.org/project/gitty/](https://pypi.org/project/gitty/)
-        
-        ```shell script
-        -> % gitty
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.0.0
-        command name:    help
-        available commands on branch "master" are:
-        
-        cleanup: ['c', 'clean']
-          # tidy up the local repository - remove obsolete branches
-          # make sure the git repo has no outstanding changes
-          $ git fetch --all --prune
-          $ git pull --rebase
-          # remove select local branches that have been merged to master
-        ...and a LOT more output here...
-        ```
-        
-        This is telling you what gitty thinks the state of your project is, and what you can do.
-        
-        # new release stabilization branch
-        
-        Let's say that we're ready to snap a 1.0.0 release of our project. From the output above, you can see the "release" 
-        command and it can be run using either `gitty release` or just `gitty r`:
-        
-        ```shell script
-        -> % gitty r
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.0.0
-        command name:    r
-        $ git checkout -b 1.0/master
-        Switched to a new branch '1.0/master'
-        $ git checkout -b 1.0/releases
-        Switched to a new branch '1.0/releases'
-        bump version to 1.0.0
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.0"
-        b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
-        $ git tag 1.0.0
-        $ git checkout 1.0/master
-        Switched to branch '1.0/master'
-        $ git merge --strategy=ours 1.0/releases
-        bump version to 1.0.1
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.1"
-        $ git checkout master
-        Switched to branch 'master'
-        $ git merge --strategy=ours 1.0/master
-        bump version to 1.1.0
-        $ git add package.json
-        $ git commit -m "bumped version to 1.1.0"
-        ```
-        
-        Wow, that's a lot of crap.
-        
-        That's showing you what's happening when you create a release - why all that stuff? I'll fill in more details later, but for now: Because.
-        
-        At the end of that, you'll be back on `master` and there will be 2 new branches:
-        
-        ```shell script
-        -> % git branch
-          1.0/master
-          1.0/releases
-        * master
-        ```
-        
-        Those branches have purpose.
-        
-        The `1.0/master` branch is used to stabilize the 1.0 release; The `1.0/releases` branch is used to give us a stable 
-        point of reference in the future for things like hot fixes, etc.
-        
-        There's also a new tag:
-        
-        ```shell script
-        -> % git tag
-        1.0.0
-        ```
-        
-        That is on the releases branch, and specifically, on the commit where the release candidate should be built from.
-        
-        # new task for forward development
-        
-        This is a common thing - so it's pretty simple:
-        
-        ```shell script
-        -> % gitty t some_new_thing_here
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  master
-        project type:    node
-        current version: 1.1.0
-        command name:    t
-        $ git checkout -b tasks/some_new_thing_here
-        Switched to a new branch 'tasks/some_new_thing_here'
-        ```
-        
-        Chuck some code here and commit it and push it - eventually, you'll merge it back to `master` and it'll be real code. Yay.
-        
-        # new task for release stabilization branch
-        
-        Yeah, this doesn't sound like a great idea, but sometimes, it's needed.
-        
-        ```shell script
-        -> % gco 1.0/master
-        Switched to branch '1.0/master'
-        -> % gitty t some_new_task_for_10
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  1.0/master
-        project type:    node
-        current version: 1.0.1
-        command name:    t
-        $ git checkout -b 1.0/tasks/some_new_task_for_10
-        Switched to a new branch '1.0/tasks/some_new_task_for_10'
-        ```
-        
-        Now, you've created a branch from the `1.0/master` branch named `1.0/tasks/some_new_task_for_10` - the naming indicates 
-        where it will end up (although eventually, you'll most likely want to merge it to `master` too, for now, we'll just work on 1.0).
-        
-        # new release candidate for 1.0
-        
-        To make a new RC for the stabilization branch, do this:
-        
-        ```shell script
-        % gco 1.0/master
-        -> % gitty r
-        $ git rev-parse --abbrev-ref HEAD
-        current branch:  1.0/master
-        project type:    node
-        current version: 1.0.1
-        command name:    r
-        $ git checkout 1.0/releases
-        Switched to branch '1.0/releases'
-        $ git merge 1.0/master
-        bump version to 1.0.1
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.1"
-        b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
-        $ git tag 1.0.1
-        $ git checkout 1.0/master
-        Switched to branch '1.0/master'
-        $ git merge 1.0/releases
-        bump version to 1.0.2
-        $ git add package.json
-        $ git commit -m "bumped version to 1.0.2"
-        ```
-        
-        Again, that's a lot of output...but it's what's happening.
-        
-        Now, the `1.0/master` branch got merged to `1.0/release`, we have a new tag for the release candidate (`1.0.1`), and 
-        the `1.0/master` project file reflects that we're now working toward `1.0.2` for the next release candidate.
-        
-        > NOTE: Because we merge back to `1.0/master`, we have a single place to look for changes to be merged to version 1.1 (on `master`).
-        
-        # wrapping up a release to prepare for the next one
-        
-        Once release 1.0 has been released and we're ready to start on the road to 1.1 (and 1.2), we'll want to get all of the 1.0 changes merged back to `master` (where 1.1 lives). There's not much to do there, so we just use git:
-        
-        ```shell script
-        % git merge 1.0/master
-        Auto-merging package.json
-        CONFLICT (content): Merge conflict in package.json
-        Automatic merge failed; fix conflicts and then commit the result.
-        % (do what you need to do to merge the conflicts here)
-        % git add package.json
-        % git commit
-        ```
-        
-        Creating the next release is exactly the same as before:
-        
-        ```shell script
-        % gcm
-        % gitty r
-        ```
-        
-        You'll see a pile of output again, and at the end, there will be `1.1/master` and `1.1/release` branches and a new `1.1.0` tag for the release candidate.
-        
-        # Versioning for python projects (i.e., eating my own dog food)
-        
-        I'm using this tool to manage the git repository for this tool, so its versioning approach is the one that it supports.
-        
-        The versioning scheme is based on [semver 2.0.0](https://semver.org/spec/v2.0.0.html), and will use a suffix of "dev0" 
-        to indicate that a version is not a release (and partly because of how setuptools behaves).
-        
-        For this project, non-release builds will not be deployed to pypi - only actual releases will be deployed.
-        
-        This versioning will start as of version 1.2.0.dev0 (currently master).
-        
-        # plugins
-        
-        You can now make plugins for gitty - there are samples in the oh so cleverly named "plugin_samples" directory.
-        
-        I'll be documenting them more in the future, unless I die or win the lottery or get busy with other things.
-        
-        # tab completion plugin (zsh - experimental)
-        
-        I'm working on making this easier, but for now, to enable tab completion:
-        
-        1. install gitty 1.5 or later 
-        1. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
-        2. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
-        
-        This is a new feature starting with the 1.4 release. It seems to be working for me, but your mileage may vary - if 
-        it's broken, let me know, and I'll try to make it better.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# gitty - a simple alternative to git flow with less rigidity
+
+This project provides an easy way to deal with git branches in an environment with multiple parallel development streams.
+
+View download stats here: https://pypistats.org/packages/gitty
+
+<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/gitty">
+
+> It is worth noting that (like git flow), this is a tool to simplify the implementation of a workflow - you can do 
+> everything manually if you want to, so don't get too hung up on the tooling.
+
+# Some sample work flows...
+
+To get started, we'll make a new empty project using node. 
+
+### But first, some assumptions!
+
+- the `master` branch is the cutting edge of new development (we will see how to change that later)
+- release stabilization branches are created for each major and minor release
+- semantic versioning will be used to track where we are
+- projects are using a supported project type:
+  - maven - solid support
+  - python - I use it for this project, so it is probably adequate
+  - nodejs - experimental - try it and let me know
+  - gradle - expreimental - I am using it, but still with dev builds
+
+Next, we'll walk through some common scenarios and see how to use this thing.
+
+```shell script
+% mkdir test-project
+% cd test-project
+% npm init --yes
+% git init
+% git add package.json
+% git commit -m "initial commit"
+```
+
+Now, we have a blank project with a package.json file in it and nothing else.
+
+# current state of affairs (and some help)
+
+To see some useful info about your project, you can just run the gitty command.
+
+> I'm assuming that you installed gitty using pip from [https://pypi.org/project/gitty/](https://pypi.org/project/gitty/)
+
+```shell script
+-> % gitty
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.0.0
+command name:              head
+for help, try "gitty help"
+```
+
+This is telling you what gitty thinks the state of your project is, if you want more information, try `gitty help`.
+
+# new release stabilization branch
+
+Let's say that we're ready to snap a 1.0.0 release of our project. From the output above, you can see the "release" 
+command and it can be run using either `gitty release` or just `gitty r`:
+
+```shell script
+-> % gitty r
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.0.0
+command name:    r
+$ git checkout -b 1.0/master
+Switched to a new branch '1.0/master'
+$ git checkout -b 1.0/releases
+Switched to a new branch '1.0/releases'
+bump version to 1.0.0
+$ git add package.json
+$ git commit -m "bumped version to 1.0.0"
+b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
+$ git tag 1.0.0
+$ git checkout 1.0/master
+Switched to branch '1.0/master'
+$ git merge --strategy=ours 1.0/releases
+bump version to 1.0.1
+$ git add package.json
+$ git commit -m "bumped version to 1.0.1"
+$ git checkout master
+Switched to branch 'master'
+$ git merge --strategy=ours 1.0/master
+bump version to 1.1.0
+$ git add package.json
+$ git commit -m "bumped version to 1.1.0"
+```
+
+Wow, that's a lot of crap.
+
+That's showing you what's happening when you create a release - why all that stuff? I'll fill in more details later, but for now: Because.
+
+At the end of that, you'll be back on `master` and there will be 2 new branches:
+
+```shell script
+-> % git branch
+  1.0/master
+  1.0/releases
+* master
+```
+
+Those branches have purpose.
+
+The `1.0/master` branch is used to stabilize the 1.0 release; The `1.0/releases` branch is used to give us a stable 
+point of reference in the future for things like hot fixes, etc.
+
+There's also a new tag:
+
+```shell script
+-> % git tag
+1.0.0
+```
+
+That is on the releases branch, and specifically, on the commit where the release candidate should be built from.
+
+# new task for forward development
+
+This is a common thing - so it's pretty simple:
+
+```shell script
+-> % gitty t some_new_thing_here
+$ git rev-parse --abbrev-ref HEAD
+current branch:  master
+project type:    node
+current version: 1.1.0
+command name:    t
+$ git checkout -b tasks/some_new_thing_here
+Switched to a new branch 'tasks/some_new_thing_here'
+```
+
+Chuck some code here and commit it and push it - eventually, you'll merge it back to `master` and it'll be real code. Yay.
+
+# new task for release stabilization branch
+
+Yeah, this doesn't sound like a great idea, but sometimes, it's needed.
+
+```shell script
+-> % gco 1.0/master
+Switched to branch '1.0/master'
+-> % gitty t some_new_task_for_10
+$ git rev-parse --abbrev-ref HEAD
+current branch:  1.0/master
+project type:    node
+current version: 1.0.1
+command name:    t
+$ git checkout -b 1.0/tasks/some_new_task_for_10
+Switched to a new branch '1.0/tasks/some_new_task_for_10'
+```
+
+Now, you've created a branch from the `1.0/master` branch named `1.0/tasks/some_new_task_for_10` - the naming indicates 
+where it will end up (although eventually, you'll most likely want to merge it to `master` too, for now, we'll just work on 1.0).
+
+# new release candidate for 1.0
+
+To make a new RC for the stabilization branch, do this:
+
+```shell script
+% gco 1.0/master
+-> % gitty r
+$ git rev-parse --abbrev-ref HEAD
+current branch:  1.0/master
+project type:    node
+current version: 1.0.1
+command name:    r
+$ git checkout 1.0/releases
+Switched to branch '1.0/releases'
+$ git merge 1.0/master
+bump version to 1.0.1
+$ git add package.json
+$ git commit -m "bumped version to 1.0.1"
+b'On branch 1.0/releases\nnothing to commit, working tree clean\n'
+$ git tag 1.0.1
+$ git checkout 1.0/master
+Switched to branch '1.0/master'
+$ git merge 1.0/releases
+bump version to 1.0.2
+$ git add package.json
+$ git commit -m "bumped version to 1.0.2"
+```
+
+Again, that's a lot of output...but it's what's happening.
+
+Now, the `1.0/master` branch got merged to `1.0/release`, we have a new tag for the release candidate (`1.0.1`), and 
+the `1.0/master` project file reflects that we're now working toward `1.0.2` for the next release candidate.
+
+> NOTE: Because we merge back to `1.0/master`, we have a single place to look for changes to be merged to version 1.1 (on `master`).
+
+# wrapping up a release to prepare for the next one
+
+Once release 1.0 has been released and we're ready to start on the road to 1.1 (and 1.2), we'll want to get all of the 1.0 changes merged back to `master` (where 1.1 lives). There's not much to do there, so we just use git:
+
+```shell script
+% git merge 1.0/master
+Auto-merging package.json
+CONFLICT (content): Merge conflict in package.json
+Automatic merge failed; fix conflicts and then commit the result.
+% (do what you need to do to merge the conflicts here)
+% git add package.json
+% git commit
+```
+
+Creating the next release is exactly the same as before:
+
+```shell script
+% gcm
+% gitty r
+```
+
+You'll see a pile of output again, and at the end, there will be `1.1/master` and `1.1/release` branches and a new `1.1.0` tag for the release candidate.
+
+# Versioning for python projects (i.e., eating my own dog food)
+
+I'm using this tool to manage the git repository for this tool, so its versioning approach is the one that it supports.
+
+The versioning scheme is based on [semver 2.0.0](https://semver.org/spec/v2.0.0.html), and will use a suffix of "dev0" 
+to indicate that a version is not a release (and partly because of how setuptools behaves).
+
+For this project, non-release builds will not be deployed to pypi - only actual releases will be deployed.
+
+This versioning will start as of version 1.2.0.dev0 (currently master).
+
+# plugins
+
+You can now make plugins for gitty - there are samples in the oh so cleverly named "plugin_samples" directory.
+
+I'll be documenting them more in the future, unless I die or win the lottery or get busy with other things.
+
+# EXPERIMENTAL: tab completion plugin (zsh)
+
+I'm working on making this easier, but for now, to enable tab completion:
+
+1. install gitty 1.5 or later 
+2. download https://raw.githubusercontent.com/lmeadors/gitty/master/plugin_samples/zsh_complete.py to ~/.gitty/
+3. create a symlink to `/usr/local/bin/gitty_completion.zsh` in your zsh custom directory
+
+This is a new feature starting with the 1.4 release. It seems to be working for me, but your mileage may vary - if 
+it's broken, let me know, and I'll try to make it better.
+
+> UPDATE: I have been using this for a few months - it seems to work fine.
+
+# EXPERIMENTAL: How can I use different branch names? I do not have a "master" branch...
+
+I have a few projects like this, too - 
+
+This should work, but I may have missed a few spots.
+ 
+Create a file named `.gittyrc` in your project directory (or your home directory if you want this to be a global 
+default) - you can override some settings with it. For example, if you just want to call your `master` 
+branch `main` instead:
+
+```
+trunk=main
+```
+
+Your working (trunk) branch(es) would be named "main"; tasks would be named "tasks/...", and releases would live 
+on "release" branches.
+
+If you really miss git flow, you can even do this:
+
+```
+trunk=develop
+tasks=features
+release=master
+```
+
+This will give you a hybrid of gitflow and gitty:
+
+- your "working branches" will be either `develop` or `x.y/develop`
+- releases will live on `x.y/master`
+- task branches will live on either `features/...` or `x.y/features/...`
+
+Because the gitty process has no concept of a "hotfix" (every release can be a hotfix; every version can be patched), 
+there is no need for those extra branch names.
```

### Comparing `gitty-1.7.0/gitty.egg-info/SOURCES.txt` & `gitty-1.8.0/gitty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/plugin_samples/finish_task.py` & `gitty-1.8.0/plugin_samples/finish_task.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/plugin_samples/merge_check.py` & `gitty-1.8.0/plugin_samples/merge_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     _bindings = ['merge-check']
     _steps = [
         # CommentStep('merge branch %s', ['current_branch']),
         CommentStep('update all local branches (using hub sync)', []),
         # GitCommandStep('hub sync', []),
         HubSyncTask(),
         GitCleanStep(),
-        CommentStep('go to master branch', []),
+        CommentStep('go to main trunk branch (%s)', ['trunk']),
         GitCheckoutMasterCommand(),
         GitCleanStep(),
         GitShowUnmergedBranchesStep(),
     ]
 
     def get_description(self, context):
         description = []
```

### Comparing `gitty-1.7.0/plugin_samples/pull_request.py` & `gitty-1.8.0/plugin_samples/pull_request.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/plugin_samples/zsh_complete.py` & `gitty-1.8.0/plugin_samples/zsh_complete.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/setup.py` & `gitty-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gitty",
-    version="1.7.0",
+    version="1.8.0",
     author="Larry Meadors",
     author_email="larry.meadors@elm-software.com",
     description="An alternate git workflow tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lmeadors/gitty",
     packages=['gitty', 'plugin_samples'],
```

### Comparing `gitty-1.7.0/tests/test_gitty_command.py` & `gitty-1.8.0/tests/test_gitty_command.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_command_task.py` & `gitty-1.8.0/tests/test_gitty_command_task.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_command_version.py` & `gitty-1.8.0/tests/test_gitty_command_version.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_git_api.py` & `gitty-1.8.0/tests/test_gitty_git_api.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_project_type.py` & `gitty-1.8.0/tests/test_gitty_project_type.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_project_type_base_test.py` & `gitty-1.8.0/tests/test_gitty_project_type_base_test.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_project_type_maven.py` & `gitty-1.8.0/tests/test_gitty_project_type_maven.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_project_type_node.py` & `gitty-1.8.0/tests/test_gitty_project_type_node.py`

 * *Files identical despite different names*

### Comparing `gitty-1.7.0/tests/test_gitty_project_type_pip.py` & `gitty-1.8.0/tests/test_gitty_project_type_pip.py`

 * *Files identical despite different names*

