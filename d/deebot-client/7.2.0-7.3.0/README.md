# Comparing `tmp/deebot_client-7.2.0.tar.gz` & `tmp/deebot_client-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot_client-7.2.0.tar", last modified: Fri May 10 10:22:14 2024, max compression
+gzip compressed data, was "deebot_client-7.3.0.tar", last modified: Thu May 30 07:52:01 2024, max compression
```

## Comparing `deebot_client-7.2.0.tar` & `deebot_client-7.3.0.tar`

### file list

```diff
@@ -1,229 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-10 10:22:09.000000 deebot_client-7.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-10 10:22:14.105971 deebot_client-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 10:22:09.000000 deebot_client-7.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.085971 deebot_client-7.2.0/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clear_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/relocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/event_bus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/efficiency_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/work_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/hardware/deebot/
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/2o4lnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/55aiho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/5xu9h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/626v6g.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/77atlz.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/85nbtp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/9ku8nu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/clojes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/e6ofmn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/itk04l.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/lf3bn4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/lx3j7m.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/p1jij8.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/p95mgv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/paeygf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/rss8xk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/umwv6z.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/vi829v.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/x5d34r.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/yna5xi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/zjavof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23602 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/deebot_client/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/deebot_client/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/countries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-10 10:22:09.000000 deebot_client-7.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-10 10:22:09.000000 deebot_client-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-10 10:22:09.000000 deebot_client-7.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-10 10:22:09.000000 deebot_client-7.2.0/scripts/check_getLogger.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-10 10:22:09.000000 deebot_client-7.2.0/scripts/run-in-env.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:22:14.105971 deebot_client-7.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.101971 deebot_client-7.2.0/tests/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/mqtt_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/hardware/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/helpers/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/mqtt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_mqtt_client_reconnect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_countries.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.205519 deebot_client-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.173518 deebot_client-7.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.173518 deebot_client-7.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.173518 deebot_client-7.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-30 07:51:55.000000 deebot_client-7.3.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-30 07:51:55.000000 deebot_client-7.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-30 07:52:01.201519 deebot_client-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-30 07:51:55.000000 deebot_client-7.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.173518 deebot_client-7.3.0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.177518 deebot_client-7.3.0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.181518 deebot_client-7.3.0/deebot_client/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/clear_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/cut_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/json/work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.185518 deebot_client-7.3.0/deebot_client/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/commands/xml/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/event_bus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.185518 deebot_client-7.3.0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/efficiency_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/events/work_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.185518 deebot_client-7.3.0/deebot_client/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.189518 deebot_client-7.3.0/deebot_client/hardware/deebot/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/2ap5uq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/2o4lnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/55aiho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/5xu9h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/626v6g.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/77atlz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/85nbtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/9ku8nu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/9s1s80.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/clojes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/e6ofmn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/guzput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/itk04l.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/lf3bn4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/lx3j7m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/p1jij8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/p95mgv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/paeygf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/rss8xk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/umwv6z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/vi829v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/x5d34r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/yna5xi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/hardware/deebot/zjavof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.189518 deebot_client-7.3.0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.189518 deebot_client-7.3.0/deebot_client/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/messages/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/messages/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/messages/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.193518 deebot_client-7.3.0/deebot_client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/util/continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 07:51:55.000000 deebot_client-7.3.0/deebot_client/util/countries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-30 07:52:01.000000 deebot_client-7.3.0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-30 07:52:01.000000 deebot_client-7.3.0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:52:01.000000 deebot_client-7.3.0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 07:52:01.000000 deebot_client-7.3.0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 07:52:01.000000 deebot_client-7.3.0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 07:51:55.000000 deebot_client-7.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-30 07:51:55.000000 deebot_client-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 07:51:55.000000 deebot_client-7.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 07:51:55.000000 deebot_client-7.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 07:51:55.000000 deebot_client-7.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 07:51:55.000000 deebot_client-7.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.193518 deebot_client-7.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-30 07:51:55.000000 deebot_client-7.3.0/scripts/check_getLogger.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-30 07:51:55.000000 deebot_client-7.3.0/scripts/run-in-env.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:52:01.205519 deebot_client-7.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.193518 deebot_client-7.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.193518 deebot_client-7.3.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.197518 deebot_client-7.3.0/tests/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_cut_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/json/test_work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/xml/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/xml/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/xml/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/commands/xml/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/fixtures/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/fixtures/mqtt_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/hardware/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/helpers/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/json/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/mqtt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/test_mqtt_client_reconnect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:52:01.201519 deebot_client-7.3.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/util/test_continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/util/test_countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-30 07:51:55.000000 deebot_client-7.3.0/tests/util/test_init.py
```

### Comparing `deebot_client-7.2.0/.devcontainer.json` & `deebot_client-7.3.0/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `deebot_client-7.3.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.github/release-drafter.yml` & `deebot_client-7.3.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.github/workflows/ci.yml` & `deebot_client-7.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.github/workflows/codeql-analysis.yml` & `deebot_client-7.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.github/workflows/python-publish.yml` & `deebot_client-7.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/.pre-commit-config.yaml` & `deebot_client-7.3.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     - verifyNoGetLogger
 
 default_language_version:
   python: python3.12
 
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.3
+    rev: v0.4.5
     hooks:
       - id: ruff
         args:
           - --fix
           # - --unsafe-fixes
       - id: ruff-format
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args:
           - --py312-plus
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.6
+    rev: v2.3.0
     hooks:
       - id: codespell
         args:
           - --ignore-words-list=deebot
           - --skip="./.*,*.csv,*.json"
           - --quiet-level=2
           - --exclude-file=deebot_client/util/continents.py
```

### Comparing `deebot_client-7.2.0/.yamllint` & `deebot_client-7.3.0/.yamllint`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/LICENSE.txt` & `deebot_client-7.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/PKG-INFO` & `deebot_client-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 7.2.0
+Version: 7.3.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
```

### Comparing `deebot_client-7.2.0/README.md` & `deebot_client-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/api_client.py` & `deebot_client-7.3.0/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/authentication.py` & `deebot_client-7.3.0/deebot_client/authentication.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/capabilities.py` & `deebot_client-7.3.0/deebot_client/capabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ChildLockEvent,
     CleanCountEvent,
     CleanLogEvent,
     CleanPreferenceEvent,
     ContinuousCleaningEvent,
     CrossMapBorderWarningEvent,
     CustomCommandEvent,
+    CutDirectionEvent,
     ErrorEvent,
     Event,
     FanSpeedEvent,
     FanSpeedLevel,
     LifeSpan,
     LifeSpanEvent,
     MajorMapEvent,
@@ -185,14 +186,15 @@
     advanced_mode: CapabilitySetEnable[AdvancedModeEvent]
     carpet_auto_fan_boost: CapabilitySetEnable[CarpetAutoFanBoostEvent] | None = None
     efficiency_mode: CapabilitySetTypes[EfficiencyModeEvent, EfficiencyMode] | None = (
         None
     )
     border_switch: CapabilitySetEnable[BorderSwitchEvent] | None = None
     child_lock: CapabilitySetEnable[ChildLockEvent] | None = None
+    cut_direction: CapabilitySet[CutDirectionEvent, int] | None = None
     moveup_warning: CapabilitySetEnable[MoveUpWarningEvent] | None = None
     cross_map_border_warning: CapabilitySetEnable[CrossMapBorderWarningEvent] | None = (
         None
     )
     safe_protect: CapabilitySetEnable[SafeProtectEvent] | None = None
     ota: CapabilitySetEnable[OtaEvent] | CapabilityEvent[OtaEvent] | None = None
     sweep_mode: CapabilitySetEnable[SweepModeEvent] | None = None
```

### Comparing `deebot_client-7.2.0/deebot_client/command.py` & `deebot_client-7.3.0/deebot_client/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 from abc import ABC, abstractmethod
 import asyncio
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, final
 
 from deebot_client.events import AvailabilityEvent
-from deebot_client.exceptions import ApiTimeoutError, DeebotError
+from deebot_client.exceptions import (
+    ApiTimeoutError,
+    DeebotError,
+)
 
 from .const import PATH_API_IOT_DEVMANAGER, REQUEST_HEADERS, DataType
 from .logging_filter import get_logger
 from .message import HandlingResult, HandlingState, Message
 
 if TYPE_CHECKING:
     from types import MappingProxyType
@@ -37,14 +40,30 @@
 
     @classmethod
     def analyse(cls) -> CommandResult:
         """Create result with handling analyse."""
         return CommandResult(HandlingState.ANALYSE)
 
 
+@dataclass(frozen=True)
+class DeviceCommandResult:
+    """Device command result object.
+
+    Returns
+    -------
+        device_reached (bool): True if the command was targeting the bot, and it responded in time. False otherwise.
+                               This value is not indicating if the command was executed successfully.
+        raw_response (dict[str, Any]): The command response data.
+
+    """
+
+    device_reached: bool
+    raw_response: dict[str, Any] = field(default_factory=dict)
+
+
 class Command(ABC):
     """Abstract command object."""
 
     _targets_bot: bool = True
 
     def __init__(self, args: dict[str, Any] | list[Any] | None = None) -> None:
         if args is None:
@@ -69,73 +88,74 @@
 
     @final
     async def execute(
         self,
         authenticator: Authenticator,
         device_info: ApiDeviceInfo,
         event_bus: EventBus,
-    ) -> bool:
-        """Execute command.
-
-        Returns
-        -------
-            bot_reached (bool): True if the command was targeting the bot, and it responded in time. False otherwise.
-                                This value is not indicating if the command was executed successfully.
-
-        """
+    ) -> DeviceCommandResult:
+        """Execute command."""
         try:
-            result = await self._execute(authenticator, device_info, event_bus)
+            result, response = await self._execute(
+                authenticator, device_info, event_bus
+            )
             if result.state == HandlingState.SUCCESS:
                 # Execute command which are requested by the handler
                 async with asyncio.TaskGroup() as tg:
                     for requested_command in result.requested_commands:
                         tg.create_task(
                             requested_command.execute(
                                 authenticator, device_info, event_bus
                             )
                         )
 
-                return self._targets_bot
+                return DeviceCommandResult(
+                    device_reached=self._targets_bot, raw_response=response
+                )
+
         except Exception:  # pylint: disable=broad-except
             _LOGGER.warning(
                 "Could not execute command %s",
                 self.name,
                 exc_info=True,
             )
-        return False
+        return DeviceCommandResult(device_reached=False)
 
     async def _execute(
         self,
         authenticator: Authenticator,
         device_info: ApiDeviceInfo,
         event_bus: EventBus,
-    ) -> CommandResult:
+    ) -> tuple[CommandResult, dict[str, Any]]:
         """Execute command."""
         try:
             response = await self._execute_api_request(authenticator, device_info)
         except ApiTimeoutError:
             _LOGGER.warning(
                 "Could not execute command %s: Timeout reached",
                 self.name,
             )
-            return CommandResult(HandlingState.ERROR)
+            return CommandResult(HandlingState.ERROR), {}
 
         result = self.__handle_response(event_bus, response)
         if result.state == HandlingState.ANALYSE:
             _LOGGER.debug(
                 "ANALYSE: Could not handle command: %s with %s", self.name, response
             )
-            return CommandResult(
-                HandlingState.ANALYSE_LOGGED,
-                result.args,
-                result.requested_commands,
+            return (
+                CommandResult(
+                    HandlingState.ANALYSE_LOGGED,
+                    result.args,
+                    result.requested_commands,
+                ),
+                response,
             )
         if result.state == HandlingState.ERROR:
             _LOGGER.warning("Could not parse %s: %s", self.name, response)
-        return result
+        return result, response
 
     async def _execute_api_request(
         self, authenticator: Authenticator, device_info: ApiDeviceInfo
     ) -> dict[str, Any]:
         payload = {
             "cmdName": self.name,
             "payload": self._get_payload(),
@@ -256,14 +276,15 @@
 
 @dataclass
 class InitParam:
     """Init param."""
 
     type_: type
     name: str | None = None
+    optional: bool = field(default=False, kw_only=True)
 
 
 class CommandMqttP2P(Command, ABC):
     """Command which can handle mqtt p2p messages."""
 
     _mqtt_params: MappingProxyType[str, InitParam | None]
 
@@ -279,28 +300,29 @@
             raise DeebotError("_mqtt_params not set")
 
         for name, param in cls._mqtt_params.items():
             if param is None:
                 # Remove field
                 data.pop(name, None)
             else:
-                values[param.name or name] = _pop_or_raise(name, param.type_, data)
+                try:
+                    values[param.name or name] = _pop_or_raise(name, param.type_, data)
+                except KeyError as err:
+                    if not param.optional:
+                        msg = f'"{name}" is missing in {data}'
+                        raise DeebotError(msg) from err
 
         if data:
             _LOGGER.debug("Following data will be ignored: %s", data)
 
         return cls(**values)
 
 
 def _pop_or_raise(name: str, type_: type, data: dict[str, Any]) -> Any:
-    try:
-        value = data.pop(name)
-    except KeyError as err:
-        msg = f'"{name}" is missing in {data}'
-        raise DeebotError(msg) from err
+    value = data.pop(name)
     try:
         return type_(value)
     except ValueError as err:
         msg = f'Could not convert "{value}" of {name} into {type_}'
         raise DeebotError(msg) from err
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/__init__.py` & `deebot_client-7.3.0/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/__init__.py` & `deebot_client-7.3.0/deebot_client/commands/json/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .clean import Clean, CleanArea, CleanV2, GetCleanInfo, GetCleanInfoV2
 from .clean_count import GetCleanCount, SetCleanCount
 from .clean_logs import GetCleanLogs
 from .clean_preference import GetCleanPreference, SetCleanPreference
 from .clear_map import ClearMap
 from .continuous_cleaning import GetContinuousCleaning, SetContinuousCleaning
 from .cross_map_border_warning import GetCrossMapBorderWarning, SetCrossMapBorderWarning
+from .cut_direction import GetCutDirection, SetCutDirection
 from .efficiency import GetEfficiencyMode, SetEfficiencyMode
 from .error import GetError
 from .fan_speed import GetFanSpeed, SetFanSpeed
 from .life_span import GetLifeSpan, ResetLifeSpan
 from .map import (
     GetCachedMapInfo,
     GetMajorMap,
@@ -73,14 +74,16 @@
     "CleanV2",
     "CleanArea",
     "GetCleanInfo",
     "GetCleanInfoV2",
     "GetCleanLogs",
     "GetContinuousCleaning",
     "SetContinuousCleaning",
+    "SetCutDirection",
+    "GetCutDirection",
     "GetCrossMapBorderWarning",
     "SetCrossMapBorderWarning",
     "GetEfficiencyMode",
     "SetEfficiencyMode",
     "GetError",
     "GetFanSpeed",
     "SetFanSpeed",
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/carpet.py` & `deebot_client-7.3.0/deebot_client/commands/json/carpet.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/charge.py` & `deebot_client-7.3.0/deebot_client/commands/json/charge.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/charge_state.py` & `deebot_client-7.3.0/deebot_client/commands/json/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/clean.py` & `deebot_client-7.3.0/deebot_client/commands/json/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         super().__init__(self._get_args(action))
 
     async def _execute(
         self,
         authenticator: Authenticator,
         device_info: ApiDeviceInfo,
         event_bus: EventBus,
-    ) -> CommandResult:
+    ) -> tuple[CommandResult, dict[str, Any]]:
         """Execute command."""
         state = event_bus.get_last_event(StateEvent)
         if state and isinstance(self._args, dict):
             if (
                 self._args["act"] == CleanAction.RESUME.value
                 and state.state != State.PAUSED
             ):
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/clean_count.py` & `deebot_client-7.3.0/deebot_client/commands/json/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/clean_logs.py` & `deebot_client-7.3.0/deebot_client/commands/json/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/common.py` & `deebot_client-7.3.0/deebot_client/commands/json/common.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/continuous_cleaning.py` & `deebot_client-7.3.0/deebot_client/commands/json/continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/cross_map_border_warning.py` & `deebot_client-7.3.0/deebot_client/commands/json/cross_map_border_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/custom.py` & `deebot_client-7.3.0/deebot_client/commands/json/custom.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/efficiency.py` & `deebot_client-7.3.0/deebot_client/commands/json/efficiency.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/error.py` & `deebot_client-7.3.0/deebot_client/commands/json/error.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,20 +24,25 @@
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
-        codes = data.get("code", [])
+        codes = data.get("code")
+        if not isinstance(codes, list):
+            return HandlingResult.analyse()
+
+        error: int | None = 0
+
         if codes:
             # the last error code
             error = codes[-1]
 
-            if error is not None:
-                description = ERROR_CODES.get(error)
-                if error != 0:
-                    event_bus.notify(StateEvent(State.ERROR))
-                event_bus.notify(ErrorEvent(error, description))
-                return HandlingResult.success()
+        if error is not None:
+            description = ERROR_CODES.get(error)
+            if error != 0:
+                event_bus.notify(StateEvent(State.ERROR))
+            event_bus.notify(ErrorEvent(error, description))
+            return HandlingResult.success()
 
         return HandlingResult.analyse()
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/fan_speed.py` & `deebot_client-7.3.0/deebot_client/commands/json/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/life_span.py` & `deebot_client-7.3.0/deebot_client/commands/json/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/map.py` & `deebot_client-7.3.0/deebot_client/commands/json/map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/network.py` & `deebot_client-7.3.0/deebot_client/commands/json/network.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/ota.py` & `deebot_client-7.3.0/deebot_client/commands/json/ota.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/pos.py` & `deebot_client-7.3.0/deebot_client/commands/json/pos.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,21 +36,25 @@
 
             if isinstance(data_positions, dict):
                 positions.append(
                     Position(
                         type=PositionType(type_str),
                         x=data_positions["x"],
                         y=data_positions["y"],
+                        a=data_positions.get("a", 0),
                     )
                 )
             else:
                 positions.extend(
                     [
                         Position(
-                            type=PositionType(type_str), x=entry["x"], y=entry["y"]
+                            type=PositionType(type_str),
+                            x=entry["x"],
+                            y=entry["y"],
+                            a=entry.get("a", 0),
                         )
                         for entry in data_positions
                     ]
                 )
 
         if positions:
             event_bus.notify(PositionsEvent(positions=positions))
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/stats.py` & `deebot_client-7.3.0/deebot_client/commands/json/stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/voice_assistant_state.py` & `deebot_client-7.3.0/deebot_client/commands/json/voice_assistant_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/volume.py` & `deebot_client-7.3.0/deebot_client/commands/json/volume.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/water_info.py` & `deebot_client-7.3.0/deebot_client/commands/json/water_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
-from deebot_client.events import WaterAmount, WaterInfoEvent
+from deebot_client.events import SweepType, WaterAmount, WaterInfoEvent
 from deebot_client.message import HandlingResult
 from deebot_client.util import get_enum
 
 from .common import JsonGetCommand, JsonSetCommand
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
@@ -29,29 +29,45 @@
 
         :return: A message response
         """
         mop_attached = data.get("enable")
         if mop_attached is not None:
             mop_attached = bool(mop_attached)
 
+        if sweep_type := data.get("sweepType"):
+            sweep_type = SweepType(int(sweep_type))
+
         event_bus.notify(
-            WaterInfoEvent(WaterAmount(int(data["amount"])), mop_attached=mop_attached)
+            WaterInfoEvent(
+                WaterAmount(int(data["amount"])),
+                sweep_type,
+                mop_attached=mop_attached,
+            )
         )
         return HandlingResult.success()
 
 
 class SetWaterInfo(JsonSetCommand):
     """Set water info command."""
 
     name = "setWaterInfo"
     get_command = GetWaterInfo
     _mqtt_params = MappingProxyType(
         {
             "amount": InitParam(WaterAmount),
             "enable": None,  # Remove it as we don't can set it (App includes it)
+            "sweepType": InitParam(SweepType, "sweep_type", optional=True),
         }
     )
 
-    def __init__(self, amount: WaterAmount | str) -> None:
+    def __init__(
+        self, amount: WaterAmount | str, sweep_type: SweepType | str | None = None
+    ) -> None:
+        params = {}
         if isinstance(amount, str):
             amount = get_enum(WaterAmount, amount)
-        super().__init__({"amount": amount.value})
+        params["amount"] = amount.value
+        if sweep_type:
+            if isinstance(sweep_type, str):
+                sweep_type = get_enum(SweepType, sweep_type)
+            params["sweepType"] = sweep_type.value
+        super().__init__(params)
```

### Comparing `deebot_client-7.2.0/deebot_client/commands/json/work_mode.py` & `deebot_client-7.3.0/deebot_client/commands/json/work_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/__init__.py` & `deebot_client-7.3.0/deebot_client/commands/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/charge_state.py` & `deebot_client-7.3.0/deebot_client/commands/xml/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/common.py` & `deebot_client-7.3.0/deebot_client/commands/xml/common.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/error.py` & `deebot_client-7.3.0/deebot_client/commands/xml/error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/fan_speed.py` & `deebot_client-7.3.0/deebot_client/commands/xml/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/commands/xml/pos.py` & `deebot_client-7.3.0/deebot_client/commands/xml/pos.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,12 +27,15 @@
         :return: A message response
         """
         if xml.attrib.get("ret") != "ok" or xml.attrib.get("t") != "p":
             return HandlingResult.analyse()
 
         if p := xml.attrib.get("p"):
             p_x, p_y = p.split(",", 2)
-            position = Position(type=PositionType.DEEBOT, x=int(p_x), y=int(p_y))
+            p_a = xml.attrib.get("a", 0)
+            position = Position(
+                type=PositionType.DEEBOT, x=int(p_x), y=int(p_y), a=int(p_a)
+            )
             event_bus.notify(PositionsEvent(positions=[position]))
             return HandlingResult.success()
 
         return HandlingResult.analyse()
```

### Comparing `deebot_client-7.2.0/deebot_client/device.py` & `deebot_client-7.3.0/deebot_client/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Device module."""
 
 from __future__ import annotations
 
 import asyncio
+from collections.abc import Callable, Coroutine
 from contextlib import suppress
 from datetime import datetime
 import json
 from typing import TYPE_CHECKING, Any, Final, Generic
 
 from deebot_client.events.network import NetworkInfoEvent
 from deebot_client.mqtt_client import MqttClient, SubscriberInfo
 from deebot_client.util import cancel
 
+from .command import Command
 from .event_bus import EventBus
 from .events import (
     AvailabilityEvent,
     CleanLogEvent,
     CustomCommandEvent,
     LifeSpanEvent,
     PositionsEvent,
@@ -26,23 +28,24 @@
 )
 from .logging_filter import get_logger
 from .map import Map
 from .messages import get_message
 from .models import DeviceCapabilities, DeviceInfo, State
 
 if TYPE_CHECKING:
-    from collections.abc import Callable
-
     from .authentication import Authenticator
-    from .command import Command
+    from .command import DeviceCommandResult
 
 _LOGGER = get_logger(__name__)
 _AVAILABLE_CHECK_INTERVAL = 60
 
 
+DeviceCommandExecute = Callable[[Command], Coroutine[Any, Any, dict[str, Any]]]
+
+
 class Device(Generic[DeviceCapabilities]):
     """Device representation."""
 
     def __init__(
         self,
         device_info: DeviceInfo[DeviceCapabilities],
         authenticator: Authenticator,
@@ -103,17 +106,23 @@
         self.events.subscribe(CustomCommandEvent, on_custom_command)
 
         async def on_network(event: NetworkInfoEvent) -> None:
             self.mac = event.mac
 
         self.events.subscribe(NetworkInfoEvent, on_network)
 
-    async def execute_command(self, command: Command) -> None:
-        """Execute given command."""
-        await self._execute_command(command)
+    async def execute_command(self, command: Command) -> dict[str, Any]:
+        """Execute given command.
+
+        Returns
+        -------
+            command_response (dict[str, Any]) The command raw response.
+
+        """
+        return (await self._execute_command(command)).raw_response
 
     async def initialize(self, client: MqttClient) -> None:
         """Initialize vacumm bot, which includes MQTT-subscription and starting the available check."""
         if self._unsubscribe is None:
             self._unsubscribe = await client.subscribe(
                 SubscriberInfo(self.device_info, self.events, self._handle_message)
             )
@@ -143,33 +152,36 @@
                 try:
                     for command in self.capabilities.get_refresh_commands(
                         AvailabilityEvent
                     ):
                         tasks.add(asyncio.create_task(self._execute_command(command)))
 
                     result = await asyncio.gather(*tasks)
-                    self._set_available(available=all(result))
+                    self._set_available(available=all(r.device_reached for r in result))
                 except Exception:  # pylint: disable=broad-exception-caught
                     _LOGGER.debug(
                         "An exception occurred during the available check",
                         exc_info=True,
                     )
                     await cancel(tasks)
             await asyncio.sleep(_AVAILABLE_CHECK_INTERVAL)
 
-    async def _execute_command(self, command: Command) -> bool:
+    async def _execute_command(
+        self,
+        command: Command,
+    ) -> DeviceCommandResult:
         """Execute given command."""
         async with self._semaphore:
-            if await command.execute(
+            result = await command.execute(
                 self._authenticator, self.device_info, self.events
-            ):
+            )
+            if result.device_reached:
                 self._set_available(available=True)
-                return True
 
-        return False
+            return result
 
     def _set_available(self, *, available: bool) -> None:
         """Set available."""
         if available:
             self._last_time_available = datetime.now()
 
         self.events.notify(AvailabilityEvent(available=available))
```

### Comparing `deebot_client-7.2.0/deebot_client/event_bus.py` & `deebot_client-7.3.0/deebot_client/event_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .models import State
 from .util import cancel, create_task
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Coroutine
 
     from .command import Command
+    from .device import DeviceCommandExecute
 
 _LOGGER = get_logger(__name__)
 
 T = TypeVar("T", bound=Event)
 
 
 class _OnSubscriptionCallback:
@@ -59,15 +60,15 @@
 
 
 class EventBus:
     """A very simple event bus system."""
 
     def __init__(
         self,
-        execute_command: Callable[[Command], Coroutine[Any, Any, None]],
+        execute_command: DeviceCommandExecute,
         get_refresh_commands: Callable[[type[Event]], list[Command]],
     ) -> None:
         self._event_processing_dict: dict[type[Event], _EventProcessingData[Any]] = {}
         self._lock = threading.Lock()
         self._tasks: set[asyncio.Future[Any]] = set()
 
         self._execute_command: Final = execute_command
```

### Comparing `deebot_client-7.2.0/deebot_client/events/__init__.py` & `deebot_client-7.3.0/deebot_client/events/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     MapTraceEvent,
     MinorMapEvent,
     Position,
     PositionsEvent,
     PositionType,
 )
 from .network import NetworkInfoEvent
-from .water_info import WaterAmount, WaterInfoEvent
+from .water_info import SweepType, WaterAmount, WaterInfoEvent
 from .work_mode import WorkMode, WorkModeEvent
 
 if TYPE_CHECKING:
     from deebot_client.models import Room, State
 
 __all__ = [
     "BatteryEvent",
@@ -48,14 +48,15 @@
     "MapTraceEvent",
     "MinorMapEvent",
     "NetworkInfoEvent",
     "Position",
     "PositionType",
     "PositionsEvent",
     "SweepModeEvent",
+    "SweepType",
     "WaterAmount",
     "WaterInfoEvent",
     "WorkMode",
     "WorkModeEvent",
 ]
 
 
@@ -131,14 +132,18 @@
     ROUND_MOP = "roundMop"
     AIR_FRESHENER = "dModule"
     UV_SANITIZER = "uv"
     HUMIDIFY = "humidify"
     HUMIDIFY_MAINTENANCE = "wbCare"
     BLADE = "blade"
     LENS_BRUSH = "lensBrush"
+    DUST_BAG = "dustBag"
+    CLEANING_FLUID = "autoWater_cleaningFluid"
+    STRAINER = "strainer"
+    HAND_FILTER = "handFilter"
 
 
 @dataclass(frozen=True)
 class LifeSpanEvent(Event):
     """Life span event representation."""
 
     type: LifeSpan
@@ -279,7 +284,14 @@
 class MoveUpWarningEvent(EnableEvent):
     """Move up warning event."""
 
 
 @dataclass(frozen=True)
 class SafeProtectEvent(EnableEvent):
     """Safe protect event."""
+
+
+@dataclass(frozen=True)
+class CutDirectionEvent(Event):
+    """Cut direction event representation."""
+
+    angle: int
```

### Comparing `deebot_client-7.2.0/deebot_client/events/map.py` & `deebot_client-7.3.0/deebot_client/events/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 @dataclass(frozen=True)
 class Position:
     """Position representation."""
 
     type: PositionType
     x: int
     y: int
+    a: int
 
 
 @dataclass(frozen=True)
 class PositionsEvent(Event):
     """Position event representation."""
 
     positions: list[Position]
```

### Comparing `deebot_client-7.2.0/deebot_client/exceptions.py` & `deebot_client-7.3.0/deebot_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/2o4lnm.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/2o4lnm.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/55aiho.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/55aiho.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/5xu9h3.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/2ap5uq.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     CapabilityStats,
     MowerCapabilities,
 )
 from deebot_client.commands.json import (
     GetBorderSwitch,
     GetChildLock,
     GetCrossMapBorderWarning,
+    GetCutDirection,
     GetMoveUpWarning,
     GetSafeProtect,
     SetBorderSwitch,
     SetChildLock,
     SetCrossMapBorderWarning,
+    SetCutDirection,
     SetMoveUpWarning,
     SetSafeProtect,
 )
 from deebot_client.commands.json.advanced_mode import GetAdvancedMode, SetAdvancedMode
 from deebot_client.commands.json.battery import GetBattery
 from deebot_client.commands.json.charge import Charge
 from deebot_client.commands.json.charge_state import GetChargeState
@@ -45,14 +47,15 @@
     AdvancedModeEvent,
     AvailabilityEvent,
     BatteryEvent,
     BorderSwitchEvent,
     ChildLockEvent,
     CrossMapBorderWarningEvent,
     CustomCommandEvent,
+    CutDirectionEvent,
     ErrorEvent,
     LifeSpan,
     LifeSpanEvent,
     MoveUpWarningEvent,
     NetworkInfoEvent,
     ReportStatsEvent,
     SafeProtectEvent,
@@ -100,14 +103,17 @@
         settings=CapabilitySettings(
             advanced_mode=CapabilitySetEnable(
                 AdvancedModeEvent, [GetAdvancedMode()], SetAdvancedMode
             ),
             border_switch=CapabilitySetEnable(
                 BorderSwitchEvent, [GetBorderSwitch()], SetBorderSwitch
             ),
+            cut_direction=CapabilitySet(
+                CutDirectionEvent, [GetCutDirection()], SetCutDirection
+            ),
             child_lock=CapabilitySetEnable(
                 ChildLockEvent, [GetChildLock()], SetChildLock
             ),
             moveup_warning=CapabilitySetEnable(
                 MoveUpWarningEvent, [GetMoveUpWarning()], SetMoveUpWarning
             ),
             cross_map_border_warning=CapabilitySetEnable(
```

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/626v6g.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/626v6g.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/77atlz.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/5xu9h3.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     CapabilityStats,
     MowerCapabilities,
 )
 from deebot_client.commands.json import (
     GetBorderSwitch,
     GetChildLock,
     GetCrossMapBorderWarning,
+    GetCutDirection,
     GetMoveUpWarning,
     GetSafeProtect,
     SetBorderSwitch,
     SetChildLock,
     SetCrossMapBorderWarning,
+    SetCutDirection,
     SetMoveUpWarning,
     SetSafeProtect,
 )
 from deebot_client.commands.json.advanced_mode import GetAdvancedMode, SetAdvancedMode
 from deebot_client.commands.json.battery import GetBattery
 from deebot_client.commands.json.charge import Charge
 from deebot_client.commands.json.charge_state import GetChargeState
@@ -45,14 +47,15 @@
     AdvancedModeEvent,
     AvailabilityEvent,
     BatteryEvent,
     BorderSwitchEvent,
     ChildLockEvent,
     CrossMapBorderWarningEvent,
     CustomCommandEvent,
+    CutDirectionEvent,
     ErrorEvent,
     LifeSpan,
     LifeSpanEvent,
     MoveUpWarningEvent,
     NetworkInfoEvent,
     ReportStatsEvent,
     SafeProtectEvent,
@@ -100,14 +103,17 @@
         settings=CapabilitySettings(
             advanced_mode=CapabilitySetEnable(
                 AdvancedModeEvent, [GetAdvancedMode()], SetAdvancedMode
             ),
             border_switch=CapabilitySetEnable(
                 BorderSwitchEvent, [GetBorderSwitch()], SetBorderSwitch
             ),
+            cut_direction=CapabilitySet(
+                CutDirectionEvent, [GetCutDirection()], SetCutDirection
+            ),
             child_lock=CapabilitySetEnable(
                 ChildLockEvent, [GetChildLock()], SetChildLock
             ),
             moveup_warning=CapabilitySetEnable(
                 MoveUpWarningEvent, [GetMoveUpWarning()], SetMoveUpWarning
             ),
             cross_map_border_warning=CapabilitySetEnable(
```

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/85nbtp.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/85nbtp.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/9ku8nu.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/9ku8nu.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/__init__.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/clojes.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/clojes.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/e6ofmn.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/e6ofmn.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,12 +216,11 @@
             event=WaterInfoEvent,
             get=[GetWaterInfo()],
             set=SetWaterInfo,
             types=(
                 WaterAmount.LOW,
                 WaterAmount.MEDIUM,
                 WaterAmount.HIGH,
-                WaterAmount.ULTRAHIGH,
             ),
         ),
     ),
 )
```

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/fallback.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/fallback.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/itk04l.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/77atlz.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     CapabilityStats,
     MowerCapabilities,
 )
 from deebot_client.commands.json import (
     GetBorderSwitch,
     GetChildLock,
     GetCrossMapBorderWarning,
+    GetCutDirection,
     GetMoveUpWarning,
     GetSafeProtect,
     SetBorderSwitch,
     SetChildLock,
     SetCrossMapBorderWarning,
+    SetCutDirection,
     SetMoveUpWarning,
     SetSafeProtect,
 )
 from deebot_client.commands.json.advanced_mode import GetAdvancedMode, SetAdvancedMode
 from deebot_client.commands.json.battery import GetBattery
 from deebot_client.commands.json.charge import Charge
 from deebot_client.commands.json.charge_state import GetChargeState
@@ -45,14 +47,15 @@
     AdvancedModeEvent,
     AvailabilityEvent,
     BatteryEvent,
     BorderSwitchEvent,
     ChildLockEvent,
     CrossMapBorderWarningEvent,
     CustomCommandEvent,
+    CutDirectionEvent,
     ErrorEvent,
     LifeSpan,
     LifeSpanEvent,
     MoveUpWarningEvent,
     NetworkInfoEvent,
     ReportStatsEvent,
     SafeProtectEvent,
@@ -100,14 +103,17 @@
         settings=CapabilitySettings(
             advanced_mode=CapabilitySetEnable(
                 AdvancedModeEvent, [GetAdvancedMode()], SetAdvancedMode
             ),
             border_switch=CapabilitySetEnable(
                 BorderSwitchEvent, [GetBorderSwitch()], SetBorderSwitch
             ),
+            cut_direction=CapabilitySet(
+                CutDirectionEvent, [GetCutDirection()], SetCutDirection
+            ),
             child_lock=CapabilitySetEnable(
                 ChildLockEvent, [GetChildLock()], SetChildLock
             ),
             moveup_warning=CapabilitySetEnable(
                 MoveUpWarningEvent, [GetMoveUpWarning()], SetMoveUpWarning
             ),
             cross_map_border_warning=CapabilitySetEnable(
```

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/lf3bn4.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/lf3bn4.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,12 +216,11 @@
             event=WaterInfoEvent,
             get=[GetWaterInfo()],
             set=SetWaterInfo,
             types=(
                 WaterAmount.LOW,
                 WaterAmount.MEDIUM,
                 WaterAmount.HIGH,
-                WaterAmount.ULTRAHIGH,
             ),
         ),
     ),
 )
```

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/lx3j7m.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/lx3j7m.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/p1jij8.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/p1jij8.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/p95mgv.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/p95mgv.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/paeygf.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/paeygf.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/rss8xk.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/rss8xk.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/umwv6z.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/umwv6z.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/vi829v.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/vi829v.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/x5d34r.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/x5d34r.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/yna5xi.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/yna5xi.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/hardware/deebot/zjavof.py` & `deebot_client-7.3.0/deebot_client/hardware/deebot/zjavof.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/logging_filter.py` & `deebot_client-7.3.0/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/map.py` & `deebot_client-7.3.0/deebot_client/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 from .util import (
     OnChangedDict,
     OnChangedList,
     decompress_7z_base64_data,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Coroutine, Sequence
+    from collections.abc import Callable, Sequence
 
-    from .command import Command
+    from .device import DeviceCommandExecute
     from .event_bus import EventBus
 
 
 def _attributes_as_str(self) -> str:  # type: ignore[no-untyped-def] # noqa: ANN001
     """Return attributes as compact svg string."""
     result = ""
     for p in dataclasses.astuple(self):
@@ -152,47 +152,33 @@
 class TracePoint(Point):
     """Trace point."""
 
     connected: bool
 
 
 @dataclasses.dataclass
-class AxisManipulation:
-    """Map manipulation."""
-
-    map_shift: float
-    svg_max: float
-    _transform: Callable[[float, float], float] | None = None
-
-    def __post_init__(self) -> None:
-        self._svg_center = self.svg_max / 2
-
-    def transform(self, value: float) -> float:
-        """Transform value."""
-        if self._transform is None:
-            return value
-        return self._transform(self._svg_center, value)
-
-
-@dataclasses.dataclass
-class MapManipulation:
-    """Map manipulation."""
-
-    x: AxisManipulation
-    y: AxisManipulation
-
-
-@dataclasses.dataclass
 class BackgroundImage:
     """Background image."""
 
     bounding_box: tuple[float, float, float, float]
     image: bytes
 
 
+class ViewBoxFloat:
+    """ViewBox where all values are converted to float."""
+
+    def __init__(self, view_box: svg.ViewBoxSpec) -> None:
+        self.min_x = float(view_box.min_x)
+        self.min_y = float(view_box.min_y)
+        self.width = float(view_box.width)
+        self.height = float(view_box.height)
+        self.max_x = self.min_x + self.width
+        self.max_y = self.min_y + self.height
+
+
 # SVG definitions referred by map elements
 _SVG_DEFS = svg.Defs(
     elements=[
         # Gradient used by Bot icon
         svg.RadialGradient(
             id=f"{_POSITIONS_SVG[PositionType.DEEBOT].svg_id}bg",
             cx=svg.Length(50, "%"),
@@ -233,41 +219,35 @@
                 svg.Circle(fill="#fff", r=2.8, cy=-6.4),
             ],
         ),
     ]
 )
 
 
-def _calc_value(value: float, axis_manipulation: AxisManipulation) -> float:
-    try:
-        if value is not None:
-            # SVG allows sub-pixel precision, so we use floating point coordinates for better placement.
-            new_value = (
-                (float(value) / _PIXEL_WIDTH) + _OFFSET - axis_manipulation.map_shift
-            )
-            new_value = axis_manipulation.transform(new_value)
-            # return value inside min and max
-            return round(
-                min(axis_manipulation.svg_max, max(0, new_value)), _ROUND_TO_DIGITS
-            )
-
-    except (ZeroDivisionError, ValueError):
-        pass
-
-    return 0
-
-
 def _calc_point(
     x: float,
     y: float,
-    map_manipulation: MapManipulation,
 ) -> Point:
     return Point(
-        _calc_value(x, map_manipulation.x),
-        _calc_value(y, map_manipulation.y),
+        0 if x is None else round(x / _PIXEL_WIDTH, _ROUND_TO_DIGITS),
+        0 if y is None else round(-y / _PIXEL_WIDTH, _ROUND_TO_DIGITS),
+    )
+
+
+def _calc_point_in_viewbox(x: float, y: float, view_box: ViewBoxFloat) -> Point:
+    point = _calc_point(x, y)
+    return Point(
+        min(
+            max(point.x, view_box.min_x),
+            view_box.max_x,
+        ),
+        min(
+            max(point.y, view_box.min_y),
+            view_box.max_y,
+        ),
     )
 
 
 def _points_to_svg_path(
     points: Sequence[Point | TracePoint],
 ) -> list[svg.PathData]:
     # Convert a set of simple point (x, y), or trace points (x, y, connected, type) to
@@ -291,39 +271,36 @@
             path_data.append(svg.HorizontalLineToRel(x))
         else:
             path_data.append(svg.LineToRel(x, y))
     return path_data
 
 
 def _get_svg_positions(
-    positions: list[Position],
-    map_manipulation: MapManipulation,
+    positions: list[Position], view_box: ViewBoxFloat
 ) -> list[svg.Element]:
     svg_positions: list[svg.Element] = []
     for position in sorted(positions, key=lambda x: _POSITIONS_SVG[x.type].order):
-        pos = _calc_point(position.x, position.y, map_manipulation)
+        pos = _calc_point_in_viewbox(position.x, position.y, view_box)
         svg_positions.append(
             svg.Use(href=f"#{_POSITIONS_SVG[position.type].svg_id}", x=pos.x, y=pos.y)
         )
 
     return svg_positions
 
 
 def _get_svg_subset(
     subset: MapSubsetEvent,
-    map_manipulation: MapManipulation,
 ) -> Path | svg.Polygon:
     _LOGGER.debug("Creating svg subset for %s", subset)
 
     subset_coordinates: list[int] = ast.literal_eval(subset.coordinates)
     points = [
         _calc_point(
             subset_coordinates[i],
             subset_coordinates[i + 1],
-            map_manipulation,
         )
         for i in range(0, len(subset_coordinates), 2)
     ]
 
     if len(points) == 2:
         # Only 2 point, use a path
         return Path(
@@ -362,15 +339,15 @@
 
 
 class Map:
     """Map representation."""
 
     def __init__(
         self,
-        execute_command: Callable[[Command], Coroutine[Any, Any, None]],
+        execute_command: DeviceCommandExecute,
         event_bus: EventBus,
     ) -> None:
         self._execute_command = execute_command
         self._event_bus = event_bus
 
         self._map_data: Final[MapData] = MapData(event_bus)
         self._amount_rooms: int = 0
@@ -444,32 +421,25 @@
                     image_x += 100
                     image_y = 0
 
             current_piece = self._map_data.map_pieces[i]
             if current_piece.in_use:
                 image.paste(current_piece.image, (image_x, image_y))
 
-    def _get_svg_traces_path(
-        self,
-        map_manipulation: MapManipulation,
-    ) -> Path | None:
+    def _get_svg_traces_path(self) -> Path | None:
         if len(self._map_data.trace_values) > 0:
             _LOGGER.debug("[get_svg_map] Draw Trace")
             return Path(
                 fill="none",
                 stroke=_COLORS[_TRACE_MAP],
                 stroke_width=1.5,
                 stroke_linejoin="round",
                 vector_effect="non-scaling-stroke",
                 transform=[
-                    svg.Translate(
-                        _OFFSET - map_manipulation.x.map_shift,
-                        _OFFSET - map_manipulation.y.map_shift,
-                    ),
-                    svg.Scale(0.2, 0.2),
+                    svg.Scale(0.2, -0.2),
                 ],
                 d=_points_to_svg_path(self._map_data.trace_values),
             )
 
         return None
 
     async def _on_first_map_changed_subscription(self) -> Callable[[], None]:
@@ -565,64 +535,47 @@
         if background is None:
             self._last_image = None
             return None
 
         # Build the SVG elements
         svg_map = svg.SVG()
         svg_map.elements = [_SVG_DEFS]
-        manipulation = MapManipulation(
-            AxisManipulation(
-                map_shift=background.bounding_box[0],
-                svg_max=background.bounding_box[2] - background.bounding_box[0],
-            ),
-            AxisManipulation(
-                map_shift=background.bounding_box[1],
-                svg_max=background.bounding_box[3] - background.bounding_box[1],
-                _transform=lambda c, v: 2 * c - v,
-            ),
-        )
 
         # Set map viewBox based on background map bounding box.
         svg_map.viewBox = svg.ViewBoxSpec(
-            0,
-            0,
-            manipulation.x.svg_max,
-            manipulation.y.svg_max,
+            background.bounding_box[0] - _OFFSET,
+            _OFFSET - background.bounding_box[3],
+            (background.bounding_box[2] - background.bounding_box[0]),
+            (background.bounding_box[3] - background.bounding_box[1]),
         )
 
         # Map background.
         svg_map.elements.append(
             svg.Image(
+                x=svg_map.viewBox.min_x,
+                y=svg_map.viewBox.min_y,
+                width=svg_map.viewBox.width,
+                height=svg_map.viewBox.height,
                 style="image-rendering: pixelated",
                 href=f"data:image/png;base64,{base64.b64encode(background.image).decode('ascii')}",
             )
         )
 
         # Additional subsets (VirtualWalls and NoMopZones)
         svg_map.elements.extend(
-            [
-                _get_svg_subset(subset, manipulation)
-                for subset in self._map_data.map_subsets.values()
-            ]
+            [_get_svg_subset(subset) for subset in self._map_data.map_subsets.values()]
         )
 
         # Traces (if any)
-        if svg_traces_path := self._get_svg_traces_path(manipulation):
-            svg_map.elements.append(
-                # Elements to vertically flip
-                svg.G(
-                    transform_origin=r"50% 50%",
-                    transform=[svg.Scale(1, -1)],
-                    elements=[svg_traces_path],
-                )
-            )
+        if svg_traces_path := self._get_svg_traces_path():
+            svg_map.elements.append(svg_traces_path)
 
         # Bot and Charge stations
         svg_map.elements.extend(
-            _get_svg_positions(self._map_data.positions, manipulation)
+            _get_svg_positions(self._map_data.positions, ViewBoxFloat(svg_map.viewBox))
         )
 
         self._last_image = str(svg_map)
         _LOGGER.debug("[get_svg_map] Finish")
         return self._last_image
 
     async def teardown(self) -> None:
```

### Comparing `deebot_client-7.2.0/deebot_client/message.py` & `deebot_client-7.3.0/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/messages/__init__.py` & `deebot_client-7.3.0/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/messages/json/__init__.py` & `deebot_client-7.3.0/deebot_client/messages/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/messages/json/battery.py` & `deebot_client-7.3.0/deebot_client/messages/json/battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/messages/json/map.py` & `deebot_client-7.3.0/deebot_client/messages/json/map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/messages/json/stats.py` & `deebot_client-7.3.0/deebot_client/messages/json/stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/models.py` & `deebot_client-7.3.0/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/mqtt_client.py` & `deebot_client-7.3.0/deebot_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/util/__init__.py` & `deebot_client-7.3.0/deebot_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client/util/continents.py` & `deebot_client-7.3.0/deebot_client/util/continents.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/deebot_client.egg-info/PKG-INFO` & `deebot_client-7.3.0/deebot_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 7.2.0
+Version: 7.3.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
```

### Comparing `deebot_client-7.2.0/deebot_client.egg-info/SOURCES.txt` & `deebot_client-7.3.0/deebot_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 deebot_client/commands/json/clean_preference.py
 deebot_client/commands/json/clear_map.py
 deebot_client/commands/json/common.py
 deebot_client/commands/json/const.py
 deebot_client/commands/json/continuous_cleaning.py
 deebot_client/commands/json/cross_map_border_warning.py
 deebot_client/commands/json/custom.py
+deebot_client/commands/json/cut_direction.py
 deebot_client/commands/json/efficiency.py
 deebot_client/commands/json/error.py
 deebot_client/commands/json/fan_speed.py
 deebot_client/commands/json/life_span.py
 deebot_client/commands/json/map.py
 deebot_client/commands/json/moveup_warning.py
 deebot_client/commands/json/multimap_state.py
@@ -93,25 +94,28 @@
 deebot_client/events/efficiency_mode.py
 deebot_client/events/fan_speed.py
 deebot_client/events/map.py
 deebot_client/events/network.py
 deebot_client/events/water_info.py
 deebot_client/events/work_mode.py
 deebot_client/hardware/__init__.py
+deebot_client/hardware/deebot/2ap5uq.py
 deebot_client/hardware/deebot/2o4lnm.py
 deebot_client/hardware/deebot/55aiho.py
 deebot_client/hardware/deebot/5xu9h3.py
 deebot_client/hardware/deebot/626v6g.py
 deebot_client/hardware/deebot/77atlz.py
 deebot_client/hardware/deebot/85nbtp.py
 deebot_client/hardware/deebot/9ku8nu.py
+deebot_client/hardware/deebot/9s1s80.py
 deebot_client/hardware/deebot/__init__.py
 deebot_client/hardware/deebot/clojes.py
 deebot_client/hardware/deebot/e6ofmn.py
 deebot_client/hardware/deebot/fallback.py
+deebot_client/hardware/deebot/guzput.py
 deebot_client/hardware/deebot/itk04l.py
 deebot_client/hardware/deebot/lf3bn4.py
 deebot_client/hardware/deebot/lx3j7m.py
 deebot_client/hardware/deebot/p1jij8.py
 deebot_client/hardware/deebot/p95mgv.py
 deebot_client/hardware/deebot/paeygf.py
 deebot_client/hardware/deebot/rss8xk.py
@@ -154,23 +158,25 @@
 tests/commands/json/test_clean_count.py
 tests/commands/json/test_clean_log.py
 tests/commands/json/test_clean_preference.py
 tests/commands/json/test_common.py
 tests/commands/json/test_continuous_cleaning.py
 tests/commands/json/test_cross_map_border_warning.py
 tests/commands/json/test_custom.py
+tests/commands/json/test_cut_direction.py
 tests/commands/json/test_efficiency.py
 tests/commands/json/test_error.py
 tests/commands/json/test_fan_speed.py
 tests/commands/json/test_life_span.py
 tests/commands/json/test_map.py
 tests/commands/json/test_moveup_warning.py
 tests/commands/json/test_mulitmap_state.py
 tests/commands/json/test_network.py
 tests/commands/json/test_ota.py
+tests/commands/json/test_pos.py
 tests/commands/json/test_safe_protect.py
 tests/commands/json/test_sweep_mode.py
 tests/commands/json/test_true_detect.py
 tests/commands/json/test_voice_assistant_state.py
 tests/commands/json/test_volume.py
 tests/commands/json/test_water_info.py
 tests/commands/json/test_work_mode.py
```

### Comparing `deebot_client-7.2.0/mypy.ini` & `deebot_client-7.3.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/pyproject.toml` & `deebot_client-7.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/scripts/check_getLogger.sh` & `deebot_client-7.3.0/scripts/check_getLogger.sh`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/__init__.py` & `deebot_client-7.3.0/tests/commands/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,52 +12,62 @@
     Credentials,
 )
 
 if TYPE_CHECKING:
     from deebot_client.events import Event
 
 
-def _wrap_command(command: Command) -> tuple[Command, Callable[[CommandResult], None]]:
+def _wrap_command(
+    command: Command,
+) -> tuple[Command, Callable[[CommandResult, dict[str, Any] | None], None]]:
     result: CommandResult | None = None
+    response: dict[str, Any] | None = None
     execute_fn = command._execute
 
     async def _execute(
         _: Command,
         authenticator: Authenticator,
         device_info: ApiDeviceInfo,
         event_bus: EventBus,
-    ) -> CommandResult:
-        nonlocal result
-        result = await execute_fn(authenticator, device_info, event_bus)
-        return result
-
-    def verify_result(expected_result: CommandResult) -> None:
+    ) -> tuple[CommandResult, dict[str, Any]]:
+        nonlocal result, response
+        result, response = await execute_fn(authenticator, device_info, event_bus)
+        return result, response
+
+    def verify_result(
+        expected_result: CommandResult, expected_response: dict[str, Any] | None = None
+    ) -> None:
         assert result == expected_result
+        if expected_response is not None:
+            assert response == expected_response
 
     command._execute = _execute.__get__(command)  # type: ignore[method-assign]
     return (command, verify_result)
 
 
 async def assert_command(
     command: Command,
     json_api_response: dict[str, Any] | tuple[dict[str, Any], ...],
     expected_events: Event | None | Sequence[Event],
     *,
     command_result: CommandResult | None = None,
+    expected_raw_response: dict[str, Any] | None = None,
 ) -> None:
     command_result = command_result or CommandResult.success()
     event_bus = Mock(spec_set=EventBus)
     authenticator = Mock(spec_set=Authenticator)
     authenticator.authenticate = AsyncMock(
         return_value=Credentials("token", "user_id", 9999)
     )
     if isinstance(json_api_response, tuple):
         authenticator.post_authenticated = AsyncMock(side_effect=json_api_response)
     else:
         authenticator.post_authenticated = AsyncMock(return_value=json_api_response)
+        if expected_raw_response is None:
+            expected_raw_response = json_api_response
     device_info = ApiDeviceInfo(
         {
             "company": "company",
             "did": "did",
             "name": "name",
             "nick": "nick",
             "resource": "resource",
@@ -66,15 +76,15 @@
     )
 
     command, verify_result = _wrap_command(command)
 
     await command.execute(authenticator, device_info, event_bus)
 
     # verify
-    verify_result(command_result)
+    verify_result(command_result, expected_raw_response)
     authenticator.post_authenticated.assert_called()
     if expected_events:
         if isinstance(expected_events, Sequence):
             event_bus.notify.assert_has_calls([call(x) for x in expected_events])
             assert event_bus.notify.call_count == len(expected_events)
         else:
             event_bus.notify.assert_called_once_with(expected_events)
```

### Comparing `deebot_client-7.2.0/tests/commands/json/__init__.py` & `deebot_client-7.3.0/tests/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_advanced_mode.py` & `deebot_client-7.3.0/tests/commands/json/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_battery.py` & `deebot_client-7.3.0/tests/commands/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_border_switch.py` & `deebot_client-7.3.0/tests/commands/json/test_border_switch.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_carpet.py` & `deebot_client-7.3.0/tests/commands/json/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_charge.py` & `deebot_client-7.3.0/tests/commands/json/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_charge_state.py` & `deebot_client-7.3.0/tests/commands/json/test_charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_child_lock.py` & `deebot_client-7.3.0/tests/commands/json/test_child_lock.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_clean.py` & `deebot_client-7.3.0/tests/commands/json/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_clean_count.py` & `deebot_client-7.3.0/tests/commands/json/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_clean_log.py` & `deebot_client-7.3.0/tests/commands/json/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_clean_preference.py` & `deebot_client-7.3.0/tests/commands/json/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_common.py` & `deebot_client-7.3.0/tests/commands/json/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     elif expected_log:
         assert (
             "deebot_client.command",
             expected_log[0],
             expected_log[1].format(command.name),
         ) in caplog.record_tuples
 
-    assert available is False
+    assert available.device_reached is False
     assert_func(event_bus)
```

### Comparing `deebot_client-7.2.0/tests/commands/json/test_continuous_cleaning.py` & `deebot_client-7.3.0/tests/commands/json/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_cross_map_border_warning.py` & `deebot_client-7.3.0/tests/commands/json/test_cross_map_border_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_custom.py` & `deebot_client-7.3.0/tests/commands/json/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_efficiency.py` & `deebot_client-7.3.0/tests/commands/json/test_efficiency.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_error.py` & `deebot_client-7.3.0/tests/commands/json/test_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import pytest
 
 from deebot_client.commands.json import GetError
 from deebot_client.events import ErrorEvent, StateEvent
 from deebot_client.models import State
 from tests.helpers import get_request_json, get_success_body
@@ -14,16 +14,22 @@
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from deebot_client.events.base import Event
 
 
 @pytest.mark.parametrize(
-    ("code", "expected_events"),
+    ("body", "expected_events"),
     [
-        (0, ErrorEvent(0, "NoError: Robot is operational")),
-        (105, [StateEvent(State.ERROR), ErrorEvent(105, "Stuck: Robot is stuck")]),
+        ({"code": [0]}, ErrorEvent(0, "NoError: Robot is operational")),
+        ({"code": []}, ErrorEvent(0, "NoError: Robot is operational")),
+        (
+            {"code": [105]},
+            [StateEvent(State.ERROR), ErrorEvent(105, "Stuck: Robot is stuck")],
+        ),
     ],
 )
-async def test_getErrors(code: int, expected_events: Event | Sequence[Event]) -> None:
-    json = get_request_json(get_success_body({"code": [code]}))
+async def test_getErrors(
+    body: dict[str, Any], expected_events: Event | Sequence[Event]
+) -> None:
+    json = get_request_json(get_success_body(body))
     await assert_command(GetError(), json, expected_events)
```

### Comparing `deebot_client-7.2.0/tests/commands/json/test_fan_speed.py` & `deebot_client-7.3.0/tests/commands/json/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_life_span.py` & `deebot_client-7.3.0/tests/commands/json/test_life_span.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,41 +23,57 @@
                     LifeSpan.SIDE_BRUSH,
                     LifeSpan.UNIT_CARE,
                     LifeSpan.ROUND_MOP,
                     LifeSpan.AIR_FRESHENER,
                     LifeSpan.UV_SANITIZER,
                     LifeSpan.HUMIDIFY,
                     LifeSpan.HUMIDIFY_MAINTENANCE,
+                    LifeSpan.DUST_BAG,
+                    LifeSpan.CLEANING_FLUID,
+                    LifeSpan.STRAINER,
+                    LifeSpan.HAND_FILTER,
                 }
             ),
             get_request_json(
                 get_success_body(
                     [
                         {"type": "brush", "left": 17979, "total": 18000},
                         {"type": "heap", "left": 7179, "total": 7200},
                         {"type": "sideBrush", "left": 8977, "total": 9000},
                         {"type": "unitCare", "left": 265, "total": 1800},
                         {"type": "roundMop", "left": 6820, "total": 9000},
                         {"type": "dModule", "left": 17537, "total": 18000},
                         {"type": "uv", "left": 898586, "total": 900000},
                         {"type": "humidify", "left": 191547, "total": 194400},
                         {"type": "wbCare", "left": 22260, "total": 43200},
+                        {
+                            "type": "autoWater_cleaningFluid",
+                            "left": 86400,
+                            "total": 86400,
+                        },
+                        {"type": "dustBag", "left": 2031, "total": 3000},
+                        {"type": "handFilter", "left": 30000, "total": 30000},
+                        {"type": "strainer", "left": 1800, "total": 1800},
                     ]
                 )
             ),
             [
                 LifeSpanEvent(LifeSpan.BRUSH, 99.88, 17979),
                 LifeSpanEvent(LifeSpan.FILTER, 99.71, 7179),
                 LifeSpanEvent(LifeSpan.SIDE_BRUSH, 99.74, 8977),
                 LifeSpanEvent(LifeSpan.UNIT_CARE, 14.72, 265),
                 LifeSpanEvent(LifeSpan.ROUND_MOP, 75.78, 6820),
                 LifeSpanEvent(LifeSpan.AIR_FRESHENER, 97.43, 17537),
                 LifeSpanEvent(LifeSpan.UV_SANITIZER, 99.84, 898586),
                 LifeSpanEvent(LifeSpan.HUMIDIFY, 98.53, 191547),
                 LifeSpanEvent(LifeSpan.HUMIDIFY_MAINTENANCE, 51.53, 22260),
+                LifeSpanEvent(LifeSpan.CLEANING_FLUID, 100.0, 86400),
+                LifeSpanEvent(LifeSpan.DUST_BAG, 67.7, 2031),
+                LifeSpanEvent(LifeSpan.HAND_FILTER, 100.0, 30000),
+                LifeSpanEvent(LifeSpan.STRAINER, 100.0, 1800),
             ],
         ),
         (
             GetLifeSpan({LifeSpan.BRUSH}),
             get_request_json(
                 get_success_body([{"type": "brush", "left": 17979, "total": 18000}])
             ),
@@ -117,14 +133,46 @@
         (
             GetLifeSpan({LifeSpan.HUMIDIFY_MAINTENANCE}),
             get_request_json(
                 get_success_body([{"type": "wbCare", "left": 22260, "total": 43200}])
             ),
             [LifeSpanEvent(LifeSpan.HUMIDIFY_MAINTENANCE, 51.53, 22260)],
         ),
+        (
+            GetLifeSpan({LifeSpan.CLEANING_FLUID}),
+            get_request_json(
+                get_success_body(
+                    [{"type": "autoWater_cleaningFluid", "left": 86400, "total": 86400}]
+                )
+            ),
+            [LifeSpanEvent(LifeSpan.CLEANING_FLUID, 100.0, 86400)],
+        ),
+        (
+            GetLifeSpan({LifeSpan.DUST_BAG}),
+            get_request_json(
+                get_success_body([{"type": "dustBag", "left": 2031, "total": 3000}])
+            ),
+            [LifeSpanEvent(LifeSpan.DUST_BAG, 67.7, 2031)],
+        ),
+        (
+            GetLifeSpan({LifeSpan.HAND_FILTER}),
+            get_request_json(
+                get_success_body(
+                    [{"type": "handFilter", "left": 30000, "total": 30000}]
+                )
+            ),
+            [LifeSpanEvent(LifeSpan.HAND_FILTER, 100.0, 30000)],
+        ),
+        (
+            GetLifeSpan({LifeSpan.STRAINER}),
+            get_request_json(
+                get_success_body([{"type": "strainer", "left": 1800, "total": 1800}])
+            ),
+            [LifeSpanEvent(LifeSpan.STRAINER, 100.0, 1800)],
+        ),
     ],
 )
 async def test_GetLifeSpan(
     command: GetLifeSpan, json: dict[str, Any], expected: list[LifeSpanEvent]
 ) -> None:
     await assert_command(command, json, expected)
```

### Comparing `deebot_client-7.2.0/tests/commands/json/test_map.py` & `deebot_client-7.3.0/tests/commands/json/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_moveup_warning.py` & `deebot_client-7.3.0/tests/commands/json/test_moveup_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_mulitmap_state.py` & `deebot_client-7.3.0/tests/commands/json/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_network.py` & `deebot_client-7.3.0/tests/commands/json/test_network.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_ota.py` & `deebot_client-7.3.0/tests/commands/json/test_ota.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_safe_protect.py` & `deebot_client-7.3.0/tests/commands/json/test_safe_protect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_sweep_mode.py` & `deebot_client-7.3.0/tests/commands/json/test_sweep_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_true_detect.py` & `deebot_client-7.3.0/tests/commands/json/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_voice_assistant_state.py` & `deebot_client-7.3.0/tests/commands/json/test_voice_assistant_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_volume.py` & `deebot_client-7.3.0/tests/commands/json/test_volume.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/json/test_work_mode.py` & `deebot_client-7.3.0/tests/commands/json/test_work_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/xml/test_charge_state.py` & `deebot_client-7.3.0/tests/commands/xml/test_charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/xml/test_error.py` & `deebot_client-7.3.0/tests/commands/xml/test_error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/xml/test_fan_speed.py` & `deebot_client-7.3.0/tests/commands/xml/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/commands/xml/test_pos.py` & `deebot_client-7.3.0/tests/commands/xml/test_pos.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from . import get_request_xml
 
 
 async def test_get_pos() -> None:
     json = get_request_xml("<ctl ret='ok' t='p' p='77,-5' a='-3' valid='1'/>")
     expected_event = PositionsEvent(
-        positions=[Position(type=PositionType.DEEBOT, x=77, y=-5)]
+        positions=[Position(type=PositionType.DEEBOT, x=77, y=-5, a=-3)]
     )
     await assert_command(GetPos(), json, expected_event)
 
 
 @pytest.mark.parametrize(
     "xml",
     ["<ctl ret='error'/>", "<ctl ret='ok' t='p'></ctl>"],
```

### Comparing `deebot_client-7.2.0/tests/conftest.py` & `deebot_client-7.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/fixtures/base.py` & `deebot_client-7.3.0/tests/fixtures/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @abstractmethod
     def check(self) -> bool:
         """Return True if container is started successfully."""
 
     def __init__(self) -> None:
         self.container: Container | None = None
-        self._start_time: datetime = datetime(1, 1, 1)
+        self._start_time: datetime | None = None
 
     @property
     def image(self) -> str:
         """Return used image."""
         return f"{self.config.image}:{self.config.version}"
 
     @property
@@ -149,15 +149,15 @@
         return image_options
 
     def logs(self, *, since_last_start: bool = True) -> str:
         """Get docker container logs."""
         if self.container is None:
             raise ContainerNotStartedError
 
-        if since_last_start:
+        if since_last_start and self._start_time:
             logs: bytes = self.container.logs(since=self._start_time)
         else:
             logs = self.container.logs()
         return logs.decode("utf-8")
 
     def run(self) -> HostPort:
         """Run container."""
```

### Comparing `deebot_client-7.2.0/tests/fixtures/mqtt_server.py` & `deebot_client-7.3.0/tests/fixtures/mqtt_server.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/hardware/test_init.py` & `deebot_client-7.3.0/tests/hardware/test_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import pytest
 
+from deebot_client.commands.json import GetCutDirection
 from deebot_client.commands.json.advanced_mode import GetAdvancedMode
 from deebot_client.commands.json.battery import GetBattery
 from deebot_client.commands.json.border_switch import GetBorderSwitch
 from deebot_client.commands.json.carpet import GetCarpetAutoFanBoost
 from deebot_client.commands.json.charge_state import GetChargeState
 from deebot_client.commands.json.child_lock import GetChildLock
 from deebot_client.commands.json.clean import GetCleanInfo, GetCleanInfoV2
@@ -45,14 +46,15 @@
     ChildLockEvent,
     CleanCountEvent,
     CleanLogEvent,
     CleanPreferenceEvent,
     ContinuousCleaningEvent,
     CrossMapBorderWarningEvent,
     CustomCommandEvent,
+    CutDirectionEvent,
     ErrorEvent,
     LifeSpan,
     LifeSpanEvent,
     MoveUpWarningEvent,
     MultimapStateEvent,
     OtaEvent,
     ReportStatsEvent,
@@ -143,14 +145,15 @@
         (
             "5xu9h3",
             {
                 AdvancedModeEvent: [GetAdvancedMode()],
                 AvailabilityEvent: [GetBattery(is_available_check=True)],
                 BatteryEvent: [GetBattery()],
                 BorderSwitchEvent: [GetBorderSwitch()],
+                CutDirectionEvent: [GetCutDirection()],
                 ChildLockEvent: [GetChildLock()],
                 CrossMapBorderWarningEvent: [GetCrossMapBorderWarning()],
                 CustomCommandEvent: [],
                 ErrorEvent: [GetError()],
                 LifeSpanEvent: [GetLifeSpan([LifeSpan.BLADE, LifeSpan.LENS_BRUSH])],
                 MoveUpWarningEvent: [GetMoveUpWarning()],
                 NetworkInfoEvent: [GetNetInfo()],
@@ -166,14 +169,15 @@
         (
             "itk04l",
             {
                 AdvancedModeEvent: [GetAdvancedMode()],
                 AvailabilityEvent: [GetBattery(is_available_check=True)],
                 BatteryEvent: [GetBattery()],
                 BorderSwitchEvent: [GetBorderSwitch()],
+                CutDirectionEvent: [GetCutDirection()],
                 ChildLockEvent: [GetChildLock()],
                 CrossMapBorderWarningEvent: [GetCrossMapBorderWarning()],
                 CustomCommandEvent: [],
                 ErrorEvent: [GetError()],
                 LifeSpanEvent: [GetLifeSpan([LifeSpan.BLADE, LifeSpan.LENS_BRUSH])],
                 MoveUpWarningEvent: [GetMoveUpWarning()],
                 NetworkInfoEvent: [GetNetInfo()],
@@ -275,24 +279,27 @@
         ), f"Refresh commands doesn't match for {event}"
 
 
 def test_all_models_loaded() -> None:
     """Test that all models are loaded."""
     _load()
     assert list(DEVICES) == [
+        "2ap5uq",
         "2o4lnm",
         "55aiho",
         "5xu9h3",
         "626v6g",
         "77atlz",
         "85nbtp",
         "9ku8nu",
+        "9s1s80",
         "clojes",
         "e6ofmn",
         "fallback",
+        "guzput",
         "itk04l",
         "lf3bn4",
         "lx3j7m",
         "p1jij8",
         "p95mgv",
         "paeygf",
         "rss8xk",
```

### Comparing `deebot_client-7.2.0/tests/helpers/__init__.py` & `deebot_client-7.3.0/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/helpers/tasks.py` & `deebot_client-7.3.0/tests/helpers/tasks.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/messages/__init__.py` & `deebot_client-7.3.0/tests/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/messages/json/test_battery.py` & `deebot_client-7.3.0/tests/messages/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/messages/json/test_map.py` & `deebot_client-7.3.0/tests/messages/json/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/messages/json/test_stats.py` & `deebot_client-7.3.0/tests/messages/json/test_stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/messages/test_get_messages.py` & `deebot_client-7.3.0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/mqtt_util.py` & `deebot_client-7.3.0/tests/mqtt_util.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/test_authentication.py` & `deebot_client-7.3.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/test_command.py` & `deebot_client-7.3.0/tests/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,13 +77,14 @@
     authenticator: Mock,
     api_device_info: ApiDeviceInfo,
     event_bus_mock: Mock,
 ) -> None:
     """Test that on api timeout the stack trace is not logged."""
     command = _TestCommand(1)
     authenticator.post_authenticated.side_effect = ApiTimeoutError("test", 60)
-    assert not await command.execute(authenticator, api_device_info, event_bus_mock)
+    result = await command.execute(authenticator, api_device_info, event_bus_mock)
+    assert not result.device_reached
     assert (
         "deebot_client.command",
         logging.WARNING,
         "Could not execute command TestCommand: Timeout reached",
     ) in caplog.record_tuples
```

### Comparing `deebot_client-7.2.0/tests/test_device.py` & `deebot_client-7.3.0/tests/test_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 from collections.abc import Callable
 import json
 from typing import TYPE_CHECKING
 from unittest.mock import Mock, patch
 
+from deebot_client.command import DeviceCommandResult
 from deebot_client.commands.json.battery import GetBattery
 from deebot_client.device import Device
 from deebot_client.events import AvailabilityEvent
 from deebot_client.events.network import NetworkInfoEvent
 from deebot_client.models import DeviceInfo
 from deebot_client.mqtt_client import MqttClient, SubscriberInfo
 from tests.helpers import mock_static_device_info
@@ -61,24 +62,24 @@
     sub_info: SubscriberInfo = mqtt_client.subscribe.call_args.args[0]
     assert bot._available_task is not None
     assert not bot._available_task.done()
     # As task was started now, no check should be performed
     execute_mock.assert_not_called()
 
     # Simulate bot not reached by returning False
-    execute_mock.return_value = False
+    execute_mock.return_value = DeviceCommandResult(device_reached=False)
 
     # Wait longer than the interval to be sure task will be executed
     await asyncio.sleep(2.1)
     # Verify command call for available check
     execute_mock.assert_awaited_once()
     await assert_received_status(expected=False)
 
     # Simulate bot reached by returning True
-    execute_mock.return_value = True
+    execute_mock.return_value = DeviceCommandResult(device_reached=True)
 
     await asyncio.sleep(2)
     execute_mock.await_count = 2
     await assert_received_status(expected=True)
 
     # reset mock for easier handling
     battery_mock.reset_mock()
```

### Comparing `deebot_client-7.2.0/tests/test_event_bus.py` & `deebot_client-7.3.0/tests/test_event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/test_mqtt_client.py` & `deebot_client-7.3.0/tests/test_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/test_mqtt_client_reconnect.py` & `deebot_client-7.3.0/tests/test_mqtt_client_reconnect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/util/test_continents.py` & `deebot_client-7.3.0/tests/util/test_continents.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.2.0/tests/util/test_init.py` & `deebot_client-7.3.0/tests/util/test_init.py`

 * *Files identical despite different names*

