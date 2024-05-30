# Comparing `tmp/recycling-1.0.0.tar.gz` & `tmp/recycling-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recycling-1.0.0.tar", max compression
+gzip compressed data, was "recycling-1.1.0.tar", max compression
```

## Comparing `recycling-1.0.0.tar` & `recycling-1.1.0.tar`

### file list

```diff
@@ -1,473 +1,666 @@
--rwxr-xr-x   0        0        0     1287 2024-05-12 04:16:50.860727 recycling-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1104 2024-05-12 04:02:44.005690 recycling-1.0.0/readme.md
--rwxr-xr-x   0        0        0     1928 2024-05-12 04:16:36.128882 recycling-1.0.0/venue.S.HTML
--rwxr-xr-x   0        0        0      394 2024-05-12 04:08:13.222189 recycling-1.0.0/venues/stages/recycling/___perf/recycling_1
--rwxr-xr-x   0        0        0   255862 2024-02-08 22:34:22.772280 recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311435_1920.jpg
--rwxr-xr-x   0        0        0   325850 2024-02-08 22:34:42.900056 recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311446_1920.jpg
--rwxr-xr-x   0        0        0   430054 2024-02-08 22:34:01.964510 recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311450_1920.jpg
--rwxr-xr-x   0        0        0      174 2024-05-12 04:08:12.522196 recycling-1.0.0/venues/stages/recycling/__init__.py
--rwxr-xr-x   0        0        0      241 2024-05-12 04:08:12.522196 recycling-1.0.0/venues/stages/recycling/__license/license.s.HTML
--rwxr-xr-x   0        0        0    37277 2024-02-25 04:11:37.778016 recycling-1.0.0/venues/stages/recycling/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      701 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/delegates/delegates.r.html
--rwxr-xr-x   0        0        0      148 2023-11-23 17:10:27.664329 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/delegates/pools.r.HTML
--rwxr-xr-x   0        0        0      348 2023-11-23 17:12:35.903844 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/fees/fees.r.HTML
--rwxr-xr-x   0        0        0      374 2023-11-23 17:18:33.203704 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/membership/joining.r.HTML
--rwxr-xr-x   0        0        0      671 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/queue/queue.r.html
--rwxr-xr-x   0        0        0      375 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/sequence/sequence.s.HTML
--rwxr-xr-x   0        0        0     1953 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/voters.s.HTML
--rwxr-xr-x   0        0        0      182 2023-11-23 18:01:40.901701 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/journal/journal structure.r.HTML
--rwxr-xr-x   0        0        0     1679 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/journal/journal.r.HTML
--rwxr-xr-x   0        0        0      270 2023-11-23 17:41:46.371555 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/journal/segments/segments.r.HTML
--rwxr-xr-x   0        0        0      479 2024-04-24 19:56:38.245353 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/treasures/escrows/escrows.r.html
--rwxr-xr-x   0        0        0      219 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/treasures/fees/fees.r.html
--rwxr-xr-x   0        0        0       70 2023-11-08 06:57:41.840464 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/treasures/giveaways/giveaways.r.html
--rwxr-xr-x   0        0        0      407 2023-11-23 17:19:28.054069 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/treasures/money.r.html
--rwxr-xr-x   0        0        0      101 2023-11-13 22:12:26.508973 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/treasures/supply/supply.r.html
--rwxr-xr-x   0        0        0      290 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/trends/trends.s.HTML
--rwxr-xr-x   0        0        0      805 2024-02-24 01:12:30.622670 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/moderation/moderation.r.html
--rwxr-xr-x   0        0        0       15 2023-11-08 06:57:41.841464 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/security/security.r.html
--rwxr-xr-x   0        0        0       55 2024-02-25 04:11:37.770016 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/shamir backups/shamir.r.html
--rwxr-xr-x   0        0        0     3106 2024-02-24 01:12:30.638670 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/wallet.svg
--rwxr-xr-x   0        0        0     2192 2024-04-24 19:48:32.704059 recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/priorities.html
--rw-r--r--   0        0        0      308 2024-04-24 18:41:44.974547 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/MVP.S.HTML
--rw-r--r--   0        0        0      234 2024-04-24 19:17:40.101250 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/asks.S.HTML
--rw-r--r--   0        0        0      593 2024-04-24 19:16:59.437435 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/off_chain/off_chain_moves.S.HTML
--rw-r--r--   0        0        0      524 2024-04-24 19:53:15.691970 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/___steps/steps.S.HTML
--rw-r--r--   0        0        0      482 2024-04-24 20:07:09.802022 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/__squashes/squashes.S.HTML
--rwxr-xr-x   0        0        0      476 2024-04-24 19:26:48.249860 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/_fees/fees.S.HTML
--rw-r--r--   0        0        0      438 2024-04-24 19:31:44.407627 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/asks.S.HTML
--rw-r--r--   0        0        0      394 2024-04-24 19:39:45.003755 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/escrow/escrow.S.HTML
--rw-r--r--   0        0        0      109 2024-04-24 19:34:04.798519 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/founder_blocks/founder_blocks.S.HTML
--rw-r--r--   0        0        0      284 2024-04-24 19:56:28.173479 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/physics/physics.S.HTML
--rw-r--r--   0        0        0   202363 2024-04-24 05:21:48.221999 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/voters/picker_queue/picker queue.jpeg
--rw-r--r--   0        0        0      471 2024-04-24 20:01:50.889614 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/voters/picker_queue/picker_queue.S.HTML
--rw-r--r--   0        0        0      329 2024-04-24 19:55:46.374005 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/voters/voters.S.HTMl
--rw-r--r--   0        0        0      537 2024-04-24 20:07:47.245609 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/assets/assets.S.HTML
--rw-r--r--   0        0        0      530 2024-04-24 19:38:44.968249 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/businesses.S.HTML
--rw-r--r--   0        0        0      376 2024-04-24 17:53:21.972043 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/keys/keys, from seed.S.HTML
--rw-r--r--   0        0        0      706 2024-04-24 20:08:05.409410 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/keys/keys, legend.S.HTML
--rwxr-xr-x   0        0        0      596 2024-04-24 19:40:26.203414 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/keys/keys.s.HTML
--rwxr-xr-x   0        0        0     1492 2024-04-24 19:59:25.923313 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/voting/voting.s.HTML
--rw-r--r--   0        0        0      115 2024-04-24 19:07:59.814569 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/nodes/nodes.S.HTML
--rw-r--r--   0        0        0      252 2024-04-24 19:57:50.536461 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/the_reel/dev_nets/dev_nets.S.HTML
--rw-r--r--   0        0        0      772 2024-04-24 20:06:06.418724 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/the_reel/reel themes.S.HTML
--rwxr-xr-x   0        0        0     1712 2024-04-24 19:58:27.628011 recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/the_reel/reel.S.HTML
--rw-r--r--   0        0        0      261 2024-04-24 19:06:32.683453 recycling-1.0.0/venues/stages/recycling/__objectives/L1/2_Next/apps/apps.S.HTML
--rwxr-xr-x   0        0        0    23774 2023-11-08 06:57:41.841464 recycling-1.0.0/venues/stages/recycling/__objectives/L1/2_Next/apps/pay wall.svg
--rwxr-xr-x   0        0        0      948 2024-04-24 20:07:36.661726 recycling-1.0.0/venues/stages/recycling/__objectives/L1/2_Next/smart_contracts/smart_contracts.S.HTML
--rw-r--r--   0        0        0      411 2024-04-24 19:18:51.216898 recycling-1.0.0/venues/stages/recycling/__objectives/L2/L2.S.HTML
--rw-r--r--   0        0        0      154 2024-04-24 18:30:19.917498 recycling-1.0.0/venues/stages/recycling/__objectives/L_physical/L_physical.S.HTML
--rwxr-xr-x   0        0        0      925 2024-04-24 18:17:42.425185 recycling-1.0.0/venues/stages/recycling/__objectives/later, vibes.S.HTML
--rwxr-xr-x   0        0        0     2349 2024-05-05 00:04:11.156777 recycling-1.0.0/venues/stages/recycling/__objectives/objectives.S.HTML
--rwxr-xr-x   0        0        0      961 2024-05-12 04:08:12.518196 recycling-1.0.0/venues/stages/recycling/_clique/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-12 04:10:57.364453 recycling-1.0.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-05 19:29:21.596475 recycling-1.0.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 01:08:10.745821 recycling-1.0.0/venues/stages/recycling/_clique/__pycache__/intro.cpython-310.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 recycling-1.0.0/venues/stages/recycling/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        4 2024-02-24 01:08:10.765821 recycling-1.0.0/venues/stages/recycling/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:52.945271 recycling-1.0.0/venues/stages/recycling/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       14 2023-11-23 22:42:42.966463 recycling-1.0.0/venues/stages/recycling/_status/.gitignore
--rwxr-xr-x   0        0        0   335656 2024-05-12 04:14:40.894095 recycling-1.0.0/venues/stages/recycling/_status/DB/records.json
--rwxr-xr-x   0        0        0      865 2024-05-12 04:14:30.230208 recycling-1.0.0/venues/stages/recycling/_status/__init__.py
--rw-r--r--   0        0        0      847 2024-05-12 04:14:33.862169 recycling-1.0.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-03-14 20:19:40.185302 recycling-1.0.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      339 2024-05-12 04:11:25.420157 recycling-1.0.0/venues/stages/recycling/_status/_stories/story_instrument_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-02-27 05:00:51.041236 recycling-1.0.0/venues/stages/recycling/_status/_stories/story_instrument_1/status_1.py
--rwxr-xr-x   0        0        0      369 2024-05-12 04:10:55.684471 recycling-1.0.0/venues/stages/recycling/_status/status.proc.py
--rwxr-xr-x   0        0        0      224 2024-02-17 01:38:10.912059 recycling-1.0.0/venues/stages/recycling/instrument/__agenda/agenda.s.HTML
--rwxr-xr-x   0        0        0   333254 2024-02-08 18:30:08.370149 recycling-1.0.0/venues/stages/recycling/instrument/__book/TheDigitalArtist--ai-generated-8228359_1920.jpg
--rwxr-xr-x   0        0        0   309408 2024-02-08 18:30:31.169965 recycling-1.0.0/venues/stages/recycling/instrument/__book/TheDigitalArtist--ai-generated-8228360_1920.jpg
--rwxr-xr-x   0        0        0      760 2024-02-05 00:38:46.633355 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/ISO_lab.s.HTML
--rwxr-xr-x   0        0        0     2783 2024-02-24 01:12:30.750668 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/ISO_lab_2.s.HTML
--rwxr-xr-x   0        0        0      672 2024-02-02 04:01:11.455302 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/write_ISO_to_drive.py
--rwxr-xr-x   0        0        0       71 2024-02-01 18:31:16.299750 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/compose/compose.s.HTML
--rwxr-xr-x   0        0        0      945 2024-02-01 19:02:46.302852 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/containers/containers.s.HTML
--rwxr-xr-x   0        0        0     1364 2024-02-25 04:11:37.782016 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/containers/installations.s.HTML
--rwxr-xr-x   0        0        0      674 2024-02-01 00:45:37.341120 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/docker.s.HTML
--rwxr-xr-x   0        0        0      260 2024-05-12 04:08:12.690195 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/essential_installations.s.HTML
--rwxr-xr-x   0        0        0      207 2024-01-31 22:35:57.782459 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/images/images.s.HTML
--rwxr-xr-x   0        0        0     1265 2024-01-30 03:31:07.323407 recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/hardware.s.HTML
--rwxr-xr-x   0        0        0   594783 2024-02-05 18:23:07.029822 recycling-1.0.0/venues/stages/recycling/instrument/__book/dlsdkcgl--hidden-8315722_1920.jpg
--rwxr-xr-x   0        0        0      195 2024-05-12 04:08:12.562196 recycling-1.0.0/venues/stages/recycling/instrument/__init__.py
--rw-r--r--   0        0        0      462 2024-05-12 04:10:57.364453 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-03-14 20:19:44.209258 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-12 19:23:01.902091 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.740472 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.687552 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique_socket.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.796471 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique_socket.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.703552 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique_tracks.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.864471 recycling-1.0.0/venues/stages/recycling/instrument/__pycache__/clique_tracks.cpython-311.pyc
--rw-r--r--   0        0        0     1391 2024-05-12 04:11:25.416157 recycling-1.0.0/venues/stages/recycling/instrument/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2024-02-25 04:12:05.725626 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger
--rwxr-xr-x   0        0        0       21 2024-02-25 04:12:05.725626 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.lock
--rwxr-xr-x   0        0        0     1463 2024-02-25 05:34:11.247537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.turtle
--rwxr-xr-x   0        0        0    49152 2024-02-25 05:34:11.251537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.wt
--rwxr-xr-x   0        0        0     4096 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTigerHS.wt
--rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/_mdb_catalog.wt
--rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-0-7108514929992687025.wt
--rwxr-xr-x   0        0        0        4 2024-03-14 20:08:40.248465 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-2-7108514929992687025.wt
--rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-4-7108514929992687025.wt
--rwxr-xr-x   0        0        0        2 2024-03-14 20:08:40.264465 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/diagnostic.data/metrics.2024-02-25T04-12-05Z-00000
--rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-1-7108514929992687025.wt
--rwxr-xr-x   0        0        0    36864 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-3-7108514929992687025.wt
--rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-5-7108514929992687025.wt
--rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-6-7108514929992687025.wt
--rwxr-xr-x   0        0        0        2 2024-03-14 20:08:40.392463 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerLog.0000000002
--rwxr-xr-x   0        0        0 104857600 2024-02-25 05:34:11.167538 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerPreplog.0000000001
--rwxr-xr-x   0        0        0 104857600 2024-02-25 05:34:11.175538 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerPreplog.0000000002
--rwxr-xr-x   0        0        0        0 2024-02-25 05:34:11.255537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/mongod.lock
--rwxr-xr-x   0        0        0    36864 2024-02-25 05:34:11.243537 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/sizeStorer.wt
--rwxr-xr-x   0        0        0      114 2024-02-25 04:12:05.821625 recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/storage.bson
--rwxr-xr-x   0        0        0     1517 2024-03-02 05:12:55.849887 recycling-1.0.0/venues/stages/recycling/instrument/_status/status_1.py
--rwxr-xr-x   0        0        0      801 2024-05-12 04:08:12.654195 recycling-1.0.0/venues/stages/recycling/instrument/climate/__init__.py
--rw-r--r--   0        0        0     1016 2024-05-12 04:10:57.436452 recycling-1.0.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.004470 recycling-1.0.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1067 2024-05-12 04:08:12.554196 recycling-1.0.0/venues/stages/recycling/instrument/clique/__init__.py
--rw-r--r--   0        0        0     1264 2024-05-12 04:10:57.364453 recycling-1.0.0/venues/stages/recycling/instrument/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-12 19:23:02.178089 recycling-1.0.0/venues/stages/recycling/instrument/clique/__pycache__/intro.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/feel-1b84c382.js
--rwxr-xr-x   0        0        0      456 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/futon-180affc4.js
--rwxr-xr-x   0        0        0   561233 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/index-d4db3b65.js
--rwxr-xr-x   0        0        0   190331 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/index-f1fd6021.css
--rwxr-xr-x   0        0        0     1877 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/perform-9529be50.js
--rwxr-xr-x   0        0        0  1214802 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-2bdf6498.js
--rwxr-xr-x   0        0        0      971 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-5131ee29.js
--rwxr-xr-x   0        0        0     3356 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-bd81103e.css
--rwxr-xr-x   0        0        0     5484 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/room-3696ea94.js
--rwxr-xr-x   0        0        0       85 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/room-4d995ba2.css
--rwxr-xr-x   0        0        0      109 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/scenery-593969b1.css
--rwxr-xr-x   0        0        0     2414 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/scenery-de5924ae.js
--rwxr-xr-x   0        0        0   377982 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/subconscious-a94f6af0.js
--rwxr-xr-x   0        0        0    18836 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/vanilla-picker-b74cad28.js
--rwxr-xr-x   0        0        0   325850 2024-03-19 04:47:13.826198 recycling-1.0.0/venues/stages/recycling/instrument/frontend/codesweeper--ai-generated-8311446_1920.jpg
--rwxr-xr-x   0        0        0     4286 2024-03-19 04:47:13.826198 recycling-1.0.0/venues/stages/recycling/instrument/frontend/favicon.ico
--rwxr-xr-x   0        0        0      434 2024-03-19 04:47:14.586189 recycling-1.0.0/venues/stages/recycling/instrument/frontend/index.html
--rwxr-xr-x   0        0        0     1031 2024-05-12 04:08:12.654195 recycling-1.0.0/venues/stages/recycling/instrument/instrument.S.HTML
--rwxr-xr-x   0        0        0      894 2024-05-12 04:08:12.970192 recycling-1.0.0/venues/stages/recycling/instrument/layer/__init__.py
--rw-r--r--   0        0        0     1102 2024-05-12 04:10:57.440452 recycling-1.0.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.108469 recycling-1.0.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      496 2024-05-12 04:10:57.628450 recycling-1.0.0/venues/stages/recycling/instrument/layer/__pycache__/start_dev.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.160469 recycling-1.0.0/venues/stages/recycling/instrument/layer/__pycache__/start_dev.cpython-311.pyc
--rwxr-xr-x   0        0        0     2907 2024-05-12 04:08:12.970192 recycling-1.0.0/venues/stages/recycling/instrument/layer/_clique/__init__.py
--rw-r--r--   0        0        0     2180 2024-05-12 04:10:58.148445 recycling-1.0.0/venues/stages/recycling/instrument/layer/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      411 2024-02-25 04:11:37.786016 recycling-1.0.0/venues/stages/recycling/instrument/layer/flask.s.HTML
--rwxr-xr-x   0        0        0      671 2024-05-12 04:08:12.974192 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__init__.py
--rw-r--r--   0        0        0     1144 2024-05-12 04:10:57.624450 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.073352 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/card_generator.cpython-310.pyc
--rw-r--r--   0        0        0     1160 2024-05-12 04:10:57.624450 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/moves.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 01:08:15.077769 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/seed_generator.cpython-310.pyc
--rwxr-xr-x   0        0        0      510 2024-03-14 20:21:43.375948 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/home/__pycache__/get.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.188468 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/home/__pycache__/get.cpython-311.pyc
--rwxr-xr-x   0        0        0      218 2024-02-13 01:00:25.822302 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/home/get.py
--rwxr-xr-x   0        0        0      849 2024-05-12 04:08:12.974192 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/moves.py
--rwxr-xr-x   0        0        0       57 2024-02-24 21:21:56.451073 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/routes.S.HTML
--rwxr-xr-x   0        0        0     2651 2024-02-25 04:11:37.786016 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vibe_generator.py
--rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.089352 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
--rwxr-xr-x   0        0        0       26 2024-02-24 21:19:00.480992 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vibes/make_ECC_448_2.py
--rwxr-xr-x   0        0        0     1387 2024-02-13 01:22:29.900593 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vue/__init__.py
--rwxr-xr-x   0        0        0     1419 2024-03-14 20:21:43.375948 recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vue/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      124 2024-05-12 04:08:12.970192 recycling-1.0.0/venues/stages/recycling/instrument/layer/start_dev.proc.py
--rwxr-xr-x   0        0        0      269 2024-05-12 04:08:12.970192 recycling-1.0.0/venues/stages/recycling/instrument/layer/start_dev.py
--rwxr-xr-x   0        0        0        0 2023-12-31 20:33:38.333168 recycling-1.0.0/venues/stages/recycling/instrument/layer/start_gunicorn.py
--rw-r--r--   0        0        0     1178 2024-05-12 04:10:57.624450 recycling-1.0.0/venues/stages/recycling/instrument/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc
--rwxr-xr-x   0        0        0     1377 2024-05-12 04:08:12.978192 recycling-1.0.0/venues/stages/recycling/instrument/layer/utilities/generate_path_inventory.py
--rwxr-xr-x   0        0        0      339 2024-02-24 23:56:53.837355 recycling-1.0.0/venues/stages/recycling/instrument/module--names.s.HTML
--rwxr-xr-x   0        0        0      970 2024-05-12 04:08:12.558196 recycling-1.0.0/venues/stages/recycling/instrument/moon/__init__.py
--rw-r--r--   0        0        0      763 2024-05-12 04:10:57.440452 recycling-1.0.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.296468 recycling-1.0.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      453 2024-05-12 04:10:57.976446 recycling-1.0.0/venues/stages/recycling/instrument/moon/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      225 2024-05-12 04:08:12.558196 recycling-1.0.0/venues/stages/recycling/instrument/moon/connect.py
--rwxr-xr-x   0        0        0       36 2023-12-11 06:24:53.248976 recycling-1.0.0/venues/stages/recycling/instrument/moon/mongo.s.HTML
--rw-r--r--   0        0        0     1088 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/enumerate.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 23:56:53.929354 recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      583 2024-05-12 04:08:12.558196 recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/enumerate.py
--rwxr-xr-x   0        0        0       44 2024-02-09 03:14:00.919819 recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/find.py
--rwxr-xr-x   0        0        0       49 2024-02-09 03:13:42.236017 recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/modify.py
--rwxr-xr-x   0        0        0     1967 2024-05-12 04:08:12.694195 recycling-1.0.0/venues/stages/recycling/instrument/moves/__init__.py
--rw-r--r--   0        0        0     2224 2024-05-12 04:10:57.432452 recycling-1.0.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.344467 recycling-1.0.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.069270 recycling-1.0.0/venues/stages/recycling/instrument/moves/__pycache__/create_wallet.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.089269 recycling-1.0.0/venues/stages/recycling/instrument/moves/__pycache__/form_proposal_keys.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-08 22:06:53.105269 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_safe.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.376467 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_safe.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.121269 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_wallet.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 01:08:14.517776 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/form_proposal_keys.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.408467 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/form_proposal_keys.cpython-311.pyc
--rwxr-xr-x   0        0        0      387 2024-03-14 20:21:43.379948 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1194 2024-05-12 04:10:57.436452 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/make.cpython-310.pyc
--rw-r--r--   0        0        0     1393 2024-05-12 04:10:57.436452 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_layer.cpython-310.pyc
--rw-r--r--   0        0        0      844 2024-05-12 04:10:57.436452 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_mongo.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-03-02 05:12:55.949886 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_thermos.cpython-310.pyc
--rw-r--r--   0        0        0     1543 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/__pycache__/feel.cpython-310.pyc
--rwxr-xr-x   0        0        0     1576 2024-05-12 04:08:12.698195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/feel.py
--rw-r--r--   0        0        0      870 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/add.cpython-310.pyc
--rw-r--r--   0        0        0      827 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/bounce.cpython-310.pyc
--rw-r--r--   0        0        0      640 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/show.cpython-310.pyc
--rwxr-xr-x   0        0        0      634 2024-05-12 04:08:12.698195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/add.py
--rwxr-xr-x   0        0        0      576 2024-05-12 04:08:12.698195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/bounce.py
--rwxr-xr-x   0        0        0      379 2024-05-12 04:08:12.702195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/show.py
--rwxr-xr-x   0        0        0      101 2024-02-24 21:49:13.531862 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/is_on.py
--rwxr-xr-x   0        0        0     1219 2024-05-12 04:08:12.706194 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/make.py
--rw-r--r--   0        0        0     1534 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/__pycache__/perform.cpython-310.pyc
--rwxr-xr-x   0        0        0     1438 2024-05-12 04:08:12.702195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/perform.py
--rwxr-xr-x   0        0        0        4 2024-03-14 20:08:41.292454 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/performances/__pycache__/perform.cpython-310.pyc
--rwxr-xr-x   0        0        0     1434 2024-05-12 04:08:12.706194 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/start_layer.py
--rwxr-xr-x   0        0        0      598 2024-05-12 04:08:12.706194 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/start_mongo.py
--rwxr-xr-x   0        0        0      204 2024-05-12 04:08:12.698195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/enumerate/__init__.py
--rw-r--r--   0        0        0      499 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/enumerate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1222 2024-05-12 04:08:12.694195 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__init__.py
--rw-r--r--   0        0        0     1266 2024-05-12 04:10:57.628450 recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1276 2024-05-12 04:08:12.714194 recycling-1.0.0/venues/stages/recycling/instrument/sockets/__init__.py
--rw-r--r--   0        0        0     1774 2024-05-12 04:10:57.364453 recycling-1.0.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.500466 recycling-1.0.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1649 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/instrument/sockets/__pycache__/clique_group.cpython-310.pyc
--rwxr-xr-x   0        0        0     1167 2024-05-12 04:08:12.718194 recycling-1.0.0/venues/stages/recycling/instrument/sockets/clique_group.py
--rwxr-xr-x   0        0        0      384 2024-05-12 04:08:12.554196 recycling-1.0.0/venues/stages/recycling/instrument/start.proc.py
--rwxr-xr-x   0        0        0     1101 2024-05-12 04:08:12.526197 recycling-1.0.0/venues/stages/recycling/module.MD
--rwxr-xr-x   0        0        0     1081 2024-05-12 04:08:12.518196 recycling-1.0.0/venues/stages/recycling/module.s.HTML
--rwxr-xr-x   0        0        0      171 2024-02-22 22:27:05.401905 recycling-1.0.0/venues/stages/recycling/modules/Aztec/Aztec.S.HTML
--rwxr-xr-x   0        0        0        4 2024-02-22 22:27:54.713318 recycling-1.0.0/venues/stages/recycling/modules/Aztec/_school/start.py
--rwxr-xr-x   0        0        0     1148 2024-02-08 21:59:01.774498 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_seed_phrase/2048.r.html
--rwxr-xr-x   0        0        0      128 2024-02-25 04:11:37.786016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_seed_phrase/seed phrase.r.html
--rw-r--r--   0        0        0     1998 2024-05-12 04:11:25.420157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1771 2024-05-12 04:08:12.514196 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_1_generator/status_1.py
--rwxr-xr-x   0        0        0       73 2024-02-25 04:09:53.203482 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_2_generators/EEC_448_1_intimate_rhythm.DER
--rw-r--r--   0        0        0     2508 2024-05-12 04:11:25.396157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_2_generators/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2348 2024-05-12 04:08:12.514196 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_2_generators/status_1.py
--rwxr-xr-x   0        0        0       73 2024-02-25 04:09:53.203482 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_3_sign_and_verify/EEC_448_1_intimate_rhythm.DER
--rw-r--r--   0        0        0     2919 2024-05-12 04:11:25.364157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2970 2024-05-12 04:08:12.514196 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_3_sign_and_verify/status_1.py
--rwxr-xr-x   0        0        0      299 2024-05-12 04:08:12.510197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/clique.py
--rwxr-xr-x   0        0        0     1363 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/module.s.HTML
--rwxr-xr-x   0        0        0      309 2023-09-28 02:28:22.890625 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/SEED--/SPLIT.py
--rwxr-xr-x   0        0        0     1876 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/BUILD.cpython-311.pyc
--rwxr-xr-x   0        0        0     2092 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/CREATE.cpython-311.pyc
--rwxr-xr-x   0        0        0      997 2023-09-27 19:47:39.055871 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/READ.cpython-311.pyc
--rwxr-xr-x   0        0        0     1124 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/SCAN.cpython-311.pyc
--rw-r--r--   0        0        0     1843 2024-05-12 04:14:36.270144 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/creator.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.006495 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/creator.cpython-311.pyc
--rw-r--r--   0        0        0     1050 2024-05-12 04:14:36.274144 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.082494 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/scan.cpython-311.pyc
--rwxr-xr-x   0        0        0      365 2024-01-17 04:01:10.530210 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/adapt/DER_to_hexadecimal.py
--rwxr-xr-x   0        0        0      249 2024-01-17 04:02:34.420248 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/adapt/hexadecimal_to_DER.py
--rwxr-xr-x   0        0        0     2635 2024-05-12 04:08:12.494197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/creator.py
--rwxr-xr-x   0        0        0        0 2024-01-17 04:03:13.555799 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/form.py
--rwxr-xr-x   0        0        0      322 2024-02-08 21:59:02.126494 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/read.py
--rwxr-xr-x   0        0        0      677 2024-05-12 04:08:12.494197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/scan.py
--rwxr-xr-x   0        0        0     1244 2024-02-25 04:10:25.159032 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/BUILD--.py
--rwxr-xr-x   0        0        0     2100 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/BUILD.cpython-311.pyc
--rwxr-xr-x   0        0        0     2365 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/CREATE.cpython-311.pyc
--rwxr-xr-x   0        0        0     1149 2024-02-25 04:11:37.790016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/SCAN.cpython-311.pyc
--rw-r--r--   0        0        0     1768 2024-05-12 04:14:36.386143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/creator.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.286492 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/creator.cpython-311.pyc
--rw-r--r--   0        0        0     1142 2024-05-12 04:14:36.274144 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/form.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.426490 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/form.cpython-311.pyc
--rw-r--r--   0        0        0      752 2024-05-12 04:14:36.390143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.498489 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/scan.cpython-311.pyc
--rw-r--r--   0        0        0      783 2024-05-12 04:14:36.274144 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/write.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.638487 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/write.cpython-311.pyc
--rwxr-xr-x   0        0        0     2073 2024-05-12 04:08:12.502197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/creator.py
--rwxr-xr-x   0        0        0     1059 2024-05-12 04:08:12.502197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/form.py
--rwxr-xr-x   0        0        0      667 2024-05-12 04:08:12.502197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/scan.py
--rwxr-xr-x   0        0        0      579 2024-05-12 04:08:12.502197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/write.py
--rwxr-xr-x   0        0        0      938 2024-05-12 04:08:12.490197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/sign/__init__.py
--rw-r--r--   0        0        0     1458 2024-05-12 04:14:36.386143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/sign/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.834485 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/sign/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2724 2024-05-12 04:08:12.490197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/tutorial.s.HTML
--rwxr-xr-x   0        0        0      838 2024-05-12 04:08:12.510197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/verify/__init__.py
--rw-r--r--   0        0        0      779 2024-05-12 04:14:36.386143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/verify/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.918484 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/verify/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1390 2024-04-24 04:36:58.990305 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/EEC_448_2.HTML
--rw-r--r--   0        0        0       73 2024-05-12 04:14:36.470142 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/EEC_448_2_private_key.DER
--rw-r--r--   0        0        0      213 2024-05-12 04:14:36.334143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/EEC_448_2_private_key.JSON
--rw-r--r--   0        0        0     2484 2024-05-12 04:11:25.364157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/__pycache__/status_DER_1.cpython-310.pyc
--rw-r--r--   0        0        0     2485 2024-05-12 04:11:25.360157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/__pycache__/status_JSON_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2538 2024-05-12 04:08:12.466197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/status_DER_1.py
--rwxr-xr-x   0        0        0     2498 2024-05-12 04:08:12.466197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/status_JSON_1.py
--rw-r--r--   0        0        0     3194 2024-05-12 04:11:25.384157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_2_private_and_public_keys/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     3448 2024-05-12 04:08:12.466197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py
--rw-r--r--   0        0        0     4525 2024-05-12 04:11:25.364157 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     5386 2024-05-12 04:08:12.462197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_3_sign_and_verify/status_1.py
--rwxr-xr-x   0        0        0      299 2024-05-12 04:08:12.458197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/clique.py
--rw-r--r--   0        0        0      951 2024-04-24 04:36:09.143244 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/cryptography.py.S.HTML
--rwxr-xr-x   0        0        0     1120 2024-05-12 04:08:12.466197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/keys/__init__.py
--rw-r--r--   0        0        0      996 2024-05-12 04:10:57.976446 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/keys/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      524 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/byte_string/__pycache__/from_UTF8.cpython-310.pyc
--rw-r--r--   0        0        0      577 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/byte_string/__pycache__/from_hexadecimal.cpython-310.pyc
--rwxr-xr-x   0        0        0      316 2024-05-12 04:08:12.446197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/byte_string/from_UTF8.py
--rwxr-xr-x   0        0        0      374 2024-05-12 04:08:12.446197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/byte_string/from_hexadecimal.py
--rw-r--r--   0        0        0      534 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/hexadecimal/__pycache__/from_byte_string.cpython-310.pyc
--rwxr-xr-x   0        0        0      327 2024-05-12 04:08:12.446197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/hexadecimal/from_byte_string.py
--rwxr-xr-x   0        0        0      407 2024-04-28 18:58:17.221951 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/names.s.HTML
--rwxr-xr-x   0        0        0     1876 2024-02-25 04:11:37.794016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/BUILD.cpython-311.pyc
--rwxr-xr-x   0        0        0     2092 2024-02-25 04:11:37.794016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/CREATE.cpython-311.pyc
--rwxr-xr-x   0        0        0      997 2023-09-27 19:47:39.055871 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/READ.cpython-311.pyc
--rwxr-xr-x   0        0        0     1124 2024-02-25 04:11:37.794016 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/SCAN.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2024-05-12 04:10:57.980446 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/creator.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.006495 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/creator.cpython-311.pyc
--rw-r--r--   0        0        0      775 2024-05-12 04:14:36.198145 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/etch.cpython-310.pyc
--rw-r--r--   0        0        0     1030 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/instance.cpython-310.pyc
--rw-r--r--   0        0        0     1303 2024-05-12 04:10:58.132445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.082494 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/scan.cpython-311.pyc
--rwxr-xr-x   0        0        0      365 2024-01-17 04:01:10.530210 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/adapt/DER_to_hexadecimal.py
--rwxr-xr-x   0        0        0      249 2024-01-17 04:02:34.420248 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/adapt/hexadecimal_to_DER.py
--rwxr-xr-x   0        0        0     1672 2024-05-12 04:08:12.438197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/creator.py
--rwxr-xr-x   0        0        0      650 2024-05-12 04:08:12.438197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/etch.py
--rwxr-xr-x   0        0        0      958 2024-05-12 04:08:12.438197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/instance.py
--rwxr-xr-x   0        0        0      216 2024-02-25 04:11:37.798015 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/private_key.s.HTML
--rwxr-xr-x   0        0        0      876 2024-05-12 04:08:12.438197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/scan.py
--rwxr-xr-x   0        0        0     2100 2024-02-25 04:11:37.798015 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/BUILD.cpython-311.pyc
--rwxr-xr-x   0        0        0     2365 2024-02-25 04:11:37.798015 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/CREATE.cpython-311.pyc
--rwxr-xr-x   0        0        0     1149 2024-02-25 04:11:37.798015 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/SCAN.cpython-311.pyc
--rw-r--r--   0        0        0     1390 2024-05-12 04:10:58.132445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/creator.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.286492 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/creator.cpython-311.pyc
--rw-r--r--   0        0        0      781 2024-05-12 04:14:36.362143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-12 20:12:29.184426 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/form.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.426490 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/form.cpython-311.pyc
--rw-r--r--   0        0        0     1030 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/instance.cpython-310.pyc
--rw-r--r--   0        0        0      886 2024-05-12 04:14:36.362143 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.498489 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/scan.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2024-02-12 20:12:29.268425 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/write.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.638487 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/write.cpython-311.pyc
--rwxr-xr-x   0        0        0     1429 2024-05-12 04:08:12.450197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/creator.py
--rwxr-xr-x   0        0        0      610 2024-05-12 04:08:12.450197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/etch.py
--rwxr-xr-x   0        0        0      959 2024-05-12 04:08:12.450197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/instance.py
--rwxr-xr-x   0        0        0       25 2024-02-12 23:23:16.361700 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/public_key.s.HTML
--rwxr-xr-x   0        0        0      839 2024-05-12 04:08:12.450197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/scan.py
--rwxr-xr-x   0        0        0     1182 2024-05-12 04:08:12.462197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/rhythms/__init__.py
--rwxr-xr-x   0        0        0        4 2024-03-14 20:08:42.728438 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/rhythms/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1054 2024-05-12 04:08:12.434198 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/sign/__init__.py
--rw-r--r--   0        0        0     1339 2024-05-12 04:10:58.136445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/sign/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.834485 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/sign/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     5677 2024-05-12 04:08:12.430198 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/tutorial.s.HTML
--rwxr-xr-x   0        0        0      860 2024-05-12 04:08:12.462197 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/verify/__init__.py
--rw-r--r--   0        0        0      658 2024-05-12 04:10:58.140445 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/verify/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.918484 recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/verify/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      133 2024-05-12 04:08:12.470197 recycling-1.0.0/venues/stages/recycling/modules/QR/UTF8/__init__.py
--rwxr-xr-x   0        0        0     1194 2024-01-16 06:43:32.902697 recycling-1.0.0/venues/stages/recycling/modules/QR/__init__.py
--rwxr-xr-x   0        0        0       28 2024-02-09 01:33:19.884331 recycling-1.0.0/venues/stages/recycling/modules/QR/module.s.HTML
--rwxr-xr-x   0        0        0        0 2024-01-16 06:33:07.558208 recycling-1.0.0/venues/stages/recycling/modules/QR/photo/interpret.py
--rwxr-xr-x   0        0        0      428 2024-02-24 01:20:41.216739 recycling-1.0.0/venues/stages/recycling/modules/barcodes/barcodes.S.HTML
--rwxr-xr-x   0        0        0        3 2024-02-22 22:32:21.434142 recycling-1.0.0/venues/stages/recycling/modules/barcodes/scan_barcode/scan.S.HTML
--rwxr-xr-x   0        0        0      140 2024-05-12 04:08:12.478197 recycling-1.0.0/venues/stages/recycling/modules/camera/__init__.py
--rwxr-xr-x   0        0        0      175 2024-02-24 01:14:21.021334 recycling-1.0.0/venues/stages/recycling/modules/camera/module.s.HTML
--rwxr-xr-x   0        0        0      261 2024-02-25 04:11:37.798015 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/SECP256K1.s.HTML
--rw-r--r--   0        0        0      588 2024-05-12 04:11:25.364157 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2024-05-12 04:08:12.474197 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/_status/status_1_generator/status_1.py
--rw-r--r--   0        0        0     1082 2024-05-12 04:14:36.242144 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/__pycache__/build.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:03.046483 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/__pycache__/build.cpython-311.pyc
--rwxr-xr-x   0        0        0     1262 2024-05-12 04:08:12.470197 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/build.py
--rwxr-xr-x   0        0        0      419 2024-02-25 04:11:37.802015 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/write.py
--rwxr-xr-x   0        0        0        0 2024-01-17 02:34:03.043494 recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/public_key/build.py
--rwxr-xr-x   0        0        0      174 2024-02-25 04:10:25.867022 recycling-1.0.0/venues/stages/recycling/modules/elliptic/elliptic.s.HTML
--rwxr-xr-x   0        0        0        5 2024-03-14 20:19:45.373245 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2195 2024-05-12 04:14:36.270144 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/__pycache__/form.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 21:59:03.110482 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/__pycache__/form.cpython-311.pyc
--rw-r--r--   0        0        0     1402 2024-05-12 04:11:25.380157 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1175 2024-05-12 04:08:12.482197 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/status_1.py
--rw-r--r--   0        0        0       73 2024-05-12 04:14:36.638140 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/temporary/proposal.private_key.DER
--rw-r--r--   0        0        0      138 2024-05-12 04:14:36.642140 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/temporary/proposal.public_key.DER
--rw-r--r--   0        0        0      114 2024-05-12 04:14:36.642140 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/temporary/proposal.seed
--rw-r--r--   0        0        0     1461 2024-05-12 04:11:25.388157 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1208 2024-05-12 04:08:12.482197 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/status_1.py
--rw-r--r--   0        0        0       73 2024-05-12 04:14:36.362143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.private_key.DER
--rw-r--r--   0        0        0      138 2024-05-12 04:14:36.366143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.public_key.hexadecimal
--rw-r--r--   0        0        0      114 2024-05-12 04:14:36.366143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.seed
--rw-r--r--   0        0        0     1452 2024-05-12 04:11:25.420157 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1218 2024-05-12 04:08:12.478197 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/status_1.py
--rw-r--r--   0        0        0      146 2024-05-12 04:14:36.402143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.private_key.hexadecimal
--rw-r--r--   0        0        0      138 2024-05-12 04:14:36.406143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.public_key.hexadecimal
--rw-r--r--   0        0        0      114 2024-05-12 04:14:36.406143 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.seed
--rwxr-xr-x   0        0        0      231 2024-05-12 04:08:12.478197 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/clique.py
--rwxr-xr-x   0        0        0     2402 2024-05-12 04:08:12.478197 recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/form.py
--rwxr-xr-x   0        0        0      370 2024-05-12 04:08:13.202189 recycling-1.0.0/venues/stages/recycling/procedure.proc.py
--rwxr-xr-x   0        0        0       72 2024-02-24 02:25:48.706413 recycling-1.0.0/venues/stages/recycling/recycling -- development.S.HTML
--rwxr-xr-x   0        0        0       56 2024-04-28 18:55:14.566113 recycling-1.0.0/venues/stages/recycling/recycling -- vocab.HTML
--rwxr-xr-x   0        0        0        2 2024-01-05 01:01:30.825976 recycling-1.0.0/venues/stages/recycling/source.zsh
--rwxr-xr-x   0        0        0      262 2024-02-25 04:11:37.802015 recycling-1.0.0/venues/stages/recycling/stage/__agenda/agenda.s.HTML
--rwxr-xr-x   0        0        0   344999 2024-02-05 18:23:32.425545 recycling-1.0.0/venues/stages/recycling/stage/__book/dlsdkcgl--ai-generated-8315813_1920.jpg
--rwxr-xr-x   0        0        0      188 2024-05-12 04:08:13.006191 recycling-1.0.0/venues/stages/recycling/stage/__init__.py
--rw-r--r--   0        0        0      445 2024-05-12 04:10:58.148445 recycling-1.0.0/venues/stages/recycling/stage/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.839550 recycling-1.0.0/venues/stages/recycling/stage/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.712464 recycling-1.0.0/venues/stages/recycling/stage/__pycache__/clique.cpython-311.pyc
--rw-r--r--   0        0        0      277 2024-05-12 04:11:25.440157 recycling-1.0.0/venues/stages/recycling/stage/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       63 2024-02-09 05:06:03.804904 recycling-1.0.0/venues/stages/recycling/stage/_status/status_1.py
--rwxr-xr-x   0        0        0      743 2024-05-12 04:08:13.150190 recycling-1.0.0/venues/stages/recycling/stage/climate/__init__.py
--rw-r--r--   0        0        0      971 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/climate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      822 2024-05-12 04:08:13.006191 recycling-1.0.0/venues/stages/recycling/stage/clique/__init__.py
--rw-r--r--   0        0        0     1152 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0   190579 2024-03-19 04:47:24.502077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/index-BizSwkP3.css
--rwxr-xr-x   0        0        0   544287 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/index-DIdFDc9G.js
--rwxr-xr-x   0        0        0     1099 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/reel-DvvsKiXw.js
--rwxr-xr-x   0        0        0  1215093 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-BPO9cr18.js
--rwxr-xr-x   0        0        0     3356 2024-03-19 04:47:24.502077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-DSl6fGcC.css
--rwxr-xr-x   0        0        0   852013 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-gSMgJBY7.js
--rwxr-xr-x   0        0        0    18836 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/vanilla-picker-DfFJQbG4.js
--rwxr-xr-x   0        0        0   430054 2024-03-19 04:47:23.618087 recycling-1.0.0/venues/stages/recycling/stage/frontend/codesweeper--ai-generated-8311450_1920.jpg
--rwxr-xr-x   0        0        0     4286 2024-03-19 04:47:23.618087 recycling-1.0.0/venues/stages/recycling/stage/frontend/favicon.ico
--rwxr-xr-x   0        0        0      442 2024-03-19 04:47:24.506077 recycling-1.0.0/venues/stages/recycling/stage/frontend/index.html
--rwxr-xr-x   0        0        0      868 2024-05-12 04:08:13.186190 recycling-1.0.0/venues/stages/recycling/stage/layer/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.108469 recycling-1.0.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      471 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/layer/__pycache__/start_dev.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.160469 recycling-1.0.0/venues/stages/recycling/stage/layer/__pycache__/start_dev.cpython-311.pyc
--rwxr-xr-x   0        0        0     1743 2024-05-12 04:08:13.186190 recycling-1.0.0/venues/stages/recycling/stage/layer/_clique/__init__.py
--rw-r--r--   0        0        0     2162 2024-05-12 04:10:58.160445 recycling-1.0.0/venues/stages/recycling/stage/layer/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      411 2024-02-25 04:11:37.786015 recycling-1.0.0/venues/stages/recycling/stage/layer/flask.s.HTML
--rwxr-xr-x   0        0        0      641 2024-05-12 04:08:13.190189 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__init__.py
--rw-r--r--   0        0        0     1109 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.073352 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/card_generator.cpython-310.pyc
--rw-r--r--   0        0        0     1145 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/moves.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-02-24 01:08:15.077769 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/seed_generator.cpython-310.pyc
--rwxr-xr-x   0        0        0      505 2024-03-14 20:21:43.975941 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/home/__pycache__/get.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.188468 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/home/__pycache__/get.cpython-311.pyc
--rwxr-xr-x   0        0        0      218 2024-02-13 01:00:25.822302 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/home/get.py
--rwxr-xr-x   0        0        0      844 2024-05-12 04:08:13.194189 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/moves.py
--rwxr-xr-x   0        0        0       57 2024-02-24 21:21:56.451073 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/routes.S.HTML
--rwxr-xr-x   0        0        0     2651 2024-02-25 04:11:37.786015 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vibe_generator.py
--rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.089352 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
--rwxr-xr-x   0        0        0       26 2024-02-24 21:19:00.480991 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vibes/make_ECC_448_2.py
--rwxr-xr-x   0        0        0     1387 2024-02-13 01:22:29.900593 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vue/__init__.py
--rwxr-xr-x   0        0        0     1414 2024-03-14 20:21:43.975941 recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vue/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-05-12 04:08:13.190189 recycling-1.0.0/venues/stages/recycling/stage/layer/start_dev.proc.py
--rwxr-xr-x   0        0        0      249 2024-05-12 04:08:13.186190 recycling-1.0.0/venues/stages/recycling/stage/layer/start_dev.py
--rwxr-xr-x   0        0        0        0 2023-12-31 20:33:38.333168 recycling-1.0.0/venues/stages/recycling/stage/layer/start_gunicorn.py
--rw-r--r--   0        0        0     1168 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc
--rwxr-xr-x   0        0        0     1372 2024-05-12 04:08:13.198189 recycling-1.0.0/venues/stages/recycling/stage/layer/utilities/generate_path_inventory.py
--rw-r--r--   0        0        0      448 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moon/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      227 2024-05-12 04:08:13.006191 recycling-1.0.0/venues/stages/recycling/stage/moon/connect.py
--rwxr-xr-x   0        0        0     2394 2024-05-12 04:08:13.166190 recycling-1.0.0/venues/stages/recycling/stage/moves/__init__.py
--rw-r--r--   0        0        0     2516 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.344467 recycling-1.0.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.069269 recycling-1.0.0/venues/stages/recycling/stage/moves/__pycache__/create_wallet.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.089269 recycling-1.0.0/venues/stages/recycling/stage/moves/__pycache__/form_proposal_keys.cpython-311.pyc
--rwxr-xr-x   0        0        0      306 2024-03-03 01:02:12.544244 recycling-1.0.0/venues/stages/recycling/stage/moves/_procedures/fees/fees.S.HTML
--rwxr-xr-x   0        0        0      382 2024-03-14 20:21:43.975941 recycling-1.0.0/venues/stages/recycling/stage/moves/names/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1339 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/__pycache__/start_layer.cpython-310.pyc
--rw-r--r--   0        0        0      839 2024-05-12 04:10:58.152445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/__pycache__/start_mongo.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2024-02-24 21:49:13.531862 recycling-1.0.0/venues/stages/recycling/stage/moves/names/is_on.py
--rw-r--r--   0        0        0     1016 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/add_splendor.cpython-310.pyc
--rw-r--r--   0        0        0      982 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/establish_rules.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-03-14 20:08:43.676428 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce.cpython-310.pyc
--rw-r--r--   0        0        0     1000 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce_Ehh.cpython-310.pyc
--rwxr-xr-x   0        0        0      850 2024-05-12 04:08:13.166190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/add_splendor.py
--rwxr-xr-x   0        0        0      981 2024-05-12 04:08:13.166190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/establish_rules.py
--rwxr-xr-x   0        0        0      803 2024-05-12 04:08:13.166190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/produce_Ehh.py
--rwxr-xr-x   0        0        0      105 2024-03-03 01:07:24.945416 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/squish/generate.py
--rw-r--r--   0        0        0      835 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/establish.cpython-310.pyc
--rw-r--r--   0        0        0      965 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/freshest.cpython-310.pyc
--rwxr-xr-x   0        0        0      646 2024-05-12 04:08:13.174190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/establish.py
--rwxr-xr-x   0        0        0      732 2024-05-12 04:08:13.174190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/freshest.py
--rwxr-xr-x   0        0        0       24 2024-03-03 00:45:01.343933 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_insights/end.py
--rw-r--r--   0        0        0      860 2024-05-12 04:10:58.156445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/__pycache__/enumerate.cpython-310.pyc
--rwxr-xr-x   0        0        0      569 2024-05-12 04:08:13.170190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/enumerate.py
--rw-r--r--   0        0        0      654 2024-05-12 04:10:58.160445 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/receive.cpython-310.pyc
--rwxr-xr-x   0        0        0      376 2024-03-14 20:21:43.979941 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/send.cpython-310.pyc
--rwxr-xr-x   0        0        0      377 2024-05-12 04:08:13.174190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/receive.py
--rwxr-xr-x   0        0        0       77 2024-03-03 02:13:17.424736 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/send.py
--rwxr-xr-x   0        0        0      378 2024-05-12 04:08:13.178190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/rules/change.py
--rwxr-xr-x   0        0        0     1256 2024-05-12 04:08:13.178190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/start_layer.py
--rwxr-xr-x   0        0        0      598 2024-05-12 04:08:13.178190 recycling-1.0.0/venues/stages/recycling/stage/moves/names/start_mongo.py
--rwxr-xr-x   0        0        0      459 2024-02-08 21:27:24.131388 recycling-1.0.0/venues/stages/recycling/stage/names.s.HTML
--rwxr-xr-x   0        0        0      770 2024-02-25 04:11:37.802015 recycling-1.0.0/venues/stages/recycling/stage/stage.s.HTML
--rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 recycling-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1357 2024-05-30 05:09:14.004157 recycling-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1660 2024-05-30 05:10:33.875484 recycling-1.1.0/venue.S.HTML
+-rwxr-xr-x   0        0        0      701 2024-02-25 04:11:37.770016 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/delegates/delegates.r.html
+-rwxr-xr-x   0        0        0      148 2023-11-23 17:10:27.664329 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/delegates/pools.r.HTML
+-rwxr-xr-x   0        0        0      348 2023-11-23 17:12:35.903844 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/fees/fees.r.HTML
+-rwxr-xr-x   0        0        0      671 2024-02-25 04:11:37.770016 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/queue/queue.r.html
+-rwxr-xr-x   0        0        0     1953 2024-02-25 04:11:37.770016 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/voters.s.HTML
+-rwxr-xr-x   0        0        0      805 2024-02-24 01:12:30.622670 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/2. advancements/moderation/moderation.r.html
+-rwxr-xr-x   0        0        0     3106 2024-02-24 01:12:30.638670 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/2. advancements/wallet.svg
+-rwxr-xr-x   0        0        0     2192 2024-04-24 19:48:32.704059 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/priorities.html
+-rwxr-xr-x   0        0        0      949 2024-05-29 04:12:49.232672 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/_themes.S.HTML
+-rwxr-xr-x   0        0        0       58 2024-05-29 03:58:03.234038 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/business.S.HTML
+-rwxr-xr-x   0        0        0      164 2024-05-29 04:01:18.899892 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/garbage.S.HTML
+-rwxr-xr-x   0        0        0       28 2024-05-29 03:59:10.433293 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/grocercies.S.HTML
+-rwxr-xr-x   0        0        0       58 2024-05-29 03:57:31.682392 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/life.S.HTML
+-rwxr-xr-x   0        0        0       86 2024-05-29 03:58:21.313837 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/motion_pictures.S.HTML
+-rwxr-xr-x   0        0        0       92 2024-05-29 04:03:02.770778 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/social.S.HTML
+-rwxr-xr-x   0        0        0      275 2024-05-29 04:28:37.891059 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/genetics.S.HTML
+-rw-r--r--   0        0        0      251 2024-05-29 21:49:43.839561 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/escrow/receive escrow.S.HTML
+-rw-r--r--   0        0        0      203 2024-05-29 21:49:08.120023 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/escrow/send escrow.S.HTML
+-rw-r--r--   0        0        0       31 2024-05-29 21:56:10.034779 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/founder/produce mottos.S.HTML
+-rw-r--r--   0        0        0      660 2024-05-29 21:46:46.585903 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/founder/produce traits.S.HTML
+-rw-r--r--   0        0        0      293 2024-05-29 21:47:50.717041 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/founder/promote to voter.S.HTML
+-rw-r--r--   0        0        0       29 2024-05-29 21:55:13.403461 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/mottos/modify.S.HTML
+-rw-r--r--   0        0        0      395 2024-05-29 21:55:58.514917 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/sequences.S.HTML
+-rw-r--r--   0        0        0      151 2024-05-29 22:10:08.525061 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/voters/demote from voter.S.HTML
+-rw-r--r--   0        0        0      152 2024-05-29 22:10:15.180986 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/1_sequences/voters/promote to voter.S.HTML
+-rw-r--r--   0        0        0       71 2024-05-29 18:37:04.914464 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/2_genes/genes.S.HTML
+-rwxr-xr-x   0        0        0     1509 2024-05-29 22:13:05.035061 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/3_genome/genome.S.HTML
+-rwxr-xr-x   0        0        0     1206 2024-05-29 21:41:47.366223 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/genetics.S.HTML
+-rw-r--r--   0        0        0      765 2024-05-29 21:41:31.582468 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics/genetics:tags.S.HTML
+-rwxr-xr-x   0        0        0      466 2024-05-29 19:09:22.721941 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/genetics.HTML
+-rw-r--r--   0        0        0      224 2024-05-29 21:08:57.044415 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/organisms.S.HTML
+-rw-r--r--   0        0        0      144 2024-05-29 18:11:57.460899 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/[_rhythms_]/rhythms.S.HTML
+-rw-r--r--   0        0        0      381 2024-05-29 21:07:40.597148 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/seeds/seeds.S.HTML
+-rwxr-xr-x   0        0        0      688 2024-05-29 18:06:17.464397 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/vibes.s.HTML
+-rwxr-xr-x   0        0        0      706 2024-04-24 20:08:05.409410 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/vibes:tags.HTML
+-rw-r--r--   0        0        0      351 2024-05-29 18:12:42.404166 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/vibes:tags2.S.HTML
+-rwxr-xr-x   0        0        0       67 2024-05-29 04:38:39.448201 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/[_rhythms_]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      270 2024-05-29 04:38:59.759886 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/[_rhythms_]/possibilities.S.HTML
+-rwxr-xr-x   0        0        0      254 2024-05-29 04:38:53.679980 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/[themes]/themes.S.HTML
+-rwxr-xr-x   0        0        0      668 2024-05-29 20:02:40.523620 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/aphrodisiac/aphrodisiac.S.HTML
+-rw-r--r--   0        0        0      140 2024-05-29 21:10:03.763769 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/aphrodisiac/delegation/delegation.S.HTML
+-rw-r--r--   0        0        0     1788 2024-05-30 04:00:14.346118 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/aphrodisiac/gene_ordering_organism/gene_ordering_organism.S.HTML
+-rw-r--r--   0        0        0      423 2024-05-29 18:39:59.712638 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/aphrodisiac/membership/membership.S.HTML
+-rwxr-xr-x   0        0        0      118 2024-05-29 04:37:13.889565 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/[themes]/themes.S.HTML
+-rwxr-xr-x   0        0        0      263 2024-05-29 19:06:59.651626 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/_nets/dev_nets.S.HTML
+-rw-r--r--   0        0        0      437 2024-05-29 21:13:40.801646 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/info/info.S.HTML
+-rwxr-xr-x   0        0        0      529 2024-05-29 05:14:48.999300 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/__anatomy/anatomy.S.HTML
+-rwxr-xr-x   0        0        0      470 2024-05-29 05:12:31.980597 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/_fees/fees.S.HTML
+-rwxr-xr-x   0        0        0      872 2024-05-29 05:08:13.574883 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/escrow/escrow.S.HTML
+-rwxr-xr-x   0        0        0      554 2024-05-29 18:35:00.603775 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/mottoes/mottoes.S.HTML
+-rwxr-xr-x   0        0        0      415 2024-05-29 05:10:04.013936 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/petitions.S.HTML
+-rwxr-xr-x   0        0        0      133 2024-05-29 22:10:11.517027 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/voters/voters.S.HTML
+-rwxr-xr-x   0        0        0     2237 2024-05-29 20:52:51.453955 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/venue.S.HTML
+-rw-r--r--   0        0        0      266 2024-05-29 19:05:58.600351 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/_ordering/ordering.S.HTML
+-rwxr-xr-x   0        0        0       51 2024-05-29 04:41:55.281284 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/active/active_voting.S.HTML
+-rwxr-xr-x   0        0        0   202363 2024-04-24 05:21:48.221999 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/passive/kinds/picker queue.jpeg
+-rwxr-xr-x   0        0        0      474 2024-05-29 05:13:10.568236 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/passive/kinds/picker_queue.HTML
+-rwxr-xr-x   0        0        0     1061 2024-05-29 04:42:06.073130 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/passive/passive_voting.S.HTML
+-rwxr-xr-x   0        0        0      443 2024-05-29 04:40:19.606678 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/voting.S.HTML
+-rw-r--r--   0        0        0      451 2024-05-29 18:59:11.369321 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/voting:tags.S.HTML
+-rwxr-xr-x   0        0        0      138 2024-05-29 19:10:49.916922 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/organs.S.HTML
+-rwxr-xr-x   0        0        0      493 2024-05-29 18:41:04.399966 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/traits/_objectives.S.HTML
+-rwxr-xr-x   0        0        0       45 2024-05-29 05:15:52.982679 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/traits/_themes.S.HTML
+-rwxr-xr-x   0        0        0      292 2024-05-29 04:20:18.036105 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/traits/traits.S.HTML
+-rwxr-xr-x   0        0        0      261 2024-04-24 19:06:32.683453 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/2_apps/apps.S.HTML
+-rwxr-xr-x   0        0        0    23774 2023-11-08 06:57:41.841464 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/2_apps/pay wall.svg
+-rwxr-xr-x   0        0        0      948 2024-04-24 20:07:36.661726 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/2_smart_contracts/smart_contracts.S.HTML
+-rwxr-xr-x   0        0        0      414 2024-05-25 05:03:38.699190 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/3_L2s/L2.S.HTML
+-rwxr-xr-x   0        0        0      156 2024-05-25 05:04:02.603139 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/4_physicals/physicals.S.HTML
+-rwxr-xr-x   0        0        0      311 2024-05-25 05:03:10.323270 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/MVP.S.HTML
+-rwxr-xr-x   0        0        0      925 2024-04-24 18:17:42.425185 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/later, vibes.S.HTML
+-rwxr-xr-x   0        0        0     2361 2024-05-25 04:38:47.270758 recycling-1.1.0/venues/stages/recycling/[_rhythms_]/proposals.S.HTML
+-rwxr-xr-x   0        0        0      241 2024-05-12 04:08:12.522196 recycling-1.1.0/venues/stages/recycling/[license]/license.s.HTML
+-rwxr-xr-x   0        0        0    37277 2024-02-25 04:11:37.778016 recycling-1.1.0/venues/stages/recycling/[license]/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      394 2024-05-12 04:08:13.222189 recycling-1.1.0/venues/stages/recycling/____shows/recycling_1
+-rwxr-xr-x   0        0        0   255862 2024-02-08 22:34:22.772280 recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311435_1920.jpg
+-rwxr-xr-x   0        0        0   325850 2024-02-08 22:34:42.900056 recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311446_1920.jpg
+-rwxr-xr-x   0        0        0   430054 2024-02-08 22:34:01.964510 recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311450_1920.jpg
+-rwxr-xr-x   0        0        0      174 2024-05-12 04:08:12.522196 recycling-1.1.0/venues/stages/recycling/__init__.py
+-rwxr-xr-x   0        0        0      916 2024-05-25 04:33:24.898153 recycling-1.1.0/venues/stages/recycling/_clique/__init__.py
+-rwxr-xr-x   0        0        0     1143 2024-05-25 04:43:25.939682 recycling-1.1.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-05 19:29:21.596475 recycling-1.1.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 01:08:10.745821 recycling-1.1.0/venues/stages/recycling/_clique/__pycache__/intro.cpython-310.pyc
+-rwxr-xr-x   0        0        0       14 2023-11-23 22:42:42.966463 recycling-1.1.0/venues/stages/recycling/_status/.gitignore
+-rwxr-xr-x   0        0        0   356182 2024-05-30 05:08:39.768439 recycling-1.1.0/venues/stages/recycling/_status/DB/records.json
+-rwxr-xr-x   0        0        0      914 2024-05-30 05:08:25.032558 recycling-1.1.0/venues/stages/recycling/_status/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-30 05:08:32.456498 recycling-1.1.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-03-14 20:19:40.185302 recycling-1.1.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      339 2024-05-12 04:11:25.420157 recycling-1.1.0/venues/stages/recycling/_status/_stories/story_instrument_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-02-27 05:00:51.041236 recycling-1.1.0/venues/stages/recycling/_status/_stories/story_instrument_1/status_1.py
+-rwxr-xr-x   0        0        0      386 2024-05-25 03:29:19.436205 recycling-1.1.0/venues/stages/recycling/_status/status.proc.py
+-rwxr-xr-x   0        0        0      224 2024-02-17 01:38:10.912059 recycling-1.1.0/venues/stages/recycling/instrument/[_proposals]/agenda.s.HTML
+-rwxr-xr-x   0        0        0   333254 2024-02-08 18:30:08.370149 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/TheDigitalArtist--ai-generated-8228359_1920.jpg
+-rwxr-xr-x   0        0        0   309408 2024-02-08 18:30:31.169965 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/TheDigitalArtist--ai-generated-8228360_1920.jpg
+-rwxr-xr-x   0        0        0      760 2024-02-05 00:38:46.633355 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/ISO_lab.s.HTML
+-rwxr-xr-x   0        0        0     2783 2024-02-24 01:12:30.750668 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/ISO_lab_2.s.HTML
+-rwxr-xr-x   0        0        0      672 2024-02-02 04:01:11.455302 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/write_ISO_to_drive.py
+-rwxr-xr-x   0        0        0       71 2024-02-01 18:31:16.299750 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/compose/compose.s.HTML
+-rwxr-xr-x   0        0        0      945 2024-02-01 19:02:46.302852 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/containers/containers.s.HTML
+-rwxr-xr-x   0        0        0     1364 2024-02-25 04:11:37.782016 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/containers/installations.s.HTML
+-rwxr-xr-x   0        0        0      674 2024-02-01 00:45:37.341120 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/docker.s.HTML
+-rwxr-xr-x   0        0        0      260 2024-05-12 04:08:12.690195 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/essential_installations.s.HTML
+-rwxr-xr-x   0        0        0      207 2024-01-31 22:35:57.782459 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/images/images.s.HTML
+-rwxr-xr-x   0        0        0     1265 2024-01-30 03:31:07.323407 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/hardware.s.HTML
+-rwxr-xr-x   0        0        0   594783 2024-02-05 18:23:07.029822 recycling-1.1.0/venues/stages/recycling/instrument/[novels]/dlsdkcgl--hidden-8315722_1920.jpg
+-rwxr-xr-x   0        0        0      195 2024-05-12 04:08:12.562196 recycling-1.1.0/venues/stages/recycling/instrument/__init__.py
+-rwxr-xr-x   0        0        0      462 2024-05-12 04:10:57.364453 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-03-14 20:19:44.209258 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-12 19:23:01.902091 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.740472 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.687552 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique_socket.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.796471 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique_socket.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.703552 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique_tracks.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:36.864471 recycling-1.1.0/venues/stages/recycling/instrument/__pycache__/clique_tracks.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1391 2024-05-12 04:11:25.416157 recycling-1.1.0/venues/stages/recycling/instrument/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2024-02-25 04:12:05.725626 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger
+-rwxr-xr-x   0        0        0       21 2024-02-25 04:12:05.725626 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.lock
+-rwxr-xr-x   0        0        0     1463 2024-02-25 05:34:11.247537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.turtle
+-rwxr-xr-x   0        0        0    49152 2024-02-25 05:34:11.251537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.wt
+-rwxr-xr-x   0        0        0     4096 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTigerHS.wt
+-rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/_mdb_catalog.wt
+-rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-0-7108514929992687025.wt
+-rwxr-xr-x   0        0        0        4 2024-03-14 20:08:40.248465 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-2-7108514929992687025.wt
+-rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-4-7108514929992687025.wt
+-rwxr-xr-x   0        0        0        2 2024-03-14 20:08:40.264465 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/diagnostic.data/metrics.2024-02-25T04-12-05Z-00000
+-rwxr-xr-x   0        0        0    20480 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-1-7108514929992687025.wt
+-rwxr-xr-x   0        0        0    36864 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-3-7108514929992687025.wt
+-rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-5-7108514929992687025.wt
+-rwxr-xr-x   0        0        0     4096 2024-02-25 04:12:06.113621 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-6-7108514929992687025.wt
+-rwxr-xr-x   0        0        0        2 2024-03-14 20:08:40.392463 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerLog.0000000002
+-rwxr-xr-x   0        0        0 104857600 2024-02-25 05:34:11.167538 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerPreplog.0000000001
+-rwxr-xr-x   0        0        0 104857600 2024-02-25 05:34:11.175538 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/journal/WiredTigerPreplog.0000000002
+-rwxr-xr-x   0        0        0        0 2024-02-25 05:34:11.255537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/mongod.lock
+-rwxr-xr-x   0        0        0    36864 2024-02-25 05:34:11.243537 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/sizeStorer.wt
+-rwxr-xr-x   0        0        0      114 2024-02-25 04:12:05.821625 recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/storage.bson
+-rwxr-xr-x   0        0        0     1517 2024-03-02 05:12:55.849887 recycling-1.1.0/venues/stages/recycling/instrument/_status/status_1.py
+-rwxr-xr-x   0        0        0      892 2024-05-26 04:20:15.664447 recycling-1.1.0/venues/stages/recycling/instrument/adventures/__pycache__/ventures.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2024-05-26 02:45:05.954251 recycling-1.1.0/venues/stages/recycling/instrument/adventures/adventures.S.HTML
+-rwxr-xr-x   0        0        0     2485 2024-05-26 03:22:09.880114 recycling-1.1.0/venues/stages/recycling/instrument/adventures/alerting/__init__.py
+-rwxr-xr-x   0        0        0     1855 2024-05-26 03:22:25.767929 recycling-1.1.0/venues/stages/recycling/instrument/adventures/alerting/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-13 01:04:39.753620 recycling-1.1.0/venues/stages/recycling/instrument/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc
+-rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.232563 recycling-1.1.0/venues/stages/recycling/instrument/adventures/alerting/parse_exception.py
+-rwxr-xr-x   0        0        0     1327 2024-01-25 05:00:54.191593 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/HA.s.HTML
+-rwxr-xr-x   0        0        0      238 2023-12-02 04:53:31.462384 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/SSL.r.HTML
+-rwxr-xr-x   0        0        0      985 2023-12-14 02:01:36.217926 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/__init__.py
+-rwxr-xr-x   0        0        0     1086 2024-05-10 01:30:13.387176 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1872 2023-12-14 02:01:38.764897 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1757 2023-12-01 23:15:16.435121 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/certificate.pem
+-rwxr-xr-x   0        0        0     3272 2023-12-01 23:15:16.430121 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/SSL/certificate.pem.key
+-rwxr-xr-x   0        0        0      346 2023-12-01 18:00:33.471576 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/__init__.py
+-rwxr-xr-x   0        0        0      576 2024-05-10 01:29:49.491477 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      661 2024-05-26 04:20:53.748044 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/__pycache__/venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      737 2024-05-12 19:04:34.064153 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      621 2024-05-26 04:25:59.555935 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/__pycache__/build.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-05-26 04:20:53.752044 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      328 2024-05-10 01:44:25.794256 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1095 2024-05-26 04:25:59.555935 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      344 2024-05-26 04:21:07.379855 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/_clique.py
+-rwxr-xr-x   0        0        0      314 2024-05-26 04:20:37.568216 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/build.py
+-rwxr-xr-x   0        0        0      622 2024-05-26 04:20:37.584215 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/is_on.py
+-rwxr-xr-x   0        0        0       77 2024-05-10 01:44:23.514282 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/off.py
+-rwxr-xr-x   0        0        0     1137 2024-05-26 04:24:59.756708 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/_controls/on.py
+-rwxr-xr-x   0        0        0     1295 2023-12-02 01:06:44.630336 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py
+-rwxr-xr-x   0        0        0      567 2023-12-04 23:16:04.198925 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML
+-rwxr-xr-x   0        0        0     1894 2024-05-26 04:20:37.604215 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py
+-rwxr-xr-x   0        0        0     1925 2024-05-26 04:20:53.752044 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2832 2023-12-14 04:27:42.320026 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1296 2023-12-01 22:31:43.018311 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTP_balancer/__init__.py
+-rwxr-xr-x   0        0        0     1774 2023-12-01 22:50:16.802479 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTP_balancer/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      277 2023-12-01 21:44:47.102165 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/HTTP_balancer/examples/example_1.cfg
+-rwxr-xr-x   0        0        0     1652 2023-12-01 18:07:24.317812 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/__pycache__/HTTP_balancer.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3286 2023-12-01 18:05:41.851249 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/examples/haproxy.cfg
+-rwxr-xr-x   0        0        0     2457 2023-12-01 21:46:11.432916 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/examples/haproxy_2.cfg
+-rwxr-xr-x   0        0        0     2191 2024-01-25 05:03:52.719628 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/configs/external_reverse/__init__.py
+-rwxr-xr-x   0        0        0      217 2024-05-10 00:51:31.625386 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/demux.S.HTML
+-rwxr-xr-x   0        0        0      229 2023-12-02 01:03:02.539647 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/journalctl/journalctl.r.HTML
+-rwxr-xr-x   0        0        0      227 2023-12-02 01:02:28.789164 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/systemctl/systemctl.S.HTML
+-rwxr-xr-x   0        0        0      453 2024-05-26 04:20:37.604215 recycling-1.1.0/venues/stages/recycling/instrument/adventures/demux_hap/venture.py
+-rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/.gitignore
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:16.221632 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      922 2024-05-26 03:14:16.245632 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/connect.py
+-rwxr-xr-x   0        0        0      134 2024-05-26 03:14:16.265632 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/goodest_inventory.S.HTML
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:16.317631 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/ion/document/__pycache__/find.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:16.369631 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/ion/document/__pycache__/insert.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1184 2024-05-26 03:14:16.393630 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/ion/document/find.py
+-rwxr-xr-x   0        0        0     2136 2024-05-26 03:14:16.413630 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/DB/template/ion/document/insert.py
+-rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      661 2024-05-26 03:14:31.205458 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/__pycache__/venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:09.837707 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:09.873706 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/__pycache__/build.cpython-310.pyc
+-rwxr-xr-x   0        0        0      995 2024-05-26 03:31:17.925732 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1763 2024-05-26 03:32:03.837198 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      998 2024-05-26 03:24:37.498395 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      768 2024-05-26 03:14:15.841637 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/_clique.py
+-rwxr-xr-x   0        0        0      736 2024-05-26 03:23:57.714858 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/build.py
+-rwxr-xr-x   0        0        0      927 2024-05-26 03:30:27.362321 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/off.py
+-rwxr-xr-x   0        0        0     2462 2024-05-26 03:31:59.077253 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/on.py
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:15.925636 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1659 2024-05-26 03:14:15.949636 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/_clique.py
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:15.965635 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/dumps/__pycache__/dump.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:15.985635 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/dumps/__pycache__/restore.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1584 2024-05-26 03:14:16.005635 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/dumps/dump.py
+-rwxr-xr-x   0        0        0     1512 2024-05-26 03:14:16.025635 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/dumps/restore.py
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:16.045634 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/exports/__pycache__/monetary_export.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-05-26 03:14:16.065634 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/exports/__pycache__/monetary_import.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1467 2024-05-26 03:14:16.085634 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/exports/monetary_export.py
+-rwxr-xr-x   0        0        0     1425 2024-05-26 03:14:16.105634 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/exports/monetary_import.py
+-rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/saves/memories.S.HTML
+-rwxr-xr-x   0        0        0     1073 2024-05-26 03:23:25.747230 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/_controls/status.py
+-rwxr-xr-x   0        0        0      176 2024-05-25 18:51:25.270088 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/monetary.S.HTML
+-rwxr-xr-x   0        0        0      637 2024-05-26 03:14:31.205458 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc
+-rwxr-xr-x   0        0        0      486 2024-05-26 03:14:16.473629 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/moves/URL/retrieve.py
+-rwxr-xr-x   0        0        0      459 2024-05-26 03:14:16.473629 recycling-1.1.0/venues/stages/recycling/instrument/adventures/monetary/venture.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      891 2024-05-26 04:03:16.782965 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/__pycache__/venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1038 2024-05-23 04:00:28.838527 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1239 2024-05-23 04:00:28.838527 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1980 2024-05-26 04:11:20.886057 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      780 2024-05-22 18:43:17.133214 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      900 2024-05-23 03:54:36.162629 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0     1061 2024-05-23 03:55:13.562189 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     2585 2024-05-26 04:10:53.130345 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0     2080 2024-05-22 19:04:00.745851 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/on_v1.py
+-rwxr-xr-x   0        0        0      548 2024-05-26 04:03:13.223000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_controls/refresh.py
+-rwxr-xr-x   0        0        0     1072 2024-05-26 04:03:13.234999 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
+-rwxr-xr-x   0        0        0     1199 2024-05-13 01:14:34.821033 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2594 2024-05-26 04:33:17.110576 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     2101 2024-05-26 04:33:58.098092 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2940 2024-05-26 04:33:55.958118 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/guest_regions_vue/__init__.py
+-rwxr-xr-x   0        0        0     2577 2024-05-26 04:33:58.382089 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/guest_regions_vue/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      563 2024-05-26 04:29:46.733100 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/guest_regions_vue/caching.S.HTML
+-rwxr-xr-x   0        0        0      427 2024-05-26 04:03:13.454997 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/guest_sockets/__init__.py
+-rwxr-xr-x   0        0        0      730 2024-05-26 04:03:17.110961 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/harbor/guest_sockets/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-05-22 20:10:50.989908 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/middles/middles.S.HTML
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      543 2024-05-26 04:03:13.470997 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      300 2024-05-26 04:03:13.486997 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      833 2024-05-26 04:03:13.486997 recycling-1.1.0/venues/stages/recycling/instrument/adventures/sanique/venture.py
+-rwxr-xr-x   0        0        0      704 2024-05-26 04:19:39.672828 recycling-1.1.0/venues/stages/recycling/instrument/adventures/ventures.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/.eslintrc.js--
+-rwxr-xr-x   0        0        0       94 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/.gitignore
+-rwxr-xr-x   0        0        0       26 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/.npmrc
+-rwxr-xr-x   0        0        0      939 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/README.md
+-rwxr-xr-x   0        0        0     1324 2024-05-22 20:32:05.875257 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/[proposals]/objectives -- possibilities.S.HTML
+-rwxr-xr-x   0        0        0       48 2024-05-22 20:31:54.975363 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/[proposals]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      857 2024-05-26 04:57:46.945595 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/__pycache__/venture_build.cpython-310.pyc
+-rwxr-xr-x   0        0        0      751 2024-05-22 19:26:12.429989 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/__pycache__/venture_dev.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-05-14 21:36:02.546959 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/_controls/build.py
+-rwxr-xr-x   0        0        0        2 2024-05-08 21:03:01.449009 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/_controls/off.py
+-rwxr-xr-x   0        0        0        0 2024-05-08 21:06:04.803018 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/_controls/on.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      353 2024-05-09 21:32:18.768121 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/index.html
+-rwxr-xr-x   0        0        0      370 2024-05-10 02:14:54.482607 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/public/vite.svg
+-rwxr-xr-x   0        0        0       23 2024-05-09 21:32:59.207717 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/src/main.js
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/tsconfig.json--
+-rwxr-xr-x   0        0        0      365 2024-05-10 02:14:10.075052 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/school/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      363 2024-05-09 21:34:48.778605 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/index.html
+-rwxr-xr-x   0        0        0      397 2024-05-10 02:10:36.785101 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/public/vite.svg
+-rwxr-xr-x   0        0        0        1 2024-05-09 21:33:50.275202 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/src/main.js
+-rwxr-xr-x   0        0        0      367 2024-05-10 02:08:38.618156 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/staff/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/.eslintrc.cjs--
+-rwxr-xr-x   0        0        0      556 2024-05-08 22:05:09.904886 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/.eslintrc.json
+-rwxr-xr-x   0        0        0      745 2024-05-26 04:20:09.120517 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/index.html
+-rwxr-xr-x   0        0        0      632 2024-05-26 04:18:14.661726 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/package.json
+-rwxr-xr-x   0        0        0      311 2024-05-26 04:56:53.858282 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/app.js
+-rwxr-xr-x   0        0        0     1888 2024-05-23 23:37:23.015065 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js
+-rwxr-xr-x   0        0        0      553 2024-05-26 04:56:46.058384 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js
+-rwxr-xr-x   0        0        0       27 2023-12-08 17:29:39.919713 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/logistics.s.HTML
+-rwxr-xr-x   0        0        0      116 2024-05-26 04:36:43.456163 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js
+-rwxr-xr-x   0        0        0      302 2024-05-26 04:56:11.662835 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue
+-rwxr-xr-x   0        0        0     1202 2024-03-21 19:29:12.760368 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js
+-rwxr-xr-x   0        0        0      373 2023-11-14 00:07:17.821680 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/assets/main.css
+-rwxr-xr-x   0        0        0       59 2024-02-11 19:01:30.792959 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/src/main.js
+-rwxr-xr-x   0        0        0      251 2024-05-26 04:57:49.053568 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/the_build/assets/0.1.0_index.css
+-rwxr-xr-x   0        0        0   904398 2024-05-26 04:57:49.053568 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/the_build/assets/0.1.0_index.js
+-rwxr-xr-x   0        0        0      827 2024-05-26 04:57:49.053568 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/the_build/index.html
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/tsconfig.json--
+-rwxr-xr-x   0        0        0      728 2024-05-15 03:49:51.737456 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/vite.config.js
+-rwxr-xr-x   0        0        0      556 2024-05-08 21:11:26.687514 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/apps/web/vitest.config.js
+-rwxr-xr-x   0        0        0   358624 2024-05-13 01:01:34.311552 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/bun.lockb
+-rwxr-xr-x   0        0        0      521 2024-05-13 00:59:57.104565 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/find_symlinks.py
+-rwxr-xr-x   0        0        0      420 2024-05-10 02:12:07.564248 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/package.json
+-rwxr-xr-x   0        0        0      236 2024-05-08 19:30:19.000000 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/turbo.json
+-rwxr-xr-x   0        0        0      809 2024-05-26 04:57:44.941621 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/venture_build.py
+-rwxr-xr-x   0        0        0      608 2024-05-22 19:26:09.810018 recycling-1.1.0/venues/stages/recycling/instrument/adventures/vv_turbo/venture_dev.py
+-rwxr-xr-x   0        0        0      801 2024-05-12 04:08:12.654195 recycling-1.1.0/venues/stages/recycling/instrument/climate/__init__.py
+-rwxr-xr-x   0        0        0     1016 2024-05-12 04:10:57.436452 recycling-1.1.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.004470 recycling-1.1.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1067 2024-05-12 04:08:12.554196 recycling-1.1.0/venues/stages/recycling/instrument/clique/__init__.py
+-rwxr-xr-x   0        0        0     1264 2024-05-12 04:10:57.364453 recycling-1.1.0/venues/stages/recycling/instrument/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-12 19:23:02.178089 recycling-1.1.0/venues/stages/recycling/instrument/clique/__pycache__/intro.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/feel-1b84c382.js
+-rwxr-xr-x   0        0        0      456 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/futon-180affc4.js
+-rwxr-xr-x   0        0        0   561233 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/index-d4db3b65.js
+-rwxr-xr-x   0        0        0   190331 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/index-f1fd6021.css
+-rwxr-xr-x   0        0        0     1877 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/perform-9529be50.js
+-rwxr-xr-x   0        0        0  1214802 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-2bdf6498.js
+-rwxr-xr-x   0        0        0      971 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-5131ee29.js
+-rwxr-xr-x   0        0        0     3356 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-bd81103e.css
+-rwxr-xr-x   0        0        0     5484 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/room-3696ea94.js
+-rwxr-xr-x   0        0        0       85 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/room-4d995ba2.css
+-rwxr-xr-x   0        0        0      109 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/scenery-593969b1.css
+-rwxr-xr-x   0        0        0     2414 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/scenery-de5924ae.js
+-rwxr-xr-x   0        0        0   377982 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/subconscious-a94f6af0.js
+-rwxr-xr-x   0        0        0    18836 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/vanilla-picker-b74cad28.js
+-rwxr-xr-x   0        0        0   325850 2024-03-19 04:47:13.826198 recycling-1.1.0/venues/stages/recycling/instrument/frontend/codesweeper--ai-generated-8311446_1920.jpg
+-rwxr-xr-x   0        0        0     4286 2024-03-19 04:47:13.826198 recycling-1.1.0/venues/stages/recycling/instrument/frontend/favicon.ico
+-rwxr-xr-x   0        0        0      434 2024-03-19 04:47:14.586189 recycling-1.1.0/venues/stages/recycling/instrument/frontend/index.html
+-rwxr-xr-x   0        0        0     1031 2024-05-12 04:08:12.654195 recycling-1.1.0/venues/stages/recycling/instrument/instrument.S.HTML
+-rwxr-xr-x   0        0        0      913 2024-05-25 04:50:34.017880 recycling-1.1.0/venues/stages/recycling/instrument/layer/__init__.py
+-rwxr-xr-x   0        0        0     1102 2024-05-25 04:51:34.416777 recycling-1.1.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.108469 recycling-1.1.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      519 2024-05-25 04:52:13.547108 recycling-1.1.0/venues/stages/recycling/instrument/layer/__pycache__/start_dev.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.160469 recycling-1.1.0/venues/stages/recycling/instrument/layer/__pycache__/start_dev.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2907 2024-05-12 04:08:12.970192 recycling-1.1.0/venues/stages/recycling/instrument/layer/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2180 2024-05-12 04:10:58.148445 recycling-1.1.0/venues/stages/recycling/instrument/layer/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      411 2024-02-25 04:11:37.786016 recycling-1.1.0/venues/stages/recycling/instrument/layer/flask.s.HTML
+-rwxr-xr-x   0        0        0      671 2024-05-12 04:08:12.974192 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__init__.py
+-rwxr-xr-x   0        0        0     1144 2024-05-12 04:10:57.624450 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.073352 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/card_generator.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1160 2024-05-12 04:10:57.624450 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/moves.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 01:08:15.077769 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/seed_generator.cpython-310.pyc
+-rwxr-xr-x   0        0        0      510 2024-03-14 20:21:43.375948 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/home/__pycache__/get.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.188468 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/home/__pycache__/get.cpython-311.pyc
+-rwxr-xr-x   0        0        0      218 2024-02-13 01:00:25.822302 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/home/get.py
+-rwxr-xr-x   0        0        0      849 2024-05-12 04:08:12.974192 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/moves.py
+-rwxr-xr-x   0        0        0       57 2024-02-24 21:21:56.451073 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/routes.S.HTML
+-rwxr-xr-x   0        0        0     2651 2024-02-25 04:11:37.786016 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vibe_generator.py
+-rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.089352 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0       26 2024-02-24 21:19:00.480992 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vibes/make_ECC_448_2.py
+-rwxr-xr-x   0        0        0     1387 2024-02-13 01:22:29.900593 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vue/__init__.py
+-rwxr-xr-x   0        0        0     1419 2024-03-14 20:21:43.375948 recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vue/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      143 2024-05-25 04:47:17.102692 recycling-1.1.0/venues/stages/recycling/instrument/layer/start_dev.proc.py
+-rwxr-xr-x   0        0        0      294 2024-05-25 04:52:08.263324 recycling-1.1.0/venues/stages/recycling/instrument/layer/start_dev.py
+-rwxr-xr-x   0        0        0     1178 2024-05-12 04:10:57.624450 recycling-1.1.0/venues/stages/recycling/instrument/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1377 2024-05-12 04:08:12.978192 recycling-1.1.0/venues/stages/recycling/instrument/layer/utilities/generate_path_inventory.py
+-rwxr-xr-x   0        0        0      347 2024-05-25 04:34:22.505481 recycling-1.1.0/venues/stages/recycling/instrument/module--names.s.HTML
+-rwxr-xr-x   0        0        0      970 2024-05-12 04:08:12.558196 recycling-1.1.0/venues/stages/recycling/instrument/moon/__init__.py
+-rwxr-xr-x   0        0        0      763 2024-05-12 04:10:57.440452 recycling-1.1.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.296468 recycling-1.1.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      453 2024-05-12 04:10:57.976446 recycling-1.1.0/venues/stages/recycling/instrument/moon/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      225 2024-05-12 04:08:12.558196 recycling-1.1.0/venues/stages/recycling/instrument/moon/connect.py
+-rwxr-xr-x   0        0        0       36 2023-12-11 06:24:53.248976 recycling-1.1.0/venues/stages/recycling/instrument/moon/mongo.s.HTML
+-rwxr-xr-x   0        0        0     1084 2024-05-25 03:29:39.636020 recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/enumerate.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 23:56:53.929354 recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      581 2024-05-25 02:58:24.648045 recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/enumerate.py
+-rwxr-xr-x   0        0        0       44 2024-02-09 03:14:00.919819 recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/find.py
+-rwxr-xr-x   0        0        0       49 2024-02-09 03:13:42.236017 recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/modify.py
+-rwxr-xr-x   0        0        0     1967 2024-05-12 04:08:12.694195 recycling-1.1.0/venues/stages/recycling/instrument/moves/__init__.py
+-rwxr-xr-x   0        0        0     2224 2024-05-12 04:10:57.432452 recycling-1.1.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.344467 recycling-1.1.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.069270 recycling-1.1.0/venues/stages/recycling/instrument/moves/__pycache__/create_wallet.cpython-311.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.089269 recycling-1.1.0/venues/stages/recycling/instrument/moves/__pycache__/form_proposal_keys.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-08 22:06:53.105269 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_safe.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.376467 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_safe.cpython-311.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.121269 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/create_wallet.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 01:08:14.517776 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/form_proposal_keys.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.408467 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/form_proposal_keys.cpython-311.pyc
+-rwxr-xr-x   0        0        0      387 2024-03-14 20:21:43.379948 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1194 2024-05-12 04:10:57.436452 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/make.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1393 2024-05-25 04:52:13.491110 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_layer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      844 2024-05-12 04:10:57.436452 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_mongo.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-03-02 05:12:55.949886 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_thermos.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1533 2024-05-25 03:29:39.644020 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/__pycache__/feel.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1568 2024-05-25 02:58:24.664045 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/feel.py
+-rwxr-xr-x   0        0        0      870 2024-05-12 04:10:58.140445 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/add.cpython-310.pyc
+-rwxr-xr-x   0        0        0      827 2024-05-12 04:10:58.140445 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/bounce.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-05-12 04:10:58.140445 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/show.cpython-310.pyc
+-rwxr-xr-x   0        0        0      634 2024-05-12 04:08:12.698195 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/add.py
+-rwxr-xr-x   0        0        0      576 2024-05-12 04:08:12.698195 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/bounce.py
+-rwxr-xr-x   0        0        0      379 2024-05-12 04:08:12.702195 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/show.py
+-rwxr-xr-x   0        0        0      101 2024-02-24 21:49:13.531862 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/is_on.py
+-rwxr-xr-x   0        0        0     1219 2024-05-12 04:08:12.706194 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/make.py
+-rwxr-xr-x   0        0        0     1526 2024-05-25 03:29:39.636020 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/__pycache__/perform.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1432 2024-05-25 02:58:24.676045 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/perform.py
+-rwxr-xr-x   0        0        0        4 2024-03-14 20:08:41.292454 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/performances/__pycache__/perform.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1434 2024-05-25 04:52:12.231161 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/start_layer.py
+-rwxr-xr-x   0        0        0      598 2024-05-12 04:08:12.706194 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/start_mongo.py
+-rwxr-xr-x   0        0        0      204 2024-05-12 04:08:12.698195 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/enumerate/__init__.py
+-rwxr-xr-x   0        0        0      499 2024-05-12 04:10:58.136445 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/enumerate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1220 2024-05-25 02:58:24.688044 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__init__.py
+-rwxr-xr-x   0        0        0     1262 2024-05-25 03:29:39.052025 recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1276 2024-05-12 04:08:12.714194 recycling-1.1.0/venues/stages/recycling/instrument/sockets/__init__.py
+-rwxr-xr-x   0        0        0     1774 2024-05-12 04:10:57.364453 recycling-1.1.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.500466 recycling-1.1.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1649 2024-05-12 04:10:58.140445 recycling-1.1.0/venues/stages/recycling/instrument/sockets/__pycache__/clique_group.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1167 2024-05-12 04:08:12.718194 recycling-1.1.0/venues/stages/recycling/instrument/sockets/clique_group.py
+-rwxr-xr-x   0        0        0      380 2024-05-25 02:58:24.700044 recycling-1.1.0/venues/stages/recycling/instrument/start.proc.py
+-rwxr-xr-x   0        0        0      321 2024-05-25 05:00:06.240399 recycling-1.1.0/venues/stages/recycling/legend.S.HTML
+-rwxr-xr-x   0        0        0     1148 2024-02-08 21:59:01.774498 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_seed_phrase/2048.r.html
+-rwxr-xr-x   0        0        0      128 2024-02-25 04:11:37.786016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_seed_phrase/seed phrase.r.html
+-rwxr-xr-x   0        0        0     1990 2024-05-29 02:57:43.455675 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1767 2024-05-25 02:58:24.736044 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_1_generator/status_1.py
+-rwxr-xr-x   0        0        0       73 2024-02-25 04:09:53.203482 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_2_generators/EEC_448_1_intimate_rhythm.DER
+-rwxr-xr-x   0        0        0     2500 2024-05-29 02:57:43.395676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_2_generators/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2344 2024-05-25 02:58:24.748044 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_2_generators/status_1.py
+-rwxr-xr-x   0        0        0       73 2024-02-25 04:09:53.203482 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_3_sign_and_verify/EEC_448_1_intimate_rhythm.DER
+-rwxr-xr-x   0        0        0     2907 2024-05-29 02:57:43.407676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2962 2024-05-25 02:58:24.760044 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_3_sign_and_verify/status_1.py
+-rwxr-xr-x   0        0        0      299 2024-05-12 04:08:12.510197 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/clique.py
+-rwxr-xr-x   0        0        0     1363 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/module.s.HTML
+-rwxr-xr-x   0        0        0      309 2023-09-28 02:28:22.890625 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/SEED--/SPLIT.py
+-rwxr-xr-x   0        0        0     1876 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/BUILD.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2092 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/CREATE.cpython-311.pyc
+-rwxr-xr-x   0        0        0      997 2023-09-27 19:47:39.055871 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/READ.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1124 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1839 2024-05-29 02:57:44.079667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/creator.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.006495 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/creator.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1046 2024-05-29 02:57:44.083667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.082494 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/scan.cpython-311.pyc
+-rwxr-xr-x   0        0        0      365 2024-01-17 04:01:10.530210 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/adapt/DER_to_hexadecimal.py
+-rwxr-xr-x   0        0        0      249 2024-01-17 04:02:34.420248 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/adapt/hexadecimal_to_DER.py
+-rwxr-xr-x   0        0        0     2633 2024-05-25 02:58:24.772044 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/creator.py
+-rwxr-xr-x   0        0        0        0 2024-01-17 04:03:13.555799 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/form.py
+-rwxr-xr-x   0        0        0      322 2024-02-08 21:59:02.126494 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/read.py
+-rwxr-xr-x   0        0        0      675 2024-05-25 02:58:24.788043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/scan.py
+-rwxr-xr-x   0        0        0     1244 2024-02-25 04:10:25.159032 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/BUILD--.py
+-rwxr-xr-x   0        0        0     2100 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/BUILD.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2365 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/CREATE.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1149 2024-02-25 04:11:37.790016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1760 2024-05-29 02:57:44.087667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/creator.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.286492 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/creator.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1134 2024-05-29 02:57:44.079667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/form.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.426490 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/form.cpython-311.pyc
+-rwxr-xr-x   0        0        0      748 2024-05-29 02:57:44.095667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.498489 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/scan.cpython-311.pyc
+-rwxr-xr-x   0        0        0      779 2024-05-29 02:57:44.083667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/write.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.638487 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/write.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2069 2024-05-25 02:58:24.800043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/creator.py
+-rwxr-xr-x   0        0        0     1055 2024-05-25 02:58:24.812043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/form.py
+-rwxr-xr-x   0        0        0      665 2024-05-25 02:58:24.828043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/scan.py
+-rwxr-xr-x   0        0        0      577 2024-05-25 02:58:24.840043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/write.py
+-rwxr-xr-x   0        0        0      934 2024-05-25 02:58:24.852043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/sign/__init__.py
+-rwxr-xr-x   0        0        0     1450 2024-05-29 02:57:44.087667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/sign/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.834485 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/sign/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2724 2024-05-12 04:08:12.490197 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/tutorial.s.HTML
+-rwxr-xr-x   0        0        0      834 2024-05-25 02:58:24.864043 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/verify/__init__.py
+-rwxr-xr-x   0        0        0      775 2024-05-29 02:57:44.091667 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/verify/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.918484 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/verify/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       73 2024-05-30 05:08:35.728472 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/EEC_448_2_private_key.DER
+-rw-r--r--   0        0        0      213 2024-05-30 05:08:35.736472 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/EEC_448_2_private_key.JSON
+-rwxr-xr-x   0        0        0     2472 2024-05-29 02:57:43.403676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/__pycache__/status_DER_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2473 2024-05-29 02:57:43.407676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/__pycache__/status_JSON_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2530 2024-05-25 02:58:24.880042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py
+-rwxr-xr-x   0        0        0     2490 2024-05-25 02:58:24.892042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py
+-rwxr-xr-x   0        0        0     3176 2024-05-29 02:57:43.411676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_2_private_and_public_keys/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3434 2024-05-25 02:58:24.908042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py
+-rwxr-xr-x   0        0        0     4497 2024-05-29 02:57:43.367676 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5362 2024-05-25 02:58:24.924042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py
+-rwxr-xr-x   0        0        0      299 2024-05-12 04:08:12.458197 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/clique.py
+-rwxr-xr-x   0        0        0      951 2024-04-24 04:36:09.143244 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/cryptography.py.S.HTML
+-rwxr-xr-x   0        0        0     1114 2024-05-25 02:58:24.940042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/keys/__init__.py
+-rwxr-xr-x   0        0        0      986 2024-05-25 03:29:39.460022 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/keys/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      520 2024-05-25 03:29:39.648020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/byte_string/__pycache__/from_UTF8.cpython-310.pyc
+-rwxr-xr-x   0        0        0      573 2024-05-25 03:29:39.644020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/byte_string/__pycache__/from_hexadecimal.cpython-310.pyc
+-rwxr-xr-x   0        0        0      314 2024-05-25 02:58:24.964042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/byte_string/from_UTF8.py
+-rwxr-xr-x   0        0        0      372 2024-05-25 02:58:24.952042 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/byte_string/from_hexadecimal.py
+-rwxr-xr-x   0        0        0      530 2024-05-25 03:29:39.640020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/hexadecimal/__pycache__/from_byte_string.cpython-310.pyc
+-rwxr-xr-x   0        0        0      325 2024-05-25 02:58:24.976041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/hexadecimal/from_byte_string.py
+-rwxr-xr-x   0        0        0     1876 2024-02-25 04:11:37.794016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/BUILD.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2092 2024-02-25 04:11:37.794016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/CREATE.cpython-311.pyc
+-rwxr-xr-x   0        0        0      997 2023-09-27 19:47:39.055871 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/READ.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1124 2024-02-25 04:11:37.794016 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1125 2024-05-25 03:29:39.460022 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/creator.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.006495 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/creator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      771 2024-05-29 02:57:44.127666 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1022 2024-05-25 03:29:39.644020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/instance.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1299 2024-05-25 03:29:39.632020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.082494 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/scan.cpython-311.pyc
+-rwxr-xr-x   0        0        0      365 2024-01-17 04:01:10.530210 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/adapt/DER_to_hexadecimal.py
+-rwxr-xr-x   0        0        0      249 2024-01-17 04:02:34.420248 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/adapt/hexadecimal_to_DER.py
+-rwxr-xr-x   0        0        0     1670 2024-05-25 02:58:24.988041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/creator.py
+-rwxr-xr-x   0        0        0      648 2024-05-25 02:58:25.000041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/etch.py
+-rwxr-xr-x   0        0        0      954 2024-05-25 02:58:25.016041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/instance.py
+-rwxr-xr-x   0        0        0      216 2024-02-25 04:11:37.798015 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/private_key.s.HTML
+-rwxr-xr-x   0        0        0      874 2024-05-25 02:58:25.028041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/scan.py
+-rwxr-xr-x   0        0        0     2100 2024-02-25 04:11:37.798015 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/BUILD.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2365 2024-02-25 04:11:37.798015 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/CREATE.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1149 2024-02-25 04:11:37.798015 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1382 2024-05-25 03:29:39.628020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/creator.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.286492 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/creator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      777 2024-05-29 02:57:44.323664 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-12 20:12:29.184426 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/form.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.426490 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/form.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1022 2024-05-25 03:29:39.648020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/instance.cpython-310.pyc
+-rwxr-xr-x   0        0        0      882 2024-05-29 02:57:44.327664 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.498489 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/scan.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-12 20:12:29.268425 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/write.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.638487 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/write.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1425 2024-05-25 02:58:25.040041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/creator.py
+-rwxr-xr-x   0        0        0      608 2024-05-25 02:58:25.052041 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/etch.py
+-rwxr-xr-x   0        0        0      955 2024-05-25 02:58:25.068040 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/instance.py
+-rwxr-xr-x   0        0        0       25 2024-02-12 23:23:16.361700 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/public_key.s.HTML
+-rwxr-xr-x   0        0        0      837 2024-05-25 02:58:25.080040 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/scan.py
+-rwxr-xr-x   0        0        0     1176 2024-05-25 02:58:25.092040 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/rhythms/__init__.py
+-rwxr-xr-x   0        0        0        4 2024-03-14 20:08:42.728438 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/rhythms/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1050 2024-05-25 02:58:25.104040 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/sign/__init__.py
+-rwxr-xr-x   0        0        0     1331 2024-05-25 03:29:39.636020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/sign/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.834485 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/sign/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1390 2024-04-24 04:36:58.990305 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/tutorial ++ EEC_448_2.S.HTML
+-rwxr-xr-x   0        0        0      407 2024-04-28 18:58:17.221951 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/tutorial ++ names.s.HTML
+-rwxr-xr-x   0        0        0     5697 2024-05-29 02:57:07.644145 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/tutorial.S.HTML
+-rwxr-xr-x   0        0        0      856 2024-05-25 02:58:25.120040 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/verify/__init__.py
+-rwxr-xr-x   0        0        0      656 2024-05-25 03:29:39.644020 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/verify/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:02.918484 recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/verify/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      131 2024-05-25 02:58:25.212039 recycling-1.1.0/venues/stages/recycling/mixes/QR/UTF8/__init__.py
+-rwxr-xr-x   0        0        0     1194 2024-01-16 06:43:32.902697 recycling-1.1.0/venues/stages/recycling/mixes/QR/__init__.py
+-rwxr-xr-x   0        0        0       28 2024-02-09 01:33:19.884331 recycling-1.1.0/venues/stages/recycling/mixes/QR/module.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-01-16 06:33:07.558208 recycling-1.1.0/venues/stages/recycling/mixes/QR/photo/interpret.py
+-rwxr-xr-x   0        0        0      171 2024-02-22 22:27:05.401905 recycling-1.1.0/venues/stages/recycling/mixes/barcodes/Aztec/Aztec.S.HTML
+-rwxr-xr-x   0        0        0        4 2024-02-22 22:27:54.713318 recycling-1.1.0/venues/stages/recycling/mixes/barcodes/Aztec/_school/start.py
+-rwxr-xr-x   0        0        0      428 2024-02-24 01:20:41.216739 recycling-1.1.0/venues/stages/recycling/mixes/barcodes/barcodes.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-02-22 22:32:21.434142 recycling-1.1.0/venues/stages/recycling/mixes/barcodes/scan_barcode/scan.S.HTML
+-rwxr-xr-x   0        0        0       88 2024-05-29 02:48:29.432310 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/Brainpool_1.S.HTML
+-rwxr-xr-x   0        0        0      448 2024-05-29 02:57:43.467675 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      344 2024-05-25 03:45:06.960278 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py
+-rwxr-xr-x   0        0        0      749 2024-05-29 02:42:46.203938 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/private_key/__pycache__/build.cpython-310.pyc
+-rwxr-xr-x   0        0        0      641 2024-05-25 03:30:09.603745 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/private_key/__pycache__/create.cpython-310.pyc
+-rwxr-xr-x   0        0        0      794 2024-05-29 02:42:44.051954 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/private_key/build.py
+-rwxr-xr-x   0        0        0      352 2024-05-29 02:43:54.595428 recycling-1.1.0/venues/stages/recycling/mixes/brainpool_1/public_key/build.py
+-rwxr-xr-x   0        0        0      138 2024-05-25 02:58:24.716044 recycling-1.1.0/venues/stages/recycling/mixes/camera/__init__.py
+-rwxr-xr-x   0        0        0      175 2024-02-24 01:14:21.021334 recycling-1.1.0/venues/stages/recycling/mixes/camera/module.s.HTML
+-rwxr-xr-x   0        0        0      261 2024-02-25 04:11:37.798015 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/SECP256K1.s.HTML
+-rwxr-xr-x   0        0        0      580 2024-05-29 02:57:43.399676 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      278 2024-05-25 02:58:25.132040 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/_status/status_1_generator/status_1.py
+-rwxr-xr-x   0        0        0     1078 2024-05-29 02:57:44.371663 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/__pycache__/build.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:03.046483 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/__pycache__/build.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1260 2024-05-25 02:58:25.144039 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/build.py
+-rwxr-xr-x   0        0        0      419 2024-02-25 04:11:37.802015 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/write.py
+-rwxr-xr-x   0        0        0        0 2024-01-17 02:34:03.043494 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/public_key/build.py
+-rwxr-xr-x   0        0        0      174 2024-02-25 04:10:25.867022 recycling-1.1.0/venues/stages/recycling/mixes/elliptic/elliptic.s.HTML
+-rwxr-xr-x   0        0        0      913 2024-05-29 02:55:10.609743 recycling-1.1.0/venues/stages/recycling/mixes/elliptic_curve/elliptic_curve.S.HTML
+-rwxr-xr-x   0        0        0        5 2024-03-14 20:19:45.373245 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2183 2024-05-29 02:57:44.075667 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/__pycache__/form.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 21:59:03.110482 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/__pycache__/form.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1394 2024-05-29 02:57:43.387676 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1171 2024-05-25 02:58:25.156040 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/status_1.py
+-rw-r--r--   0        0        0       73 2024-05-30 05:08:35.812471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/temporary/proposal.private_key.DER
+-rw-r--r--   0        0        0      138 2024-05-30 05:08:35.816471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/temporary/proposal.public_key.DER
+-rw-r--r--   0        0        0      114 2024-05-30 05:08:35.816471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/temporary/proposal.seed
+-rwxr-xr-x   0        0        0     1453 2024-05-29 02:57:43.371676 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1204 2024-05-25 02:58:25.172039 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/status_1.py
+-rw-r--r--   0        0        0       73 2024-05-30 05:08:35.848471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.private_key.DER
+-rw-r--r--   0        0        0      138 2024-05-30 05:08:35.856471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.public_key.hexadecimal
+-rw-r--r--   0        0        0      114 2024-05-30 05:08:35.856471 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/temporary/proposal.seed
+-rwxr-xr-x   0        0        0     1444 2024-05-29 02:57:43.403676 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1214 2024-05-25 02:58:25.184039 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py
+-rw-r--r--   0        0        0      146 2024-05-30 05:08:35.412474 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.private_key.hexadecimal
+-rw-r--r--   0        0        0      138 2024-05-30 05:08:35.420474 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.public_key.hexadecimal
+-rw-r--r--   0        0        0      114 2024-05-30 05:08:35.420474 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/temporary/proposal.seed
+-rwxr-xr-x   0        0        0      231 2024-05-12 04:08:12.478197 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/clique.py
+-rwxr-xr-x   0        0        0     2394 2024-05-25 02:58:25.196039 recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/form.py
+-rwxr-xr-x   0        0        0     1081 2024-05-12 04:08:12.518196 recycling-1.1.0/venues/stages/recycling/module.s.HTML
+-rwxr-xr-x   0        0        0      366 2024-05-25 02:58:25.224039 recycling-1.1.0/venues/stages/recycling/procedure.proc.py
+-rwxr-xr-x   0        0        0     1108 2024-05-25 04:37:44.979369 recycling-1.1.0/venues/stages/recycling/readme.md
+-rwxr-xr-x   0        0        0       72 2024-02-24 02:25:48.706413 recycling-1.1.0/venues/stages/recycling/recycling -- development.S.HTML
+-rwxr-xr-x   0        0        0      128 2024-05-25 05:05:03.155074 recycling-1.1.0/venues/stages/recycling/recycling -- vocab.HTML
+-rwxr-xr-x   0        0        0        2 2024-01-05 01:01:30.825976 recycling-1.1.0/venues/stages/recycling/source.zsh
+-rwxr-xr-x   0        0        0      262 2024-02-25 04:11:37.802015 recycling-1.1.0/venues/stages/recycling/stage/__agenda/agenda.s.HTML
+-rwxr-xr-x   0        0        0   344999 2024-02-05 18:23:32.425545 recycling-1.1.0/venues/stages/recycling/stage/__book/dlsdkcgl--ai-generated-8315813_1920.jpg
+-rwxr-xr-x   0        0        0      188 2024-05-12 04:08:13.006191 recycling-1.1.0/venues/stages/recycling/stage/__init__.py
+-rwxr-xr-x   0        0        0      445 2024-05-12 04:10:58.148445 recycling-1.1.0/venues/stages/recycling/stage/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-08 19:00:52.839550 recycling-1.1.0/venues/stages/recycling/stage/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.712464 recycling-1.1.0/venues/stages/recycling/stage/__pycache__/clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0      277 2024-05-12 04:11:25.440157 recycling-1.1.0/venues/stages/recycling/stage/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       63 2024-02-09 05:06:03.804904 recycling-1.1.0/venues/stages/recycling/stage/_status/status_1.py
+-rwxr-xr-x   0        0        0      743 2024-05-12 04:08:13.150190 recycling-1.1.0/venues/stages/recycling/stage/climate/__init__.py
+-rwxr-xr-x   0        0        0      971 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/climate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      822 2024-05-12 04:08:13.006191 recycling-1.1.0/venues/stages/recycling/stage/clique/__init__.py
+-rwxr-xr-x   0        0        0     1152 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0   190579 2024-03-19 04:47:24.502077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/index-BizSwkP3.css
+-rwxr-xr-x   0        0        0   544287 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/index-DIdFDc9G.js
+-rwxr-xr-x   0        0        0     1099 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/reel-DvvsKiXw.js
+-rwxr-xr-x   0        0        0  1215093 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-BPO9cr18.js
+-rwxr-xr-x   0        0        0     3356 2024-03-19 04:47:24.502077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-DSl6fGcC.css
+-rwxr-xr-x   0        0        0   852013 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-gSMgJBY7.js
+-rwxr-xr-x   0        0        0    18836 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/vanilla-picker-DfFJQbG4.js
+-rwxr-xr-x   0        0        0   430054 2024-03-19 04:47:23.618087 recycling-1.1.0/venues/stages/recycling/stage/frontend/codesweeper--ai-generated-8311450_1920.jpg
+-rwxr-xr-x   0        0        0     4286 2024-03-19 04:47:23.618087 recycling-1.1.0/venues/stages/recycling/stage/frontend/favicon.ico
+-rwxr-xr-x   0        0        0      442 2024-03-19 04:47:24.506077 recycling-1.1.0/venues/stages/recycling/stage/frontend/index.html
+-rwxr-xr-x   0        0        0      868 2024-05-12 04:08:13.186190 recycling-1.1.0/venues/stages/recycling/stage/layer/__init__.py
+-rwxr-xr-x   0        0        0     1072 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.108469 recycling-1.1.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      471 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/layer/__pycache__/start_dev.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.160469 recycling-1.1.0/venues/stages/recycling/stage/layer/__pycache__/start_dev.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1743 2024-05-12 04:08:13.186190 recycling-1.1.0/venues/stages/recycling/stage/layer/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2162 2024-05-12 04:10:58.160445 recycling-1.1.0/venues/stages/recycling/stage/layer/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      411 2024-02-25 04:11:37.786015 recycling-1.1.0/venues/stages/recycling/stage/layer/flask.s.HTML
+-rwxr-xr-x   0        0        0      641 2024-05-12 04:08:13.190189 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__init__.py
+-rwxr-xr-x   0        0        0     1109 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.073352 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/card_generator.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1145 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/moves.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-24 01:08:15.077769 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/seed_generator.cpython-310.pyc
+-rwxr-xr-x   0        0        0      505 2024-03-14 20:21:43.975941 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/home/__pycache__/get.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.188468 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/home/__pycache__/get.cpython-311.pyc
+-rwxr-xr-x   0        0        0      218 2024-02-13 01:00:25.822302 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/home/get.py
+-rwxr-xr-x   0        0        0      844 2024-05-12 04:08:13.194189 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/moves.py
+-rwxr-xr-x   0        0        0       57 2024-02-24 21:21:56.451073 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/routes.S.HTML
+-rwxr-xr-x   0        0        0     2651 2024-02-25 04:11:37.786015 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vibe_generator.py
+-rwxr-xr-x   0        0        0        4 2024-02-24 23:56:54.089352 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vibes/__pycache__/make_ECC_448_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0       26 2024-02-24 21:19:00.480991 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vibes/make_ECC_448_2.py
+-rwxr-xr-x   0        0        0     1387 2024-02-13 01:22:29.900593 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vue/__init__.py
+-rwxr-xr-x   0        0        0     1414 2024-03-14 20:21:43.975941 recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vue/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-05-12 04:08:13.190189 recycling-1.1.0/venues/stages/recycling/stage/layer/start_dev.proc.py
+-rwxr-xr-x   0        0        0      249 2024-05-12 04:08:13.186190 recycling-1.1.0/venues/stages/recycling/stage/layer/start_dev.py
+-rwxr-xr-x   0        0        0        0 2023-12-31 20:33:38.333168 recycling-1.1.0/venues/stages/recycling/stage/layer/start_gunicorn.py
+-rwxr-xr-x   0        0        0     1168 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1372 2024-05-12 04:08:13.198189 recycling-1.1.0/venues/stages/recycling/stage/layer/utilities/generate_path_inventory.py
+-rwxr-xr-x   0        0        0      448 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moon/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      227 2024-05-12 04:08:13.006191 recycling-1.1.0/venues/stages/recycling/stage/moon/connect.py
+-rwxr-xr-x   0        0        0     2394 2024-05-12 04:08:13.166190 recycling-1.1.0/venues/stages/recycling/stage/moves/__init__.py
+-rwxr-xr-x   0        0        0     2516 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 18:33:37.344467 recycling-1.1.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.069269 recycling-1.1.0/venues/stages/recycling/stage/moves/__pycache__/create_wallet.cpython-311.pyc
+-rwxr-xr-x   0        0        0        5 2024-02-08 22:06:53.089269 recycling-1.1.0/venues/stages/recycling/stage/moves/__pycache__/form_proposal_keys.cpython-311.pyc
+-rwxr-xr-x   0        0        0      306 2024-03-03 01:02:12.544244 recycling-1.1.0/venues/stages/recycling/stage/moves/_procedures/fees/fees.S.HTML
+-rwxr-xr-x   0        0        0      382 2024-03-14 20:21:43.975941 recycling-1.1.0/venues/stages/recycling/stage/moves/names/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1339 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/__pycache__/start_layer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      839 2024-05-12 04:10:58.152445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/__pycache__/start_mongo.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2024-02-24 21:49:13.531862 recycling-1.1.0/venues/stages/recycling/stage/moves/names/is_on.py
+-rwxr-xr-x   0        0        0     1016 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/add_splendor.cpython-310.pyc
+-rwxr-xr-x   0        0        0      982 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/establish_rules.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-03-14 20:08:43.676428 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1000 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce_Ehh.cpython-310.pyc
+-rwxr-xr-x   0        0        0      850 2024-05-12 04:08:13.166190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/add_splendor.py
+-rwxr-xr-x   0        0        0      981 2024-05-12 04:08:13.166190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/establish_rules.py
+-rwxr-xr-x   0        0        0      803 2024-05-12 04:08:13.166190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/produce_Ehh.py
+-rwxr-xr-x   0        0        0      105 2024-03-03 01:07:24.945416 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/squish/generate.py
+-rwxr-xr-x   0        0        0      835 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0      965 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/freshest.cpython-310.pyc
+-rwxr-xr-x   0        0        0      646 2024-05-12 04:08:13.174190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/establish.py
+-rwxr-xr-x   0        0        0      732 2024-05-12 04:08:13.174190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/freshest.py
+-rwxr-xr-x   0        0        0       24 2024-03-03 00:45:01.343933 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_insights/end.py
+-rwxr-xr-x   0        0        0      860 2024-05-12 04:10:58.156445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/__pycache__/enumerate.cpython-310.pyc
+-rwxr-xr-x   0        0        0      569 2024-05-12 04:08:13.170190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/enumerate.py
+-rwxr-xr-x   0        0        0      654 2024-05-12 04:10:58.160445 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/receive.cpython-310.pyc
+-rwxr-xr-x   0        0        0      376 2024-03-14 20:21:43.979941 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/send.cpython-310.pyc
+-rwxr-xr-x   0        0        0      377 2024-05-12 04:08:13.174190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/receive.py
+-rwxr-xr-x   0        0        0       77 2024-03-03 02:13:17.424736 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/send.py
+-rwxr-xr-x   0        0        0      378 2024-05-12 04:08:13.178190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/rules/change.py
+-rwxr-xr-x   0        0        0     1256 2024-05-12 04:08:13.178190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/start_layer.py
+-rwxr-xr-x   0        0        0      598 2024-05-12 04:08:13.178190 recycling-1.1.0/venues/stages/recycling/stage/moves/names/start_mongo.py
+-rwxr-xr-x   0        0        0      459 2024-02-08 21:27:24.131388 recycling-1.1.0/venues/stages/recycling/stage/names.s.HTML
+-rwxr-xr-x   0        0        0      770 2024-02-25 04:11:37.802015 recycling-1.1.0/venues/stages/recycling/stage/stage.s.HTML
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 recycling-1.1.0/PKG-INFO
```

### Comparing `recycling-1.0.0/pyproject.toml` & `recycling-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 
 
 
 
 [tool.poetry]
 name = "recycling"
-version = "1.0.0"
+version = "1.1.0"
 description = "The dreams that found there way to a canvas."
 authors = []
-readme = "readme.md"
+readme = "venues/stages/recycling/readme.md"
 
 packages = [
     { include = "recycling", from = "venues/stages" }
 ]
 exclude = ["venues/stages/apoplast/data_nodes/ingredients/_data"]
 include = [ 
 	"*.HTML", 
@@ -46,16 +46,18 @@
 python = "^3.10"
 biotech = "^1.1.10"
 somatic = "^3.0.2"
 ships = "^1.2.7"
 asn1crypto = "^1.5.1"
 aztec-code-generator = "^0.11"
 click = "^8.1.7"
+cryptography = "^42.0.7"
 ecdsa = "^0.19.0"
 ecpy = "^1.2.5"
+fastecdsa = "^2.3.2"
 flask = "^3.0.3"
 flask-cors = "^4.0.0"
 flask-openapi3 = "^3.1.0"
 rich = "^13.7.1"
 selenium = "^4.19.0"
 textual = "^0.56.4"
 websockets = "^12.0"
```

### Comparing `recycling-1.0.0/readme.md` & `recycling-1.1.0/venues/stages/recycling/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 
 
+
+
+
+
 ******
 
 Bravo!  You have received a Mercantilism Diploma in "recycling" from   
 the Simulated Parallel Science Universe Fictional Fantasy Orbital Convergence University   
 International Air and Water Embassy Naturalization Department of the Mango Planet
 (the planet that is one ellipse closer to the Sun than Earth's ellipse).
```

### Comparing `recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311435_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311435_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311446_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311446_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311450_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/__book/codesweeper--ai-generated-8311450_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__license/options/gpl-3.0-standalone.html` & `recycling-1.1.0/venues/stages/recycling/[license]/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/delegates/delegates.r.html` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/delegates/delegates.r.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/queue/queue.r.html` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/queue/queue.r.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/1. seed/nodes/essentials/approvers/voters.s.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/1. seed/nodes/essentials/approvers/voters.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/moderation/moderation.r.html` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/2. advancements/moderation/moderation.r.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/2. advancements/wallet.svg` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/2. advancements/wallet.svg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/0_v1/priorities.html` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/0_v1/priorities.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/off_chain/off_chain_moves.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/aphrodisiac/aphrodisiac.S.HTML`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 
 
 
 <pre>
 
-	<h1>off chain moves</h1>
+	<h1>aphrodisiac</h1>
+	
+	<h2>tags</h2>
+		# origin
+		# sex organ
+		
+		# aphrodisiac
+		# pheromones
+		
 	
 	<h2>summary</h2>
 	
 	
 	<h2>objectives ranked</h2>
 	
 		<h3>app level</h3>
```

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/___steps/steps.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/petitions/__anatomy/anatomy.S.HTML`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 
 <pre>
 
-	<h1>steps</h1>
+	<h1>anatomy</h1>
 	
 	<h2>objectives</h2>
 	
 		off chain: 
 			1. 	write the ask 
 			2. 	sign the ask
 			3. 	ask the voters to sign (approve) the ask
@@ -35,8 +35,10 @@
 
 
 
 
 
 
 
-</pre>
+</pre>
+
+
```

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/asks/on_chain/voters/picker_queue/picker queue.jpeg` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/passive/kinds/picker queue.jpeg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/keys/keys, legend.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organisms/vibes/vibes:tags.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/businesses/voting/voting.s.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/organs/heredity/voting/passive/passive_voting.S.HTML`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,60 @@
 
 
-<pre>
 
-	<h1>voting</h1>
-		# voting
-		# picking
-		# choosing
-		# share
-		
-		# consensus
-			# course	
-			# governance
-			# forward
-			# management
-			# directions
-			# strategy
-			# procedures
-		
-		# laws, rules, physics
-		
-		# citizens,
-			# councilor,
-			# accountants,
 
-			# choosers,
-			# authors,
-			
-			# voters, 
-			# governments, 
-			# politicians,  
-			# rulers,
-			# writers,
-			# producers,
-			# board,
-			# family
+<pre>
+
+	<h1>passive voting</h1>
 		
 	<h2>summary</h2>
 	
-	
 	<h2>questions</h2>
 
 		[ ] who chooses transaction order per block?
 			
-				could be rotational based on order in which
-				accounts were added to the stamina database.
-					
-					for example:
-						account 1 [1000 staked]
-						account 3 [1000 staked]
-						account 4
-						account 5
-						account 2
+			could be rotational based on order in which
+			accounts were added to the stamina database.
 				
-					operation:
-						stake 1000
-						unstake 1000
+				for example:
+					account 1 [1000 staked]
+					account 3 [1000 staked]
+					account 4
+					account 5
+					account 2
+			
+				operation:
+					stake 1000
+					unstake 1000
+					
+					unless stake goes to 0,
+					order in stamina order 
+					remains the same.
+					
+				conditionals:
+					if account is non-responsive:
+						accounts can vote to skip account in the order
 						
-						unless stake goes to 0,
-						order in stamina order 
-						remains the same.
+						like after 5 seconds of non-reponsiveness,
+						from the stamina leader, the tool could
+						be programmed to propose going to the next tool in the order.
 						
-					conditionals:
-						if account is non-responsive:
-							accounts can vote to skip account in the order
-							
-							like after 5 seconds of non-reponsiveness,
-							from the stamina leader, the tool could
-							be programmed to propose going to the next tool in the order.
-							
-								{
-									"proposal": {
-										"name": "skip stamina leader",
-										"fields": {
-											"stamina leader": 4,
-
-											"squash": 245,											
-											"block": 941
-										},
+							{
+								"proposal": {
+									"name": "skip stamina leader",
+									"fields": {
+										"stamina leader": 4,
+
+										"squash": 245,											
+										"block": 941
 									},
-									"signature": 
-								}
-						
+								},
+								"signature": 
+							}
 					
+				
 					
 					
 						
 </pre>
```

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/1_MVP/the_reel/reel themes.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics/[themes]/_maybes/_themes.S.HTML`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 
 
 
+
+
+
 <pre>
 
 	<h1>themes</h1>
 	
 	<h2>objectives</h2>
 	
 		reel, chapters, scenes, gestures = blockchain, squeeze, block, tx
 	
+		# theme: biotech
+		
+		# theme: multisong
+		
+		# theme: trash
+			# garbage
+		
+		# theme: electronics
+			# current
+			
+		# asset
+		# treasures
+		# gifts
+		# money
+		# eco
+		# treats
+		# trends
+	
 	<h2>possibilities</h2>
 		
 		<h3>conformity</h3>
 			blockchain, squeeze, block, tx
 			
 			blockchain, squeeze, batch, jump,  
 			blockchain, squeeze, block, leap
 		
 		<h3>movies</h3>
 			reel, chapters, scenes, gestures	
-				
-		
 		
 			story, scenes, gestures
-		
 			reel, scenes, steps
-			
 			reel, scenes, dynamics
 			reel, scenes, lines
-		
 			reel, scenes, moves
 			reel, scenes, actions
-		
 			performance, 
 			
 		<h3>music</h3>
 			
 		
 		<h3>genetics</h3>
 			genome, genes, bases
```

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/2_Next/apps/pay wall.svg` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/2_apps/pay wall.svg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/L1/2_Next/smart_contracts/smart_contracts.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/genetics_v1/2_smart_contracts/smart_contracts.S.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/later, vibes.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/later, vibes.S.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/__objectives/objectives.S.HTML` & `recycling-1.1.0/venues/stages/recycling/[_rhythms_]/proposals.S.HTML`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 
 <pre>
 
-	<h1>objectives</h1>
+	<h1>proposals</h1>
+		# objective
 		# itinerary
 		# later
 	
 	<h2>ranked</h2>
-	
-	
+		
 	
 	
 	<h2>possibilities</h2>
 	
 		[ ] BRAINPOOLP512r1
 			[ ] https://github.com/tlsfuzzer/python-ecdsa
```

### Comparing `recycling-1.0.0/venues/stages/recycling/_clique/__init__.py` & `recycling-1.1.0/venues/stages/recycling/_clique/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
 
-
-
-
-#from recycling._clique.group import clique as clique_group
-
+#/
+#
 import recycling.instrument.clique as instrument_clique
 import recycling.stage.clique as stage_clique
-
+#
+#
 import somatic
-
+#
+#
 import click
-
+#
+#
 import pathlib
 from os.path import dirname, join, normpath
+#
+#\
 
 def intro ():
 	@click.group ()
 	def group ():
 		pass
 
 	@click.command ("tutorial")
```

### Comparing `recycling-1.0.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 961 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 c103 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 146a 5166 9403 0000  o........jQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 0200 0100 6d02 5a03 0100  d.l.m.....m.Z...
 00000040: 6400 6401 6c04 6d05 0200 0100 6d02 5a06  d.d.l.m.....m.Z.
 00000050: 0100 6400 6401 6c07 5a07 6400 6401 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a08 6400 6401 6c09 5a09 6400 6402 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6403  m.Z.m.Z.m.Z...d.
@@ -18,15 +18,15 @@
 00000110: 0101 007c 0053 0029 064e 6300 0000 0000  ...|.S.).Nc.....
 00000120: 0000 0000 0000 0000 0000 0001 0000 0053  ...............S
 00000130: 0000 0073 0400 0000 6400 5300 2901 4ea9  ...s....d.S.).N.
 00000140: 0072 0500 0000 7205 0000 0072 0500 0000  .r....r....r....
 00000150: fa34 2f68 6162 6974 6174 2f76 656e 7565  .4/habitat/venue
 00000160: 732f 7374 6167 6573 2f72 6563 7963 6c69  s/stages/recycli
 00000170: 6e67 2f5f 636c 6971 7565 2f5f 5f69 6e69  ng/_clique/__ini
-00000180: 745f 5f2e 7079 da05 6772 6f75 7013 0000  t__.py..group...
+00000180: 745f 5f2e 7079 da05 6772 6f75 7015 0000  t__.py..group...
 00000190: 0073 0200 0000 0402 7a14 696e 7472 6f2e  .s......z.intro.
 000001a0: 3c6c 6f63 616c 733e 2e67 726f 7570 da08  <locals>.group..
 000001b0: 7475 746f 7269 616c 6300 0000 0000 0000  tutorialc.......
 000001c0: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
 000001d0: 0073 4c00 0000 7400 7401 a002 7403 a101  .sL...t.t...t...
 000001e0: 6a04 a005 a100 8301 7d00 7400 7406 7407  j.......}.t.t.t.
 000001f0: 7c00 6401 8302 8301 8301 7d01 7408 a009  |.d.......}.t...
@@ -41,32 +41,32 @@
 00000280: 6572 0400 0000 7203 0000 00da 0773 6f6d  er....r......som
 00000290: 6174 6963 da05 7374 6172 74da 0474 696d  atic..start..tim
 000002a0: 65da 0573 6c65 6570 2903 da0e 7468 6973  e..sleep)...this
 000002b0: 5f64 6972 6563 746f 7279 da10 6d6f 6475  _directory..modu
 000002c0: 6c65 5f64 6972 6563 746f 7279 7212 0000  le_directoryr...
 000002d0: 0072 0500 0000 7205 0000 0072 0600 0000  .r....r....r....
 000002e0: da10 7475 746f 7269 616c 5f63 6f6d 6d61  ..tutorial_comma
-000002f0: 6e64 1700 0000 7314 0000 0014 0312 0104  nd....s.........
+000002f0: 6e64 1900 0000 7314 0000 0014 0312 0104  nd....s.........
 00000300: 0202 0402 0508 f708 0c02 010a 0102 ff7a  ...............z
 00000310: 1f69 6e74 726f 2e3c 6c6f 6361 6c73 3e2e  .intro.<locals>.
 00000320: 7475 746f 7269 616c 5f63 6f6d 6d61 6e64  tutorial_command
 00000330: 2907 da05 636c 6963 6b72 0700 0000 da07  )...clickr......
 00000340: 636f 6d6d 616e 64da 0b61 6464 5f63 6f6d  command..add_com
 00000350: 6d61 6e64 da11 696e 7374 7275 6d65 6e74  mand..instrument
 00000360: 5f63 6c69 7175 6572 1100 0000 da0c 7374  _cliquer......st
 00000370: 6167 655f 636c 6971 7565 2902 7207 0000  age_clique).r...
 00000380: 0072 1600 0000 7205 0000 0072 0500 0000  .r....r....r....
-00000390: 7206 0000 00da 0569 6e74 726f 1200 0000  r......intro....
+00000390: 7206 0000 00da 0569 6e74 726f 1400 0000  r......intro....
 000003a0: 7310 0000 0006 010a 0108 030a 010a 150e  s...............
 000003b0: 010e 0104 0272 1c00 0000 290f da1b 7265  .....r....)...re
 000003c0: 6379 636c 696e 672e 696e 7374 7275 6d65  cycling.instrume
 000003d0: 6e74 2e63 6c69 7175 65da 0a69 6e73 7472  nt.clique..instr
 000003e0: 756d 656e 74da 0663 6c69 7175 6572 1a00  ument..cliquer..
 000003f0: 0000 da16 7265 6379 636c 696e 672e 7374  ....recycling.st
 00000400: 6167 652e 636c 6971 7565 da05 7374 6167  age.clique..stag
 00000410: 6572 1b00 0000 7210 0000 0072 1700 0000  er....r....r....
 00000420: 720b 0000 00da 076f 732e 7061 7468 7202  r......os.pathr.
 00000430: 0000 0072 0300 0000 7204 0000 0072 1c00  ...r....r....r..
 00000440: 0000 7205 0000 0072 0500 0000 7205 0000  ..r....r....r...
 00000450: 0072 0600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000460: 0100 0000 730e 0000 0012 0712 0108 0208  ....s...........
-00000470: 0208 0214 010c 02                        .......
+00000460: 0100 0000 730e 0000 0012 0412 0108 0308  ....s...........
+00000470: 0308 0314 010c 04                        .......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/_status/DB/records.json` & `recycling-1.1.0/venues/stages/recycling/_status/DB/records.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9726027397260274%*

 * *Differences: {"'_default'": "{'70': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'elliptic public and private key generation'), ('elapsed', [0.40933606600083294, "*

 * *               "'seconds']), ('passed', True)])]), ('empty', False), ('parsed', True), ('path', "*

 * *               "'modules/EEC_448_2/_status/status_3_sign_and_verify/status_1.py'), ('records', "*

 * *               "[]), ('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), "*

 * *               "OrderedDict([('checks',  […]*

```diff
@@ -13873,14 +13873,1255 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 4
                 },
                 "empty": 0
             }
         },
+        "70": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.40933606600083294,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_2/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.16343849999975646,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_2/_status/status_1_private_key/status_JSON_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.1443870600014634,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_2/_status/status_1_private_key/status_DER_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.16732667300129833,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/elliptic/SECP256K1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.17557796299843176,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/proposals/keys/_status/3_hexadecimal_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10317911499987531,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/proposals/keys/_status/1_DER/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11442332899969188,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/proposals/keys/_status/2_hexadecimal_public_key/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.676531873001295,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_1/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.1986832359998516,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_1/_status/status_2_generators/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.186437329999535,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/EEC_448_1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.020728428000439,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "instrument/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0130006558028981e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stage/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                8.269998943433166e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/_stories/story_instrument_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "71": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.30463950499870407,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.09385400000064692,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.15290212299987616,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.13207182299993292,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/elliptic/SECP256K1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0845915320005588,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.21326984799998172,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/1_DER/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.1342661529997713,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/2_hexadecimal_public_key/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.5750742630007153,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.20811996799966437,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_2_generators/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.06015981699965778,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.009352880000733,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "instrument/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.76999513618648e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stage/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                5.83999280934222e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/_stories/story_instrument_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "72": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.34298532500542933,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.10660369900142541,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.19938746899424586,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.1467601249969448,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/elliptic/SECP256K1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14643577000242658,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06622678099665791,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/1_DER/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.15793613600544631,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/2_hexadecimal_public_key/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.30398424599843565,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.26476768900465686,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_2_generators/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.09341081199818291,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.004915382000036,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "instrument/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.790004019625485e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stage/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                4.930043360218406e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/_stories/story_instrument_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "73": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.39957441000296967,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.09585729699756484,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.14083688700338826,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generation",
+                            "elapsed": [
+                                0.16288436600007117,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/elliptic/SECP256K1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10583035399758955,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07311360599851469,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/1_DER/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.08235078799771145,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/proposals/keys/_status/2_hexadecimal_public_key/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.32496655399882,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_3_sign_and_verify/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic public and private key generators",
+                            "elapsed": [
+                                0.19516809199558338,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_2_generators/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "elliptic private key generation",
+                            "elapsed": [
+                                0.12213516599877039,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "mixes/EEC_448_1/_status/status_1_generator/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ModuleNotFoundError(\"No module named 'recycling.mixes.Brainpool_1'\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/habitat/venues/stages/recycling/mixes/brainpool_1/_status/status_1.py\", line 9, in <module>",
+                        "    from recycling.mixes.Brainpool_1.private_key.create import create_private_key",
+                        "ModuleNotFoundError: No module named 'recycling.mixes.Brainpool_1'"
+                    ],
+                    "parsed": false,
+                    "path": "mixes/brainpool_1/_status/status_1.py",
+                    "records": []
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.016253367997706,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "instrument/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.480048225261271e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stage/_status/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "status 1",
+                            "elapsed": [
+                                6.560003384947777e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/_stories/story_instrument_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
         "8": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [],
                     "empty": false,
                     "parsed": true,
```

### Comparing `recycling-1.0.0/venues/stages/recycling/_status/__init__.py` & `recycling-1.1.0/venues/stages/recycling/_status/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 
 #----
 #
 import biotech
 #
 #
+import rich
+#
+#
 import json
 import pathlib
 from os.path import dirname, join, normpath
 import sys
 #
 #----
 
@@ -39,8 +42,10 @@
 		simultaneous = True,
 		module_paths = [
 			stages
 		],
 		relative_path = status_assurances_path,
 		
 		db_directory = db_directory
-	)
+	)
+	
+	rich.print_json (data = scan)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/_status/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:14:30 2024 UTC, .py size: 865 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-00000000: 6f0d 0d0a 0000 0000 2642 4066 6103 0000  o.......&B@fa...
+00000000: 6f0d 0d0a 0000 0000 c909 5866 9203 0000  o.........Xf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
-00000060: 5a07 6403 6404 8400 5a08 6401 5300 2905  Z.d.d...Z.d.S.).
-00000070: e900 0000 004e 2903 da07 6469 726e 616d  .....N)...dirnam
-00000080: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
-00000090: 6863 0000 0000 0000 0000 0000 0000 0600  hc..............
-000000a0: 0000 0700 0000 4300 0000 7394 0000 0074  ......C...s....t
-000000b0: 00a0 0174 02a1 016a 03a0 04a1 007d 0074  ...t...j.....}.t
-000000c0: 0574 0674 077c 0064 0183 0283 0183 017d  .t.t.|.d.......}
-000000d0: 0174 0574 0674 077c 0064 0283 0283 0183  .t.t.t.|.d......
-000000e0: 017d 0274 0874 096a 0a83 0164 036b 0572  .}.t.t.j...d.k.r
-000000f0: 2d7c 0264 0417 0074 096a 0a64 0519 0017  -|.d...t.j.d....
-00000100: 007d 0364 067d 046e 0b7c 0264 0717 007d  .}.d.}.n.|.d...}
-00000110: 0374 0674 077c 0064 0883 0283 017d 0474  .t.t.|.d.....}.t
-00000120: 0b64 097c 0383 0201 0074 0c6a 0d7c 0364  .d.|.....t.j.|.d
-00000130: 0a7c 0167 017c 027c 0464 0b8d 057d 0564  .|.g.|.|.d...}.d
-00000140: 0053 0029 0c4e 7a0f 2e2e 2f2e 2e2f 2e2e  .S.).Nz.../../..
-00000150: 2f73 7461 6765 737a 022e 2ee9 0200 0000  /stagesz........
-00000160: fa01 2fe9 0100 0000 467a 0f2f 2a2a 2f73  ../.....Fz./**/s
-00000170: 7461 7475 735f 2a2e 7079 da02 4442 7a0c  tatus_*.py..DBz.
-00000180: 676c 6f62 2073 7472 696e 673a 5429 05da  glob string:T)..
-00000190: 0b67 6c6f 625f 7374 7269 6e67 da0c 7369  .glob_string..si
-000001a0: 6d75 6c74 616e 656f 7573 da0c 6d6f 6475  multaneous..modu
-000001b0: 6c65 5f70 6174 6873 da0d 7265 6c61 7469  le_paths..relati
-000001c0: 7665 5f70 6174 68da 0c64 625f 6469 7265  ve_path..db_dire
-000001d0: 6374 6f72 7929 0eda 0770 6174 686c 6962  ctory)...pathlib
-000001e0: da04 5061 7468 da08 5f5f 6669 6c65 5f5f  ..Path..__file__
-000001f0: da06 7061 7265 6e74 da07 7265 736f 6c76  ..parent..resolv
-00000200: 65da 0373 7472 7204 0000 0072 0300 0000  e..strr....r....
-00000210: da03 6c65 6eda 0373 7973 da04 6172 6776  ..len..sys..argv
-00000220: da05 7072 696e 74da 0762 696f 7465 6368  ..print..biotech
-00000230: da05 7374 6172 7429 06da 0b74 6869 735f  ..start)...this_
-00000240: 666f 6c64 6572 da06 7374 6167 6573 da16  folder..stages..
-00000250: 7374 6174 7573 5f61 7373 7572 616e 6365  status_assurance
-00000260: 735f 7061 7468 7209 0000 0072 0d00 0000  s_pathr....r....
-00000270: da04 7363 616e a900 721e 0000 00fa 342f  ..scan..r.....4/
-00000280: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
-00000290: 7461 6765 732f 7265 6379 636c 696e 672f  tages/recycling/
-000002a0: 5f73 7461 7475 732f 5f5f 696e 6974 5f5f  _status/__init__
-000002b0: 2e70 7972 1900 0000 1000 0000 7322 0000  .pyr........s"..
-000002c0: 0010 0412 0112 040e 0312 0106 0108 020e  ................
-000002d0: 010a 0204 0202 0102 0102 0202 ff02 0302  ................
-000002e0: 020a f872 1900 0000 2909 7218 0000 00da  ...r....).r.....
-000002f0: 046a 736f 6e72 0e00 0000 da07 6f73 2e70  .jsonr......os.p
-00000300: 6174 6872 0200 0000 7203 0000 0072 0400  athr....r....r..
-00000310: 0000 7215 0000 0072 1900 0000 721e 0000  ..r....r....r...
-00000320: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000330: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
-00000340: 0000 0008 0408 0308 0114 0108 010c 05    ...............
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6402 6c04 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
+00000060: 0100 6400 6401 6c08 5a08 6403 6404 8400  ..d.d.l.Z.d.d...
+00000070: 5a09 6401 5300 2905 e900 0000 004e 2903  Z.d.S.)......N).
+00000080: da07 6469 726e 616d 65da 046a 6f69 6eda  ..dirname..join.
+00000090: 086e 6f72 6d70 6174 6863 0000 0000 0000  .normpathc......
+000000a0: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
+000000b0: 0000 73a0 0000 0074 00a0 0174 02a1 016a  ..s....t...t...j
+000000c0: 03a0 04a1 007d 0074 0574 0674 077c 0064  .....}.t.t.t.|.d
+000000d0: 0183 0283 0183 017d 0174 0574 0674 077c  .......}.t.t.t.|
+000000e0: 0064 0283 0283 0183 017d 0274 0874 096a  .d.......}.t.t.j
+000000f0: 0a83 0164 036b 0572 2d7c 0264 0417 0074  ...d.k.r-|.d...t
+00000100: 096a 0a64 0519 0017 007d 0364 067d 046e  .j.d.....}.d.}.n
+00000110: 0b7c 0264 0717 007d 0374 0674 077c 0064  .|.d...}.t.t.|.d
+00000120: 0883 0283 017d 0474 0b64 097c 0383 0201  .....}.t.d.|....
+00000130: 0074 0c6a 0d7c 0364 0a7c 0167 017c 027c  .t.j.|.d.|.g.|.|
+00000140: 0464 0b8d 057d 0574 0e6a 0f7c 0564 0c8d  .d...}.t.j.|.d..
+00000150: 0101 0064 0053 0029 0d4e 7a0f 2e2e 2f2e  ...d.S.).Nz.../.
+00000160: 2e2f 2e2e 2f73 7461 6765 737a 022e 2ee9  ./../stagesz....
+00000170: 0200 0000 fa01 2fe9 0100 0000 467a 0f2f  ....../.....Fz./
+00000180: 2a2a 2f73 7461 7475 735f 2a2e 7079 da02  **/status_*.py..
+00000190: 4442 7a0c 676c 6f62 2073 7472 696e 673a  DBz.glob string:
+000001a0: 5429 05da 0b67 6c6f 625f 7374 7269 6e67  T)...glob_string
+000001b0: da0c 7369 6d75 6c74 616e 656f 7573 da0c  ..simultaneous..
+000001c0: 6d6f 6475 6c65 5f70 6174 6873 da0d 7265  module_paths..re
+000001d0: 6c61 7469 7665 5f70 6174 68da 0c64 625f  lative_path..db_
+000001e0: 6469 7265 6374 6f72 7929 01da 0464 6174  directory)...dat
+000001f0: 6129 10da 0770 6174 686c 6962 da04 5061  a)...pathlib..Pa
+00000200: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
+00000210: 7265 6e74 da07 7265 736f 6c76 65da 0373  rent..resolve..s
+00000220: 7472 7204 0000 0072 0300 0000 da03 6c65  trr....r......le
+00000230: 6eda 0373 7973 da04 6172 6776 da05 7072  n..sys..argv..pr
+00000240: 696e 74da 0762 696f 7465 6368 da05 7374  int..biotech..st
+00000250: 6172 74da 0472 6963 68da 0a70 7269 6e74  art..rich..print
+00000260: 5f6a 736f 6e29 06da 0b74 6869 735f 666f  _json)...this_fo
+00000270: 6c64 6572 da06 7374 6167 6573 da16 7374  lder..stages..st
+00000280: 6174 7573 5f61 7373 7572 616e 6365 735f  atus_assurances_
+00000290: 7061 7468 7209 0000 0072 0d00 0000 da04  pathr....r......
+000002a0: 7363 616e a900 7221 0000 00fa 342f 6861  scan..r!....4/ha
+000002b0: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
+000002c0: 6765 732f 7265 6379 636c 696e 672f 5f73  ges/recycling/_s
+000002d0: 7461 7475 732f 5f5f 696e 6974 5f5f 2e70  tatus/__init__.p
+000002e0: 7972 1a00 0000 1300 0000 7324 0000 0010  yr........s$....
+000002f0: 0412 0112 040e 0312 0106 0108 020e 010a  ................
+00000300: 0204 0202 0102 0102 0202 ff02 0302 0206  ................
+00000310: f810 0b72 1a00 0000 290a 7219 0000 0072  ...r....).r....r
+00000320: 1b00 0000 da04 6a73 6f6e 720f 0000 00da  ......jsonr.....
+00000330: 076f 732e 7061 7468 7202 0000 0072 0300  .os.pathr....r..
+00000340: 0000 7204 0000 0072 1600 0000 721a 0000  ..r....r....r...
+00000350: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00000360: 7222 0000 00da 083c 6d6f 6475 6c65 3e01  r".....<module>.
+00000370: 0000 0073 0e00 0000 0804 0803 0803 0801  ...s............
+00000380: 1401 0801 0c05                           ......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/TheDigitalArtist--ai-generated-8228359_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/TheDigitalArtist--ai-generated-8228359_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/TheDigitalArtist--ai-generated-8228360_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/TheDigitalArtist--ai-generated-8228360_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/ISO_lab.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/ISO_lab.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/ISO_lab_2.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/ISO_lab_2.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/ISO/write_ISO_to_drive.py` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/ISO/write_ISO_to_drive.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/containers/containers.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/containers/containers.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/containers/installations.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/containers/installations.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/docker/docker.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/docker/docker.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/_hardware/hardware.s.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/_hardware/hardware.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/__book/dlsdkcgl--hidden-8315722_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/instrument/[novels]/dlsdkcgl--hidden-8315722_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.turtle` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.turtle`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/WiredTiger.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/_mdb_catalog.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/_mdb_catalog.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-0-7108514929992687025.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/collection-0-7108514929992687025.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-1-7108514929992687025.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-1-7108514929992687025.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-3-7108514929992687025.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/index-3-7108514929992687025.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/sizeStorer.wt` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/instrument/mongo_DB_directory/sizeStorer.wt`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/_status/status_1.py` & `recycling-1.1.0/venues/stages/recycling/instrument/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/climate/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/climate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/clique/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/clique/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/feel-1b84c382.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/feel-1b84c382.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/index-d4db3b65.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/index-d4db3b65.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/index-f1fd6021.css` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/index-f1fd6021.css`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/perform-9529be50.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/perform-9529be50.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-2bdf6498.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-2bdf6498.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-5131ee29.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-5131ee29.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/region-bd81103e.css` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/region-bd81103e.css`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/room-3696ea94.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/room-3696ea94.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/scenery-de5924ae.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/scenery-de5924ae.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/subconscious-a94f6af0.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/subconscious-a94f6af0.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/assets/vanilla-picker-b74cad28.js` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/assets/vanilla-picker-b74cad28.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/codesweeper--ai-generated-8311446_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/codesweeper--ai-generated-8311446_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/frontend/favicon.ico` & `recycling-1.1.0/venues/stages/recycling/instrument/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/instrument.S.HTML` & `recycling-1.1.0/venues/stages/recycling/instrument/instrument.S.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,29 @@
 
 
 import json
 from os.path import dirname, join, normpath
 import os
 import traceback
 
-
 import rich
 from flask import Flask, request
 import flask_cors
 
-import recycling.instrument.layer.utilities.generate_path_inventory as generate_path_inventory
-import recycling.instrument.climate as instrument_climate
+import recycling.stage.layer.utilities.generate_path_inventory as generate_path_inventory
+import recycling.stage.climate as stage_climate
 	
 from .routes import connect_routes
 
 def build (
 	records = 1
 ):
-	climate = instrument_climate.retrieve ()
+	climate = stage_climate.retrieve ()
 
-	print ("starting instrument flask service")
+	print ("starting stage flask service")
 	rich.print_json (data = {
 		"variables": {
 			"frontend dist": climate ["paths"] ["frontend dist"]
 		}
 	})
 
 	app = Flask (__name__)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 894 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 7e03 0000  o........@@f~...
+00000000: 6f0d 0d0a 0000 0000 1a6e 5166 9103 0000  o........nQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6401  m.Z.m.Z.m.Z...d.
-00000050: 6402 6c06 5a06 6401 6402 6c07 5a07 6401  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c08 5a08 6401 6404 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
-00000070: 6d0b 5a0b 0100 6401 6402 6c0c 5a0c 6401  m.Z...d.d.l.Z.d.
-00000080: 6402 6c0d 6d0e 0200 0100 6d0f 0200 0100  d.l.m.....m.....
-00000090: 6d10 0200 0100 6d11 5a11 0100 6401 6402  m.....m.Z...d.d.
-000000a0: 6c12 6d0e 0200 0100 6d13 5a14 0100 6405  l.m.....m.Z...d.
-000000b0: 6406 6c15 6d16 5a16 0100 0905 6409 6407  d.l.m.Z.....d.d.
+00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
+00000040: 0200 0100 6d04 0200 0100 6d05 5a05 0100  ....m.....m.Z...
+00000050: 6401 6402 6c06 6d02 0200 0100 6d07 5a08  d.d.l.m.....m.Z.
+00000060: 0100 6403 6404 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6402 6c0b 5a0b 6401 6405 6c0c 6d0d 5a0d  d.l.Z.d.d.l.m.Z.
+00000080: 6d0e 5a0e 0100 6401 6402 6c0f 5a0f 6401  m.Z...d.d.l.Z.d.
+00000090: 6402 6c10 5a10 6401 6406 6c11 6d12 5a12  d.l.Z.d.d.l.m.Z.
+000000a0: 6d13 5a13 6d14 5a14 0100 6401 6402 6c15  m.Z.m.Z...d.d.l.
+000000b0: 5a15 6401 6402 6c16 5a16 0903 6409 6407  Z.d.d.l.Z...d.d.
 000000c0: 6408 8401 5a17 6402 5300 290a 7a02 0a0a  d...Z.d.S.).z...
-000000d0: e900 0000 004e 2903 da07 6469 726e 616d  .....N)...dirnam
-000000e0: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
-000000f0: 6829 02da 0546 6c61 736b da07 7265 7175  h)...Flask..requ
-00000100: 6573 74e9 0100 0000 2901 da0e 636f 6e6e  est.....)...conn
-00000110: 6563 745f 726f 7574 6573 6301 0000 0000  ect_routesc.....
+000000d0: e900 0000 004e e901 0000 0029 01da 0e63  .....N.....)...c
+000000e0: 6f6e 6e65 6374 5f72 6f75 7465 7329 02da  onnect_routes)..
+000000f0: 0546 6c61 736b da07 7265 7175 6573 7429  .Flask..request)
+00000100: 03da 0764 6972 6e61 6d65 da04 6a6f 696e  ...dirname..join
+00000110: da08 6e6f 726d 7061 7468 6301 0000 0000  ..normpathc.....
 00000120: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
 00000130: 0000 0073 6000 0000 7400 a001 a100 7d01  ...s`...t.....}.
 00000140: 7402 6401 8301 0100 7403 6a04 6402 6403  t.d.....t.j.d.d.
 00000150: 7c01 6404 1900 6403 1900 6901 6901 6405  |.d...d...i.i.d.
 00000160: 8d01 0100 7405 7406 8301 7d02 7407 a008  ....t.t...}.t...
 00000170: 7c02 a101 0100 0900 7409 a00a 7c01 6404  |.......t...|.d.
 00000180: 1900 6403 1900 a101 7d03 740b 7c02 7c03  ..d.....}.t.|.|.
@@ -28,42 +28,42 @@
 000001b0: 2066 6c61 736b 2073 6572 7669 6365 da09   flask service..
 000001c0: 7661 7269 6162 6c65 737a 0d66 726f 6e74  variablesz.front
 000001d0: 656e 6420 6469 7374 da05 7061 7468 7329  end dist..paths)
 000001e0: 01da 0464 6174 6129 0cda 1269 6e73 7472  ...data)...instr
 000001f0: 756d 656e 745f 636c 696d 6174 65da 0872  ument_climate..r
 00000200: 6574 7269 6576 65da 0570 7269 6e74 da04  etrieve..print..
 00000210: 7269 6368 da0a 7072 696e 745f 6a73 6f6e  rich..print_json
-00000220: 7205 0000 00da 085f 5f6e 616d 655f 5fda  r......__name__.
+00000220: 7204 0000 00da 085f 5f6e 616d 655f 5fda  r......__name__.
 00000230: 0a66 6c61 736b 5f63 6f72 73da 0443 4f52  .flask_cors..COR
 00000240: 53da 1767 656e 6572 6174 655f 7061 7468  S..generate_path
 00000250: 5f69 6e76 656e 746f 7279 da0b 6265 6175  _inventory..beau
-00000260: 7469 6675 6c6c 7972 0800 0000 2904 da07  tifullyr....)...
+00000260: 7469 6675 6c6c 7972 0300 0000 2904 da07  tifullyr....)...
 00000270: 7265 636f 7264 73da 0763 6c69 6d61 7465  records..climate
 00000280: da03 6170 70da 1276 7565 5f64 6973 745f  ..app..vue_dist_
 00000290: 696e 7665 6e74 6f72 79a9 0072 1a00 0000  inventory..r....
 000002a0: fa3d 2f68 6162 6974 6174 2f76 656e 7565  .=/habitat/venue
 000002b0: 732f 7374 6167 6573 2f72 6563 7963 6c69  s/stages/recycli
 000002c0: 6e67 2f69 6e73 7472 756d 656e 742f 6c61  ng/instrument/la
 000002d0: 7965 722f 5f5f 696e 6974 5f5f 2e70 79da  yer/__init__.py.
-000002e0: 0562 7569 6c64 1700 0000 7324 0000 0008  .build....s$....
+000002e0: 0562 7569 6c64 2000 0000 7324 0000 0008  .build ...s$....
 000002f0: 0308 0204 0102 010c 0102 ff08 ff08 060a  ................
 00000300: 0102 0204 030a 0104 ff02 0602 0102 0104  ................
-00000310: fe04 0972 1c00 0000 2901 7207 0000 0029  ...r....).r....)
-00000320: 18da 075f 5f64 6f63 5f5f da04 6a73 6f6e  ...__doc__..json
-00000330: da07 6f73 2e70 6174 6872 0200 0000 7203  ..os.pathr....r.
-00000340: 0000 0072 0400 0000 da02 6f73 da09 7472  ...r......os..tr
-00000350: 6163 6562 6163 6b72 0f00 0000 da05 666c  acebackr......fl
-00000360: 6173 6b72 0500 0000 7206 0000 0072 1200  askr....r....r..
-00000370: 0000 da3c 7265 6379 636c 696e 672e 696e  ...<recycling.in
-00000380: 7374 7275 6d65 6e74 2e6c 6179 6572 2e75  strument.layer.u
-00000390: 7469 6c69 7469 6573 2e67 656e 6572 6174  tilities.generat
-000003a0: 655f 7061 7468 5f69 6e76 656e 746f 7279  e_path_inventory
-000003b0: da0a 696e 7374 7275 6d65 6e74 da05 6c61  ..instrument..la
-000003c0: 7965 72da 0975 7469 6c69 7469 6573 7214  yer..utilitiesr.
-000003d0: 0000 00da 1c72 6563 7963 6c69 6e67 2e69  .....recycling.i
-000003e0: 6e73 7472 756d 656e 742e 636c 696d 6174  nstrument.climat
-000003f0: 6572 1700 0000 720c 0000 00da 0672 6f75  er....r......rou
-00000400: 7465 7372 0800 0000 721c 0000 0072 1a00  tesr....r....r..
+00000310: fe04 0972 1c00 0000 2901 7202 0000 0029  ...r....).r....)
+00000320: 18da 075f 5f64 6f63 5f5f da3c 7265 6379  ...__doc__.<recy
+00000330: 636c 696e 672e 696e 7374 7275 6d65 6e74  cling.instrument
+00000340: 2e6c 6179 6572 2e75 7469 6c69 7469 6573  .layer.utilities
+00000350: 2e67 656e 6572 6174 655f 7061 7468 5f69  .generate_path_i
+00000360: 6e76 656e 746f 7279 da0a 696e 7374 7275  nventory..instru
+00000370: 6d65 6e74 da05 6c61 7965 72da 0975 7469  ment..layer..uti
+00000380: 6c69 7469 6573 7214 0000 00da 1c72 6563  litiesr......rec
+00000390: 7963 6c69 6e67 2e69 6e73 7472 756d 656e  ycling.instrumen
+000003a0: 742e 636c 696d 6174 6572 1700 0000 720c  t.climater....r.
+000003b0: 0000 00da 0672 6f75 7465 7372 0300 0000  .....routesr....
+000003c0: 720f 0000 00da 0566 6c61 736b 7204 0000  r......flaskr...
+000003d0: 0072 0500 0000 7212 0000 00da 046a 736f  .r....r......jso
+000003e0: 6eda 076f 732e 7061 7468 7206 0000 0072  n..os.pathr....r
+000003f0: 0700 0000 7208 0000 00da 026f 73da 0974  ....r......os..t
+00000400: 7261 6365 6261 636b 721c 0000 0072 1a00  racebackr....r..
 00000410: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
 00000420: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000430: 1a00 0000 0402 0805 1401 0801 0801 0803  ................
-00000440: 1001 0801 1e02 1201 0c02 0203 0eff       ..............
+00000430: 1a00 0000 0402 1e0b 1201 0c02 0803 1001  ................
+00000440: 0801 0803 1401 0801 0801 0205 0eff       ..............
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/_clique/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/_clique/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/__pycache__/moves.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/__pycache__/moves.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/moves.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/moves.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vibe_generator.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vibe_generator.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vue/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vue/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/routes/vue/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/routes/vue/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/layer/utilities/generate_path_inventory.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/utilities/generate_path_inventory.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moon/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moon/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/enumerate.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/__pycache__/enumerate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 583 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 4702 0000  o........@@fG...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 4502 0000  o........SQfE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 5a06  m.....m.....m.Z.
 00000050: 0100 6401 6402 6c07 6d08 0200 0100 6d09  ..d.d.l.m.....m.
 00000060: 0200 0100 6d0a 5a0b 0100 6403 6404 8400  ....m.Z...d.d...
 00000070: 5a0c 6402 5300 2905 7a6f 0a09 696d 706f  Z.d.S.).zo..impo
@@ -53,16 +53,16 @@
 00000340: 0f00 0000 1000 0000 730e 0000 0008 010c  ........s.......
 00000350: 0110 0206 0402 0106 ff04 0472 0f00 0000  ...........r....
 00000360: 290d da07 5f5f 646f 635f 5fda 0770 796d  )...__doc__..pym
 00000370: 6f6e 676f da21 7265 6379 636c 696e 672e  ongo.!recycling.
 00000380: 696e 7374 7275 6d65 6e74 2e6d 6f6f 6e2e  instrument.moon.
 00000390: 636f 6e6e 6563 74da 0a69 6e73 7472 756d  connect..instrum
 000003a0: 656e 74da 046d 6f6f 6eda 0763 6f6e 6e65  ent..moon..conne
-000003b0: 6374 720e 0000 00da 2072 6563 7963 6c69  ctr..... recycli
-000003c0: 6e67 2e6d 6f64 756c 6573 2e45 4543 5f34  ng.modules.EEC_4
-000003d0: 3438 5f32 2e6b 6579 73da 076d 6f64 756c  48_2.keys..modul
-000003e0: 6573 da09 4545 435f 3434 385f 32da 046b  es..EEC_448_2..k
-000003f0: 6579 73da 1545 4543 5f34 3438 5f32 5f6b  eys..EEC_448_2_k
-00000400: 6579 5f63 7265 6174 6f72 720f 0000 0072  ey_creatorr....r
-00000410: 0500 0000 7205 0000 0072 0500 0000 7209  ....r....r....r.
-00000420: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000430: 0073 0a00 0000 0403 0805 1802 1801 0c04  .s..............
+000003b0: 6374 720e 0000 00da 1e72 6563 7963 6c69  ctr......recycli
+000003c0: 6e67 2e6d 6978 6573 2e45 4543 5f34 3438  ng.mixes.EEC_448
+000003d0: 5f32 2e6b 6579 73da 056d 6978 6573 da09  _2.keys..mixes..
+000003e0: 4545 435f 3434 385f 32da 046b 6579 73da  EEC_448_2..keys.
+000003f0: 1545 4543 5f34 3438 5f32 5f6b 6579 5f63  .EEC_448_2_key_c
+00000400: 7265 6174 6f72 720f 0000 0072 0500 0000  reatorr....r....
+00000410: 7205 0000 0072 0500 0000 7209 0000 00da  r....r....r.....
+00000420: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
+00000430: 0000 0403 0805 1802 1801 0c04            ............
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moon/pocket/vibes/enumerate.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moon/pocket/vibes/enumerate.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	import recycling.instrument.moon.pocket.vibes.enumerate as enumerate_vibes
 	vibes = enumerate_vibes.start ()
 '''
 
 import pymongo
 
 import recycling.instrument.moon.connect as moon_connect
-import recycling.modules.EEC_448_2.keys as EEC_448_2_key_creator	
+import recycling.mixes.EEC_448_2.keys as EEC_448_2_key_creator	
 
 
 
 def start ():
 	moon_connection = moon_connect.start ()
 	vibes = moon_connection ["pocket"] ["vibes"]
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/make.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/make.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_layer.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_layer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9a05 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 7c6e 5166 9a05 0000  o.......|nQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 6d05 5a05 0100  l.m.Z.m.Z.m.Z...
 00000050: 6401 6402 6c06 5a06 6401 6402 6c07 5a07  d.d.l.Z.d.d.l.Z.
 00000060: 6401 6404 6c08 6d09 5a09 0100 6405 6406  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0c 0100 6401 6402 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_mongo.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/__pycache__/start_mongo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/__pycache__/feel.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/__pycache__/feel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1576 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 2806 0000  o........@@f(...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 2006 0000  o........SQf ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6402  Z...d.d.l.Z.d.d.
 00000040: 6c02 6d03 0200 0100 6d04 0200 0100 6d05  l.m.....m.....m.
 00000050: 5a05 0100 6401 6402 6c06 6d03 0200 0100  Z...d.d.l.m.....
 00000060: 6d04 0200 0100 6d07 0200 0100 6d08 0200  m.....m.....m...
 00000070: 0100 6d09 5a0a 0100 6401 6402 6c0b 6d03  ..m.Z...d.d.l.m.
@@ -66,32 +66,31 @@
 00000410: 6665 656c 696e 6773 2f45 4343 5f34 3438  feelings/ECC_448
 00000420: 5f32 2f66 6565 6c2e 7079 da0b 7065 7266  _2/feel.py..perf
 00000430: 6f72 6d61 6e63 6521 0000 0073 2a00 0000  ormance!...s*...
 00000440: 0c03 0c02 0801 0801 0402 0201 04ff 0e04  ................
 00000450: 0e01 0407 0201 0802 0801 06fc 0806 0601  ................
 00000460: 0402 0203 0402 02ff 06fe 721e 0000 0029  ..........r....)
 00000470: 13da 075f 5f64 6f63 5f5f 720c 0000 00da  ...__doc__r.....
-00000480: 2272 6563 7963 6c69 6e67 2e6d 6f64 756c  "recycling.modul
-00000490: 6573 2e45 4543 5f34 3438 5f32 2e76 6572  es.EEC_448_2.ver
-000004a0: 6966 79da 076d 6f64 756c 6573 da09 4545  ify..modules..EE
-000004b0: 435f 3434 385f 3272 1300 0000 da3c 7265  C_448_2r.....<re
-000004c0: 6379 636c 696e 672e 6d6f 6475 6c65 732e  cycling.modules.
-000004d0: 4545 435f 3434 385f 322e 6d6f 6475 6c61  EEC_448_2.modula
-000004e0: 746f 7273 2e62 7974 655f 7374 7269 6e67  tors.byte_string
-000004f0: 2e66 726f 6d5f 5554 4638 da0a 6d6f 6475  .from_UTF8..modu
-00000500: 6c61 746f 7273 da0b 6279 7465 5f73 7472  lators..byte_str
-00000510: 696e 67da 0966 726f 6d5f 5554 4638 7211  ing..from_UTF8r.
-00000520: 0000 00da 4372 6563 7963 6c69 6e67 2e6d  ....Crecycling.m
-00000530: 6f64 756c 6573 2e45 4543 5f34 3438 5f32  odules.EEC_448_2
-00000540: 2e6d 6f64 756c 6174 6f72 732e 6279 7465  .modulators.byte
-00000550: 5f73 7472 696e 672e 6672 6f6d 5f68 6578  _string.from_hex
-00000560: 6164 6563 696d 616c da10 6672 6f6d 5f68  adecimal..from_h
-00000570: 6578 6164 6563 696d 616c 7215 0000 00da  exadecimalr.....
-00000580: 2f72 6563 7963 6c69 6e67 2e6d 6f64 756c  /recycling.modul
-00000590: 6573 2e45 4543 5f34 3438 5f32 2e70 7562  es.EEC_448_2.pub
-000005a0: 6c69 635f 6b65 792e 696e 7374 616e 6365  lic_key.instance
-000005b0: da0a 7075 626c 6963 5f6b 6579 da08 696e  ..public_key..in
-000005c0: 7374 616e 6365 720e 0000 0072 1e00 0000  stancer....r....
-000005d0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-000005e0: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000005f0: 0000 7310 0000 0004 0102 0608 0f18 0224  ..s............$
-00000600: 0224 011e 020c 03                        .$.....
+00000480: 2072 6563 7963 6c69 6e67 2e6d 6978 6573   recycling.mixes
+00000490: 2e45 4543 5f34 3438 5f32 2e76 6572 6966  .EEC_448_2.verif
+000004a0: 79da 056d 6978 6573 da09 4545 435f 3434  y..mixes..EEC_44
+000004b0: 385f 3272 1300 0000 da3a 7265 6379 636c  8_2r.....:recycl
+000004c0: 696e 672e 6d69 7865 732e 4545 435f 3434  ing.mixes.EEC_44
+000004d0: 385f 322e 6d6f 6475 6c61 746f 7273 2e62  8_2.modulators.b
+000004e0: 7974 655f 7374 7269 6e67 2e66 726f 6d5f  yte_string.from_
+000004f0: 5554 4638 da0a 6d6f 6475 6c61 746f 7273  UTF8..modulators
+00000500: da0b 6279 7465 5f73 7472 696e 67da 0966  ..byte_string..f
+00000510: 726f 6d5f 5554 4638 7211 0000 00da 4172  rom_UTF8r.....Ar
+00000520: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00000530: 4543 5f34 3438 5f32 2e6d 6f64 756c 6174  EC_448_2.modulat
+00000540: 6f72 732e 6279 7465 5f73 7472 696e 672e  ors.byte_string.
+00000550: 6672 6f6d 5f68 6578 6164 6563 696d 616c  from_hexadecimal
+00000560: da10 6672 6f6d 5f68 6578 6164 6563 696d  ..from_hexadecim
+00000570: 616c 7215 0000 00da 2d72 6563 7963 6c69  alr.....-recycli
+00000580: 6e67 2e6d 6978 6573 2e45 4543 5f34 3438  ng.mixes.EEC_448
+00000590: 5f32 2e70 7562 6c69 635f 6b65 792e 696e  _2.public_key.in
+000005a0: 7374 616e 6365 da0a 7075 626c 6963 5f6b  stance..public_k
+000005b0: 6579 da08 696e 7374 616e 6365 720e 0000  ey..instancer...
+000005c0: 0072 1e00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+000005d0: 721c 0000 0072 1d00 0000 da08 3c6d 6f64  r....r......<mod
+000005e0: 756c 653e 0100 0000 7310 0000 0004 0102  ule>....s.......
+000005f0: 0608 0f18 0224 0224 011e 020c 03         .....$.$.....
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/feel.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/feelings/ECC_448_2/feel.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 }
 
 '''
 
 	
 import rich	
 
-import recycling.modules.EEC_448_2.verify as verify
+import recycling.mixes.EEC_448_2.verify as verify
 
-import recycling.modules.EEC_448_2.modulators.byte_string.from_UTF8 as UTF8_to_byte_string
-import recycling.modules.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
+import recycling.mixes.EEC_448_2.modulators.byte_string.from_UTF8 as UTF8_to_byte_string
+import recycling.mixes.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
 
-import recycling.modules.EEC_448_2.public_key.instance as instantiate_public_key
+import recycling.mixes.EEC_448_2.public_key.instance as instantiate_public_key
 	
 
 def performance (
 	fields
 ):
 	rich.print_json (data = fields)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/add.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/add.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/bounce.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/bounce.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/show.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/__pycache__/show.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/add.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/add.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/hotties/bounce.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/hotties/bounce.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/make.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/make.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/__pycache__/perform.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/__pycache__/perform.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9e05 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 9805 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 0200  Z.....d.d.l.m...
 00000040: 0100 6d03 0200 0100 6d04 5a05 0100 6401  ..m.....m.Z...d.
 00000050: 6402 6c06 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
 00000060: 6d07 0200 0100 6d08 5a09 0100 6401 6402  m.....m.Z...d.d.
 00000070: 6c0a 5a0a 6403 6404 8400 5a0b 6402 5300  l.Z.d.d...Z.d.S.
-00000080: 2905 6137 0200 000a 756e 6963 6f64 655f  ).a7....unicode_
+00000080: 2905 6135 0200 000a 756e 6963 6f64 655f  ).a5....unicode_
 00000090: 7374 7269 6e67 203d 206a 736f 6e2e 6475  string = json.du
 000000a0: 6d70 7320 287b 0a09 226d 6f76 6522 3a20  mps ({.."move": 
 000000b0: 2273 656e 6422 2c0a 0922 6669 656c 6473  "send",.."fields
 000000c0: 223a 207b 0a09 0922 746f 223a 207b 0a09  ": {..."to": {..
 000000d0: 0909 226b 696e 6422 3a20 2245 4543 5f34  .."kind": "EEC_4
 000000e0: 3438 5f31 222c 0a09 0909 2261 6464 7265  48_1",...."addre
 000000f0: 7373 223a 2022 3330 3433 3330 3035 3036  ss": "3043300506
@@ -25,72 +25,72 @@
 00000180: 220a 0909 7d2c 0a09 0922 616d 6f75 6e74  "...},..."amount
 00000190: 223a 2022 3430 3332 3437 3839 3332 3438  ": "403247893248
 000001a0: 3733 220a 097d 0a7d 2c20 696e 6465 6e74  73"..}.}, indent
 000001b0: 203d 2034 2909 090a 756e 7369 676e 6564   = 4)...unsigned
 000001c0: 5f62 7974 6573 203d 2075 6e69 636f 6465  _bytes = unicode
 000001d0: 5f73 7472 696e 672e 656e 636f 6465 2028  _string.encode (
 000001e0: 2275 7466 2d38 2229 0a0a 696d 706f 7274  "utf-8")..import
-000001f0: 2072 6563 7963 6c69 6e67 2e6d 6f64 756c   recycling.modul
-00000200: 6573 2e45 4543 5f34 3438 5f32 2e73 6967  es.EEC_448_2.sig
-00000210: 6e20 6173 2045 4543 5f34 3438 5f32 5f73  n as EEC_448_2_s
-00000220: 6967 6e0a 7369 676e 6564 203d 2045 4543  ign.signed = EEC
-00000230: 5f34 3438 5f32 5f73 6967 6e2e 7374 6172  _448_2_sign.star
-00000240: 7420 280a 0970 7269 7661 7465 5f6b 6579  t (..private_key
-00000250: 5f69 6e73 7461 6e63 652c 0a09 756e 7369  _instance,..unsi
-00000260: 676e 6564 5f62 7974 6573 203d 2075 6e73  gned_bytes = uns
-00000270: 6967 6e65 645f 6279 7465 730a 290a 0a73  igned_bytes.)..s
-00000280: 6967 6e65 645f 6279 7465 735f 6865 7861  igned_bytes_hexa
-00000290: 6465 6369 6d61 6c20 3d20 7369 676e 6564  decimal = signed
-000002a0: 205b 2273 6967 6e65 6420 6279 7465 7320   ["signed bytes 
-000002b0: 6865 7861 6465 6369 6d61 6c22 5d0a e900  hexadecimal"]...
-000002c0: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
-000002d0: 0006 0000 0004 0000 0043 0000 0073 5400  .........C...sT.
-000002e0: 0000 7400 6a01 7c00 6401 8d01 0100 7c00  ..t.j.|.d.....|.
-000002f0: 6402 1900 6403 1900 7d01 7c00 6404 1900  d...d...}.|.d...
-00000300: 7d02 7c02 a002 6405 a101 7d03 7403 a004  }.|...d...}.t...
-00000310: 7c01 a101 7d04 7405 6a06 7c04 7c03 6406  |...}.t.j.|.|.d.
-00000320: 8d02 7d05 6407 6408 7c05 6409 1900 6901  ..}.d.d.|.d...i.
-00000330: 640a 9c02 5300 290b 4e29 01da 0464 6174  d...S.).N)...dat
-00000340: 617a 0f69 6e74 696d 6174 6520 7268 7974  az.intimate rhyt
-00000350: 686d 7a12 6865 7861 6465 6369 6d61 6c20  hmz.hexadecimal 
-00000360: 7374 7269 6e67 7a0b 5554 4638 2073 7472  stringz.UTF8 str
-00000370: 696e 677a 0575 7466 2d38 2901 da0e 756e  ingz.utf-8)...un
-00000380: 7369 676e 6564 5f62 7974 6573 da04 7061  signed_bytes..pa
-00000390: 7373 da0b 7065 7266 6f72 6d61 6e63 657a  ss..performancez
-000003a0: 1873 6967 6e65 6420 6279 7465 7320 6865  .signed bytes he
-000003b0: 7861 6465 6369 6d61 6c29 02da 0673 7461  xadecimal)...sta
-000003c0: 7475 73da 046e 6f74 6529 07da 0472 6963  tus..note)...ric
-000003d0: 68da 0a70 7269 6e74 5f6a 736f 6eda 0665  h..print_json..e
-000003e0: 6e63 6f64 65da 1769 6e73 7461 6e74 6961  ncode..instantia
-000003f0: 7465 5f70 7269 7661 7465 5f6b 6579 da1b  te_private_key..
-00000400: 6672 6f6d 5f44 4552 5f68 6578 6164 6563  from_DER_hexadec
-00000410: 696d 616c 5f73 7472 696e 67da 0e45 4543  imal_string..EEC
-00000420: 5f34 3438 5f32 5f73 6967 6eda 0573 7461  _448_2_sign..sta
-00000430: 7274 2906 da06 6669 656c 6473 da22 7072  rt)...fields."pr
-00000440: 6976 6174 655f 6b65 795f 4445 525f 6865  ivate_key_DER_he
-00000450: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
-00000460: da0b 5554 4638 5f73 7472 696e 6772 0300  ..UTF8_stringr..
-00000470: 0000 da14 7072 6976 6174 655f 6b65 795f  ....private_key_
-00000480: 696e 7374 616e 6365 da06 7369 676e 6564  instance..signed
-00000490: a900 7214 0000 00fa 592f 6861 6269 7461  ..r.....Y/habita
-000004a0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-000004b0: 7265 6379 636c 696e 672f 696e 7374 7275  recycling/instru
-000004c0: 6d65 6e74 2f6d 6f76 6573 2f6e 616d 6573  ment/moves/names
-000004d0: 2f70 6572 666f 726d 616e 6365 732f 4543  /performances/EC
-000004e0: 435f 3434 385f 322f 7065 7266 6f72 6d2e  C_448_2/perform.
-000004f0: 7079 da05 7374 6f72 792c 0000 0073 1e00  py..story,...s..
-00000500: 0000 0c03 0c02 0801 0a02 0402 0201 04ff  ................
-00000510: 0403 0201 0201 06fe 0206 0802 02ff 06fe  ................
-00000520: 7216 0000 0029 0cda 075f 5f64 6f63 5f5f  r....)...__doc__
-00000530: da20 7265 6379 636c 696e 672e 6d6f 6475  . recycling.modu
-00000540: 6c65 732e 4545 435f 3434 385f 322e 7369  les.EEC_448_2.si
-00000550: 676e da07 6d6f 6475 6c65 73da 0945 4543  gn..modules..EEC
-00000560: 5f34 3438 5f32 da04 7369 676e 720d 0000  _448_2..signr...
-00000570: 00da 3072 6563 7963 6c69 6e67 2e6d 6f64  ..0recycling.mod
-00000580: 756c 6573 2e45 4543 5f34 3438 5f32 2e70  ules.EEC_448_2.p
-00000590: 7269 7661 7465 5f6b 6579 2e69 6e73 7461  rivate_key.insta
-000005a0: 6e63 65da 0b70 7269 7661 7465 5f6b 6579  nce..private_key
-000005b0: da08 696e 7374 616e 6365 720b 0000 0072  ..instancer....r
-000005c0: 0800 0000 7216 0000 0072 1400 0000 7214  ....r....r....r.
-000005d0: 0000 0072 1400 0000 7215 0000 00da 083c  ...r....r......<
-000005e0: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-000005f0: 0401 0216 020b 1804 1e01 0802 0c02       ..............
+000001f0: 2072 6563 7963 6c69 6e67 2e6d 6978 6573   recycling.mixes
+00000200: 2e45 4543 5f34 3438 5f32 2e73 6967 6e20  .EEC_448_2.sign 
+00000210: 6173 2045 4543 5f34 3438 5f32 5f73 6967  as EEC_448_2_sig
+00000220: 6e0a 7369 676e 6564 203d 2045 4543 5f34  n.signed = EEC_4
+00000230: 3438 5f32 5f73 6967 6e2e 7374 6172 7420  48_2_sign.start 
+00000240: 280a 0970 7269 7661 7465 5f6b 6579 5f69  (..private_key_i
+00000250: 6e73 7461 6e63 652c 0a09 756e 7369 676e  nstance,..unsign
+00000260: 6564 5f62 7974 6573 203d 2075 6e73 6967  ed_bytes = unsig
+00000270: 6e65 645f 6279 7465 730a 290a 0a73 6967  ned_bytes.)..sig
+00000280: 6e65 645f 6279 7465 735f 6865 7861 6465  ned_bytes_hexade
+00000290: 6369 6d61 6c20 3d20 7369 676e 6564 205b  cimal = signed [
+000002a0: 2273 6967 6e65 6420 6279 7465 7320 6865  "signed bytes he
+000002b0: 7861 6465 6369 6d61 6c22 5d0a e900 0000  xadecimal"].....
+000002c0: 004e 6301 0000 0000 0000 0000 0000 0006  .Nc.............
+000002d0: 0000 0004 0000 0043 0000 0073 5400 0000  .......C...sT...
+000002e0: 7400 6a01 7c00 6401 8d01 0100 7c00 6402  t.j.|.d.....|.d.
+000002f0: 1900 6403 1900 7d01 7c00 6404 1900 7d02  ..d...}.|.d...}.
+00000300: 7c02 a002 6405 a101 7d03 7403 a004 7c01  |...d...}.t...|.
+00000310: a101 7d04 7405 6a06 7c04 7c03 6406 8d02  ..}.t.j.|.|.d...
+00000320: 7d05 6407 6408 7c05 6409 1900 6901 640a  }.d.d.|.d...i.d.
+00000330: 9c02 5300 290b 4e29 01da 0464 6174 617a  ..S.).N)...dataz
+00000340: 0f69 6e74 696d 6174 6520 7268 7974 686d  .intimate rhythm
+00000350: 7a12 6865 7861 6465 6369 6d61 6c20 7374  z.hexadecimal st
+00000360: 7269 6e67 7a0b 5554 4638 2073 7472 696e  ringz.UTF8 strin
+00000370: 677a 0575 7466 2d38 2901 da0e 756e 7369  gz.utf-8)...unsi
+00000380: 676e 6564 5f62 7974 6573 da04 7061 7373  gned_bytes..pass
+00000390: da0b 7065 7266 6f72 6d61 6e63 657a 1873  ..performancez.s
+000003a0: 6967 6e65 6420 6279 7465 7320 6865 7861  igned bytes hexa
+000003b0: 6465 6369 6d61 6c29 02da 0673 7461 7475  decimal)...statu
+000003c0: 73da 046e 6f74 6529 07da 0472 6963 68da  s..note)...rich.
+000003d0: 0a70 7269 6e74 5f6a 736f 6eda 0665 6e63  .print_json..enc
+000003e0: 6f64 65da 1769 6e73 7461 6e74 6961 7465  ode..instantiate
+000003f0: 5f70 7269 7661 7465 5f6b 6579 da1b 6672  _private_key..fr
+00000400: 6f6d 5f44 4552 5f68 6578 6164 6563 696d  om_DER_hexadecim
+00000410: 616c 5f73 7472 696e 67da 0e45 4543 5f34  al_string..EEC_4
+00000420: 3438 5f32 5f73 6967 6eda 0573 7461 7274  48_2_sign..start
+00000430: 2906 da06 6669 656c 6473 da22 7072 6976  )...fields."priv
+00000440: 6174 655f 6b65 795f 4445 525f 6865 7861  ate_key_DER_hexa
+00000450: 6465 6369 6d61 6c5f 7374 7269 6e67 da0b  decimal_string..
+00000460: 5554 4638 5f73 7472 696e 6772 0300 0000  UTF8_stringr....
+00000470: da14 7072 6976 6174 655f 6b65 795f 696e  ..private_key_in
+00000480: 7374 616e 6365 da06 7369 676e 6564 a900  stance..signed..
+00000490: 7214 0000 00fa 592f 6861 6269 7461 742f  r.....Y/habitat/
+000004a0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+000004b0: 6379 636c 696e 672f 696e 7374 7275 6d65  cycling/instrume
+000004c0: 6e74 2f6d 6f76 6573 2f6e 616d 6573 2f70  nt/moves/names/p
+000004d0: 6572 666f 726d 616e 6365 732f 4543 435f  erformances/ECC_
+000004e0: 3434 385f 322f 7065 7266 6f72 6d2e 7079  448_2/perform.py
+000004f0: da05 7374 6f72 792c 0000 0073 1e00 0000  ..story,...s....
+00000500: 0c03 0c02 0801 0a02 0402 0201 04ff 0403  ................
+00000510: 0201 0201 06fe 0206 0802 02ff 06fe 7216  ..............r.
+00000520: 0000 0029 0cda 075f 5f64 6f63 5f5f da1e  ...)...__doc__..
+00000530: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+00000540: 4545 435f 3434 385f 322e 7369 676e da05  EEC_448_2.sign..
+00000550: 6d69 7865 73da 0945 4543 5f34 3438 5f32  mixes..EEC_448_2
+00000560: da04 7369 676e 720d 0000 00da 2e72 6563  ..signr......rec
+00000570: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000580: 5f34 3438 5f32 2e70 7269 7661 7465 5f6b  _448_2.private_k
+00000590: 6579 2e69 6e73 7461 6e63 65da 0b70 7269  ey.instance..pri
+000005a0: 7661 7465 5f6b 6579 da08 696e 7374 616e  vate_key..instan
+000005b0: 6365 720b 0000 0072 0800 0000 7216 0000  cer....r....r...
+000005c0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+000005d0: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000005e0: 0000 0073 0e00 0000 0401 0216 020b 1804  ...s............
+000005f0: 1e01 0802 0c02                           ......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/perform.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/performances/ECC_448_2/perform.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 			"address": "3043300506032b6571033a00e26960a83c45c0bb86e356cd727473e96682e76c6dd01c991a6ea0a394ecca27b467554d73e2a22b05425c1926a7a92befda5c1937d6876f00"
 		},
 		"amount": "40324789324873"
 	}
 }, indent = 4)		
 unsigned_bytes = unicode_string.encode ("utf-8")
 
-import recycling.modules.EEC_448_2.sign as EEC_448_2_sign
+import recycling.mixes.EEC_448_2.sign as EEC_448_2_sign
 signed = EEC_448_2_sign.start (
 	private_key_instance,
 	unsigned_bytes = unsigned_bytes
 )
 
 signed_bytes_hexadecimal = signed ["signed bytes hexadecimal"]
 '''
@@ -32,16 +32,16 @@
 		}
 	}
 '''
 '''
 
 '''
 
-import recycling.modules.EEC_448_2.sign as EEC_448_2_sign
-import recycling.modules.EEC_448_2.private_key.instance as instantiate_private_key
+import recycling.mixes.EEC_448_2.sign as EEC_448_2_sign
+import recycling.mixes.EEC_448_2.private_key.instance as instantiate_private_key
 	
 import rich	
 	
 def story (
 	fields
 ):
 	rich.print_json (data = fields)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/start_layer.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/start_layer.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/start_mongo.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/start_mongo.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	}
 '''
 
 import pymongo
 
 import recycling.instrument.climate as instrument_climate
 import recycling.instrument.moon.connect as moon_connect
-import recycling.modules.EEC_448_2.keys as EEC_448_2_key_creator	
+import recycling.mixes.EEC_448_2.keys as EEC_448_2_key_creator	
 
 def perform (fields):
 	assert (len (fields ["seed"]) == 114) 
 	assert (len (fields ["name"]) >= 1)
 
 	moon_connection = moon_connect.start ()
 	vibes = moon_connection ["pocket"] ["vibes"]
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/moves/names/vibes/make_ECC_448_2/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1222 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 c604 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 c404 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 5a05 0100 6401 6402  m.....m.Z...d.d.
 00000050: 6c06 6d03 0200 0100 6d07 0200 0100 6d08  l.m.....m.....m.
 00000060: 5a09 0100 6401 6402 6c0a 6d0b 0200 0100  Z...d.d.l.m.....
 00000070: 6d0c 0200 0100 6d0d 5a0e 0100 6403 6404  m.....m.Z...d.d.
@@ -65,16 +65,15 @@
 00000400: 6379 636c 696e 672e 696e 7374 7275 6d65  cycling.instrume
 00000410: 6e74 2e63 6c69 6d61 7465 da0a 696e 7374  nt.climate..inst
 00000420: 7275 6d65 6e74 da07 636c 696d 6174 65da  rument..climate.
 00000430: 1269 6e73 7472 756d 656e 745f 636c 696d  .instrument_clim
 00000440: 6174 65da 2172 6563 7963 6c69 6e67 2e69  ate.!recycling.i
 00000450: 6e73 7472 756d 656e 742e 6d6f 6f6e 2e63  nstrument.moon.c
 00000460: 6f6e 6e65 6374 da04 6d6f 6f6e da07 636f  onnect..moon..co
-00000470: 6e6e 6563 7472 1400 0000 da20 7265 6379  nnectr..... recy
-00000480: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000490: 435f 3434 385f 322e 6b65 7973 da07 6d6f  C_448_2.keys..mo
-000004a0: 6475 6c65 73da 0945 4543 5f34 3438 5f32  dules..EEC_448_2
-000004b0: 721c 0000 0072 1600 0000 7221 0000 0072  r....r....r!...r
-000004c0: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
-000004d0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000004e0: 0073 0c00 0000 0401 080a 1202 1801 1801  .s..............
-000004f0: 0c02                                     ..
+00000470: 6e6e 6563 7472 1400 0000 da1e 7265 6379  nnectr......recy
+00000480: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+00000490: 3434 385f 322e 6b65 7973 da05 6d69 7865  448_2.keys..mixe
+000004a0: 73da 0945 4543 5f34 3438 5f32 721c 0000  s..EEC_448_2r...
+000004b0: 0072 1600 0000 7221 0000 0072 1f00 0000  .r....r!...r....
+000004c0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+000004d0: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
+000004e0: 0000 0401 080a 1202 1801 1801 0c02       ..............
```

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/sockets/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/sockets/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/sockets/__pycache__/clique_group.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/instrument/sockets/__pycache__/clique_group.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/instrument/sockets/clique_group.py` & `recycling-1.1.0/venues/stages/recycling/instrument/sockets/clique_group.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/module.s.HTML` & `recycling-1.1.0/venues/stages/recycling/module.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_seed_phrase/2048.r.html` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_seed_phrase/2048.r.html`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_1_generator/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 eb06 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 e706 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 5a07 6401 6403 6c08 6d09  d.d.l.Z.d.d.l.m.
 00000060: 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401 6402  Z.m.Z.m.Z...d.d.
 00000070: 6c0c 5a0c 6404 6405 8400 5a0d 6406 650d  l.Z.d.d...Z.d.e.
-00000080: 6901 5a0e 6402 5300 2907 7a57 0a09 7079  i.Z.d.S.).zW..py
+00000080: 6901 5a0e 6402 5300 2907 7a55 0a09 7079  i.Z.d.S.).zU..py
 00000090: 7468 6f6e 3320 696e 7375 7261 6e63 652e  thon3 insurance.
-000000a0: 7072 6f63 2e70 7920 226d 6f64 756c 6573  proc.py "modules
-000000b0: 2f45 4543 5f34 3438 5f31 2f5f 7374 6174  /EEC_448_1/_stat
-000000c0: 7573 2f73 7461 7475 735f 315f 6765 6e65  us/status_1_gene
-000000d0: 7261 746f 722f 7374 6174 7573 5f31 2e70  rator/status_1.p
-000000e0: 7922 0ae9 0000 0000 4e29 03da 0764 6972  y"......N)...dir
-000000f0: 6e61 6d65 da04 6a6f 696e da08 6e6f 726d  name..join..norm
-00000100: 7061 7468 6300 0000 0000 0000 0000 0000  pathc...........
-00000110: 0008 0000 0007 0000 0043 0000 0073 7200  .........C...sr.
-00000120: 0000 6700 6401 a201 7d00 6402 6403 6702  ..g.d...}.d.d.g.
-00000130: 7d01 7c00 4400 5d2c 7d02 7c01 4400 5d27  }.|.D.],}.|.D.]'
-00000140: 7d03 7400 7401 7402 a003 7404 a101 6a05  }.t.t.t...t...j.
-00000150: a006 a100 6404 8302 8301 6405 1700 7c03  ....d.....d...|.
-00000160: 1700 7d04 7407 a008 7c02 7c03 7c04 a103  ..}.t...|.|.|...
-00000170: 7d05 7c05 6406 1900 7d06 7c05 6407 1900  }.|.d...}.|.d...
-00000180: 7d07 7409 a00a 7c04 a101 0100 710e 710a  }.t...|.....q.q.
-00000190: 6400 5300 2908 4e29 08da 7234 3938 3638  d.S.).N)..r49868
-000001a0: 3838 6231 3133 3538 6266 3364 3534 3162  88b11358bf3d541b
-000001b0: 3431 6565 6135 6461 6563 6531 6336 6566  41eea5daece1c6ef
-000001c0: 6636 3431 3330 6134 3566 6338 6239 6361  f64130a45fc8b9ca
-000001d0: 3438 6633 6530 6530 3234 3633 6339 3963  48f3e0e02463c99c
-000001e0: 3561 6564 6338 6138 3437 3638 3664 3636  5aedc8a847686d66
-000001f0: 3962 3764 3534 3763 3138 6665 3434 3866  9b7d547c18fe448f
-00000200: 6335 3131 3163 6138 3866 3465 38da 7235  c5111ca88f4e8.r5
-00000210: 3938 3638 3838 6231 3133 3538 6266 3364  986888b11358bf3d
-00000220: 3534 3162 3431 6565 6135 6461 6563 6531  541b41eea5daece1
-00000230: 6336 6566 6636 3431 3330 6134 3566 6338  c6eff64130a45fc8
-00000240: 6239 6361 3438 6633 6530 6530 3234 3633  b9ca48f3e0e02463
-00000250: 6339 3963 3561 6564 6338 6138 3437 3638  c99c5aedc8a84768
-00000260: 3664 3636 3962 3764 3534 3763 3138 6665  6d669b7d547c18fe
-00000270: 3434 3866 6335 3131 3163 6138 3866 3465  448fc5111ca88f4e
-00000280: 38da 7230 3030 3030 3030 3030 3030 3030  8.r0000000000000
+000000a0: 7072 6f63 2e70 7920 226d 6978 6573 2f45  proc.py "mixes/E
+000000b0: 4543 5f34 3438 5f31 2f5f 7374 6174 7573  EC_448_1/_status
+000000c0: 2f73 7461 7475 735f 315f 6765 6e65 7261  /status_1_genera
+000000d0: 746f 722f 7374 6174 7573 5f31 2e70 7922  tor/status_1.py"
+000000e0: 0ae9 0000 0000 4e29 03da 0764 6972 6e61  ......N)...dirna
+000000f0: 6d65 da04 6a6f 696e da08 6e6f 726d 7061  me..join..normpa
+00000100: 7468 6300 0000 0000 0000 0000 0000 0008  thc.............
+00000110: 0000 0007 0000 0043 0000 0073 7200 0000  .......C...sr...
+00000120: 6700 6401 a201 7d00 6402 6403 6702 7d01  g.d...}.d.d.g.}.
+00000130: 7c00 4400 5d2c 7d02 7c01 4400 5d27 7d03  |.D.],}.|.D.]'}.
+00000140: 7400 7401 7402 a003 7404 a101 6a05 a006  t.t.t...t...j...
+00000150: a100 6404 8302 8301 6405 1700 7c03 1700  ..d.....d...|...
+00000160: 7d04 7407 a008 7c02 7c03 7c04 a103 7d05  }.t...|.|.|...}.
+00000170: 7c05 6406 1900 7d06 7c05 6407 1900 7d07  |.d...}.|.d...}.
+00000180: 7409 a00a 7c04 a101 0100 710e 710a 6400  t...|.....q.q.d.
+00000190: 5300 2908 4e29 08da 7234 3938 3638 3838  S.).N)..r4986888
+000001a0: 6231 3133 3538 6266 3364 3534 3162 3431  b11358bf3d541b41
+000001b0: 6565 6135 6461 6563 6531 6336 6566 6636  eea5daece1c6eff6
+000001c0: 3431 3330 6134 3566 6338 6239 6361 3438  4130a45fc8b9ca48
+000001d0: 6633 6530 6530 3234 3633 6339 3963 3561  f3e0e02463c99c5a
+000001e0: 6564 6338 6138 3437 3638 3664 3636 3962  edc8a847686d669b
+000001f0: 3764 3534 3763 3138 6665 3434 3866 6335  7d547c18fe448fc5
+00000200: 3131 3163 6138 3866 3465 38da 7235 3938  111ca88f4e8.r598
+00000210: 3638 3838 6231 3133 3538 6266 3364 3534  6888b11358bf3d54
+00000220: 3162 3431 6565 6135 6461 6563 6531 6336  1b41eea5daece1c6
+00000230: 6566 6636 3431 3330 6134 3566 6338 6239  eff64130a45fc8b9
+00000240: 6361 3438 6633 6530 6530 3234 3633 6339  ca48f3e0e02463c9
+00000250: 3963 3561 6564 6338 6138 3437 3638 3664  9c5aedc8a847686d
+00000260: 3636 3962 3764 3534 3763 3138 6665 3434  669b7d547c18fe44
+00000270: 3866 6335 3131 3163 6138 3866 3465 38da  8fc5111ca88f4e8.
+00000280: 7230 3030 3030 3030 3030 3030 3030 3030  r000000000000000
 00000290: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000002a0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000002b0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000002c0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000002d0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000002e0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-000002f0: 3030 3030 30da 7266 6666 6666 6666 6666  00000.rfffffffff
+000002f0: 3030 30da 7266 6666 6666 6666 6666 6666  000.rfffffffffff
 00000300: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000310: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000320: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000330: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000340: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000350: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-00000360: 6666 6666 6666 6666 66da 7231 3233 3431  fffffffff.r12341
-00000370: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000380: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000390: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-000003a0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-000003b0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-000003c0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-000003d0: 3233 3431 3233 3431 3233 3431 32da 7230  2341234123412.r0
-000003e0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000003f0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000400: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000410: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000420: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000430: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000440: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000450: 66da 7231 3335 3739 3133 3537 3931 3335  f.r1357913579135
-00000460: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000470: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000480: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000490: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-000004a0: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-000004b0: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-000004c0: 3931 3335 37da 7232 3436 3865 6632 3436  91357.r2468ef246
-000004d0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-000004e0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-000004f0: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-00000500: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-00000510: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-00000520: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-00000530: 3865 6632 3436 3865 66da 0344 4552 da03  8ef2468ef..DER..
-00000540: 5045 4dda 1545 4543 5f34 3438 5f31 5f70  PEM..EEC_448_1_p
-00000550: 7269 7661 7465 5f6b 6579 da01 2eda 0869  rivate_key.....i
-00000560: 6e73 7461 6e63 65da 0673 7472 696e 6729  nstance..string)
-00000570: 0b72 0400 0000 7203 0000 00da 0770 6174  .r....r......pat
-00000580: 686c 6962 da04 5061 7468 da08 5f5f 6669  hlib..Path..__fi
-00000590: 6c65 5f5f da06 7061 7265 6e74 da07 7265  le__..parent..re
-000005a0: 736f 6c76 65da 1d45 4543 5f34 3438 5f31  solve..EEC_448_1
-000005b0: 5f70 7269 7661 7465 5f6b 6579 5f63 7265  _private_key_cre
-000005c0: 6174 6f72 da06 6372 6561 7465 da02 6f73  ator..create..os
-000005d0: da06 7265 6d6f 7665 2908 da05 7365 6564  ..remove)...seed
-000005e0: 73da 0766 6f72 6d61 7473 da04 7365 6564  s..formats..seed
-000005f0: da06 666f 726d 6174 da10 7072 6976 6174  ..format..privat
-00000600: 655f 6b65 795f 7061 7468 da0b 7072 6976  e_key_path..priv
-00000610: 6174 655f 6b65 79da 1470 7269 7661 7465  ate_key..private
-00000620: 5f6b 6579 5f69 6e73 7461 6e63 65da 1270  _key_instance..p
-00000630: 7269 7661 7465 5f6b 6579 5f73 7472 696e  rivate_key_strin
-00000640: 67a9 0072 2400 0000 fa59 2f68 6162 6974  g..r$....Y/habit
-00000650: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-00000660: 2f72 6563 7963 6c69 6e67 2f6d 6f64 756c  /recycling/modul
-00000670: 6573 2f45 4543 5f34 3438 5f31 2f5f 7374  es/EEC_448_1/_st
-00000680: 6174 7573 2f73 7461 7475 735f 315f 6765  atus/status_1_ge
-00000690: 6e65 7261 746f 722f 7374 6174 7573 5f31  nerator/status_1
-000006a0: 2e70 79da 0763 6865 636b 5f31 0e00 0000  .py..check_1....
-000006b0: 732a 0000 0008 0108 0a08 0208 0102 0114  s*..............
-000006c0: 0102 ff02 0202 fe02 0204 fe04 0402 0102  ................
-000006d0: 0102 0104 fd08 0608 010c 0202 f204 ff72  ...............r
-000006e0: 2600 0000 7a1f 656c 6c69 7074 6963 2070  &...z.elliptic p
-000006f0: 7269 7661 7465 206b 6579 2067 656e 6572  rivate key gener
-00000700: 6174 696f 6e29 0fda 075f 5f64 6f63 5f5f  ation)...__doc__
-00000710: da2f 7265 6379 636c 696e 672e 6d6f 6475  ./recycling.modu
-00000720: 6c65 732e 4545 435f 3434 385f 312e 7072  les.EEC_448_1.pr
-00000730: 6976 6174 655f 6b65 792e 6372 6561 746f  ivate_key.creato
-00000740: 72da 076d 6f64 756c 6573 da09 4545 435f  r..modules..EEC_
-00000750: 3434 385f 3172 2100 0000 da07 6372 6561  448_1r!.....crea
-00000760: 746f 7272 1800 0000 7213 0000 00da 076f  torr....r......o
-00000770: 732e 7061 7468 7202 0000 0072 0300 0000  s.pathr....r....
-00000780: 7204 0000 0072 1a00 0000 7226 0000 00da  r....r....r&....
-00000790: 0663 6865 636b 7372 2400 0000 7224 0000  .checksr$...r$..
-000007a0: 0072 2400 0000 7225 0000 00da 083c 6d6f  .r$...r%.....<mo
-000007b0: 6475 6c65 3e01 0000 0073 1000 0000 0401  dule>....s......
-000007c0: 1e05 0802 1401 0801 0803 0420 08ff       ........... ..
+00000360: 6666 6666 6666 66da 7231 3233 3431 3233  fffffff.r1234123
+00000370: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000380: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000390: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+000003a0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+000003b0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+000003c0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+000003d0: 3431 3233 3431 3233 3431 32da 7230 6631  41234123412.r0f1
+000003e0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000003f0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000400: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000410: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000420: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000430: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000440: 6530 6631 6530 6631 6530 6631 6530 66da  e0f1e0f1e0f1e0f.
+00000450: 7231 3335 3739 3133 3537 3931 3335 3739  r135791357913579
+00000460: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000470: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000480: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000490: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+000004a0: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+000004b0: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+000004c0: 3335 37da 7232 3436 3865 6632 3436 3865  357.r2468ef2468e
+000004d0: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+000004e0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+000004f0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+00000500: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+00000510: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+00000520: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+00000530: 6632 3436 3865 66da 0344 4552 da03 5045  f2468ef..DER..PE
+00000540: 4dda 1545 4543 5f34 3438 5f31 5f70 7269  M..EEC_448_1_pri
+00000550: 7661 7465 5f6b 6579 da01 2eda 0869 6e73  vate_key.....ins
+00000560: 7461 6e63 65da 0673 7472 696e 6729 0b72  tance..string).r
+00000570: 0400 0000 7203 0000 00da 0770 6174 686c  ....r......pathl
+00000580: 6962 da04 5061 7468 da08 5f5f 6669 6c65  ib..Path..__file
+00000590: 5f5f da06 7061 7265 6e74 da07 7265 736f  __..parent..reso
+000005a0: 6c76 65da 1d45 4543 5f34 3438 5f31 5f70  lve..EEC_448_1_p
+000005b0: 7269 7661 7465 5f6b 6579 5f63 7265 6174  rivate_key_creat
+000005c0: 6f72 da06 6372 6561 7465 da02 6f73 da06  or..create..os..
+000005d0: 7265 6d6f 7665 2908 da05 7365 6564 73da  remove)...seeds.
+000005e0: 0766 6f72 6d61 7473 da04 7365 6564 da06  .formats..seed..
+000005f0: 666f 726d 6174 da10 7072 6976 6174 655f  format..private_
+00000600: 6b65 795f 7061 7468 da0b 7072 6976 6174  key_path..privat
+00000610: 655f 6b65 79da 1470 7269 7661 7465 5f6b  e_key..private_k
+00000620: 6579 5f69 6e73 7461 6e63 65da 1270 7269  ey_instance..pri
+00000630: 7661 7465 5f6b 6579 5f73 7472 696e 67a9  vate_key_string.
+00000640: 0072 2400 0000 fa57 2f68 6162 6974 6174  .r$....W/habitat
+00000650: 2f76 656e 7565 732f 7374 6167 6573 2f72  /venues/stages/r
+00000660: 6563 7963 6c69 6e67 2f6d 6978 6573 2f45  ecycling/mixes/E
+00000670: 4543 5f34 3438 5f31 2f5f 7374 6174 7573  EC_448_1/_status
+00000680: 2f73 7461 7475 735f 315f 6765 6e65 7261  /status_1_genera
+00000690: 746f 722f 7374 6174 7573 5f31 2e70 79da  tor/status_1.py.
+000006a0: 0763 6865 636b 5f31 0e00 0000 732a 0000  .check_1....s*..
+000006b0: 0008 0108 0a08 0208 0102 0114 0102 ff02  ................
+000006c0: 0202 fe02 0204 fe04 0402 0102 0102 0104  ................
+000006d0: fd08 0608 010c 0202 f204 ff72 2600 0000  ...........r&...
+000006e0: 7a1f 656c 6c69 7074 6963 2070 7269 7661  z.elliptic priva
+000006f0: 7465 206b 6579 2067 656e 6572 6174 696f  te key generatio
+00000700: 6e29 0fda 075f 5f64 6f63 5f5f da2d 7265  n)...__doc__.-re
+00000710: 6379 636c 696e 672e 6d69 7865 732e 4545  cycling.mixes.EE
+00000720: 435f 3434 385f 312e 7072 6976 6174 655f  C_448_1.private_
+00000730: 6b65 792e 6372 6561 746f 72da 056d 6978  key.creator..mix
+00000740: 6573 da09 4545 435f 3434 385f 3172 2100  es..EEC_448_1r!.
+00000750: 0000 da07 6372 6561 746f 7272 1800 0000  ....creatorr....
+00000760: 7213 0000 00da 076f 732e 7061 7468 7202  r......os.pathr.
+00000770: 0000 0072 0300 0000 7204 0000 0072 1a00  ...r....r....r..
+00000780: 0000 7226 0000 00da 0663 6865 636b 7372  ..r&.....checksr
+00000790: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
+000007a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000007b0: 0073 1000 0000 0401 1e05 0802 1401 0801  .s..............
+000007c0: 0803 0420 08ff                           ... ..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_1_generator/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_1_generator/status_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 '''
-	python3 insurance.proc.py "modules/EEC_448_1/_status/status_1_generator/status_1.py"
+	python3 insurance.proc.py "mixes/EEC_448_1/_status/status_1_generator/status_1.py"
 '''
 
 
-import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
 		
 import pathlib
 from os.path import dirname, join, normpath
 import os
 
 		
 def check_1 ():
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_2_generators/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_2_generators/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2348 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 2c09 0000  o........@@f,...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 2809 0000  o........SQf(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d08 0200 0100 6d05 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 5a0a 6401 6403 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
@@ -20,138 +20,138 @@
 00000130: 0002 0000 000a 0000 0043 0000 0073 3800  .........C...s8.
 00000140: 0000 7a08 7400 a001 7c00 a101 0100 5700  ..z.t...|.....W.
 00000150: 6400 5300 0400 7402 791b 0100 7d01 0100  d.S...t.y...}...
 00000160: 7a07 5700 5900 6400 7d01 7e01 6400 5300  z.W.Y.d.}.~.d.S.
 00000170: 6400 7d01 7e01 7701 7700 2901 4e29 03da  d.}.~.w.w.).N)..
 00000180: 026f 73da 0672 656d 6f76 65da 0945 7863  .os..remove..Exc
 00000190: 6570 7469 6f6e 2902 da04 7061 7468 da01  eption)...path..
-000001a0: 45a9 0072 0a00 0000 fa5a 2f68 6162 6974  E..r.....Z/habit
+000001a0: 45a9 0072 0a00 0000 fa58 2f68 6162 6974  E..r.....X/habit
 000001b0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-000001c0: 2f72 6563 7963 6c69 6e67 2f6d 6f64 756c  /recycling/modul
-000001d0: 6573 2f45 4543 5f34 3438 5f31 2f5f 7374  es/EEC_448_1/_st
-000001e0: 6174 7573 2f73 7461 7475 735f 325f 6765  atus/status_2_ge
-000001f0: 6e65 7261 746f 7273 2f73 7461 7475 735f  nerators/status_
-00000200: 312e 7079 da05 6572 6173 650e 0000 0073  1.py..erase....s
-00000210: 1000 0000 0201 0c01 0405 0efd 0a01 0402  ................
-00000220: 0880 02fd 720c 0000 0063 0000 0000 0000  ....r....c......
-00000230: 0000 0000 0000 0a00 0000 0700 0000 4300  ..............C.
-00000240: 0000 73ba 0000 0067 0064 01a2 017d 0064  ..s....g.d...}.d
-00000250: 0264 0367 027d 017c 0044 005d 507d 027c  .d.g.}.|.D.]P}.|
-00000260: 0144 005d 4b7d 0374 0074 0174 02a0 0374  .D.]K}.t.t.t...t
-00000270: 04a1 016a 05a0 06a1 0064 0483 0283 0164  ...j.....d.....d
-00000280: 0517 007c 0317 007d 0474 0074 0174 02a0  ...|...}.t.t.t..
-00000290: 0374 04a1 016a 05a0 06a1 0064 0683 0283  .t...j.....d....
-000002a0: 0164 0517 007c 0317 007d 0574 077c 0483  .d...|...}.t.|..
-000002b0: 0101 0074 077c 0583 0101 0074 08a0 097c  ...t.|.....t...|
-000002c0: 027c 037c 04a1 037d 0674 0a6a 097c 047c  .|.|...}.t.j.|.|
-000002d0: 057c 0364 078d 037d 077c 0764 0819 007d  .|.d...}.|.d...}
-000002e0: 087c 0764 0919 007d 0974 077c 0483 0101  .|.d...}.t.|....
-000002f0: 0074 077c 0583 0101 0071 0e71 0a64 0a53  .t.|.....q.q.d.S
-00000300: 0029 0b7a 320a 0909 6c65 6e67 7468 2009  .).z2...length .
-00000310: 3d20 3131 3420 0a09 0909 093d 2036 202a  = 114 .....= 6 *
-00000320: 2031 3920 0a09 0909 093d 2032 202a 2033   19 .....= 2 * 3
-00000330: 202a 2031 390a 0929 08da 7234 3938 3638   * 19..)..r49868
-00000340: 3838 6231 3133 3538 6266 3364 3534 3162  88b11358bf3d541b
-00000350: 3431 6565 6135 6461 6563 6531 6336 6566  41eea5daece1c6ef
-00000360: 6636 3431 3330 6134 3566 6338 6239 6361  f64130a45fc8b9ca
-00000370: 3438 6633 6530 6530 3234 3633 6339 3963  48f3e0e02463c99c
-00000380: 3561 6564 6338 6138 3437 3638 3664 3636  5aedc8a847686d66
-00000390: 3962 3764 3534 3763 3138 6665 3434 3866  9b7d547c18fe448f
-000003a0: 6335 3131 3163 6138 3866 3465 38da 7235  c5111ca88f4e8.r5
-000003b0: 3938 3638 3838 6231 3133 3538 6266 3364  986888b11358bf3d
-000003c0: 3534 3162 3431 6565 6135 6461 6563 6531  541b41eea5daece1
-000003d0: 6336 6566 6636 3431 3330 6134 3566 6338  c6eff64130a45fc8
-000003e0: 6239 6361 3438 6633 6530 6530 3234 3633  b9ca48f3e0e02463
-000003f0: 6339 3963 3561 6564 6338 6138 3437 3638  c99c5aedc8a84768
-00000400: 3664 3636 3962 3764 3534 3763 3138 6665  6d669b7d547c18fe
-00000410: 3434 3866 6335 3131 3163 6138 3866 3465  448fc5111ca88f4e
-00000420: 38da 7230 3030 3030 3030 3030 3030 3030  8.r0000000000000
+000001c0: 2f72 6563 7963 6c69 6e67 2f6d 6978 6573  /recycling/mixes
+000001d0: 2f45 4543 5f34 3438 5f31 2f5f 7374 6174  /EEC_448_1/_stat
+000001e0: 7573 2f73 7461 7475 735f 325f 6765 6e65  us/status_2_gene
+000001f0: 7261 746f 7273 2f73 7461 7475 735f 312e  rators/status_1.
+00000200: 7079 da05 6572 6173 650e 0000 0073 1000  py..erase....s..
+00000210: 0000 0201 0c01 0405 0efd 0a01 0402 0880  ................
+00000220: 02fd 720c 0000 0063 0000 0000 0000 0000  ..r....c........
+00000230: 0000 0000 0a00 0000 0700 0000 4300 0000  ............C...
+00000240: 73ba 0000 0067 0064 01a2 017d 0064 0264  s....g.d...}.d.d
+00000250: 0367 027d 017c 0044 005d 507d 027c 0144  .g.}.|.D.]P}.|.D
+00000260: 005d 4b7d 0374 0074 0174 02a0 0374 04a1  .]K}.t.t.t...t..
+00000270: 016a 05a0 06a1 0064 0483 0283 0164 0517  .j.....d.....d..
+00000280: 007c 0317 007d 0474 0074 0174 02a0 0374  .|...}.t.t.t...t
+00000290: 04a1 016a 05a0 06a1 0064 0683 0283 0164  ...j.....d.....d
+000002a0: 0517 007c 0317 007d 0574 077c 0483 0101  ...|...}.t.|....
+000002b0: 0074 077c 0583 0101 0074 08a0 097c 027c  .t.|.....t...|.|
+000002c0: 037c 04a1 037d 0674 0a6a 097c 047c 057c  .|...}.t.j.|.|.|
+000002d0: 0364 078d 037d 077c 0764 0819 007d 087c  .d...}.|.d...}.|
+000002e0: 0764 0919 007d 0974 077c 0483 0101 0074  .d...}.t.|.....t
+000002f0: 077c 0583 0101 0071 0e71 0a64 0a53 0029  .|.....q.q.d.S.)
+00000300: 0b7a 320a 0909 6c65 6e67 7468 2009 3d20  .z2...length .= 
+00000310: 3131 3420 0a09 0909 093d 2036 202a 2031  114 .....= 6 * 1
+00000320: 3920 0a09 0909 093d 2032 202a 2033 202a  9 .....= 2 * 3 *
+00000330: 2031 390a 0929 08da 7234 3938 3638 3838   19..)..r4986888
+00000340: 6231 3133 3538 6266 3364 3534 3162 3431  b11358bf3d541b41
+00000350: 6565 6135 6461 6563 6531 6336 6566 6636  eea5daece1c6eff6
+00000360: 3431 3330 6134 3566 6338 6239 6361 3438  4130a45fc8b9ca48
+00000370: 6633 6530 6530 3234 3633 6339 3963 3561  f3e0e02463c99c5a
+00000380: 6564 6338 6138 3437 3638 3664 3636 3962  edc8a847686d669b
+00000390: 3764 3534 3763 3138 6665 3434 3866 6335  7d547c18fe448fc5
+000003a0: 3131 3163 6138 3866 3465 38da 7235 3938  111ca88f4e8.r598
+000003b0: 3638 3838 6231 3133 3538 6266 3364 3534  6888b11358bf3d54
+000003c0: 3162 3431 6565 6135 6461 6563 6531 6336  1b41eea5daece1c6
+000003d0: 6566 6636 3431 3330 6134 3566 6338 6239  eff64130a45fc8b9
+000003e0: 6361 3438 6633 6530 6530 3234 3633 6339  ca48f3e0e02463c9
+000003f0: 3963 3561 6564 6338 6138 3437 3638 3664  9c5aedc8a847686d
+00000400: 3636 3962 3764 3534 3763 3138 6665 3434  669b7d547c18fe44
+00000410: 3866 6335 3131 3163 6138 3866 3465 38da  8fc5111ca88f4e8.
+00000420: 7230 3030 3030 3030 3030 3030 3030 3030  r000000000000000
 00000430: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000440: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000450: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000460: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000470: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000480: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-00000490: 3030 3030 30da 7266 6666 6666 6666 6666  00000.rfffffffff
+00000490: 3030 30da 7266 6666 6666 6666 6666 6666  000.rfffffffffff
 000004a0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000004b0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000004c0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000004d0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000004e0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000004f0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-00000500: 6666 6666 6666 6666 66da 7231 3233 3431  fffffffff.r12341
-00000510: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000520: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000530: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000540: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000550: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000560: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
-00000570: 3233 3431 3233 3431 3233 3431 32da 7230  2341234123412.r0
-00000580: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-00000590: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005a0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005b0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005c0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005d0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005e0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
-000005f0: 66da 7231 3335 3739 3133 3537 3931 3335  f.r1357913579135
-00000600: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000610: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000620: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000630: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000640: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000650: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000660: 3931 3335 37da 7232 3436 3865 6632 3436  91357.r2468ef246
-00000670: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-00000680: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-00000690: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-000006a0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-000006b0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-000006c0: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-000006d0: 3865 6632 3436 3865 66da 0344 4552 da03  8ef2468ef..DER..
-000006e0: 5045 4dda 1545 4543 5f34 3438 5f31 5f70  PEM..EEC_448_1_p
-000006f0: 7269 7661 7465 5f6b 6579 da01 2eda 1445  rivate_key.....E
-00000700: 4543 5f34 3438 5f31 5f70 7562 6c69 635f  EC_448_1_public_
-00000710: 6b65 7929 03da 1070 7269 7661 7465 5f6b  key)...private_k
-00000720: 6579 5f70 6174 68da 0f70 7562 6c69 635f  ey_path..public_
-00000730: 6b65 795f 7061 7468 da11 7075 626c 6963  key_path..public
-00000740: 5f6b 6579 5f66 6f72 6d61 74da 0869 6e73  _key_format..ins
-00000750: 7461 6e63 65da 0673 7472 696e 674e 290b  tance..stringN).
-00000760: 7204 0000 0072 0300 0000 da07 7061 7468  r....r......path
-00000770: 6c69 62da 0450 6174 68da 085f 5f66 696c  lib..Path..__fil
-00000780: 655f 5fda 0670 6172 656e 74da 0772 6573  e__..parent..res
-00000790: 6f6c 7665 720c 0000 00da 1d45 4543 5f34  olver......EEC_4
-000007a0: 3438 5f31 5f70 7269 7661 7465 5f6b 6579  48_1_private_key
-000007b0: 5f63 7265 6174 6f72 da06 6372 6561 7465  _creator..create
-000007c0: da1c 4545 435f 3434 385f 315f 7075 626c  ..EEC_448_1_publ
-000007d0: 6963 5f6b 6579 5f63 7265 6174 6f72 290a  ic_key_creator).
-000007e0: da05 7365 6564 73da 0766 6f72 6d61 7473  ..seeds..formats
-000007f0: da04 7365 6564 da06 666f 726d 6174 721a  ..seed..formatr.
-00000800: 0000 0072 1b00 0000 da0b 7072 6976 6174  ...r......privat
-00000810: 655f 6b65 79da 0a70 7562 6c69 635f 6b65  e_key..public_ke
-00000820: 79da 1070 7562 6c69 635f 6b65 795f 636c  y..public_key_cl
-00000830: 6173 73da 1170 7562 6c69 635f 6b65 795f  ass..public_key_
-00000840: 7374 7269 6e67 720a 0000 0072 0a00 0000  stringr....r....
-00000850: 720b 0000 00da 0763 6865 636b 5f31 1700  r......check_1..
-00000860: 0000 7328 0000 0008 0608 0a08 0208 0122  ..s(..........."
-00000870: 0122 0108 0208 010e 0204 0102 0102 0102  ."..............
-00000880: 0106 fd08 0508 0108 020a 0102 ef04 ff72  ...............r
-00000890: 2f00 0000 7a2a 656c 6c69 7074 6963 2070  /...z*elliptic p
-000008a0: 7562 6c69 6320 616e 6420 7072 6976 6174  ublic and privat
-000008b0: 6520 6b65 7920 6765 6e65 7261 746f 7273  e key generators
-000008c0: 2913 da07 5f5f 646f 635f 5fda 2f72 6563  )...__doc__./rec
-000008d0: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-000008e0: 4543 5f34 3438 5f31 2e70 7269 7661 7465  EC_448_1.private
-000008f0: 5f6b 6579 2e63 7265 6174 6f72 da07 6d6f  _key.creator..mo
-00000900: 6475 6c65 73da 0945 4543 5f34 3438 5f31  dules..EEC_448_1
-00000910: 722b 0000 00da 0763 7265 6174 6f72 7224  r+.....creatorr$
-00000920: 0000 00da 2e72 6563 7963 6c69 6e67 2e6d  .....recycling.m
-00000930: 6f64 756c 6573 2e45 4543 5f34 3438 5f31  odules.EEC_448_1
-00000940: 2e70 7562 6c69 635f 6b65 792e 6372 6561  .public_key.crea
-00000950: 746f 7272 2c00 0000 7226 0000 0072 1f00  torr,...r&...r..
-00000960: 0000 da07 6f73 2e70 6174 6872 0200 0000  ....os.pathr....
-00000970: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00000980: 0c00 0000 722f 0000 00da 0663 6865 636b  ....r/.....check
-00000990: 7372 0a00 0000 720a 0000 0072 0a00 0000  sr....r....r....
-000009a0: 720b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000009b0: 0000 0073 1400 0000 0402 1e03 1e01 0802  ...s............
-000009c0: 1401 0801 0803 0809 042a 08ff            .........*..
+00000500: 6666 6666 6666 66da 7231 3233 3431 3233  fffffff.r1234123
+00000510: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000520: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000530: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000540: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000550: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000560: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
+00000570: 3431 3233 3431 3233 3431 32da 7230 6631  41234123412.r0f1
+00000580: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+00000590: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000005a0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000005b0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000005c0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000005d0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
+000005e0: 6530 6631 6530 6631 6530 6631 6530 66da  e0f1e0f1e0f1e0f.
+000005f0: 7231 3335 3739 3133 3537 3931 3335 3739  r135791357913579
+00000600: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000610: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000620: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000630: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000640: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000650: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000660: 3335 37da 7232 3436 3865 6632 3436 3865  357.r2468ef2468e
+00000670: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+00000680: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+00000690: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+000006a0: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+000006b0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+000006c0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+000006d0: 6632 3436 3865 66da 0344 4552 da03 5045  f2468ef..DER..PE
+000006e0: 4dda 1545 4543 5f34 3438 5f31 5f70 7269  M..EEC_448_1_pri
+000006f0: 7661 7465 5f6b 6579 da01 2eda 1445 4543  vate_key.....EEC
+00000700: 5f34 3438 5f31 5f70 7562 6c69 635f 6b65  _448_1_public_ke
+00000710: 7929 03da 1070 7269 7661 7465 5f6b 6579  y)...private_key
+00000720: 5f70 6174 68da 0f70 7562 6c69 635f 6b65  _path..public_ke
+00000730: 795f 7061 7468 da11 7075 626c 6963 5f6b  y_path..public_k
+00000740: 6579 5f66 6f72 6d61 74da 0869 6e73 7461  ey_format..insta
+00000750: 6e63 65da 0673 7472 696e 674e 290b 7204  nce..stringN).r.
+00000760: 0000 0072 0300 0000 da07 7061 7468 6c69  ...r......pathli
+00000770: 62da 0450 6174 68da 085f 5f66 696c 655f  b..Path..__file_
+00000780: 5fda 0670 6172 656e 74da 0772 6573 6f6c  _..parent..resol
+00000790: 7665 720c 0000 00da 1d45 4543 5f34 3438  ver......EEC_448
+000007a0: 5f31 5f70 7269 7661 7465 5f6b 6579 5f63  _1_private_key_c
+000007b0: 7265 6174 6f72 da06 6372 6561 7465 da1c  reator..create..
+000007c0: 4545 435f 3434 385f 315f 7075 626c 6963  EEC_448_1_public
+000007d0: 5f6b 6579 5f63 7265 6174 6f72 290a da05  _key_creator)...
+000007e0: 7365 6564 73da 0766 6f72 6d61 7473 da04  seeds..formats..
+000007f0: 7365 6564 da06 666f 726d 6174 721a 0000  seed..formatr...
+00000800: 0072 1b00 0000 da0b 7072 6976 6174 655f  .r......private_
+00000810: 6b65 79da 0a70 7562 6c69 635f 6b65 79da  key..public_key.
+00000820: 1070 7562 6c69 635f 6b65 795f 636c 6173  .public_key_clas
+00000830: 73da 1170 7562 6c69 635f 6b65 795f 7374  s..public_key_st
+00000840: 7269 6e67 720a 0000 0072 0a00 0000 720b  ringr....r....r.
+00000850: 0000 00da 0763 6865 636b 5f31 1700 0000  .....check_1....
+00000860: 7328 0000 0008 0608 0a08 0208 0122 0122  s(..........."."
+00000870: 0108 0208 010e 0204 0102 0102 0102 0106  ................
+00000880: fd08 0508 0108 020a 0102 ef04 ff72 2f00  .............r/.
+00000890: 0000 7a2a 656c 6c69 7074 6963 2070 7562  ..z*elliptic pub
+000008a0: 6c69 6320 616e 6420 7072 6976 6174 6520  lic and private 
+000008b0: 6b65 7920 6765 6e65 7261 746f 7273 2913  key generators).
+000008c0: da07 5f5f 646f 635f 5fda 2d72 6563 7963  ..__doc__.-recyc
+000008d0: 6c69 6e67 2e6d 6978 6573 2e45 4543 5f34  ling.mixes.EEC_4
+000008e0: 3438 5f31 2e70 7269 7661 7465 5f6b 6579  48_1.private_key
+000008f0: 2e63 7265 6174 6f72 da05 6d69 7865 73da  .creator..mixes.
+00000900: 0945 4543 5f34 3438 5f31 722b 0000 00da  .EEC_448_1r+....
+00000910: 0763 7265 6174 6f72 7224 0000 00da 2c72  .creatorr$....,r
+00000920: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00000930: 4543 5f34 3438 5f31 2e70 7562 6c69 635f  EC_448_1.public_
+00000940: 6b65 792e 6372 6561 746f 7272 2c00 0000  key.creatorr,...
+00000950: 7226 0000 0072 1f00 0000 da07 6f73 2e70  r&...r......os.p
+00000960: 6174 6872 0200 0000 7203 0000 0072 0400  athr....r....r..
+00000970: 0000 7205 0000 0072 0c00 0000 722f 0000  ..r....r....r/..
+00000980: 00da 0663 6865 636b 7372 0a00 0000 720a  ...checksr....r.
+00000990: 0000 0072 0a00 0000 720b 0000 00da 083c  ...r....r......<
+000009a0: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+000009b0: 0402 1e03 1e01 0802 1401 0801 0803 0809  ................
+000009c0: 042a 08ff                                .*..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_2_generators/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_2_generators/status_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 '''
 	python3 insurance.proc.py "_status/guarantees/status_2_generators/status_1.py"
 '''
-import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
-import recycling.modules.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
+import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+import recycling.mixes.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
 
 import pathlib
 from os.path import dirname, join, normpath
 import os
 
 
 def erase (path):
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2970 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9a0b 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 920b 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d08 0200 0100 6d05 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
@@ -23,161 +23,160 @@
 00000160: 0000 0000 0000 0200 0000 0a00 0000 4300  ..............C.
 00000170: 0000 7338 0000 007a 0874 00a0 017c 00a1  ..s8...z.t...|..
 00000180: 0101 0057 0064 0053 0004 0074 0279 1b01  ...W.d.S...t.y..
 00000190: 007d 0101 007a 0757 0059 0064 007d 017e  .}...z.W.Y.d.}.~
 000001a0: 0164 0053 0064 007d 017e 0177 0177 0029  .d.S.d.}.~.w.w.)
 000001b0: 014e 2903 da02 6f73 da06 7265 6d6f 7665  .N)...os..remove
 000001c0: da09 4578 6365 7074 696f 6e29 02da 0470  ..Exception)...p
-000001d0: 6174 68da 0145 a900 720a 0000 00fa 5f2f  ath..E..r....._/
+000001d0: 6174 68da 0145 a900 720a 0000 00fa 5d2f  ath..E..r.....]/
 000001e0: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
 000001f0: 7461 6765 732f 7265 6379 636c 696e 672f  tages/recycling/
-00000200: 6d6f 6475 6c65 732f 4545 435f 3434 385f  modules/EEC_448_
-00000210: 312f 5f73 7461 7475 732f 7374 6174 7573  1/_status/status
-00000220: 5f33 5f73 6967 6e5f 616e 645f 7665 7269  _3_sign_and_veri
-00000230: 6679 2f73 7461 7475 735f 312e 7079 da05  fy/status_1.py..
-00000240: 6572 6173 6513 0000 0073 1000 0000 0201  erase....s......
-00000250: 0c01 0405 0efd 0a01 0402 0880 02fd 720c  ..............r.
-00000260: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000270: 1000 0000 0700 0000 4300 0000 7302 0100  ........C...s...
-00000280: 0067 0064 01a2 017d 0064 0264 0367 027d  .g.d...}.d.d.g.}
-00000290: 017c 0044 005d 747d 027c 0144 005d 6f7d  .|.D.]t}.|.D.]o}
-000002a0: 0374 0074 0174 02a0 0374 04a1 016a 05a0  .t.t.t...t...j..
-000002b0: 06a1 0064 0483 0283 0164 0517 007c 0317  ...d.....d...|..
-000002c0: 007d 0474 0074 0174 02a0 0374 04a1 016a  .}.t.t.t...t...j
-000002d0: 05a0 06a1 0064 0683 0283 0164 0517 007c  .....d.....d...|
-000002e0: 0317 007d 0574 077c 0483 0101 0074 077c  ...}.t.|.....t.|
-000002f0: 0583 0101 0074 08a0 097c 027c 037c 04a1  .....t...|.|.|..
-00000300: 037d 067c 0664 0719 007d 077c 0664 0819  .}.|.d...}.|.d..
-00000310: 007d 0874 0a6a 097c 047c 057c 0364 098d  .}.t.j.|.|.|.d..
-00000320: 037d 097c 0964 0719 007d 0a7c 0964 0819  .}.|.d...}.|.d..
-00000330: 007d 0b64 0a7d 0c74 0b6a 0c7c 047c 0c64  .}.d.}.t.j.|.|.d
-00000340: 0b8d 027d 0d7c 0d6a 0d7d 0e74 0e6a 0c7c  ...}.|.j.}.t.j.|
-00000350: 057c 0e7c 0c64 0c8d 037d 0f7c 0f64 0d6b  .|.|.d...}.|.d.k
-00000360: 0273 754a 007c 0f83 0182 0174 077c 0483  .suJ.|.....t.|..
-00000370: 0101 0074 077c 0583 0101 0071 0e71 0a64  ...t.|.....q.q.d
-00000380: 0e53 0029 0f7a 320a 0909 6c65 6e67 7468  .S.).z2...length
-00000390: 2009 3d20 3131 3420 0a09 0909 093d 2036   .= 114 .....= 6
-000003a0: 202a 2031 3920 0a09 0909 093d 2032 202a   * 19 .....= 2 *
-000003b0: 2033 202a 2031 390a 0929 08da 7234 3938   3 * 19..)..r498
-000003c0: 3638 3838 6231 3133 3538 6266 3364 3534  6888b11358bf3d54
-000003d0: 3162 3431 6565 6135 6461 6563 6531 6336  1b41eea5daece1c6
-000003e0: 6566 6636 3431 3330 6134 3566 6338 6239  eff64130a45fc8b9
-000003f0: 6361 3438 6633 6530 6530 3234 3633 6339  ca48f3e0e02463c9
-00000400: 3963 3561 6564 6338 6138 3437 3638 3664  9c5aedc8a847686d
-00000410: 3636 3962 3764 3534 3763 3138 6665 3434  669b7d547c18fe44
-00000420: 3866 6335 3131 3163 6138 3866 3465 38da  8fc5111ca88f4e8.
-00000430: 7235 3938 3638 3838 6231 3133 3538 6266  r5986888b11358bf
-00000440: 3364 3534 3162 3431 6565 6135 6461 6563  3d541b41eea5daec
-00000450: 6531 6336 6566 6636 3431 3330 6134 3566  e1c6eff64130a45f
-00000460: 6338 6239 6361 3438 6633 6530 6530 3234  c8b9ca48f3e0e024
-00000470: 3633 6339 3963 3561 6564 6338 6138 3437  63c99c5aedc8a847
-00000480: 3638 3664 3636 3962 3764 3534 3763 3138  686d669b7d547c18
-00000490: 6665 3434 3866 6335 3131 3163 6138 3866  fe448fc5111ca88f
-000004a0: 3465 38da 7230 3030 3030 3030 3030 3030  4e8.r00000000000
+00000200: 6d69 7865 732f 4545 435f 3434 385f 312f  mixes/EEC_448_1/
+00000210: 5f73 7461 7475 732f 7374 6174 7573 5f33  _status/status_3
+00000220: 5f73 6967 6e5f 616e 645f 7665 7269 6679  _sign_and_verify
+00000230: 2f73 7461 7475 735f 312e 7079 da05 6572  /status_1.py..er
+00000240: 6173 6513 0000 0073 1000 0000 0201 0c01  ase....s........
+00000250: 0405 0efd 0a01 0402 0880 02fd 720c 0000  ............r...
+00000260: 0063 0000 0000 0000 0000 0000 0000 1000  .c..............
+00000270: 0000 0700 0000 4300 0000 7302 0100 0067  ......C...s....g
+00000280: 0064 01a2 017d 0064 0264 0367 027d 017c  .d...}.d.d.g.}.|
+00000290: 0044 005d 747d 027c 0144 005d 6f7d 0374  .D.]t}.|.D.]o}.t
+000002a0: 0074 0174 02a0 0374 04a1 016a 05a0 06a1  .t.t...t...j....
+000002b0: 0064 0483 0283 0164 0517 007c 0317 007d  .d.....d...|...}
+000002c0: 0474 0074 0174 02a0 0374 04a1 016a 05a0  .t.t.t...t...j..
+000002d0: 06a1 0064 0683 0283 0164 0517 007c 0317  ...d.....d...|..
+000002e0: 007d 0574 077c 0483 0101 0074 077c 0583  .}.t.|.....t.|..
+000002f0: 0101 0074 08a0 097c 027c 037c 04a1 037d  ...t...|.|.|...}
+00000300: 067c 0664 0719 007d 077c 0664 0819 007d  .|.d...}.|.d...}
+00000310: 0874 0a6a 097c 047c 057c 0364 098d 037d  .t.j.|.|.|.d...}
+00000320: 097c 0964 0719 007d 0a7c 0964 0819 007d  .|.d...}.|.d...}
+00000330: 0b64 0a7d 0c74 0b6a 0c7c 047c 0c64 0b8d  .d.}.t.j.|.|.d..
+00000340: 027d 0d7c 0d6a 0d7d 0e74 0e6a 0c7c 057c  .}.|.j.}.t.j.|.|
+00000350: 0e7c 0c64 0c8d 037d 0f7c 0f64 0d6b 0273  .|.d...}.|.d.k.s
+00000360: 754a 007c 0f83 0182 0174 077c 0483 0101  uJ.|.....t.|....
+00000370: 0074 077c 0583 0101 0071 0e71 0a64 0e53  .t.|.....q.q.d.S
+00000380: 0029 0f7a 320a 0909 6c65 6e67 7468 2009  .).z2...length .
+00000390: 3d20 3131 3420 0a09 0909 093d 2036 202a  = 114 .....= 6 *
+000003a0: 2031 3920 0a09 0909 093d 2032 202a 2033   19 .....= 2 * 3
+000003b0: 202a 2031 390a 0929 08da 7234 3938 3638   * 19..)..r49868
+000003c0: 3838 6231 3133 3538 6266 3364 3534 3162  88b11358bf3d541b
+000003d0: 3431 6565 6135 6461 6563 6531 6336 6566  41eea5daece1c6ef
+000003e0: 6636 3431 3330 6134 3566 6338 6239 6361  f64130a45fc8b9ca
+000003f0: 3438 6633 6530 6530 3234 3633 6339 3963  48f3e0e02463c99c
+00000400: 3561 6564 6338 6138 3437 3638 3664 3636  5aedc8a847686d66
+00000410: 3962 3764 3534 3763 3138 6665 3434 3866  9b7d547c18fe448f
+00000420: 6335 3131 3163 6138 3866 3465 38da 7235  c5111ca88f4e8.r5
+00000430: 3938 3638 3838 6231 3133 3538 6266 3364  986888b11358bf3d
+00000440: 3534 3162 3431 6565 6135 6461 6563 6531  541b41eea5daece1
+00000450: 6336 6566 6636 3431 3330 6134 3566 6338  c6eff64130a45fc8
+00000460: 6239 6361 3438 6633 6530 6530 3234 3633  b9ca48f3e0e02463
+00000470: 6339 3963 3561 6564 6338 6138 3437 3638  c99c5aedc8a84768
+00000480: 3664 3636 3962 3764 3534 3763 3138 6665  6d669b7d547c18fe
+00000490: 3434 3866 6335 3131 3163 6138 3866 3465  448fc5111ca88f4e
+000004a0: 38da 7230 3030 3030 3030 3030 3030 3030  8.r0000000000000
 000004b0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000004c0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000004d0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000004e0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 000004f0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000500: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-00000510: 3030 3030 3030 30da 7266 6666 6666 6666  0000000.rfffffff
+00000510: 3030 3030 30da 7266 6666 6666 6666 6666  00000.rfffffffff
 00000520: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000530: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000540: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000550: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000560: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000570: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-00000580: 6666 6666 6666 6666 6666 66da 7231 3233  fffffffffff.r123
-00000590: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005a0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005b0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005c0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005d0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005e0: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-000005f0: 3431 3233 3431 3233 3431 3233 3431 32da  412341234123412.
-00000600: 7230 6631 6530 6631 6530 6631 6530 6631  r0f1e0f1e0f1e0f1
-00000610: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000620: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000630: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000640: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000650: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000660: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000670: 6530 66da 7231 3335 3739 3133 3537 3931  e0f.r13579135791
-00000680: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000690: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-000006a0: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-000006b0: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-000006c0: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-000006d0: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-000006e0: 3537 3931 3335 37da 7232 3436 3865 6632  5791357.r2468ef2
-000006f0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-00000700: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-00000710: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-00000720: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-00000730: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-00000740: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-00000750: 3436 3865 6632 3436 3865 66da 0344 4552  468ef2468ef..DER
-00000760: da03 5045 4dda 1545 4543 5f34 3438 5f31  ..PEM..EEC_448_1
-00000770: 5f70 7269 7661 7465 5f6b 6579 da01 2eda  _private_key....
-00000780: 1445 4543 5f34 3438 5f31 5f70 7562 6c69  .EEC_448_1_publi
-00000790: 635f 6b65 79da 0869 6e73 7461 6e63 65da  c_key..instance.
-000007a0: 0673 7472 696e 6729 03da 1070 7269 7661  .string)...priva
-000007b0: 7465 5f6b 6579 5f70 6174 68da 0f70 7562  te_key_path..pub
-000007c0: 6c69 635f 6b65 795f 7061 7468 da11 7075  lic_key_path..pu
-000007d0: 626c 6963 5f6b 6579 5f66 6f72 6d61 7473  blic_key_formats
-000007e0: 0200 0000 7b7d 2902 721c 0000 00da 0e75  ....{}).r......u
-000007f0: 6e73 6967 6e65 645f 6279 7465 7329 0372  nsigned_bytes).r
-00000800: 1d00 0000 da0c 7369 676e 6564 5f62 7974  ......signed_byt
-00000810: 6573 721f 0000 0054 4e29 0f72 0400 0000  esr....TN).r....
-00000820: 7203 0000 00da 0770 6174 686c 6962 da04  r......pathlib..
-00000830: 5061 7468 da08 5f5f 6669 6c65 5f5f da06  Path..__file__..
-00000840: 7061 7265 6e74 da07 7265 736f 6c76 6572  parent..resolver
-00000850: 0c00 0000 da1d 4545 435f 3434 385f 315f  ......EEC_448_1_
-00000860: 7072 6976 6174 655f 6b65 795f 6372 6561  private_key_crea
-00000870: 746f 72da 0663 7265 6174 65da 1c45 4543  tor..create..EEC
-00000880: 5f34 3438 5f31 5f70 7562 6c69 635f 6b65  _448_1_public_ke
-00000890: 795f 6372 6561 746f 72da 0473 6967 6eda  y_creator..sign.
-000008a0: 0573 7461 7274 da05 6279 7465 73da 0676  .start..bytes..v
-000008b0: 6572 6966 7929 10da 0573 6565 6473 da07  erify)...seeds..
-000008c0: 666f 726d 6174 73da 0473 6565 64da 0666  formats..seed..f
-000008d0: 6f72 6d61 7472 1c00 0000 721d 0000 00da  ormatr....r.....
-000008e0: 0b70 7269 7661 7465 5f6b 6579 da14 7072  .private_key..pr
-000008f0: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
-00000900: 6365 da12 7072 6976 6174 655f 6b65 795f  ce..private_key_
-00000910: 7374 7269 6e67 da0a 7075 626c 6963 5f6b  string..public_k
-00000920: 6579 da13 7075 626c 6963 5f6b 6579 5f69  ey..public_key_i
-00000930: 6e73 7461 6e63 65da 1170 7562 6c69 635f  nstance..public_
-00000940: 6b65 795f 7374 7269 6e67 721f 0000 00da  key_stringr.....
-00000950: 0673 6967 6e65 6472 2000 0000 da13 7665  .signedr .....ve
-00000960: 7269 6669 6361 7469 6f6e 5f73 7461 7475  rification_statu
-00000970: 7372 0a00 0000 720a 0000 0072 0b00 0000  sr....r....r....
-00000980: da07 6368 6563 6b5f 311c 0000 0073 4400  ..check_1....sD.
-00000990: 0000 0806 080a 0802 0801 2201 2201 0802  .........."."...
-000009a0: 0801 0e02 0801 0801 0403 0201 0201 0201  ................
-000009b0: 06fd 0805 0801 0403 0402 0201 0201 06fe  ................
-000009c0: 0605 0402 0201 0202 0201 06fc 1007 0802  ................
-000009d0: 0a01 02d8 04ff 7239 0000 007a 2a65 6c6c  ......r9...z*ell
-000009e0: 6970 7469 6320 7075 626c 6963 2061 6e64  iptic public and
-000009f0: 2070 7269 7661 7465 206b 6579 2067 656e   private key gen
-00000a00: 6572 6174 6f72 7329 17da 075f 5f64 6f63  erators)...__doc
-00000a10: 5f5f da2f 7265 6379 636c 696e 672e 6d6f  __./recycling.mo
-00000a20: 6475 6c65 732e 4545 435f 3434 385f 312e  dules.EEC_448_1.
-00000a30: 7072 6976 6174 655f 6b65 792e 6372 6561  private_key.crea
-00000a40: 746f 72da 076d 6f64 756c 6573 da09 4545  tor..modules..EE
-00000a50: 435f 3434 385f 3172 3100 0000 da07 6372  C_448_1r1.....cr
-00000a60: 6561 746f 7272 2600 0000 da2e 7265 6379  eatorr&.....recy
-00000a70: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000a80: 435f 3434 385f 312e 7075 626c 6963 5f6b  C_448_1.public_k
-00000a90: 6579 2e63 7265 6174 6f72 7234 0000 0072  ey.creatorr4...r
-00000aa0: 2800 0000 da20 7265 6379 636c 696e 672e  (.... recycling.
-00000ab0: 6d6f 6475 6c65 732e 4545 435f 3434 385f  modules.EEC_448_
-00000ac0: 312e 7369 676e 7229 0000 00da 2272 6563  1.signr)...."rec
-00000ad0: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-00000ae0: 4543 5f34 3438 5f31 2e76 6572 6966 7972  EC_448_1.verifyr
-00000af0: 2c00 0000 7221 0000 00da 076f 732e 7061  ,...r!.....os.pa
-00000b00: 7468 7202 0000 0072 0300 0000 7204 0000  thr....r....r...
-00000b10: 0072 0500 0000 720c 0000 0072 3900 0000  .r....r....r9...
-00000b20: da06 6368 6563 6b73 720a 0000 0072 0a00  ..checksr....r..
-00000b30: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
-00000b40: 6f64 756c 653e 0100 0000 7318 0000 0004  odule>....s.....
-00000b50: 031e 051e 0118 0118 0108 0214 0108 0108  ................
-00000b60: 0308 0904 4108 ff                        ....A..
+00000580: 6666 6666 6666 6666 66da 7231 3233 3431  fffffffff.r12341
+00000590: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005a0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005b0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005c0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005d0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005e0: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+000005f0: 3233 3431 3233 3431 3233 3431 32da 7230  2341234123412.r0
+00000600: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000610: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000620: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000630: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000640: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000650: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000660: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000670: 66da 7231 3335 3739 3133 3537 3931 3335  f.r1357913579135
+00000680: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000690: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+000006a0: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+000006b0: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+000006c0: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+000006d0: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+000006e0: 3931 3335 37da 7232 3436 3865 6632 3436  91357.r2468ef246
+000006f0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+00000700: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+00000710: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+00000720: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+00000730: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+00000740: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+00000750: 3865 6632 3436 3865 66da 0344 4552 da03  8ef2468ef..DER..
+00000760: 5045 4dda 1545 4543 5f34 3438 5f31 5f70  PEM..EEC_448_1_p
+00000770: 7269 7661 7465 5f6b 6579 da01 2eda 1445  rivate_key.....E
+00000780: 4543 5f34 3438 5f31 5f70 7562 6c69 635f  EC_448_1_public_
+00000790: 6b65 79da 0869 6e73 7461 6e63 65da 0673  key..instance..s
+000007a0: 7472 696e 6729 03da 1070 7269 7661 7465  tring)...private
+000007b0: 5f6b 6579 5f70 6174 68da 0f70 7562 6c69  _key_path..publi
+000007c0: 635f 6b65 795f 7061 7468 da11 7075 626c  c_key_path..publ
+000007d0: 6963 5f6b 6579 5f66 6f72 6d61 7473 0200  ic_key_formats..
+000007e0: 0000 7b7d 2902 721c 0000 00da 0e75 6e73  ..{}).r......uns
+000007f0: 6967 6e65 645f 6279 7465 7329 0372 1d00  igned_bytes).r..
+00000800: 0000 da0c 7369 676e 6564 5f62 7974 6573  ....signed_bytes
+00000810: 721f 0000 0054 4e29 0f72 0400 0000 7203  r....TN).r....r.
+00000820: 0000 00da 0770 6174 686c 6962 da04 5061  .....pathlib..Pa
+00000830: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
+00000840: 7265 6e74 da07 7265 736f 6c76 6572 0c00  rent..resolver..
+00000850: 0000 da1d 4545 435f 3434 385f 315f 7072  ....EEC_448_1_pr
+00000860: 6976 6174 655f 6b65 795f 6372 6561 746f  ivate_key_creato
+00000870: 72da 0663 7265 6174 65da 1c45 4543 5f34  r..create..EEC_4
+00000880: 3438 5f31 5f70 7562 6c69 635f 6b65 795f  48_1_public_key_
+00000890: 6372 6561 746f 72da 0473 6967 6eda 0573  creator..sign..s
+000008a0: 7461 7274 da05 6279 7465 73da 0676 6572  tart..bytes..ver
+000008b0: 6966 7929 10da 0573 6565 6473 da07 666f  ify)...seeds..fo
+000008c0: 726d 6174 73da 0473 6565 64da 0666 6f72  rmats..seed..for
+000008d0: 6d61 7472 1c00 0000 721d 0000 00da 0b70  matr....r......p
+000008e0: 7269 7661 7465 5f6b 6579 da14 7072 6976  rivate_key..priv
+000008f0: 6174 655f 6b65 795f 696e 7374 616e 6365  ate_key_instance
+00000900: da12 7072 6976 6174 655f 6b65 795f 7374  ..private_key_st
+00000910: 7269 6e67 da0a 7075 626c 6963 5f6b 6579  ring..public_key
+00000920: da13 7075 626c 6963 5f6b 6579 5f69 6e73  ..public_key_ins
+00000930: 7461 6e63 65da 1170 7562 6c69 635f 6b65  tance..public_ke
+00000940: 795f 7374 7269 6e67 721f 0000 00da 0673  y_stringr......s
+00000950: 6967 6e65 6472 2000 0000 da13 7665 7269  ignedr .....veri
+00000960: 6669 6361 7469 6f6e 5f73 7461 7475 7372  fication_statusr
+00000970: 0a00 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
+00000980: 6368 6563 6b5f 311c 0000 0073 4400 0000  check_1....sD...
+00000990: 0806 080a 0802 0801 2201 2201 0802 0801  ........".".....
+000009a0: 0e02 0801 0801 0403 0201 0201 0201 06fd  ................
+000009b0: 0805 0801 0403 0402 0201 0201 06fe 0605  ................
+000009c0: 0402 0201 0202 0201 06fc 1007 0802 0a01  ................
+000009d0: 02d8 04ff 7239 0000 007a 2a65 6c6c 6970  ....r9...z*ellip
+000009e0: 7469 6320 7075 626c 6963 2061 6e64 2070  tic public and p
+000009f0: 7269 7661 7465 206b 6579 2067 656e 6572  rivate key gener
+00000a00: 6174 6f72 7329 17da 075f 5f64 6f63 5f5f  ators)...__doc__
+00000a10: da2d 7265 6379 636c 696e 672e 6d69 7865  .-recycling.mixe
+00000a20: 732e 4545 435f 3434 385f 312e 7072 6976  s.EEC_448_1.priv
+00000a30: 6174 655f 6b65 792e 6372 6561 746f 72da  ate_key.creator.
+00000a40: 056d 6978 6573 da09 4545 435f 3434 385f  .mixes..EEC_448_
+00000a50: 3172 3100 0000 da07 6372 6561 746f 7272  1r1.....creatorr
+00000a60: 2600 0000 da2c 7265 6379 636c 696e 672e  &....,recycling.
+00000a70: 6d69 7865 732e 4545 435f 3434 385f 312e  mixes.EEC_448_1.
+00000a80: 7075 626c 6963 5f6b 6579 2e63 7265 6174  public_key.creat
+00000a90: 6f72 7234 0000 0072 2800 0000 da1e 7265  orr4...r(.....re
+00000aa0: 6379 636c 696e 672e 6d69 7865 732e 4545  cycling.mixes.EE
+00000ab0: 435f 3434 385f 312e 7369 676e 7229 0000  C_448_1.signr)..
+00000ac0: 00da 2072 6563 7963 6c69 6e67 2e6d 6978  .. recycling.mix
+00000ad0: 6573 2e45 4543 5f34 3438 5f31 2e76 6572  es.EEC_448_1.ver
+00000ae0: 6966 7972 2c00 0000 7221 0000 00da 076f  ifyr,...r!.....o
+00000af0: 732e 7061 7468 7202 0000 0072 0300 0000  s.pathr....r....
+00000b00: 7204 0000 0072 0500 0000 720c 0000 0072  r....r....r....r
+00000b10: 3900 0000 da06 6368 6563 6b73 720a 0000  9.....checksr...
+00000b20: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000b30: da08 3c6d 6f64 756c 653e 0100 0000 7318  ..<module>....s.
+00000b40: 0000 0004 031e 051e 0118 0118 0108 0214  ................
+00000b50: 0108 0108 0308 0904 4108 ff              ........A..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/_status/status_3_sign_and_verify/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/_status/status_3_sign_and_verify/status_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 
 '''
 	python3 insurance.proc.py "_status/guarantees/status_3_sign_and_verify/status_1.py"
 '''
 
 
-import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
-import recycling.modules.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
-import recycling.modules.EEC_448_1.sign as sign
-import recycling.modules.EEC_448_1.verify as verify
+import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+import recycling.mixes.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
+import recycling.mixes.EEC_448_1.sign as sign
+import recycling.mixes.EEC_448_1.verify as verify
 	
 import pathlib
 from os.path import dirname, join, normpath
 import os
 
 
 def erase (path):
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/module.s.HTML` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/module.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/BUILD.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/BUILD.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/CREATE.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/CREATE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/READ.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/READ.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/SCAN.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/creator.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/creator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2635 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 4b0a 0000  o........@@fK...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 490a 0000  o........SQfI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a02  Z.....d.d.l.m.Z.
 00000040: 0100 6401 6403 6c03 5a04 6404 6405 8400  ..d.d.l.Z.d.d...
 00000050: 5a05 0906 6409 6407 6408 8401 5a06 6403  Z...d.d.d...Z.d.
-00000060: 5300 290a 615d 0200 000a 0923 0a09 2309  S.).a].....#..#.
+00000060: 5300 290a 615b 0200 000a 0923 0a09 2309  S.).a[.....#..#.
 00000070: 7772 6974 6520 7072 6976 6174 6520 6b65  write private ke
 00000080: 7920 746f 2070 6174 680a 0923 0a09 0a09  y to path..#....
 00000090: 0a09 230a 0923 0941 4243 4445 4647 4849  ..#..#.ABCDEFGHI
 000000a0: 4a4b 4c4d 0a09 2309 4e4f 5051 5253 5455  JKLM..#.NOPQRSTU
 000000b0: 5657 5859 5a0a 0923 0a09 2309 4142 4344  VWXYZ..#..#.ABCD
 000000c0: 4546 4748 494a 4b4c 4d20 4e4f 5020 2d3e  EFGHIJKLM NOP ->
 000000d0: 2075 7369 6e67 2074 6865 7365 2031 3620   using these 16 
@@ -23,94 +23,93 @@
 00000160: 6663 3862 3963 6134 3866 3365 3065 3032  fc8b9ca48f3e0e02
 00000170: 3436 3363 3939 6335 6165 6463 3861 3834  463c99c5aedc8a84
 00000180: 3736 3836 6436 3639 6237 6435 3437 6331  7686d669b7d547c1
 00000190: 3866 6534 3438 6663 3531 3131 6361 3838  8fe448fc5111ca88
 000001a0: 6634 6538 220a 0966 6f72 6d61 7420 3d20  f4e8"..format = 
 000001b0: 2250 454d 220a 0970 6174 6820 3d20 2222  "PEM"..path = ""
 000001c0: 0a09 0a09 696d 706f 7274 2072 6563 7963  ....import recyc
-000001d0: 6c69 6e67 2e6d 6f64 756c 6573 2e45 4543  ling.modules.EEC
-000001e0: 5f34 3438 5f31 2e70 7269 7661 7465 5f6b  _448_1.private_k
-000001f0: 6579 2e63 7265 6174 6f72 2061 7320 4545  ey.creator as EE
-00000200: 435f 3434 385f 315f 7072 6976 6174 655f  C_448_1_private_
-00000210: 6b65 795f 6372 6561 746f 720a 0970 7269  key_creator..pri
-00000220: 7661 7465 5f6b 6579 203d 2045 4543 5f34  vate_key = EEC_4
-00000230: 3438 5f31 5f70 7269 7661 7465 5f6b 6579  48_1_private_key
-00000240: 5f63 7265 6174 6f72 2e63 7265 6174 6520  _creator.create 
-00000250: 2873 6565 642c 2066 6f72 6d61 742c 2070  (seed, format, p
-00000260: 6174 6829 0a09 7072 6976 6174 655f 6b65  ath)..private_ke
-00000270: 795f 696e 7374 616e 6365 203d 2070 7269  y_instance = pri
-00000280: 7661 7465 5f6b 6579 205b 2269 6e73 7461  vate_key ["insta
-00000290: 6e63 6522 5d0a 0970 7269 7661 7465 5f6b  nce"]..private_k
-000002a0: 6579 5f73 7472 696e 6720 3d20 7072 6976  ey_string = priv
-000002b0: 6174 655f 6b65 7920 5b22 7374 7269 6e67  ate_key ["string
-000002c0: 225d 0a09 090a e900 0000 0029 01da 0645  "].........)...E
-000002d0: 6363 4b65 794e 6303 0000 0000 0000 0000  ccKeyNc.........
-000002e0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-000002f0: 6a00 0000 7400 6a01 a002 7c00 a101 720e  j...t.j...|...r.
-00000300: 7403 6401 7c00 9b00 6402 9d03 8301 8201  t.d.|...d.......
-00000310: 7c02 6403 6b02 7218 7404 7c00 6404 8302  |.d.k.r.t.|.d...
-00000320: 7d03 6e12 7c02 6405 7600 7222 7404 7c00  }.n.|.d.v.r"t.|.
-00000330: 6406 8302 7d03 6e08 7403 6407 7c02 9b00  d...}.n.t.d.|...
-00000340: 6408 9d03 8301 8201 7c03 a005 7c01 a101  d.......|...|...
-00000350: 0100 7c03 a006 a100 0100 6409 5300 290a  ..|.......d.S.).
-00000360: 4e7a 3054 6865 2070 6174 6820 666f 7220  Nz0The path for 
-00000370: 7468 6520 7072 6976 6174 655f 6b65 7920  the private_key 
-00000380: 6973 206e 6f74 2061 7661 696c 6162 6c65  is not available
-00000390: 2e20 27fa 0127 da03 4445 52da 0277 6229  . '..'..DER..wb)
-000003a0: 02da 0350 454d da0b 6865 7861 6465 6369  ...PEM..hexadeci
-000003b0: 6d61 6cda 0177 7a08 666f 726d 6174 2027  mal..wz.format '
-000003c0: 7a18 2720 7761 7320 6e6f 7420 6163 636f  z.' was not acco
-000003d0: 756e 7465 6420 666f 722e 5429 07da 026f  unted for.T)...o
-000003e0: 73da 0470 6174 68da 0665 7869 7374 73da  s..path..exists.
-000003f0: 0945 7863 6570 7469 6f6e da04 6f70 656e  .Exception..open
-00000400: da05 7772 6974 65da 0563 6c6f 7365 2904  ..write..close).
-00000410: 720a 0000 00da 1270 7269 7661 7465 5f6b  r......private_k
-00000420: 6579 5f73 7472 696e 67da 0666 6f72 6d61  ey_string..forma
-00000430: 74da 0166 a900 7213 0000 00fa 492f 6861  t..f..r.....I/ha
-00000440: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
-00000450: 6765 732f 7265 6379 636c 696e 672f 6d6f  ges/recycling/mo
-00000460: 6475 6c65 732f 4545 435f 3434 385f 312f  dules/EEC_448_1/
-00000470: 7072 6976 6174 655f 6b65 792f 6372 6561  private_key/crea
-00000480: 746f 722e 7079 da11 7772 6974 655f 7072  tor.py..write_pr
-00000490: 6976 6174 655f 6b65 792e 0000 0073 1400  ivate_key....s..
-000004a0: 0000 0c01 1001 0802 0c01 0801 0c01 1002  ................
-000004b0: 0a02 0801 0402 7215 0000 00da 0063 0300  ......r......c..
-000004c0: 0000 0000 0000 0000 0000 0700 0000 0500  ................
-000004d0: 0000 4300 0000 73a8 0000 0074 007c 0283  ..C...s....t.|..
-000004e0: 0164 016b 0573 084a 0082 0174 007c 0083  .d.k.s.J...t.|..
-000004f0: 0164 026b 0273 104a 0082 017c 0164 036b  .d.k.s.J...|.d.k
-00000500: 0272 1764 047d 036e 027c 017d 0374 0164  .r.d.}.n.|.}.t.d
-00000510: 0574 02a0 037c 00a1 0164 068d 027d 047c  .t...|...d...}.|
-00000520: 046a 047c 0364 078d 017d 057c 0164 036b  .j.|.d...}.|.d.k
-00000530: 0272 497c 05a0 05a1 00a0 06a1 007d 0674  .rI|.........}.t
-00000540: 007c 0683 0164 086b 0273 3e4a 0074 007c  .|...d.k.s>J.t.|
-00000550: 0683 0183 0182 0174 02a0 037c 06a1 017c  .......t...|...|
-00000560: 056b 0273 474a 0082 017c 067d 0574 077c  .k.sGJ...|.}.t.|
-00000570: 027c 057c 0183 0301 007c 047c 0564 099c  .|.|.....|.|.d..
-00000580: 0253 0029 0a4e e901 0000 00e9 7200 0000  .S.).N......r...
-00000590: 7207 0000 0072 0400 0000 da05 4564 3434  r....r......Ed44
-000005a0: 3829 02da 0563 7572 7665 da04 7365 6564  8)...curve..seed
-000005b0: 2901 7211 0000 00e9 9200 0000 2902 da08  ).r.........)...
-000005c0: 696e 7374 616e 6365 da06 7374 7269 6e67  instance..string
-000005d0: 2908 da03 6c65 6e72 0200 0000 da05 6279  )...lenr......by
-000005e0: 7465 73da 0766 726f 6d68 6578 da0a 6578  tes..fromhex..ex
-000005f0: 706f 7274 5f6b 6579 da03 6865 78da 0575  port_key..hex..u
-00000600: 7070 6572 7215 0000 0029 0772 1b00 0000  pperr....).r....
-00000610: 7211 0000 0072 0a00 0000 da0d 6578 706f  r....r......expo
-00000620: 7274 5f66 6f72 6d61 74da 1470 7269 7661  rt_format..priva
-00000630: 7465 5f6b 6579 5f69 6e73 7461 6e63 6572  te_key_instancer
-00000640: 1000 0000 da1e 7072 6976 6174 655f 6b65  ......private_ke
-00000650: 795f 6865 7861 6465 6369 6d61 6c5f 7374  y_hexadecimal_st
-00000660: 7269 6e67 7213 0000 0072 1300 0000 7214  ringr....r....r.
-00000670: 0000 00da 0663 7265 6174 653f 0000 0073  .....create?...s
-00000680: 2e00 0000 1006 1001 0802 0601 0402 0202  ................
-00000690: 0201 0801 06fe 0404 0201 06ff 0804 0c07  ................
-000006a0: 1801 0804 0201 08ff 0404 0c03 0203 0201  ................
-000006b0: 06fe 7228 0000 0029 0172 1600 0000 2907  ..r(...).r....).
-000006c0: da07 5f5f 646f 635f 5fda 1443 7279 7074  ..__doc__..Crypt
-000006d0: 6f2e 5075 626c 6963 4b65 792e 4543 4372  o.PublicKey.ECCr
-000006e0: 0200 0000 da07 6f73 2e70 6174 6872 0900  ......os.pathr..
-000006f0: 0000 7215 0000 0072 2800 0000 7213 0000  ..r....r(...r...
-00000700: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000710: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
-00000720: 0000 0004 0202 1a02 0b0c 0308 0108 0202  ................
-00000730: 150e fc                                  ...
+000001d0: 6c69 6e67 2e6d 6978 6573 2e45 4543 5f34  ling.mixes.EEC_4
+000001e0: 3438 5f31 2e70 7269 7661 7465 5f6b 6579  48_1.private_key
+000001f0: 2e63 7265 6174 6f72 2061 7320 4545 435f  .creator as EEC_
+00000200: 3434 385f 315f 7072 6976 6174 655f 6b65  448_1_private_ke
+00000210: 795f 6372 6561 746f 720a 0970 7269 7661  y_creator..priva
+00000220: 7465 5f6b 6579 203d 2045 4543 5f34 3438  te_key = EEC_448
+00000230: 5f31 5f70 7269 7661 7465 5f6b 6579 5f63  _1_private_key_c
+00000240: 7265 6174 6f72 2e63 7265 6174 6520 2873  reator.create (s
+00000250: 6565 642c 2066 6f72 6d61 742c 2070 6174  eed, format, pat
+00000260: 6829 0a09 7072 6976 6174 655f 6b65 795f  h)..private_key_
+00000270: 696e 7374 616e 6365 203d 2070 7269 7661  instance = priva
+00000280: 7465 5f6b 6579 205b 2269 6e73 7461 6e63  te_key ["instanc
+00000290: 6522 5d0a 0970 7269 7661 7465 5f6b 6579  e"]..private_key
+000002a0: 5f73 7472 696e 6720 3d20 7072 6976 6174  _string = privat
+000002b0: 655f 6b65 7920 5b22 7374 7269 6e67 225d  e_key ["string"]
+000002c0: 0a09 090a e900 0000 0029 01da 0645 6363  .........)...Ecc
+000002d0: 4b65 794e 6303 0000 0000 0000 0000 0000  KeyNc...........
+000002e0: 0004 0000 0004 0000 0043 0000 0073 6a00  .........C...sj.
+000002f0: 0000 7400 6a01 a002 7c00 a101 720e 7403  ..t.j...|...r.t.
+00000300: 6401 7c00 9b00 6402 9d03 8301 8201 7c02  d.|...d.......|.
+00000310: 6403 6b02 7218 7404 7c00 6404 8302 7d03  d.k.r.t.|.d...}.
+00000320: 6e12 7c02 6405 7600 7222 7404 7c00 6406  n.|.d.v.r"t.|.d.
+00000330: 8302 7d03 6e08 7403 6407 7c02 9b00 6408  ..}.n.t.d.|...d.
+00000340: 9d03 8301 8201 7c03 a005 7c01 a101 0100  ......|...|.....
+00000350: 7c03 a006 a100 0100 6409 5300 290a 4e7a  |.......d.S.).Nz
+00000360: 3054 6865 2070 6174 6820 666f 7220 7468  0The path for th
+00000370: 6520 7072 6976 6174 655f 6b65 7920 6973  e private_key is
+00000380: 206e 6f74 2061 7661 696c 6162 6c65 2e20   not available. 
+00000390: 27fa 0127 da03 4445 52da 0277 6229 02da  '..'..DER..wb)..
+000003a0: 0350 454d da0b 6865 7861 6465 6369 6d61  .PEM..hexadecima
+000003b0: 6cda 0177 7a08 666f 726d 6174 2027 7a18  l..wz.format 'z.
+000003c0: 2720 7761 7320 6e6f 7420 6163 636f 756e  ' was not accoun
+000003d0: 7465 6420 666f 722e 5429 07da 026f 73da  ted for.T)...os.
+000003e0: 0470 6174 68da 0665 7869 7374 73da 0945  .path..exists..E
+000003f0: 7863 6570 7469 6f6e da04 6f70 656e da05  xception..open..
+00000400: 7772 6974 65da 0563 6c6f 7365 2904 720a  write..close).r.
+00000410: 0000 00da 1270 7269 7661 7465 5f6b 6579  .....private_key
+00000420: 5f73 7472 696e 67da 0666 6f72 6d61 74da  _string..format.
+00000430: 0166 a900 7213 0000 00fa 472f 6861 6269  .f..r.....G/habi
+00000440: 7461 742f 7665 6e75 6573 2f73 7461 6765  tat/venues/stage
+00000450: 732f 7265 6379 636c 696e 672f 6d69 7865  s/recycling/mixe
+00000460: 732f 4545 435f 3434 385f 312f 7072 6976  s/EEC_448_1/priv
+00000470: 6174 655f 6b65 792f 6372 6561 746f 722e  ate_key/creator.
+00000480: 7079 da11 7772 6974 655f 7072 6976 6174  py..write_privat
+00000490: 655f 6b65 792e 0000 0073 1400 0000 0c01  e_key....s......
+000004a0: 1001 0802 0c01 0801 0c01 1002 0a02 0801  ................
+000004b0: 0402 7215 0000 00da 0063 0300 0000 0000  ..r......c......
+000004c0: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+000004d0: 0000 73a8 0000 0074 007c 0283 0164 016b  ..s....t.|...d.k
+000004e0: 0573 084a 0082 0174 007c 0083 0164 026b  .s.J...t.|...d.k
+000004f0: 0273 104a 0082 017c 0164 036b 0272 1764  .s.J...|.d.k.r.d
+00000500: 047d 036e 027c 017d 0374 0164 0574 02a0  .}.n.|.}.t.d.t..
+00000510: 037c 00a1 0164 068d 027d 047c 046a 047c  .|...d...}.|.j.|
+00000520: 0364 078d 017d 057c 0164 036b 0272 497c  .d...}.|.d.k.rI|
+00000530: 05a0 05a1 00a0 06a1 007d 0674 007c 0683  .........}.t.|..
+00000540: 0164 086b 0273 3e4a 0074 007c 0683 0183  .d.k.s>J.t.|....
+00000550: 0182 0174 02a0 037c 06a1 017c 056b 0273  ...t...|...|.k.s
+00000560: 474a 0082 017c 067d 0574 077c 027c 057c  GJ...|.}.t.|.|.|
+00000570: 0183 0301 007c 047c 0564 099c 0253 0029  .....|.|.d...S.)
+00000580: 0a4e e901 0000 00e9 7200 0000 7207 0000  .N......r...r...
+00000590: 0072 0400 0000 da05 4564 3434 3829 02da  .r......Ed448)..
+000005a0: 0563 7572 7665 da04 7365 6564 2901 7211  .curve..seed).r.
+000005b0: 0000 00e9 9200 0000 2902 da08 696e 7374  ........)...inst
+000005c0: 616e 6365 da06 7374 7269 6e67 2908 da03  ance..string)...
+000005d0: 6c65 6e72 0200 0000 da05 6279 7465 73da  lenr......bytes.
+000005e0: 0766 726f 6d68 6578 da0a 6578 706f 7274  .fromhex..export
+000005f0: 5f6b 6579 da03 6865 78da 0575 7070 6572  _key..hex..upper
+00000600: 7215 0000 0029 0772 1b00 0000 7211 0000  r....).r....r...
+00000610: 0072 0a00 0000 da0d 6578 706f 7274 5f66  .r......export_f
+00000620: 6f72 6d61 74da 1470 7269 7661 7465 5f6b  ormat..private_k
+00000630: 6579 5f69 6e73 7461 6e63 6572 1000 0000  ey_instancer....
+00000640: da1e 7072 6976 6174 655f 6b65 795f 6865  ..private_key_he
+00000650: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
+00000660: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00000670: 0663 7265 6174 653f 0000 0073 2e00 0000  .create?...s....
+00000680: 1006 1001 0802 0601 0402 0202 0201 0801  ................
+00000690: 06fe 0404 0201 06ff 0804 0c07 1801 0804  ................
+000006a0: 0201 08ff 0404 0c03 0203 0201 06fe 7228  ..............r(
+000006b0: 0000 0029 0172 1600 0000 2907 da07 5f5f  ...).r....)...__
+000006c0: 646f 635f 5fda 1443 7279 7074 6f2e 5075  doc__..Crypto.Pu
+000006d0: 626c 6963 4b65 792e 4543 4372 0200 0000  blicKey.ECCr....
+000006e0: da07 6f73 2e70 6174 6872 0900 0000 7215  ..os.pathr....r.
+000006f0: 0000 0072 2800 0000 7213 0000 0072 1300  ...r(...r....r..
+00000700: 0000 7213 0000 0072 1400 0000 da08 3c6d  ..r....r......<m
+00000710: 6f64 756c 653e 0100 0000 7310 0000 0004  odule>....s.....
+00000720: 0202 1a02 0b0c 0308 0108 0202 150e fc    ...............
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/__pycache__/scan.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/__pycache__/scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 a502 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 a302 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 8400  d.l.m.Z...d.d...
-00000050: 5a05 6406 5300 2907 7a6f 0a09 696d 706f  Z.d.S.).zo..impo
-00000060: 7274 2072 6563 7963 6c69 6e67 2e6d 6f64  rt recycling.mod
-00000070: 756c 6573 2e45 4543 5f34 3438 5f31 2e70  ules.EEC_448_1.p
-00000080: 7269 7661 7465 5f6b 6579 2e73 6361 6e20  rivate_key.scan 
-00000090: 6173 2070 7269 7661 7465 5f73 6361 6e0a  as private_scan.
-000000a0: 0970 7269 7661 7465 5f6b 6579 203d 2070  .private_key = p
-000000b0: 7269 7661 7465 5f73 6361 6e2e 7374 6172  rivate_scan.star
-000000c0: 7420 2870 6174 6829 0ae9 0000 0000 2901  t (path)......).
-000000d0: da03 4543 4329 01da 0846 7261 6374 696f  ..ECC)...Fractio
-000000e0: 6e63 0100 0000 0000 0000 0000 0000 0600  nc..............
-000000f0: 0000 0800 0000 4300 0000 7364 0000 0074  ......C...sd...t
-00000100: 007c 0064 0164 028d 028f 227d 017c 01a0  .|.d.d...."}.|..
-00000110: 01a1 007d 0274 026a 037c 0264 0364 048d  ...}.t.j.|.d.d..
-00000120: 027d 037c 02a0 04a1 007d 0447 0064 0564  .}.|.....}.G.d.d
-00000130: 0684 0064 0683 027d 057c 057c 0383 0157  ...d...}.|.|...W
-00000140: 0002 0064 0004 0004 0083 0301 0053 0031  ...d.........S.1
-00000150: 0073 2b77 0101 0001 0001 0059 0001 0064  .s+w.......Y...d
-00000160: 0053 0029 074e da02 7262 2901 da04 6d6f  .S.).N..rb)...mo
-00000170: 6465 da05 4564 3434 3829 01da 0a63 7572  de..Ed448)...cur
-00000180: 7665 5f6e 616d 6563 0000 0000 0000 0000  ve_namec........
-00000190: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000001a0: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-000001b0: 0284 005a 0364 0353 0029 047a 1a73 7461  ...Z.d.S.).z.sta
-000001c0: 7274 2e3c 6c6f 6361 6c73 3e2e 7072 6976  rt.<locals>.priv
-000001d0: 6174 655f 6b65 7963 0200 0000 0000 0000  ate_keyc........
-000001e0: 0000 0000 0200 0000 0200 0000 5300 0000  ............S...
-000001f0: 730a 0000 007c 017c 005f 0064 0053 0029  s....|.|._.d.S.)
-00000200: 014e 2901 da08 696e 7374 616e 6365 2902  .N)...instance).
-00000210: da04 7468 6973 7208 0000 00a9 0072 0a00  ..thisr......r..
-00000220: 0000 fa46 2f68 6162 6974 6174 2f76 656e  ...F/habitat/ven
-00000230: 7565 732f 7374 6167 6573 2f72 6563 7963  ues/stages/recyc
-00000240: 6c69 6e67 2f6d 6f64 756c 6573 2f45 4543  ling/modules/EEC
-00000250: 5f34 3438 5f31 2f70 7269 7661 7465 5f6b  _448_1/private_k
-00000260: 6579 2f73 6361 6e2e 7079 da08 5f5f 696e  ey/scan.py..__in
-00000270: 6974 5f5f 1600 0000 7302 0000 000a 017a  it__....s......z
-00000280: 2373 7461 7274 2e3c 6c6f 6361 6c73 3e2e  #start.<locals>.
-00000290: 7072 6976 6174 655f 6b65 792e 5f5f 696e  private_key.__in
-000002a0: 6974 5f5f 4e29 04da 085f 5f6e 616d 655f  it__N)...__name_
-000002b0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000002c0: 5f71 7561 6c6e 616d 655f 5f72 0c00 0000  _qualname__r....
-000002d0: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-000002e0: 0b00 0000 da0b 7072 6976 6174 655f 6b65  ......private_ke
-000002f0: 7915 0000 0073 0400 0000 0800 0c01 7210  y....s........r.
-00000300: 0000 0029 05da 046f 7065 6eda 0472 6561  ...)...open..rea
-00000310: 6472 0200 0000 da0a 696d 706f 7274 5f6b  dr......import_k
-00000320: 6579 da03 6865 7829 06da 0470 6174 68da  ey..hex)...path.
-00000330: 0466 696c 65da 1170 7269 7661 7465 5f6b  .file..private_k
-00000340: 6579 5f62 7974 6573 da14 7072 6976 6174  ey_bytes..privat
-00000350: 655f 6b65 795f 696e 7374 616e 6365 da12  e_key_instance..
-00000360: 7072 6976 6174 655f 6b65 795f 7374 7269  private_key_stri
-00000370: 6e67 7210 0000 0072 0a00 0000 720a 0000  ngr....r....r...
-00000380: 0072 0b00 0000 da05 7374 6172 740c 0000  .r......start...
-00000390: 0073 1800 0000 0e01 0801 0401 0201 0201  .s..............
-000003a0: 06fe 0804 0e02 0204 0201 02ff 24f4 721a  ............$.r.
-000003b0: 0000 004e 2906 da07 5f5f 646f 635f 5fda  ...N)...__doc__.
-000003c0: 1043 7279 7074 6f2e 5075 626c 6963 4b65  .Crypto.PublicKe
-000003d0: 7972 0200 0000 da09 6672 6163 7469 6f6e  yr......fraction
-000003e0: 7372 0300 0000 721a 0000 0072 0a00 0000  sr....r....r....
-000003f0: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000400: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000410: 0000 0403 0c05 0c01 0c02                 ..........
+00000050: 5a05 6406 5300 2907 7a6d 0a09 696d 706f  Z.d.S.).zm..impo
+00000060: 7274 2072 6563 7963 6c69 6e67 2e6d 6978  rt recycling.mix
+00000070: 6573 2e45 4543 5f34 3438 5f31 2e70 7269  es.EEC_448_1.pri
+00000080: 7661 7465 5f6b 6579 2e73 6361 6e20 6173  vate_key.scan as
+00000090: 2070 7269 7661 7465 5f73 6361 6e0a 0970   private_scan..p
+000000a0: 7269 7661 7465 5f6b 6579 203d 2070 7269  rivate_key = pri
+000000b0: 7661 7465 5f73 6361 6e2e 7374 6172 7420  vate_scan.start 
+000000c0: 2870 6174 6829 0ae9 0000 0000 2901 da03  (path)......)...
+000000d0: 4543 4329 01da 0846 7261 6374 696f 6e63  ECC)...Fractionc
+000000e0: 0100 0000 0000 0000 0000 0000 0600 0000  ................
+000000f0: 0800 0000 4300 0000 7364 0000 0074 007c  ....C...sd...t.|
+00000100: 0064 0164 028d 028f 227d 017c 01a0 01a1  .d.d...."}.|....
+00000110: 007d 0274 026a 037c 0264 0364 048d 027d  .}.t.j.|.d.d...}
+00000120: 037c 02a0 04a1 007d 0447 0064 0564 0684  .|.....}.G.d.d..
+00000130: 0064 0683 027d 057c 057c 0383 0157 0002  .d...}.|.|...W..
+00000140: 0064 0004 0004 0083 0301 0053 0031 0073  .d.........S.1.s
+00000150: 2b77 0101 0001 0001 0059 0001 0064 0053  +w.......Y...d.S
+00000160: 0029 074e da02 7262 2901 da04 6d6f 6465  .).N..rb)...mode
+00000170: da05 4564 3434 3829 01da 0a63 7572 7665  ..Ed448)...curve
+00000180: 5f6e 616d 6563 0000 0000 0000 0000 0000  _namec..........
+00000190: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
+000001a0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+000001b0: 005a 0364 0353 0029 047a 1a73 7461 7274  .Z.d.S.).z.start
+000001c0: 2e3c 6c6f 6361 6c73 3e2e 7072 6976 6174  .<locals>.privat
+000001d0: 655f 6b65 7963 0200 0000 0000 0000 0000  e_keyc..........
+000001e0: 0000 0200 0000 0200 0000 5300 0000 730a  ..........S...s.
+000001f0: 0000 007c 017c 005f 0064 0053 0029 014e  ...|.|._.d.S.).N
+00000200: 2901 da08 696e 7374 616e 6365 2902 da04  )...instance)...
+00000210: 7468 6973 7208 0000 00a9 0072 0a00 0000  thisr......r....
+00000220: fa44 2f68 6162 6974 6174 2f76 656e 7565  .D/habitat/venue
+00000230: 732f 7374 6167 6573 2f72 6563 7963 6c69  s/stages/recycli
+00000240: 6e67 2f6d 6978 6573 2f45 4543 5f34 3438  ng/mixes/EEC_448
+00000250: 5f31 2f70 7269 7661 7465 5f6b 6579 2f73  _1/private_key/s
+00000260: 6361 6e2e 7079 da08 5f5f 696e 6974 5f5f  can.py..__init__
+00000270: 1600 0000 7302 0000 000a 017a 2373 7461  ....s......z#sta
+00000280: 7274 2e3c 6c6f 6361 6c73 3e2e 7072 6976  rt.<locals>.priv
+00000290: 6174 655f 6b65 792e 5f5f 696e 6974 5f5f  ate_key.__init__
+000002a0: 4e29 04da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000002b0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000002c0: 6c6e 616d 655f 5f72 0c00 0000 720a 0000  lname__r....r...
+000002d0: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+000002e0: da0b 7072 6976 6174 655f 6b65 7915 0000  ..private_key...
+000002f0: 0073 0400 0000 0800 0c01 7210 0000 0029  .s........r....)
+00000300: 05da 046f 7065 6eda 0472 6561 6472 0200  ...open..readr..
+00000310: 0000 da0a 696d 706f 7274 5f6b 6579 da03  ....import_key..
+00000320: 6865 7829 06da 0470 6174 68da 0466 696c  hex)...path..fil
+00000330: 65da 1170 7269 7661 7465 5f6b 6579 5f62  e..private_key_b
+00000340: 7974 6573 da14 7072 6976 6174 655f 6b65  ytes..private_ke
+00000350: 795f 696e 7374 616e 6365 da12 7072 6976  y_instance..priv
+00000360: 6174 655f 6b65 795f 7374 7269 6e67 7210  ate_key_stringr.
+00000370: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+00000380: 0000 da05 7374 6172 740c 0000 0073 1800  ....start....s..
+00000390: 0000 0e01 0801 0401 0201 0201 06fe 0804  ................
+000003a0: 0e02 0204 0201 02ff 24f4 721a 0000 004e  ........$.r....N
+000003b0: 2906 da07 5f5f 646f 635f 5fda 1043 7279  )...__doc__..Cry
+000003c0: 7074 6f2e 5075 626c 6963 4b65 7972 0200  pto.PublicKeyr..
+000003d0: 0000 da09 6672 6163 7469 6f6e 7372 0300  ....fractionsr..
+000003e0: 0000 721a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+000003f0: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
+00000400: 6475 6c65 3e01 0000 0073 0800 0000 0403  dule>....s......
+00000410: 0c05 0c01 0c02                           ......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/creator.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	#	seed length = 114 nibbles
 	#				=  57 bytes
 	#
 	seed = "4986888b11358bf3d541b41eea5daece1c6eff64130a45fc8b9ca48f3e0e02463c99c5aedc8a847686d669b7d547c18fe448fc5111ca88f4e8"
 	format = "PEM"
 	path = ""
 	
-	import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+	import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
 	private_key = EEC_448_1_private_key_creator.create (seed, format, path)
 	private_key_instance = private_key ["instance"]
 	private_key_string = private_key ["string"]
 		
 '''
 
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/private_key/scan.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/private_key/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 '''
-	import recycling.modules.EEC_448_1.private_key.scan as private_scan
+	import recycling.mixes.EEC_448_1.private_key.scan as private_scan
 	private_key = private_scan.start (path)
 '''
 
 from Crypto.PublicKey import ECC
 from fractions import Fraction
 
 def start (path):
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/BUILD--.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/BUILD--.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/BUILD.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/BUILD.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/CREATE.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/CREATE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/SCAN.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/creator.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/creator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2073 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,110 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 1908 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 1508 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6401 6402 6c06 6d07 0200 0100  Z...d.d.l.m.....
 00000060: 6d08 0200 0100 6d09 0200 0100 6d0a 5a0b  m.....m.....m.Z.
 00000070: 0100 6405 6406 8400 5a0c 0907 0907 0907  ..d.d...Z.......
 00000080: 640a 6408 6409 8401 5a0d 6402 5300 290b  d.d.d...Z.d.S.).
-00000090: 615b 0100 000a 0923 0a09 2309 7772 6974  a[.....#..#.writ
+00000090: 6159 0100 000a 0923 0a09 2309 7772 6974  aY.....#..#.writ
 000000a0: 6520 7075 626c 6963 206b 6579 2074 6f20  e public key to 
 000000b0: 7061 7468 0a09 230a 0969 6d70 6f72 7420  path..#..import 
-000000c0: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-000000d0: 732e 4545 435f 3434 385f 312e 7075 626c  s.EEC_448_1.publ
-000000e0: 6963 5f6b 6579 2e63 7265 6174 6f72 2061  ic_key.creator a
-000000f0: 7320 4545 435f 3434 385f 315f 7075 626c  s EEC_448_1_publ
-00000100: 6963 5f6b 6579 5f63 7265 6174 6f72 0a09  ic_key_creator..
-00000110: 7075 626c 6963 5f6b 6579 203d 2045 4543  public_key = EEC
-00000120: 5f34 3438 5f31 5f70 7562 6c69 635f 6b65  _448_1_public_ke
-00000130: 795f 6372 6561 746f 722e 6372 6561 7465  y_creator.create
-00000140: 2028 0a09 0970 7269 7661 7465 5f6b 6579   (...private_key
-00000150: 5f70 6174 6820 3d20 2222 2c0a 0909 0a09  _path = "",.....
-00000160: 0970 7562 6c69 635f 6b65 795f 7061 7468  .public_key_path
-00000170: 203d 2022 222c 0a09 0970 7562 6c69 635f   = "",...public_
-00000180: 6b65 795f 666f 726d 6174 203d 2022 220a  key_format = "".
-00000190: 0929 0a09 7075 626c 6963 5f6b 6579 5f69  .)..public_key_i
-000001a0: 6e73 7461 6e63 6520 3d20 7075 626c 6963  nstance = public
-000001b0: 5f6b 6579 205b 2269 6e73 7461 6e63 6522  _key ["instance"
-000001c0: 5d0a 0970 7562 6c69 635f 6b65 795f 7374  ]..public_key_st
-000001d0: 7269 6e67 203d 2070 7562 6c69 635f 6b65  ring = public_ke
-000001e0: 7920 5b22 7374 7269 6e67 225d 0a09 090a  y ["string"]....
-000001f0: e900 0000 004e 2901 da06 4563 634b 6579  .....N)...EccKey
-00000200: 2901 da03 4543 4363 0300 0000 0000 0000  )...ECCc........
-00000210: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00000220: 736a 0000 0074 006a 01a0 027c 00a1 0172  sj...t.j...|...r
-00000230: 0e74 0364 017c 009b 0064 029d 0383 0182  .t.d.|...d......
-00000240: 017c 0264 036b 0272 1874 047c 0064 0483  .|.d.k.r.t.|.d..
-00000250: 027d 036e 127c 0264 0576 0072 2274 047c  .}.n.|.d.v.r"t.|
-00000260: 0064 0683 027d 036e 0874 0364 077c 029b  .d...}.n.t.d.|..
-00000270: 0064 089d 0383 0182 017c 03a0 057c 01a1  .d.......|...|..
-00000280: 0101 007c 03a0 06a1 0001 0064 0953 0029  ...|.......d.S.)
-00000290: 0a4e 7a1d 5468 6520 7061 7468 2066 6f72  .Nz.The path for
-000002a0: 2074 6865 2070 7562 6c69 6320 6b65 7920   the public key 
-000002b0: 277a 1327 2069 7320 6e6f 7420 6176 6169  'z.' is not avai
-000002c0: 6c61 626c 652e da03 4445 52da 0277 6229  lable...DER..wb)
-000002d0: 02da 0350 454d da0b 6865 7861 6465 6369  ...PEM..hexadeci
-000002e0: 6d61 6cda 0177 7a08 666f 726d 6174 2027  mal..wz.format '
-000002f0: 7a18 2720 7761 7320 6e6f 7420 6163 636f  z.' was not acco
-00000300: 756e 7465 6420 666f 722e 5429 07da 026f  unted for.T)...o
-00000310: 73da 0470 6174 68da 0665 7869 7374 73da  s..path..exists.
-00000320: 0945 7863 6570 7469 6f6e da04 6f70 656e  .Exception..open
-00000330: da05 7772 6974 65da 0563 6c6f 7365 2904  ..write..close).
-00000340: 720a 0000 00da 0a6b 6579 5f73 7472 696e  r......key_strin
-00000350: 67da 0666 6f72 6d61 74da 0166 a900 7213  g..format..f..r.
-00000360: 0000 00fa 482f 6861 6269 7461 742f 7665  ....H/habitat/ve
-00000370: 6e75 6573 2f73 7461 6765 732f 7265 6379  nues/stages/recy
-00000380: 636c 696e 672f 6d6f 6475 6c65 732f 4545  cling/modules/EE
-00000390: 435f 3434 385f 312f 7075 626c 6963 5f6b  C_448_1/public_k
-000003a0: 6579 2f63 7265 6174 6f72 2e70 79da 1077  ey/creator.py..w
-000003b0: 7269 7465 5f70 7562 6c69 635f 6b65 791e  rite_public_key.
-000003c0: 0000 0073 1800 0000 0c01 0201 0a01 04ff  ...s............
-000003d0: 0804 0c01 0801 0c01 1002 0a02 0801 0402  ................
-000003e0: 7215 0000 00da 0063 0300 0000 0000 0000  r......c........
-000003f0: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
-00000400: 737e 0000 0074 00a0 017c 00a1 017d 037c  s~...t...|...}.|
-00000410: 0264 016b 0272 0c64 027d 046e 027c 027d  .d.k.r.d.}.n.|.}
-00000420: 047c 036a 02a0 03a1 007d 057c 056a 047c  .|.j.....}.|.j.|
-00000430: 0464 038d 017d 067c 0264 016b 0272 347c  .d...}.|.d.k.r4|
-00000440: 06a0 05a1 007d 0774 067c 0783 0164 046b  .....}.t.|...d.k
-00000450: 0273 294a 0082 0174 07a0 087c 07a1 017c  .s)J...t...|...|
-00000460: 066b 0273 324a 0082 017c 077d 0674 097c  .k.s2J...|.}.t.|
-00000470: 017c 067c 0283 0301 007c 057c 0664 059c  .|.|.....|.|.d..
-00000480: 0253 0029 064e 7207 0000 0072 0400 0000  .S.).Nr....r....
-00000490: 2901 7211 0000 00e9 8a00 0000 2902 da08  ).r.........)...
-000004a0: 696e 7374 616e 6365 da06 7374 7269 6e67  instance..string
-000004b0: 290a da0c 7072 6976 6174 655f 7363 616e  )...private_scan
-000004c0: da05 7374 6172 7472 1800 0000 da0a 7075  ..startr......pu
-000004d0: 626c 6963 5f6b 6579 da0a 6578 706f 7274  blic_key..export
-000004e0: 5f6b 6579 da03 6865 78da 036c 656e da05  _key..hex..len..
-000004f0: 6279 7465 73da 0766 726f 6d68 6578 7215  bytes..fromhexr.
-00000500: 0000 0029 08da 1070 7269 7661 7465 5f6b  ...)...private_k
-00000510: 6579 5f70 6174 68da 0f70 7562 6c69 635f  ey_path..public_
-00000520: 6b65 795f 7061 7468 da11 7075 626c 6963  key_path..public
-00000530: 5f6b 6579 5f66 6f72 6d61 74da 0b70 7269  _key_format..pri
-00000540: 7661 7465 5f6b 6579 da18 7075 626c 6963  vate_key..public
-00000550: 5f6b 6579 5f65 7870 6f72 745f 666f 726d  _key_export_form
-00000560: 6174 da13 7075 626c 6963 5f6b 6579 5f69  at..public_key_i
-00000570: 6e73 7461 6e63 65da 1170 7562 6c69 635f  nstance..public_
-00000580: 6b65 795f 7374 7269 6e67 da1d 7075 626c  key_string..publ
-00000590: 6963 5f6b 6579 5f68 6578 6164 6563 696d  ic_key_hexadecim
-000005a0: 616c 5f73 7472 696e 6772 1300 0000 7213  al_stringr....r.
-000005b0: 0000 0072 1400 0000 da06 6372 6561 7465  ...r......create
-000005c0: 3100 0000 732e 0000 000a 0508 0206 0104  1...s...........
-000005d0: 020a 0204 0102 0106 ff08 0408 0710 0108  ................
-000005e0: 0402 0108 ff04 0402 0202 0102 0202 0104  ................
-000005f0: fc02 0802 0106 fe72 2a00 0000 2903 7216  .......r*...).r.
-00000600: 0000 0072 1600 0000 7216 0000 0029 0eda  ...r....r....)..
-00000610: 075f 5f64 6f63 5f5f 7209 0000 00da 1443  .__doc__r......C
-00000620: 7279 7074 6f2e 5075 626c 6963 4b65 792e  rypto.PublicKey.
-00000630: 4543 4372 0200 0000 da10 4372 7970 746f  ECCr......Crypto
-00000640: 2e50 7562 6c69 634b 6579 7203 0000 00da  .PublicKeyr.....
-00000650: 2c72 6563 7963 6c69 6e67 2e6d 6f64 756c  ,recycling.modul
-00000660: 6573 2e45 4543 5f34 3438 5f31 2e70 7269  es.EEC_448_1.pri
-00000670: 7661 7465 5f6b 6579 2e73 6361 6eda 076d  vate_key.scan..m
-00000680: 6f64 756c 6573 da09 4545 435f 3434 385f  odules..EEC_448_
-00000690: 3172 2500 0000 da04 7363 616e 721a 0000  1r%.....scanr...
-000006a0: 0072 1500 0000 722a 0000 0072 1300 0000  .r....r*...r....
-000006b0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000006c0: 083c 6d6f 6475 6c65 3e01 0000 0073 1600  .<module>....s..
-000006d0: 0000 0401 0210 0805 0c02 0c01 1e02 0802  ................
-000006e0: 0214 0201 0201 0efd                      ........
+000000c0: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+000000d0: 4545 435f 3434 385f 312e 7075 626c 6963  EEC_448_1.public
+000000e0: 5f6b 6579 2e63 7265 6174 6f72 2061 7320  _key.creator as 
+000000f0: 4545 435f 3434 385f 315f 7075 626c 6963  EEC_448_1_public
+00000100: 5f6b 6579 5f63 7265 6174 6f72 0a09 7075  _key_creator..pu
+00000110: 626c 6963 5f6b 6579 203d 2045 4543 5f34  blic_key = EEC_4
+00000120: 3438 5f31 5f70 7562 6c69 635f 6b65 795f  48_1_public_key_
+00000130: 6372 6561 746f 722e 6372 6561 7465 2028  creator.create (
+00000140: 0a09 0970 7269 7661 7465 5f6b 6579 5f70  ...private_key_p
+00000150: 6174 6820 3d20 2222 2c0a 0909 0a09 0970  ath = "",......p
+00000160: 7562 6c69 635f 6b65 795f 7061 7468 203d  ublic_key_path =
+00000170: 2022 222c 0a09 0970 7562 6c69 635f 6b65   "",...public_ke
+00000180: 795f 666f 726d 6174 203d 2022 220a 0929  y_format = ""..)
+00000190: 0a09 7075 626c 6963 5f6b 6579 5f69 6e73  ..public_key_ins
+000001a0: 7461 6e63 6520 3d20 7075 626c 6963 5f6b  tance = public_k
+000001b0: 6579 205b 2269 6e73 7461 6e63 6522 5d0a  ey ["instance"].
+000001c0: 0970 7562 6c69 635f 6b65 795f 7374 7269  .public_key_stri
+000001d0: 6e67 203d 2070 7562 6c69 635f 6b65 7920  ng = public_key 
+000001e0: 5b22 7374 7269 6e67 225d 0a09 090a e900  ["string"]......
+000001f0: 0000 004e 2901 da06 4563 634b 6579 2901  ...N)...EccKey).
+00000200: da03 4543 4363 0300 0000 0000 0000 0000  ..ECCc..........
+00000210: 0000 0400 0000 0400 0000 4300 0000 736a  ..........C...sj
+00000220: 0000 0074 006a 01a0 027c 00a1 0172 0e74  ...t.j...|...r.t
+00000230: 0364 017c 009b 0064 029d 0383 0182 017c  .d.|...d.......|
+00000240: 0264 036b 0272 1874 047c 0064 0483 027d  .d.k.r.t.|.d...}
+00000250: 036e 127c 0264 0576 0072 2274 047c 0064  .n.|.d.v.r"t.|.d
+00000260: 0683 027d 036e 0874 0364 077c 029b 0064  ...}.n.t.d.|...d
+00000270: 089d 0383 0182 017c 03a0 057c 01a1 0101  .......|...|....
+00000280: 007c 03a0 06a1 0001 0064 0953 0029 0a4e  .|.......d.S.).N
+00000290: 7a1d 5468 6520 7061 7468 2066 6f72 2074  z.The path for t
+000002a0: 6865 2070 7562 6c69 6320 6b65 7920 277a  he public key 'z
+000002b0: 1327 2069 7320 6e6f 7420 6176 6169 6c61  .' is not availa
+000002c0: 626c 652e da03 4445 52da 0277 6229 02da  ble...DER..wb)..
+000002d0: 0350 454d da0b 6865 7861 6465 6369 6d61  .PEM..hexadecima
+000002e0: 6cda 0177 7a08 666f 726d 6174 2027 7a18  l..wz.format 'z.
+000002f0: 2720 7761 7320 6e6f 7420 6163 636f 756e  ' was not accoun
+00000300: 7465 6420 666f 722e 5429 07da 026f 73da  ted for.T)...os.
+00000310: 0470 6174 68da 0665 7869 7374 73da 0945  .path..exists..E
+00000320: 7863 6570 7469 6f6e da04 6f70 656e da05  xception..open..
+00000330: 7772 6974 65da 0563 6c6f 7365 2904 720a  write..close).r.
+00000340: 0000 00da 0a6b 6579 5f73 7472 696e 67da  .....key_string.
+00000350: 0666 6f72 6d61 74da 0166 a900 7213 0000  .format..f..r...
+00000360: 00fa 462f 6861 6269 7461 742f 7665 6e75  ..F/habitat/venu
+00000370: 6573 2f73 7461 6765 732f 7265 6379 636c  es/stages/recycl
+00000380: 696e 672f 6d69 7865 732f 4545 435f 3434  ing/mixes/EEC_44
+00000390: 385f 312f 7075 626c 6963 5f6b 6579 2f63  8_1/public_key/c
+000003a0: 7265 6174 6f72 2e70 79da 1077 7269 7465  reator.py..write
+000003b0: 5f70 7562 6c69 635f 6b65 791e 0000 0073  _public_key....s
+000003c0: 1800 0000 0c01 0201 0a01 04ff 0804 0c01  ................
+000003d0: 0801 0c01 1002 0a02 0801 0402 7215 0000  ............r...
+000003e0: 00da 0063 0300 0000 0000 0000 0000 0000  ...c............
+000003f0: 0800 0000 0400 0000 4300 0000 737e 0000  ........C...s~..
+00000400: 0074 00a0 017c 00a1 017d 037c 0264 016b  .t...|...}.|.d.k
+00000410: 0272 0c64 027d 046e 027c 027d 047c 036a  .r.d.}.n.|.}.|.j
+00000420: 02a0 03a1 007d 057c 056a 047c 0464 038d  .....}.|.j.|.d..
+00000430: 017d 067c 0264 016b 0272 347c 06a0 05a1  .}.|.d.k.r4|....
+00000440: 007d 0774 067c 0783 0164 046b 0273 294a  .}.t.|...d.k.s)J
+00000450: 0082 0174 07a0 087c 07a1 017c 066b 0273  ...t...|...|.k.s
+00000460: 324a 0082 017c 077d 0674 097c 017c 067c  2J...|.}.t.|.|.|
+00000470: 0283 0301 007c 057c 0664 059c 0253 0029  .....|.|.d...S.)
+00000480: 064e 7207 0000 0072 0400 0000 2901 7211  .Nr....r....).r.
+00000490: 0000 00e9 8a00 0000 2902 da08 696e 7374  ........)...inst
+000004a0: 616e 6365 da06 7374 7269 6e67 290a da0c  ance..string)...
+000004b0: 7072 6976 6174 655f 7363 616e da05 7374  private_scan..st
+000004c0: 6172 7472 1800 0000 da0a 7075 626c 6963  artr......public
+000004d0: 5f6b 6579 da0a 6578 706f 7274 5f6b 6579  _key..export_key
+000004e0: da03 6865 78da 036c 656e da05 6279 7465  ..hex..len..byte
+000004f0: 73da 0766 726f 6d68 6578 7215 0000 0029  s..fromhexr....)
+00000500: 08da 1070 7269 7661 7465 5f6b 6579 5f70  ...private_key_p
+00000510: 6174 68da 0f70 7562 6c69 635f 6b65 795f  ath..public_key_
+00000520: 7061 7468 da11 7075 626c 6963 5f6b 6579  path..public_key
+00000530: 5f66 6f72 6d61 74da 0b70 7269 7661 7465  _format..private
+00000540: 5f6b 6579 da18 7075 626c 6963 5f6b 6579  _key..public_key
+00000550: 5f65 7870 6f72 745f 666f 726d 6174 da13  _export_format..
+00000560: 7075 626c 6963 5f6b 6579 5f69 6e73 7461  public_key_insta
+00000570: 6e63 65da 1170 7562 6c69 635f 6b65 795f  nce..public_key_
+00000580: 7374 7269 6e67 da1d 7075 626c 6963 5f6b  string..public_k
+00000590: 6579 5f68 6578 6164 6563 696d 616c 5f73  ey_hexadecimal_s
+000005a0: 7472 696e 6772 1300 0000 7213 0000 0072  tringr....r....r
+000005b0: 1400 0000 da06 6372 6561 7465 3100 0000  ......create1...
+000005c0: 732e 0000 000a 0508 0206 0104 020a 0204  s...............
+000005d0: 0102 0106 ff08 0408 0710 0108 0402 0108  ................
+000005e0: ff04 0402 0202 0102 0202 0104 fc02 0802  ................
+000005f0: 0106 fe72 2a00 0000 2903 7216 0000 0072  ...r*...).r....r
+00000600: 1600 0000 7216 0000 0029 0eda 075f 5f64  ....r....)...__d
+00000610: 6f63 5f5f 7209 0000 00da 1443 7279 7074  oc__r......Crypt
+00000620: 6f2e 5075 626c 6963 4b65 792e 4543 4372  o.PublicKey.ECCr
+00000630: 0200 0000 da10 4372 7970 746f 2e50 7562  ......Crypto.Pub
+00000640: 6c69 634b 6579 7203 0000 00da 2a72 6563  licKeyr.....*rec
+00000650: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000660: 5f34 3438 5f31 2e70 7269 7661 7465 5f6b  _448_1.private_k
+00000670: 6579 2e73 6361 6eda 056d 6978 6573 da09  ey.scan..mixes..
+00000680: 4545 435f 3434 385f 3172 2500 0000 da04  EEC_448_1r%.....
+00000690: 7363 616e 721a 0000 0072 1500 0000 722a  scanr....r....r*
+000006a0: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
+000006b0: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000006c0: 3e01 0000 0073 1600 0000 0401 0210 0805  >....s..........
+000006d0: 0c02 0c01 1e02 0802 0214 0201 0201 0efd  ................
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/form.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/creator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1059 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,87 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 2304 0000  o........@@f#...
+00000000: 6f0d 0d0a 0000 0000 d153 5166 9105 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6401 6402 6c06 6d07 0200 0100 6d08  ..d.d.l.m.....m.
-00000060: 0200 0100 6d09 0200 0100 6d0a 5a0b 0100  ....m.....m.Z...
-00000070: 0902 6407 6405 6406 8401 5a0c 6402 5300  ..d.d.d...Z.d.S.
-00000080: 2908 6140 0100 000a 0969 6d70 6f72 7420  ).a@.....import 
-00000090: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-000000a0: 732e 4545 435f 3434 385f 312e 7075 626c  s.EEC_448_1.publ
-000000b0: 6963 5f6b 6579 2e66 6f72 6d20 6173 2066  ic_key.form as f
-000000c0: 6f72 6d5f 4545 435f 3434 385f 315f 7075  orm_EEC_448_1_pu
-000000d0: 626c 6963 5f6b 6579 0a09 7075 626c 6963  blic_key..public
-000000e0: 5f6b 6579 203d 2066 6f72 6d5f 4545 435f  _key = form_EEC_
-000000f0: 3434 385f 315f 7075 626c 6963 5f6b 6579  448_1_public_key
-00000100: 2e73 6d6f 6f74 686c 7920 280a 0909 7072  .smoothly (...pr
-00000110: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
-00000120: 6365 203d 204e 6f6e 650a 0929 0a09 7075  ce = None..)..pu
-00000130: 626c 6963 5f6b 6579 5f69 6e73 7461 6e63  blic_key_instanc
-00000140: 6520 3d20 7075 626c 6963 5f6b 6579 205b  e = public_key [
-00000150: 2269 6e73 7461 6e63 6522 5d0a 0970 7562  "instance"]..pub
-00000160: 6c69 635f 6b65 795f 4445 525f 7374 7269  lic_key_DER_stri
-00000170: 6e67 203d 2070 7562 6c69 635f 6b65 7920  ng = public_key 
-00000180: 5b22 4445 5222 5d0a 0970 7562 6c69 635f  ["DER"]..public_
-00000190: 6b65 795f 6865 7861 6465 6369 6d61 6c5f  key_hexadecimal_
-000001a0: 7374 7269 6e67 203d 2070 7562 6c69 635f  string = public_
-000001b0: 6b65 7920 5b22 6865 7861 6465 6369 6d61  key ["hexadecima
-000001c0: 6c22 5d0a 0909 0ae9 0000 0000 4e29 01da  l"].........N)..
-000001d0: 0645 6363 4b65 7929 01da 0345 4343 6301  .EccKey)...ECCc.
-000001e0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000001f0: 0000 0043 0000 0073 4e00 0000 7c00 a000  ...C...sN...|...
-00000200: a100 7d01 7c01 6a01 6401 6402 8d01 7d02  ..}.|.j.d.d...}.
-00000210: 7c02 a002 a100 a003 a100 7d03 7404 7c03  |.........}.t.|.
-00000220: 8301 6403 6b02 7318 4a00 8201 7c02 7405  ..d.k.s.J...|.t.
-00000230: a006 7c03 a101 6b02 7321 4a00 8201 7c01  ..|...k.s!J...|.
-00000240: 7c02 7c03 6404 9c03 5300 2905 4eda 0344  |.|.d...S.).N..D
-00000250: 4552 2901 da06 666f 726d 6174 e98a 0000  ER)...format....
-00000260: 0029 03da 0869 6e73 7461 6e63 6572 0400  .)...instancer..
-00000270: 0000 da0b 6865 7861 6465 6369 6d61 6c29  ....hexadecimal)
-00000280: 07da 0a70 7562 6c69 635f 6b65 79da 0a65  ...public_key..e
-00000290: 7870 6f72 745f 6b65 79da 0368 6578 da05  xport_key..hex..
-000002a0: 7570 7065 72da 036c 656e da05 6279 7465  upper..len..byte
-000002b0: 73da 0766 726f 6d68 6578 2904 da14 7072  s..fromhex)...pr
-000002c0: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
-000002d0: 6365 da13 7075 626c 6963 5f6b 6579 5f69  ce..public_key_i
-000002e0: 6e73 7461 6e63 65da 1570 7562 6c69 635f  nstance..public_
-000002f0: 6b65 795f 4445 525f 7374 7269 6e67 da1d  key_DER_string..
-00000300: 7075 626c 6963 5f6b 6579 5f68 6578 6164  public_key_hexad
-00000310: 6563 696d 616c 5f73 7472 696e 67a9 0072  ecimal_string..r
-00000320: 1400 0000 fa45 2f68 6162 6974 6174 2f76  .....E/habitat/v
-00000330: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
-00000340: 7963 6c69 6e67 2f6d 6f64 756c 6573 2f45  ycling/modules/E
-00000350: 4543 5f34 3438 5f31 2f70 7562 6c69 635f  EC_448_1/public_
-00000360: 6b65 792f 666f 726d 2e70 79da 0873 6d6f  key/form.py..smo
-00000370: 6f74 686c 7914 0000 0073 1200 0000 0805  othly....s......
-00000380: 0c01 0c02 1001 1201 0203 0202 0201 06fc  ................
-00000390: 7216 0000 0029 014e 290d da07 5f5f 646f  r....).N)...__do
-000003a0: 635f 5fda 026f 73da 1443 7279 7074 6f2e  c__..os..Crypto.
-000003b0: 5075 626c 6963 4b65 792e 4543 4372 0200  PublicKey.ECCr..
-000003c0: 0000 da10 4372 7970 746f 2e50 7562 6c69  ....Crypto.Publi
-000003d0: 634b 6579 7203 0000 00da 2c72 6563 7963  cKeyr.....,recyc
-000003e0: 6c69 6e67 2e6d 6f64 756c 6573 2e45 4543  ling.modules.EEC
-000003f0: 5f34 3438 5f31 2e70 7269 7661 7465 5f6b  _448_1.private_k
-00000400: 6579 2e73 6361 6eda 076d 6f64 756c 6573  ey.scan..modules
-00000410: da09 4545 435f 3434 385f 31da 0b70 7269  ..EEC_448_1..pri
-00000420: 7661 7465 5f6b 6579 da04 7363 616e da0c  vate_key..scan..
-00000430: 7072 6976 6174 655f 7363 616e 7216 0000  private_scanr...
-00000440: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000450: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000460: 0000 0073 0e00 0000 0401 080b 0c02 0c01  ...s............
-00000470: 1e02 0203 0eff                           ......
+00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
+00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
+00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
+00000050: 5a05 0100 6401 6402 6c06 6d07 0200 0100  Z...d.d.l.m.....
+00000060: 6d08 0200 0100 6d09 0200 0100 6d0a 5a0b  m.....m.....m.Z.
+00000070: 0100 6405 6406 8400 5a0c 0902 6409 6407  ..d.d...Z...d.d.
+00000080: 6408 8401 5a0d 6402 5300 290a 6143 0100  d...Z.d.S.).aC..
+00000090: 000a 0923 0a09 2309 7772 6974 6520 7075  ...#..#.write pu
+000000a0: 626c 6963 206b 6579 2074 6f20 7061 7468  blic key to path
+000000b0: 0a09 230a 0969 6d70 6f72 7420 7265 6379  ..#..import recy
+000000c0: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+000000d0: 3434 385f 322e 7075 626c 6963 5f6b 6579  448_2.public_key
+000000e0: 2e63 7265 6174 6f72 2061 7320 4545 435f  .creator as EEC_
+000000f0: 3434 385f 325f 7075 626c 6963 5f6b 6579  448_2_public_key
+00000100: 5f63 7265 6174 6f72 0a09 7075 626c 6963  _creator..public
+00000110: 5f6b 6579 203d 2045 4543 5f34 3438 5f32  _key = EEC_448_2
+00000120: 5f70 7562 6c69 635f 6b65 795f 6372 6561  _public_key_crea
+00000130: 746f 722e 6372 6561 7465 2028 0a09 0970  tor.create (...p
+00000140: 7269 7661 7465 5f6b 6579 5f69 6e73 7461  rivate_key_insta
+00000150: 6e63 650a 0929 0a09 7075 626c 6963 5f6b  nce..)..public_k
+00000160: 6579 5f69 6e73 7461 6e63 6520 3d20 7075  ey_instance = pu
+00000170: 626c 6963 5f6b 6579 205b 2269 6e73 7461  blic_key ["insta
+00000180: 6e63 6522 5d0a 0970 7562 6c69 635f 6b65  nce"]..public_ke
+00000190: 795f 4445 525f 6865 7861 6465 6369 6d61  y_DER_hexadecima
+000001a0: 6c5f 7374 7269 6e67 203d 2070 7562 6c69  l_string = publi
+000001b0: 635f 6b65 7920 5b22 4445 5220 6865 7861  c_key ["DER hexa
+000001c0: 6465 6369 6d61 6c20 7374 7269 6e67 225d  decimal string"]
+000001d0: 0a09 090a e900 0000 004e 2901 da06 4563  .........N)...Ec
+000001e0: 634b 6579 2901 da03 4543 4363 0100 0000  cKey)...ECCc....
+000001f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000200: 4300 0000 732e 0000 007c 00a0 00a1 007d  C...s....|.....}
+00000210: 0174 017c 0183 0164 016b 0273 0c4a 0082  .t.|...d.k.s.J..
+00000220: 0174 02a0 037c 01a1 017c 006b 0273 154a  .t...|...|.k.s.J
+00000230: 0082 017c 0153 0029 024e e98a 0000 0029  ...|.S.).N.....)
+00000240: 04da 0368 6578 da03 6c65 6eda 0562 7974  ...hex..len..byt
+00000250: 6573 da07 6672 6f6d 6865 7829 02da 1a70  es..fromhex)...p
+00000260: 7562 6c69 635f 6b65 795f 4445 525f 6279  ublic_key_DER_by
+00000270: 7465 5f73 7472 696e 67da 2170 7562 6c69  te_string.!publi
+00000280: 635f 6b65 795f 4445 525f 6865 7861 6465  c_key_DER_hexade
+00000290: 6369 6d61 6c5f 7374 7269 6e67 a900 720b  cimal_string..r.
+000002a0: 0000 00fa 462f 6861 6269 7461 742f 7665  ....F/habitat/ve
+000002b0: 6e75 6573 2f73 7461 6765 732f 7265 6379  nues/stages/recy
+000002c0: 636c 696e 672f 6d69 7865 732f 4545 435f  cling/mixes/EEC_
+000002d0: 3434 385f 322f 7075 626c 6963 5f6b 6579  448_2/public_key
+000002e0: 2f63 7265 6174 6f72 2e70 79da 1d63 7265  /creator.py..cre
+000002f0: 6174 655f 4445 525f 6865 7861 6465 6369  ate_DER_hexadeci
+00000300: 6d61 6c5f 7374 7269 6e67 1c00 0000 730c  mal_string....s.
+00000310: 0000 0008 0110 0108 0202 0108 ff04 0472  ...............r
+00000320: 0d00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000330: 0005 0000 0005 0000 0043 0000 0073 3600  .........C...s6.
+00000340: 0000 7c00 a000 a100 7d01 7c01 6a01 6401  ..|.....}.|.j.d.
+00000350: 6402 8d01 7d02 7c01 6a01 6403 6402 8d01  d...}.|.j.d.d...
+00000360: 7d03 7402 7c02 8301 7d04 7c01 7c02 7c04  }.t.|...}.|.|.|.
+00000370: 7c03 6404 9c04 5300 2905 4eda 0344 4552  |.d...S.).N..DER
+00000380: 2901 da06 666f 726d 6174 da03 5045 4d29  )...format..PEM)
+00000390: 04da 0869 6e73 7461 6e63 657a 0f44 4552  ...instancez.DER
+000003a0: 2062 7974 6520 7374 7269 6e67 7a16 4445   byte stringz.DE
+000003b0: 5220 6865 7861 6465 6369 6d61 6c20 7374  R hexadecimal st
+000003c0: 7269 6e67 7a0a 5045 4d20 7374 7269 6e67  ringz.PEM string
+000003d0: 2903 da0a 7075 626c 6963 5f6b 6579 da0a  )...public_key..
+000003e0: 6578 706f 7274 5f6b 6579 720d 0000 0029  export_keyr....)
+000003f0: 05da 1470 7269 7661 7465 5f6b 6579 5f69  ...private_key_i
+00000400: 6e73 7461 6e63 65da 1370 7562 6c69 635f  nstance..public_
+00000410: 6b65 795f 696e 7374 616e 6365 7209 0000  key_instancer...
+00000420: 00da 1570 7562 6c69 635f 6b65 795f 5045  ...public_key_PE
+00000430: 4d5f 7374 7269 6e67 720a 0000 0072 0b00  M_stringr....r..
+00000440: 0000 720b 0000 0072 0c00 0000 da06 6372  ..r....r......cr
+00000450: 6561 7465 2600 0000 731e 0000 0008 0304  eate&...s.......
+00000460: 0102 0106 ff04 0302 0106 ff02 0402 0104  ................
+00000470: ff02 0502 0202 0102 0206 fa72 1700 0000  ...........r....
+00000480: 2901 4e29 0eda 075f 5f64 6f63 5f5f da02  ).N)...__doc__..
+00000490: 6f73 da14 4372 7970 746f 2e50 7562 6c69  os..Crypto.Publi
+000004a0: 634b 6579 2e45 4343 7202 0000 00da 1043  cKey.ECCr......C
+000004b0: 7279 7074 6f2e 5075 626c 6963 4b65 7972  rypto.PublicKeyr
+000004c0: 0300 0000 da2a 7265 6379 636c 696e 672e  .....*recycling.
+000004d0: 6d69 7865 732e 4545 435f 3434 385f 322e  mixes.EEC_448_2.
+000004e0: 7072 6976 6174 655f 6b65 792e 7363 616e  private_key.scan
+000004f0: da05 6d69 7865 73da 0945 4543 5f34 3438  ..mixes..EEC_448
+00000500: 5f32 da0b 7072 6976 6174 655f 6b65 79da  _2..private_key.
+00000510: 0473 6361 6eda 0c70 7269 7661 7465 5f73  .scan..private_s
+00000520: 6361 6e72 0d00 0000 7217 0000 0072 0b00  canr....r....r..
+00000530: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000540: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000550: 1200 0000 0401 020d 0805 0c02 0c01 1e02  ................
+00000560: 0803 020b 0eff                           ......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/scan.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9b02 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 9902 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
-00000040: 6404 8400 5a03 6405 5300 2906 7aac 0a09  d...Z.d.S.).z...
+00000040: 6404 8400 5a03 6405 5300 2906 7aaa 0a09  d...Z.d.S.).z...
 00000050: 6672 6f6d 2072 6563 7963 6c69 6e67 2e6d  from recycling.m
-00000060: 6f64 756c 6573 2e45 4543 5f34 3438 5f31  odules.EEC_448_1
-00000070: 2e70 7562 6c69 635f 6b65 792e 7363 616e  .public_key.scan
-00000080: 2069 6d70 6f72 7420 7363 616e 5f70 7562   import scan_pub
-00000090: 6c69 635f 6b65 790a 095b 2070 7562 6c69  lic_key..[ publi
-000000a0: 635f 6b65 795f 696e 7374 616e 6365 2c20  c_key_instance, 
-000000b0: 7075 626c 6963 5f6b 6579 5f62 7974 6573  public_key_bytes
-000000c0: 2c20 7075 626c 6963 5f6b 6579 5f73 7472  , public_key_str
-000000d0: 696e 6720 5d20 3d20 7363 616e 5f70 7562  ing ] = scan_pub
-000000e0: 6c69 635f 6b65 7920 2870 7562 6c69 635f  lic_key (public_
-000000f0: 6b65 795f 7061 7468 290a e900 0000 0029  key_path)......)
-00000100: 01da 0345 4343 6301 0000 0000 0000 0000  ...ECCc.........
-00000110: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00000120: 5c00 0000 7400 7c00 6401 6402 8d02 8f1c  \...t.|.d.d.....
-00000130: 7d01 7c01 a001 a100 7d02 7402 6a03 7c02  }.|.....}.t.j.|.
-00000140: 6403 6404 8d02 7d03 7c02 a004 a100 7d04  d.d...}.|.....}.
-00000150: 7c03 7c02 7c04 6703 5700 0200 6400 0400  |.|.|.g.W...d...
-00000160: 0400 8303 0100 5300 3100 7325 7701 0100  ......S.1.s%w...
-00000170: 0100 0100 5900 0100 7405 6405 8301 8201  ....Y...t.d.....
-00000180: 2906 4eda 0272 6229 01da 046d 6f64 65da  ).N..rb)...mode.
-00000190: 0545 6434 3438 2901 da0a 6375 7276 655f  .Ed448)...curve_
-000001a0: 6e61 6d65 da00 2906 da04 6f70 656e da04  name..)...open..
-000001b0: 7265 6164 7202 0000 00da 0a69 6d70 6f72  readr......impor
-000001c0: 745f 6b65 79da 0368 6578 da09 4578 6365  t_key..hex..Exce
-000001d0: 7074 696f 6e29 05da 0470 6174 68da 0466  ption)...path..f
-000001e0: 696c 65da 1070 7562 6c69 635f 6b65 795f  ile..public_key_
-000001f0: 6279 7465 73da 0a70 7562 6c69 635f 6b65  bytes..public_ke
-00000200: 79da 1170 7562 6c69 635f 6b65 795f 7374  y..public_key_st
-00000210: 7269 6e67 a900 7212 0000 00fa 452f 6861  ring..r.....E/ha
-00000220: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
-00000230: 6765 732f 7265 6379 636c 696e 672f 6d6f  ges/recycling/mo
-00000240: 6475 6c65 732f 4545 435f 3434 385f 312f  dules/EEC_448_1/
-00000250: 7075 626c 6963 5f6b 6579 2f73 6361 6e2e  public_key/scan.
-00000260: 7079 da0f 7363 616e 5f70 7562 6c69 635f  py..scan_public_
-00000270: 6b65 7911 0000 0073 1a00 0000 0e01 0801  key....s........
-00000280: 0402 0201 0201 06fe 0805 0203 0201 0201  ................
-00000290: 02fd 20f6 0810 7214 0000 004e 2904 da07  .. ...r....N)...
-000002a0: 5f5f 646f 635f 5fda 1043 7279 7074 6f2e  __doc__..Crypto.
-000002b0: 5075 626c 6963 4b65 7972 0200 0000 7214  PublicKeyr....r.
-000002c0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-000002d0: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002e0: 3e01 0000 0073 0600 0000 0403 0c0a 0c03  >....s..........
+00000060: 6978 6573 2e45 4543 5f34 3438 5f31 2e70  ixes.EEC_448_1.p
+00000070: 7562 6c69 635f 6b65 792e 7363 616e 2069  ublic_key.scan i
+00000080: 6d70 6f72 7420 7363 616e 5f70 7562 6c69  mport scan_publi
+00000090: 635f 6b65 790a 095b 2070 7562 6c69 635f  c_key..[ public_
+000000a0: 6b65 795f 696e 7374 616e 6365 2c20 7075  key_instance, pu
+000000b0: 626c 6963 5f6b 6579 5f62 7974 6573 2c20  blic_key_bytes, 
+000000c0: 7075 626c 6963 5f6b 6579 5f73 7472 696e  public_key_strin
+000000d0: 6720 5d20 3d20 7363 616e 5f70 7562 6c69  g ] = scan_publi
+000000e0: 635f 6b65 7920 2870 7562 6c69 635f 6b65  c_key (public_ke
+000000f0: 795f 7061 7468 290a e900 0000 0029 01da  y_path)......)..
+00000100: 0345 4343 6301 0000 0000 0000 0000 0000  .ECCc...........
+00000110: 0005 0000 0008 0000 0043 0000 0073 5c00  .........C...s\.
+00000120: 0000 7400 7c00 6401 6402 8d02 8f1c 7d01  ..t.|.d.d.....}.
+00000130: 7c01 a001 a100 7d02 7402 6a03 7c02 6403  |.....}.t.j.|.d.
+00000140: 6404 8d02 7d03 7c02 a004 a100 7d04 7c03  d...}.|.....}.|.
+00000150: 7c02 7c04 6703 5700 0200 6400 0400 0400  |.|.g.W...d.....
+00000160: 8303 0100 5300 3100 7325 7701 0100 0100  ....S.1.s%w.....
+00000170: 0100 5900 0100 7405 6405 8301 8201 2906  ..Y...t.d.....).
+00000180: 4eda 0272 6229 01da 046d 6f64 65da 0545  N..rb)...mode..E
+00000190: 6434 3438 2901 da0a 6375 7276 655f 6e61  d448)...curve_na
+000001a0: 6d65 da00 2906 da04 6f70 656e da04 7265  me..)...open..re
+000001b0: 6164 7202 0000 00da 0a69 6d70 6f72 745f  adr......import_
+000001c0: 6b65 79da 0368 6578 da09 4578 6365 7074  key..hex..Except
+000001d0: 696f 6e29 05da 0470 6174 68da 0466 696c  ion)...path..fil
+000001e0: 65da 1070 7562 6c69 635f 6b65 795f 6279  e..public_key_by
+000001f0: 7465 73da 0a70 7562 6c69 635f 6b65 79da  tes..public_key.
+00000200: 1170 7562 6c69 635f 6b65 795f 7374 7269  .public_key_stri
+00000210: 6e67 a900 7212 0000 00fa 432f 6861 6269  ng..r.....C/habi
+00000220: 7461 742f 7665 6e75 6573 2f73 7461 6765  tat/venues/stage
+00000230: 732f 7265 6379 636c 696e 672f 6d69 7865  s/recycling/mixe
+00000240: 732f 4545 435f 3434 385f 312f 7075 626c  s/EEC_448_1/publ
+00000250: 6963 5f6b 6579 2f73 6361 6e2e 7079 da0f  ic_key/scan.py..
+00000260: 7363 616e 5f70 7562 6c69 635f 6b65 7911  scan_public_key.
+00000270: 0000 0073 1a00 0000 0e01 0801 0402 0201  ...s............
+00000280: 0201 06fe 0805 0203 0201 0201 02fd 20f6  .............. .
+00000290: 0810 7214 0000 004e 2904 da07 5f5f 646f  ..r....N)...__do
+000002a0: 635f 5fda 1043 7279 7074 6f2e 5075 626c  c__..Crypto.Publ
+000002b0: 6963 4b65 7972 0200 0000 7214 0000 0072  icKeyr....r....r
+000002c0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+000002d0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000002e0: 0073 0600 0000 0403 0c0a 0c03            .s..........
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/__pycache__/write.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/__pycache__/write.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 4302 0000  o........@@fC...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 4102 0000  o........SQfA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6403 6404 8400  Z.d.d.l.Z.d.d...
-00000040: 5a02 6402 5300 2905 7aac 0a09 696d 706f  Z.d.S.).z...impo
-00000050: 7274 2072 6563 7963 6c69 6e67 2e6d 6f64  rt recycling.mod
-00000060: 756c 6573 2e45 4543 5f34 3438 5f31 2e70  ules.EEC_448_1.p
-00000070: 7562 6c69 635f 6b65 792e 7772 6974 6520  ublic_key.write 
-00000080: 6173 2077 7269 7465 5f45 4543 5f34 3438  as write_EEC_448
-00000090: 5f31 5f70 7562 6c69 635f 6b65 790a 0977  _1_public_key..w
-000000a0: 7269 7465 5f45 4543 5f34 3438 5f31 5f70  rite_EEC_448_1_p
-000000b0: 7562 6c69 635f 6b65 792e 736d 6f6f 7468  ublic_key.smooth
-000000c0: 6c79 2028 0a09 0970 6174 6820 3d20 2222  ly (...path = ""
-000000d0: 2c0a 0909 6b65 795f 7374 7269 6e67 203d  ,...key_string =
-000000e0: 2022 222c 0a09 0966 6f72 6d61 7420 3d20   "",...format = 
-000000f0: 2222 0a09 290a e900 0000 004e 6303 0000  ""..)......Nc...
-00000100: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000110: 0043 0000 0073 6a00 0000 7400 6a01 a002  .C...sj...t.j...
-00000120: 7c00 a101 720e 7403 6401 7c00 9b00 6402  |...r.t.d.|...d.
-00000130: 9d03 8301 8201 7c02 6403 6b02 7218 7404  ......|.d.k.r.t.
-00000140: 7c00 6404 8302 7d03 6e12 7c02 6405 7600  |.d...}.n.|.d.v.
-00000150: 7222 7404 7c00 6406 8302 7d03 6e08 7403  r"t.|.d...}.n.t.
-00000160: 6407 7c02 9b00 6408 9d03 8301 8201 7c03  d.|...d.......|.
-00000170: a005 7c01 a101 0100 7c03 a006 a100 0100  ..|.....|.......
-00000180: 6400 5300 2909 4e7a 1d54 6865 2070 6174  d.S.).Nz.The pat
-00000190: 6820 666f 7220 7468 6520 7075 626c 6963  h for the public
-000001a0: 206b 6579 2027 7a13 2720 6973 206e 6f74   key 'z.' is not
-000001b0: 2061 7661 696c 6162 6c65 2eda 0344 4552   available...DER
-000001c0: da02 7762 2902 da03 5045 4dda 0b68 6578  ..wb)...PEM..hex
-000001d0: 6164 6563 696d 616c da01 777a 0866 6f72  adecimal..wz.for
-000001e0: 6d61 7420 277a 1827 2077 6173 206e 6f74  mat 'z.' was not
-000001f0: 2061 6363 6f75 6e74 6564 2066 6f72 2e29   accounted for.)
-00000200: 07da 026f 73da 0470 6174 68da 0665 7869  ...os..path..exi
-00000210: 7374 73da 0945 7863 6570 7469 6f6e da04  sts..Exception..
-00000220: 6f70 656e da05 7772 6974 65da 0563 6c6f  open..write..clo
-00000230: 7365 2904 7208 0000 00da 0a6b 6579 5f73  se).r......key_s
-00000240: 7472 696e 67da 0666 6f72 6d61 74da 0166  tring..format..f
-00000250: a900 7211 0000 00fa 462f 6861 6269 7461  ..r.....F/habita
-00000260: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-00000270: 7265 6379 636c 696e 672f 6d6f 6475 6c65  recycling/module
-00000280: 732f 4545 435f 3434 385f 312f 7075 626c  s/EEC_448_1/publ
-00000290: 6963 5f6b 6579 2f77 7269 7465 2e70 79da  ic_key/write.py.
-000002a0: 0873 6d6f 6f74 686c 7910 0000 0073 1600  .smoothly....s..
-000002b0: 0000 0c01 0201 0a01 04ff 0804 0c01 0801  ................
-000002c0: 0c01 1002 0a02 0c01 7213 0000 0029 03da  ........r....)..
-000002d0: 075f 5f64 6f63 5f5f 7207 0000 0072 1300  .__doc__r....r..
-000002e0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-000002f0: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000300: 0100 0000 7306 0000 0004 0408 090c 02    ....s..........
+00000040: 5a02 6402 5300 2905 7aaa 0a09 696d 706f  Z.d.S.).z...impo
+00000050: 7274 2072 6563 7963 6c69 6e67 2e6d 6978  rt recycling.mix
+00000060: 6573 2e45 4543 5f34 3438 5f31 2e70 7562  es.EEC_448_1.pub
+00000070: 6c69 635f 6b65 792e 7772 6974 6520 6173  lic_key.write as
+00000080: 2077 7269 7465 5f45 4543 5f34 3438 5f31   write_EEC_448_1
+00000090: 5f70 7562 6c69 635f 6b65 790a 0977 7269  _public_key..wri
+000000a0: 7465 5f45 4543 5f34 3438 5f31 5f70 7562  te_EEC_448_1_pub
+000000b0: 6c69 635f 6b65 792e 736d 6f6f 7468 6c79  lic_key.smoothly
+000000c0: 2028 0a09 0970 6174 6820 3d20 2222 2c0a   (...path = "",.
+000000d0: 0909 6b65 795f 7374 7269 6e67 203d 2022  ..key_string = "
+000000e0: 222c 0a09 0966 6f72 6d61 7420 3d20 2222  ",...format = ""
+000000f0: 0a09 290a e900 0000 004e 6303 0000 0000  ..)......Nc.....
+00000100: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00000110: 0000 0073 6a00 0000 7400 6a01 a002 7c00  ...sj...t.j...|.
+00000120: a101 720e 7403 6401 7c00 9b00 6402 9d03  ..r.t.d.|...d...
+00000130: 8301 8201 7c02 6403 6b02 7218 7404 7c00  ....|.d.k.r.t.|.
+00000140: 6404 8302 7d03 6e12 7c02 6405 7600 7222  d...}.n.|.d.v.r"
+00000150: 7404 7c00 6406 8302 7d03 6e08 7403 6407  t.|.d...}.n.t.d.
+00000160: 7c02 9b00 6408 9d03 8301 8201 7c03 a005  |...d.......|...
+00000170: 7c01 a101 0100 7c03 a006 a100 0100 6400  |.....|.......d.
+00000180: 5300 2909 4e7a 1d54 6865 2070 6174 6820  S.).Nz.The path 
+00000190: 666f 7220 7468 6520 7075 626c 6963 206b  for the public k
+000001a0: 6579 2027 7a13 2720 6973 206e 6f74 2061  ey 'z.' is not a
+000001b0: 7661 696c 6162 6c65 2eda 0344 4552 da02  vailable...DER..
+000001c0: 7762 2902 da03 5045 4dda 0b68 6578 6164  wb)...PEM..hexad
+000001d0: 6563 696d 616c da01 777a 0866 6f72 6d61  ecimal..wz.forma
+000001e0: 7420 277a 1827 2077 6173 206e 6f74 2061  t 'z.' was not a
+000001f0: 6363 6f75 6e74 6564 2066 6f72 2e29 07da  ccounted for.)..
+00000200: 026f 73da 0470 6174 68da 0665 7869 7374  .os..path..exist
+00000210: 73da 0945 7863 6570 7469 6f6e da04 6f70  s..Exception..op
+00000220: 656e da05 7772 6974 65da 0563 6c6f 7365  en..write..close
+00000230: 2904 7208 0000 00da 0a6b 6579 5f73 7472  ).r......key_str
+00000240: 696e 67da 0666 6f72 6d61 74da 0166 a900  ing..format..f..
+00000250: 7211 0000 00fa 442f 6861 6269 7461 742f  r.....D/habitat/
+00000260: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+00000270: 6379 636c 696e 672f 6d69 7865 732f 4545  cycling/mixes/EE
+00000280: 435f 3434 385f 312f 7075 626c 6963 5f6b  C_448_1/public_k
+00000290: 6579 2f77 7269 7465 2e70 79da 0873 6d6f  ey/write.py..smo
+000002a0: 6f74 686c 7910 0000 0073 1600 0000 0c01  othly....s......
+000002b0: 0201 0a01 04ff 0804 0c01 0801 0c01 1002  ................
+000002c0: 0a02 0c01 7213 0000 0029 03da 075f 5f64  ....r....)...__d
+000002d0: 6f63 5f5f 7207 0000 0072 1300 0000 7211  oc__r....r....r.
+000002e0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+000002f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000300: 7306 0000 0004 0408 090c 02              s..........
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/creator.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/creator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 '''
 	#
 	#	write public key to path
 	#
-	import recycling.modules.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
+	import recycling.mixes.EEC_448_1.public_key.creator as EEC_448_1_public_key_creator
 	public_key = EEC_448_1_public_key_creator.create (
 		private_key_path = "",
 		
 		public_key_path = "",
 		public_key_format = ""
 	)
 	public_key_instance = public_key ["instance"]
@@ -21,15 +21,15 @@
 		PEM
 '''
 import os
 
 from Crypto.PublicKey.ECC import EccKey
 from Crypto.PublicKey import ECC
 
-import recycling.modules.EEC_448_1.private_key.scan as private_scan
+import recycling.mixes.EEC_448_1.private_key.scan as private_scan
 
 def write_public_key (path, key_string, format):
 	if (os.path.exists (path)):
 		raise Exception (
 			f"The path for the public key '{ path }' is not available."
 		)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/form.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/form.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 '''
-	import recycling.modules.EEC_448_1.public_key.form as form_EEC_448_1_public_key
+	import recycling.mixes.EEC_448_1.public_key.form as form_EEC_448_1_public_key
 	public_key = form_EEC_448_1_public_key.smoothly (
 		private_key_instance = None
 	)
 	public_key_instance = public_key ["instance"]
 	public_key_DER_string = public_key ["DER"]
 	public_key_hexadecimal_string = public_key ["hexadecimal"]
 		
 '''
 
 import os
 
 from Crypto.PublicKey.ECC import EccKey
 from Crypto.PublicKey import ECC
 
-import recycling.modules.EEC_448_1.private_key.scan as private_scan
+import recycling.mixes.EEC_448_1.private_key.scan as private_scan
 
 def smoothly (
 	private_key_instance = None
 ):	
 	#private_key = private_scan.start (private_key_path)
 
 	public_key_instance = private_key_instance.public_key ()
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/scan.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 '''
-	from recycling.modules.EEC_448_1.public_key.scan import scan_public_key
+	from recycling.mixes.EEC_448_1.public_key.scan import scan_public_key
 	[ public_key_instance, public_key_bytes, public_key_string ] = scan_public_key (public_key_path)
 '''
 
 
 #
 #	https://pycryptodome.readthedocs.io/en/latest/src/public_key/ecc.html#Crypto.PublicKey.ECC.import_key
 #
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/public_key/write.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/public_key/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 
 
 '''
-	import recycling.modules.EEC_448_1.public_key.write as write_EEC_448_1_public_key
+	import recycling.mixes.EEC_448_1.public_key.write as write_EEC_448_1_public_key
 	write_EEC_448_1_public_key.smoothly (
 		path = "",
 		key_string = "",
 		format = ""
 	)
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/sign/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/sign/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 
 '''
-	import recycling.modules.EEC_448_1.sign as sign
+	import recycling.mixes.EEC_448_1.sign as sign
 	signed = sign.start (
 		private_key_string,
 		unsigned_bytes = unsigned_bytes
 	)
 	
 	signed_bytes = signed.bytes
 '''
 
 from Crypto.PublicKey import ECC
 from Crypto.Signature import eddsa
 
-import recycling.modules.EEC_448_1.private_key.scan as private_scan
+import recycling.mixes.EEC_448_1.private_key.scan as private_scan
 
 def WRITE (PATH, SIGNED_MESSAGE):
 	import os.path
 	if (os.path.exists (PATH)):
 		print ("PATH FOR SIGNED MESSAGE ISN'T EMPTY, EXITING.");
 		exit ()
 		return False;
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/sign/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/sign/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 938 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 aa03 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 a603 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 0200 0100 6d07 0200 0100 6d08 0200  m.....m.....m...
 00000060: 0100 6d09 5a0a 0100 6405 6406 8400 5a0b  ..m.Z...d.d...Z.
 00000070: 0904 0904 6409 6407 6408 8401 5a0c 6404  ....d.d.d...Z.d.
-00000080: 5300 290a 7aa3 0a09 696d 706f 7274 2072  S.).z...import r
-00000090: 6563 7963 6c69 6e67 2e6d 6f64 756c 6573  ecycling.modules
-000000a0: 2e45 4543 5f34 3438 5f31 2e73 6967 6e20  .EEC_448_1.sign 
-000000b0: 6173 2073 6967 6e0a 0973 6967 6e65 6420  as sign..signed 
-000000c0: 3d20 7369 676e 2e73 7461 7274 2028 0a09  = sign.start (..
-000000d0: 0970 7269 7661 7465 5f6b 6579 5f73 7472  .private_key_str
-000000e0: 696e 672c 0a09 0975 6e73 6967 6e65 645f  ing,...unsigned_
-000000f0: 6279 7465 7320 3d20 756e 7369 676e 6564  bytes = unsigned
-00000100: 5f62 7974 6573 0a09 290a 090a 0973 6967  _bytes..)....sig
-00000110: 6e65 645f 6279 7465 7320 3d20 7369 676e  ned_bytes = sign
-00000120: 6564 2e62 7974 6573 0ae9 0000 0000 2901  ed.bytes......).
-00000130: da03 4543 4329 01da 0565 6464 7361 4e63  ..ECC)...eddsaNc
-00000140: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000150: 0300 0000 4300 0000 7346 0000 0064 0164  ....C...sF...d.d
-00000160: 006c 007d 027c 026a 01a0 027c 00a1 0172  .l.}.|.j...|...r
-00000170: 1374 0364 0283 0101 0074 0483 0001 0064  .t.d.....t.....d
-00000180: 0353 0074 057c 0064 0483 027d 037c 03a0  .S.t.|.d...}.|..
-00000190: 067c 01a1 0101 007c 03a0 07a1 0001 0064  .|.....|.......d
-000001a0: 0053 0029 054e 7201 0000 007a 2d50 4154  .S.).Nr....z-PAT
-000001b0: 4820 464f 5220 5349 474e 4544 204d 4553  H FOR SIGNED MES
-000001c0: 5341 4745 2049 534e 2754 2045 4d50 5459  SAGE ISN'T EMPTY
-000001d0: 2c20 4558 4954 494e 472e 46da 0277 6229  , EXITING.F..wb)
-000001e0: 08da 076f 732e 7061 7468 da04 7061 7468  ...os.path..path
-000001f0: da06 6578 6973 7473 da05 7072 696e 74da  ..exists..print.
-00000200: 0465 7869 74da 046f 7065 6eda 0577 7269  .exit..open..wri
-00000210: 7465 da05 636c 6f73 6529 04da 0450 4154  te..close)...PAT
-00000220: 48da 0e53 4947 4e45 445f 4d45 5353 4147  H..SIGNED_MESSAG
-00000230: 45da 026f 73da 0166 a900 7211 0000 00fa  E..os..f..r.....
-00000240: 432f 6861 6269 7461 742f 7665 6e75 6573  C/habitat/venues
-00000250: 2f73 7461 6765 732f 7265 6379 636c 696e  /stages/recyclin
-00000260: 672f 6d6f 6475 6c65 732f 4545 435f 3434  g/modules/EEC_44
-00000270: 385f 312f 7369 676e 2f5f 5f69 6e69 745f  8_1/sign/__init_
-00000280: 5f2e 7079 da05 5752 4954 4512 0000 0073  _.py..WRITE....s
-00000290: 1000 0000 0801 0c01 0801 0601 0401 0a02  ................
-000002a0: 0a01 0c01 7213 0000 0063 0200 0000 0000  ....r....c......
-000002b0: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
-000002c0: 0000 7338 0000 0074 00a0 017c 00a1 017d  ..s8...t...|...}
-000002d0: 0274 02a0 037c 026a 0464 01a1 027d 037c  .t...|.j.d...}.|
-000002e0: 03a0 057c 01a1 017d 0447 0064 0264 0384  ...|...}.G.d.d..
-000002f0: 0064 0383 027d 057c 057c 0483 0153 0029  .d...}.|.|...S.)
-00000300: 044e da07 7266 6338 3033 3263 0000 0000  .N..rfc8032c....
-00000310: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000320: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000330: 0264 0164 0284 005a 0364 0353 0029 047a  .d.d...Z.d.S.).z
-00000340: 1573 7461 7274 2e3c 6c6f 6361 6c73 3e2e  .start.<locals>.
-00000350: 7369 676e 6564 6302 0000 0000 0000 0000  signedc.........
-00000360: 0000 0002 0000 0002 0000 0053 0000 0073  ...........S...s
-00000370: 0a00 0000 7c01 7c00 5f00 6400 5300 2901  ....|.|._.d.S.).
-00000380: 4e29 01da 0562 7974 6573 2902 da04 7468  N)...bytes)...th
-00000390: 6973 da0c 7369 676e 6564 5f62 7974 6573  is..signed_bytes
-000003a0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-000003b0: 085f 5f69 6e69 745f 5f2b 0000 0073 0200  .__init__+...s..
-000003c0: 0000 0a01 7a1e 7374 6172 742e 3c6c 6f63  ....z.start.<loc
-000003d0: 616c 733e 2e73 6967 6e65 642e 5f5f 696e  als>.signed.__in
-000003e0: 6974 5f5f 4e29 04da 085f 5f6e 616d 655f  it__N)...__name_
-000003f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000400: 5f71 7561 6c6e 616d 655f 5f72 1800 0000  _qualname__r....
-00000410: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000420: 1200 0000 da06 7369 676e 6564 2a00 0000  ......signed*...
-00000430: 7304 0000 0008 000c 0172 1c00 0000 2906  s........r....).
-00000440: da0c 7072 6976 6174 655f 7363 616e da05  ..private_scan..
-00000450: 7374 6172 7472 0300 0000 da03 6e65 77da  startr......new.
-00000460: 0869 6e73 7461 6e63 65da 0473 6967 6e29  .instance..sign)
-00000470: 06da 1070 7269 7661 7465 5f6b 6579 5f70  ...private_key_p
-00000480: 6174 68da 0e75 6e73 6967 6e65 645f 6279  ath..unsigned_by
-00000490: 7465 73da 0b70 7269 7661 7465 5f6b 6579  tes..private_key
-000004a0: da06 7369 676e 6572 7217 0000 0072 1c00  ..signerr....r..
-000004b0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000004c0: 0072 1e00 0000 1e00 0000 730e 0000 000a  .r........s.....
-000004d0: 040e 020a 010e 0502 0402 0104 ff72 1e00  .............r..
-000004e0: 0000 2902 4e4e 290d da07 5f5f 646f 635f  ..).NN)...__doc_
-000004f0: 5fda 1043 7279 7074 6f2e 5075 626c 6963  _..Crypto.Public
-00000500: 4b65 7972 0200 0000 da10 4372 7970 746f  Keyr......Crypto
-00000510: 2e53 6967 6e61 7475 7265 7203 0000 00da  .Signaturer.....
-00000520: 2c72 6563 7963 6c69 6e67 2e6d 6f64 756c  ,recycling.modul
-00000530: 6573 2e45 4543 5f34 3438 5f31 2e70 7269  es.EEC_448_1.pri
-00000540: 7661 7465 5f6b 6579 2e73 6361 6eda 076d  vate_key.scan..m
-00000550: 6f64 756c 6573 da09 4545 435f 3434 385f  odules..EEC_448_
-00000560: 3172 2400 0000 da04 7363 616e 721d 0000  1r$.....scanr...
-00000570: 0072 1300 0000 721e 0000 0072 1100 0000  .r....r....r....
-00000580: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000590: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
-000005a0: 0000 0402 0c0a 0c01 1e02 0802 020d 0201  ................
-000005b0: 0efe                                     ..
+00000080: 5300 290a 7aa1 0a09 696d 706f 7274 2072  S.).z...import r
+00000090: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+000000a0: 4543 5f34 3438 5f31 2e73 6967 6e20 6173  EC_448_1.sign as
+000000b0: 2073 6967 6e0a 0973 6967 6e65 6420 3d20   sign..signed = 
+000000c0: 7369 676e 2e73 7461 7274 2028 0a09 0970  sign.start (...p
+000000d0: 7269 7661 7465 5f6b 6579 5f73 7472 696e  rivate_key_strin
+000000e0: 672c 0a09 0975 6e73 6967 6e65 645f 6279  g,...unsigned_by
+000000f0: 7465 7320 3d20 756e 7369 676e 6564 5f62  tes = unsigned_b
+00000100: 7974 6573 0a09 290a 090a 0973 6967 6e65  ytes..)....signe
+00000110: 645f 6279 7465 7320 3d20 7369 676e 6564  d_bytes = signed
+00000120: 2e62 7974 6573 0ae9 0000 0000 2901 da03  .bytes......)...
+00000130: 4543 4329 01da 0565 6464 7361 4e63 0200  ECC)...eddsaNc..
+00000140: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+00000150: 0000 4300 0000 7346 0000 0064 0164 006c  ..C...sF...d.d.l
+00000160: 007d 027c 026a 01a0 027c 00a1 0172 1374  .}.|.j...|...r.t
+00000170: 0364 0283 0101 0074 0483 0001 0064 0353  .d.....t.....d.S
+00000180: 0074 057c 0064 0483 027d 037c 03a0 067c  .t.|.d...}.|...|
+00000190: 01a1 0101 007c 03a0 07a1 0001 0064 0053  .....|.......d.S
+000001a0: 0029 054e 7201 0000 007a 2d50 4154 4820  .).Nr....z-PATH 
+000001b0: 464f 5220 5349 474e 4544 204d 4553 5341  FOR SIGNED MESSA
+000001c0: 4745 2049 534e 2754 2045 4d50 5459 2c20  GE ISN'T EMPTY, 
+000001d0: 4558 4954 494e 472e 46da 0277 6229 08da  EXITING.F..wb)..
+000001e0: 076f 732e 7061 7468 da04 7061 7468 da06  .os.path..path..
+000001f0: 6578 6973 7473 da05 7072 696e 74da 0465  exists..print..e
+00000200: 7869 74da 046f 7065 6eda 0577 7269 7465  xit..open..write
+00000210: da05 636c 6f73 6529 04da 0450 4154 48da  ..close)...PATH.
+00000220: 0e53 4947 4e45 445f 4d45 5353 4147 45da  .SIGNED_MESSAGE.
+00000230: 026f 73da 0166 a900 7211 0000 00fa 412f  .os..f..r.....A/
+00000240: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
+00000250: 7461 6765 732f 7265 6379 636c 696e 672f  tages/recycling/
+00000260: 6d69 7865 732f 4545 435f 3434 385f 312f  mixes/EEC_448_1/
+00000270: 7369 676e 2f5f 5f69 6e69 745f 5f2e 7079  sign/__init__.py
+00000280: da05 5752 4954 4512 0000 0073 1000 0000  ..WRITE....s....
+00000290: 0801 0c01 0801 0601 0401 0a02 0a01 0c01  ................
+000002a0: 7213 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000002b0: 0000 0600 0000 0400 0000 4300 0000 7338  ..........C...s8
+000002c0: 0000 0074 00a0 017c 00a1 017d 0274 02a0  ...t...|...}.t..
+000002d0: 037c 026a 0464 01a1 027d 037c 03a0 057c  .|.j.d...}.|...|
+000002e0: 01a1 017d 0447 0064 0264 0384 0064 0383  ...}.G.d.d...d..
+000002f0: 027d 057c 057c 0483 0153 0029 044e da07  .}.|.|...S.).N..
+00000300: 7266 6338 3033 3263 0000 0000 0000 0000  rfc8032c........
+00000310: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00000320: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+00000330: 0284 005a 0364 0353 0029 047a 1573 7461  ...Z.d.S.).z.sta
+00000340: 7274 2e3c 6c6f 6361 6c73 3e2e 7369 676e  rt.<locals>.sign
+00000350: 6564 6302 0000 0000 0000 0000 0000 0002  edc.............
+00000360: 0000 0002 0000 0053 0000 0073 0a00 0000  .......S...s....
+00000370: 7c01 7c00 5f00 6400 5300 2901 4e29 01da  |.|._.d.S.).N)..
+00000380: 0562 7974 6573 2902 da04 7468 6973 da0c  .bytes)...this..
+00000390: 7369 676e 6564 5f62 7974 6573 7211 0000  signed_bytesr...
+000003a0: 0072 1100 0000 7212 0000 00da 085f 5f69  .r....r......__i
+000003b0: 6e69 745f 5f2b 0000 0073 0200 0000 0a01  nit__+...s......
+000003c0: 7a1e 7374 6172 742e 3c6c 6f63 616c 733e  z.start.<locals>
+000003d0: 2e73 6967 6e65 642e 5f5f 696e 6974 5f5f  .signed.__init__
+000003e0: 4e29 04da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000003f0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000400: 6c6e 616d 655f 5f72 1800 0000 7211 0000  lname__r....r...
+00000410: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000420: da06 7369 676e 6564 2a00 0000 7304 0000  ..signed*...s...
+00000430: 0008 000c 0172 1c00 0000 2906 da0c 7072  .....r....)...pr
+00000440: 6976 6174 655f 7363 616e da05 7374 6172  ivate_scan..star
+00000450: 7472 0300 0000 da03 6e65 77da 0869 6e73  tr......new..ins
+00000460: 7461 6e63 65da 0473 6967 6e29 06da 1070  tance..sign)...p
+00000470: 7269 7661 7465 5f6b 6579 5f70 6174 68da  rivate_key_path.
+00000480: 0e75 6e73 6967 6e65 645f 6279 7465 73da  .unsigned_bytes.
+00000490: 0b70 7269 7661 7465 5f6b 6579 da06 7369  .private_key..si
+000004a0: 676e 6572 7217 0000 0072 1c00 0000 7211  gnerr....r....r.
+000004b0: 0000 0072 1100 0000 7212 0000 0072 1e00  ...r....r....r..
+000004c0: 0000 1e00 0000 730e 0000 000a 040e 020a  ......s.........
+000004d0: 010e 0502 0402 0104 ff72 1e00 0000 2902  .........r....).
+000004e0: 4e4e 290d da07 5f5f 646f 635f 5fda 1043  NN)...__doc__..C
+000004f0: 7279 7074 6f2e 5075 626c 6963 4b65 7972  rypto.PublicKeyr
+00000500: 0200 0000 da10 4372 7970 746f 2e53 6967  ......Crypto.Sig
+00000510: 6e61 7475 7265 7203 0000 00da 2a72 6563  naturer.....*rec
+00000520: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000530: 5f34 3438 5f31 2e70 7269 7661 7465 5f6b  _448_1.private_k
+00000540: 6579 2e73 6361 6eda 056d 6978 6573 da09  ey.scan..mixes..
+00000550: 4545 435f 3434 385f 3172 2400 0000 da04  EEC_448_1r$.....
+00000560: 7363 616e 721d 0000 0072 1300 0000 721e  scanr....r....r.
+00000570: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
+00000580: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000590: 3e01 0000 0073 1000 0000 0402 0c0a 0c01  >....s..........
+000005a0: 1e02 0802 020d 0201 0efe                 ..........
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/tutorial.s.HTML` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/verify/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/verify/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 
 '''
 	{ verify, approve, validate, certify, vouch }
 '''
 
 '''
-	import recycling.modules.EEC_448_1.verify as verify
+	import recycling.mixes.EEC_448_1.verify as verify
 	verified = verify.start (
 		public_key_string,
 		
 		signed_bytes = signed_bytes,
 		unsigned_bytes = unsigned_bytes
 	)
 '''
 
 from Crypto.Signature import eddsa
 from Crypto.PublicKey import ECC
 
-from recycling.modules.EEC_448_1.public_key.scan import scan_public_key
+from recycling.mixes.EEC_448_1.public_key.scan import scan_public_key
 
 def start (
 	#public_key_string = None,
 	public_key_path = None,
 	
 	unsigned_bytes = None,
 	signed_bytes = None
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_1/verify/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_1/verify/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 838 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 4603 0000  o........@@fF...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 4203 0000  o........SQfB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 0905 0905 0905 6408  l.m.Z.........d.
 00000060: 6406 6407 8401 5a07 6405 5300 2909 7a30  d.d...Z.d.S.).z0
 00000070: 0a09 7b20 7665 7269 6679 2c20 6170 7072  ..{ verify, appr
@@ -24,26 +24,26 @@
 00000170: da0f 7075 626c 6963 5f6b 6579 5f70 6174  ..public_key_pat
 00000180: 68da 0e75 6e73 6967 6e65 645f 6279 7465  h..unsigned_byte
 00000190: 73da 0c73 6967 6e65 645f 6279 7465 73da  s..signed_bytes.
 000001a0: 1370 7562 6c69 635f 6b65 795f 696e 7374  .public_key_inst
 000001b0: 616e 6365 da10 7075 626c 6963 5f6b 6579  ance..public_key
 000001c0: 5f62 7974 6573 da11 7075 626c 6963 5f6b  _bytes..public_k
 000001d0: 6579 5f73 7472 696e 67da 0876 6572 6966  ey_string..verif
-000001e0: 6965 72da 0145 a900 7211 0000 00fa 452f  ier..E..r.....E/
+000001e0: 6965 72da 0145 a900 7211 0000 00fa 432f  ier..E..r.....C/
 000001f0: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
 00000200: 7461 6765 732f 7265 6379 636c 696e 672f  tages/recycling/
-00000210: 6d6f 6475 6c65 732f 4545 435f 3434 385f  modules/EEC_448_
-00000220: 312f 7665 7269 6679 2f5f 5f69 6e69 745f  1/verify/__init_
-00000230: 5f2e 7079 da05 7374 6172 7416 0000 0073  _.py..start....s
-00000240: 1400 0000 0e07 0c03 0202 0c01 0601 0e02  ................
-00000250: 0a01 0402 0880 02fd 7213 0000 0029 034e  ........r....).N
-00000260: 4e4e 2908 da07 5f5f 646f 635f 5fda 1043  NN)...__doc__..C
-00000270: 7279 7074 6f2e 5369 676e 6174 7572 6572  rypto.Signaturer
-00000280: 0200 0000 da10 4372 7970 746f 2e50 7562  ......Crypto.Pub
-00000290: 6c69 634b 6579 7203 0000 00da 2b72 6563  licKeyr.....+rec
-000002a0: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-000002b0: 4543 5f34 3438 5f31 2e70 7562 6c69 635f  EC_448_1.public_
-000002c0: 6b65 792e 7363 616e 7204 0000 0072 1300  key.scanr....r..
-000002d0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-000002e0: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000002f0: 0100 0000 7312 0000 0004 0202 040c 0a0c  ....s...........
-00000300: 010c 0202 0402 0202 010e fb              ...........
+00000210: 6d69 7865 732f 4545 435f 3434 385f 312f  mixes/EEC_448_1/
+00000220: 7665 7269 6679 2f5f 5f69 6e69 745f 5f2e  verify/__init__.
+00000230: 7079 da05 7374 6172 7416 0000 0073 1400  py..start....s..
+00000240: 0000 0e07 0c03 0202 0c01 0601 0e02 0a01  ................
+00000250: 0402 0880 02fd 7213 0000 0029 034e 4e4e  ......r....).NNN
+00000260: 2908 da07 5f5f 646f 635f 5fda 1043 7279  )...__doc__..Cry
+00000270: 7074 6f2e 5369 676e 6174 7572 6572 0200  pto.Signaturer..
+00000280: 0000 da10 4372 7970 746f 2e50 7562 6c69  ....Crypto.Publi
+00000290: 634b 6579 7203 0000 00da 2972 6563 7963  cKeyr.....)recyc
+000002a0: 6c69 6e67 2e6d 6978 6573 2e45 4543 5f34  ling.mixes.EEC_4
+000002b0: 3438 5f31 2e70 7562 6c69 635f 6b65 792e  48_1.public_key.
+000002c0: 7363 616e 7204 0000 0072 1300 0000 7211  scanr....r....r.
+000002d0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+000002e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000002f0: 7312 0000 0004 0202 040c 0a0c 010c 0202  s...............
+00000300: 0402 0202 010e fb                        .......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/EEC_448_2.HTML` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/tutorial ++ EEC_448_2.S.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/__pycache__/status_DER_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/__pycache__/status_DER_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2538 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,156 +1,155 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 ea09 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 e209 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d04 0200 0100 6d08 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
 00000080: 6d04 0200 0100 6d0b 5a0c 0100 6401 6402  m.....m.Z...d.d.
 00000090: 6c0d 5a0d 6401 6403 6c0e 6d0f 5a0f 6d10  l.Z.d.d.l.m.Z.m.
 000000a0: 5a10 6d11 5a11 0100 6401 6402 6c12 5a12  Z.m.Z...d.d.l.Z.
 000000b0: 6401 6402 6c13 5a13 6404 6405 8400 5a14  d.d.l.Z.d.d...Z.
-000000c0: 6406 6514 6901 5a15 6402 5300 2907 7a5a  d.e.i.Z.d.S.).zZ
+000000c0: 6406 6514 6901 5a15 6402 5300 2907 7a58  d.e.i.Z.d.S.).zX
 000000d0: 0a09 7079 7468 6f6e 3320 7374 6174 7573  ..python3 status
-000000e0: 2e70 726f 632e 7079 2022 6d6f 6475 6c65  .proc.py "module
-000000f0: 732f 4545 435f 3434 385f 322f 5f73 7461  s/EEC_448_2/_sta
-00000100: 7475 732f 7374 6174 7573 5f31 5f70 7269  tus/status_1_pri
-00000110: 7661 7465 5f6b 6579 2f73 7461 7475 735f  vate_key/status_
-00000120: 4445 525f 312e 7079 220a e900 0000 004e  DER_1.py"......N
-00000130: 2903 da07 6469 726e 616d 65da 046a 6f69  )...dirname..joi
-00000140: 6eda 086e 6f72 6d70 6174 6863 0000 0000  n..normpathc....
-00000150: 0000 0000 0000 0000 0800 0000 0900 0000  ................
-00000160: 4300 0000 73cc 0000 0067 0064 01a2 017d  C...s....g.d...}
-00000170: 007c 0044 005d 5d7d 0174 0074 0174 02a0  .|.D.]]}.t.t.t..
-00000180: 0374 04a1 016a 05a0 06a1 0064 0283 0283  .t...j.....d....
-00000190: 0164 0317 007d 027a 0774 07a0 087c 02a1  .d...}.z.t...|..
-000001a0: 0101 0057 006e 0904 0074 0979 2701 0001  ...W.n...t.y'...
-000001b0: 0001 0059 006e 0177 0074 0aa0 0b7c 01a1  ...Y.n.w.t...|..
-000001c0: 017d 037c 0364 0419 007d 047c 0364 0519  .}.|.d...}.|.d..
-000001d0: 007d 057c 0364 0619 007d 0674 0c7c 0364  .}.|.d...}.t.|.d
-000001e0: 0519 0083 0101 0074 0da0 0e7c 027c 0664  .......t...|.|.d
-000001f0: 07a1 0301 0074 0fa0 0e7c 0264 07a1 027d  .....t...|.d...}
-00000200: 077c 0764 0519 007c 0364 0519 006b 0273  .|.d...|.d...k.s
-00000210: 5e4a 007c 0764 0519 007c 0364 0519 0067  ^J.|.d...|.d...g
-00000220: 0283 0182 0174 0c64 087c 0783 0201 0071  .....t.d.|.....q
-00000230: 0664 0053 0029 094e 2908 da72 3439 3836  .d.S.).N)..r4986
-00000240: 3838 3862 3131 3335 3862 6633 6435 3431  888b11358bf3d541
-00000250: 6234 3165 6561 3564 6165 6365 3163 3665  b41eea5daece1c6e
-00000260: 6666 3634 3133 3061 3435 6663 3862 3963  ff64130a45fc8b9c
-00000270: 6134 3866 3365 3065 3032 3436 3363 3939  a48f3e0e02463c99
-00000280: 6335 6165 6463 3861 3834 3736 3836 6436  c5aedc8a847686d6
-00000290: 3639 6237 6435 3437 6331 3866 6534 3438  69b7d547c18fe448
-000002a0: 6663 3531 3131 6361 3838 6634 6538 da72  fc5111ca88f4e8.r
-000002b0: 3539 3836 3838 3862 3131 3335 3862 6633  5986888b11358bf3
-000002c0: 6435 3431 6234 3165 6561 3564 6165 6365  d541b41eea5daece
-000002d0: 3163 3665 6666 3634 3133 3061 3435 6663  1c6eff64130a45fc
-000002e0: 3862 3963 6134 3866 3365 3065 3032 3436  8b9ca48f3e0e0246
-000002f0: 3363 3939 6335 6165 6463 3861 3834 3736  3c99c5aedc8a8476
-00000300: 3836 6436 3639 6237 6435 3437 6331 3866  86d669b7d547c18f
-00000310: 6534 3438 6663 3531 3131 6361 3838 6634  e448fc5111ca88f4
-00000320: 6538 da72 3030 3030 3030 3030 3030 3030  e8.r000000000000
+000000e0: 2e70 726f 632e 7079 2022 6d69 7865 732f  .proc.py "mixes/
+000000f0: 4545 435f 3434 385f 322f 5f73 7461 7475  EEC_448_2/_statu
+00000100: 732f 7374 6174 7573 5f31 5f70 7269 7661  s/status_1_priva
+00000110: 7465 5f6b 6579 2f73 7461 7475 735f 4445  te_key/status_DE
+00000120: 525f 312e 7079 220a e900 0000 004e 2903  R_1.py"......N).
+00000130: da07 6469 726e 616d 65da 046a 6f69 6eda  ..dirname..join.
+00000140: 086e 6f72 6d70 6174 6863 0000 0000 0000  .normpathc......
+00000150: 0000 0000 0000 0800 0000 0900 0000 4300  ..............C.
+00000160: 0000 73cc 0000 0067 0064 01a2 017d 007c  ..s....g.d...}.|
+00000170: 0044 005d 5d7d 0174 0074 0174 02a0 0374  .D.]]}.t.t.t...t
+00000180: 04a1 016a 05a0 06a1 0064 0283 0283 0164  ...j.....d.....d
+00000190: 0317 007d 027a 0774 07a0 087c 02a1 0101  ...}.z.t...|....
+000001a0: 0057 006e 0904 0074 0979 2701 0001 0001  .W.n...t.y'.....
+000001b0: 0059 006e 0177 0074 0aa0 0b7c 01a1 017d  .Y.n.w.t...|...}
+000001c0: 037c 0364 0419 007d 047c 0364 0519 007d  .|.d...}.|.d...}
+000001d0: 057c 0364 0619 007d 0674 0c7c 0364 0519  .|.d...}.t.|.d..
+000001e0: 0083 0101 0074 0da0 0e7c 027c 0664 07a1  .....t...|.|.d..
+000001f0: 0301 0074 0fa0 0e7c 0264 07a1 027d 077c  ...t...|.d...}.|
+00000200: 0764 0519 007c 0364 0519 006b 0273 5e4a  .d...|.d...k.s^J
+00000210: 007c 0764 0519 007c 0364 0519 0067 0283  .|.d...|.d...g..
+00000220: 0182 0174 0c64 087c 0783 0201 0071 0664  ...t.d.|.....q.d
+00000230: 0053 0029 094e 2908 da72 3439 3836 3838  .S.).N)..r498688
+00000240: 3862 3131 3335 3862 6633 6435 3431 6234  8b11358bf3d541b4
+00000250: 3165 6561 3564 6165 6365 3163 3665 6666  1eea5daece1c6eff
+00000260: 3634 3133 3061 3435 6663 3862 3963 6134  64130a45fc8b9ca4
+00000270: 3866 3365 3065 3032 3436 3363 3939 6335  8f3e0e02463c99c5
+00000280: 6165 6463 3861 3834 3736 3836 6436 3639  aedc8a847686d669
+00000290: 6237 6435 3437 6331 3866 6534 3438 6663  b7d547c18fe448fc
+000002a0: 3531 3131 6361 3838 6634 6538 da72 3539  5111ca88f4e8.r59
+000002b0: 3836 3838 3862 3131 3335 3862 6633 6435  86888b11358bf3d5
+000002c0: 3431 6234 3165 6561 3564 6165 6365 3163  41b41eea5daece1c
+000002d0: 3665 6666 3634 3133 3061 3435 6663 3862  6eff64130a45fc8b
+000002e0: 3963 6134 3866 3365 3065 3032 3436 3363  9ca48f3e0e02463c
+000002f0: 3939 6335 6165 6463 3861 3834 3736 3836  99c5aedc8a847686
+00000300: 6436 3639 6237 6435 3437 6331 3866 6534  d669b7d547c18fe4
+00000310: 3438 6663 3531 3131 6361 3838 6634 6538  48fc5111ca88f4e8
+00000320: da72 3030 3030 3030 3030 3030 3030 3030  .r00000000000000
 00000330: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000340: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000350: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000360: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000370: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000380: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-00000390: 3030 3030 3030 da72 6666 6666 6666 6666  000000.rffffffff
+00000390: 3030 3030 da72 6666 6666 6666 6666 6666  0000.rffffffffff
 000003a0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003b0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003c0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003d0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003e0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003f0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-00000400: 6666 6666 6666 6666 6666 da72 3132 3334  ffffffffff.r1234
-00000410: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000420: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000430: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000440: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000450: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000460: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000470: 3132 3334 3132 3334 3132 3334 3132 da72  12341234123412.r
-00000480: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-00000490: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004a0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004b0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004c0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004d0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004e0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-000004f0: 3066 da72 3133 3537 3931 3335 3739 3133  0f.r135791357913
-00000500: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000510: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000520: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000530: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000540: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000550: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000560: 3739 3133 3537 da72 3234 3638 6566 3234  791357.r2468ef24
-00000570: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-00000580: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-00000590: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-000005a0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-000005b0: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-000005c0: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-000005d0: 3638 6566 3234 3638 6566 da15 4545 435f  68ef2468ef..EEC_
-000005e0: 3434 385f 325f 7072 6976 6174 655f 6b65  448_2_private_ke
-000005f0: 797a 042e 4445 52da 0869 6e73 7461 6e63  yz..DER..instanc
-00000600: 657a 1644 4552 2068 6578 6164 6563 696d  ez.DER hexadecim
-00000610: 616c 2073 7472 696e 677a 0f44 4552 2062  al stringz.DER b
-00000620: 7974 6520 7374 7269 6e67 da03 4445 527a  yte string..DERz
-00000630: 1670 7269 7661 7465 5f6b 6579 5f66 726f  .private_key_fro
-00000640: 6d5f 7363 616e 3a29 1072 0400 0000 7203  m_scan:).r....r.
-00000650: 0000 00da 0770 6174 686c 6962 da04 5061  .....pathlib..Pa
-00000660: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
-00000670: 7265 6e74 da07 7265 736f 6c76 65da 026f  rent..resolve..o
-00000680: 73da 0672 656d 6f76 65da 0945 7863 6570  s..remove..Excep
-00000690: 7469 6f6e da1d 4545 435f 3434 385f 325f  tion..EEC_448_2_
-000006a0: 7072 6976 6174 655f 6b65 795f 6372 6561  private_key_crea
-000006b0: 746f 72da 0663 7265 6174 65da 0570 7269  tor..create..pri
-000006c0: 6e74 da18 6574 6368 5f45 4543 5f34 3438  nt..etch_EEC_448
-000006d0: 5f70 7269 7661 7465 5f6b 6579 da05 7374  _private_key..st
-000006e0: 6172 74da 0c70 7269 7661 7465 5f73 6361  art..private_sca
-000006f0: 6e29 08da 0573 6565 6473 da04 7365 6564  n)...seeds..seed
-00000700: da10 7072 6976 6174 655f 6b65 795f 7061  ..private_key_pa
-00000710: 7468 da0b 7072 6976 6174 655f 6b65 79da  th..private_key.
-00000720: 1470 7269 7661 7465 5f6b 6579 5f69 6e73  .private_key_ins
-00000730: 7461 6e63 65da 2270 7269 7661 7465 5f6b  tance."private_k
-00000740: 6579 5f44 4552 5f68 6578 6164 6563 696d  ey_DER_hexadecim
-00000750: 616c 5f73 7472 696e 67da 1b70 7269 7661  al_string..priva
-00000760: 7465 5f6b 6579 5f44 4552 5f62 7974 655f  te_key_DER_byte_
-00000770: 7374 7269 6e67 da15 7072 6976 6174 655f  string..private_
-00000780: 6b65 795f 6672 6f6d 5f73 6361 6ea9 0072  key_from_scan..r
-00000790: 2600 0000 fa5f 2f68 6162 6974 6174 2f76  &...._/habitat/v
-000007a0: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
-000007b0: 7963 6c69 6e67 2f6d 6f64 756c 6573 2f45  ycling/modules/E
-000007c0: 4543 5f34 3438 5f32 2f5f 7374 6174 7573  EC_448_2/_status
-000007d0: 2f73 7461 7475 735f 315f 7072 6976 6174  /status_1_privat
-000007e0: 655f 6b65 792f 7374 6174 7573 5f44 4552  e_key/status_DER
-000007f0: 5f31 2e70 79da 0763 6865 636b 5f31 0f00  _1.py..check_1..
-00000800: 0000 7340 0000 0008 0108 0b02 0114 0102  ..s@............
-00000810: ff02 0204 fe02 040e 010c 0104 0102 ff0a  ................
-00000820: 0808 0108 0108 010c 0204 0502 0102 0102  ................
-00000830: 0104 fd0c 0a06 0306 0106 ff06 0306 0102  ................
-00000840: fe04 fe0c 0704 d372 2800 0000 7a1f 656c  .......r(...z.el
-00000850: 6c69 7074 6963 2070 7269 7661 7465 206b  liptic private k
-00000860: 6579 2067 656e 6572 6174 696f 6e29 16da  ey generation)..
-00000870: 075f 5f64 6f63 5f5f da2f 7265 6379 636c  .__doc__./recycl
-00000880: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-00000890: 3434 385f 322e 7072 6976 6174 655f 6b65  448_2.private_ke
-000008a0: 792e 6372 6561 746f 72da 076d 6f64 756c  y.creator..modul
-000008b0: 6573 da09 4545 435f 3434 385f 3272 2100  es..EEC_448_2r!.
-000008c0: 0000 da07 6372 6561 746f 7272 1800 0000  ....creatorr....
-000008d0: da2c 7265 6379 636c 696e 672e 6d6f 6475  .,recycling.modu
-000008e0: 6c65 732e 4545 435f 3434 385f 322e 7072  les.EEC_448_2.pr
-000008f0: 6976 6174 655f 6b65 792e 6574 6368 da04  ivate_key.etch..
-00000900: 6574 6368 721b 0000 00da 2c72 6563 7963  etchr.....,recyc
-00000910: 6c69 6e67 2e6d 6f64 756c 6573 2e45 4543  ling.modules.EEC
-00000920: 5f34 3438 5f32 2e70 7269 7661 7465 5f6b  _448_2.private_k
-00000930: 6579 2e73 6361 6eda 0473 6361 6e72 1d00  ey.scan..scanr..
-00000940: 0000 7210 0000 00da 076f 732e 7061 7468  ..r......os.path
-00000950: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00000960: 1500 0000 da04 6a73 6f6e 7228 0000 00da  ......jsonr(....
-00000970: 0663 6865 636b 7372 2600 0000 7226 0000  .checksr&...r&..
-00000980: 0072 2600 0000 7227 0000 00da 083c 6d6f  .r&...r'.....<mo
-00000990: 6475 6c65 3e01 0000 0073 1600 0000 0401  dule>....s......
-000009a0: 1e04 1e01 1e01 0802 1401 0801 0801 0802  ................
-000009b0: 043f 08ff                                .?..
+00000400: 6666 6666 6666 6666 da72 3132 3334 3132  ffffffff.r123412
+00000410: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000420: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000430: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000440: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000450: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000460: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
+00000470: 3334 3132 3334 3132 3334 3132 da72 3066  341234123412.r0f
+00000480: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+00000490: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004a0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004b0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004c0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004d0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004e0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
+000004f0: da72 3133 3537 3931 3335 3739 3133 3537  .r13579135791357
+00000500: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000510: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000520: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000530: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000540: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000550: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000560: 3133 3537 da72 3234 3638 6566 3234 3638  1357.r2468ef2468
+00000570: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+00000580: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+00000590: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+000005a0: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+000005b0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+000005c0: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+000005d0: 6566 3234 3638 6566 da15 4545 435f 3434  ef2468ef..EEC_44
+000005e0: 385f 325f 7072 6976 6174 655f 6b65 797a  8_2_private_keyz
+000005f0: 042e 4445 52da 0869 6e73 7461 6e63 657a  ..DER..instancez
+00000600: 1644 4552 2068 6578 6164 6563 696d 616c  .DER hexadecimal
+00000610: 2073 7472 696e 677a 0f44 4552 2062 7974   stringz.DER byt
+00000620: 6520 7374 7269 6e67 da03 4445 527a 1670  e string..DERz.p
+00000630: 7269 7661 7465 5f6b 6579 5f66 726f 6d5f  rivate_key_from_
+00000640: 7363 616e 3a29 1072 0400 0000 7203 0000  scan:).r....r...
+00000650: 00da 0770 6174 686c 6962 da04 5061 7468  ...pathlib..Path
+00000660: da08 5f5f 6669 6c65 5f5f da06 7061 7265  ..__file__..pare
+00000670: 6e74 da07 7265 736f 6c76 65da 026f 73da  nt..resolve..os.
+00000680: 0672 656d 6f76 65da 0945 7863 6570 7469  .remove..Excepti
+00000690: 6f6e da1d 4545 435f 3434 385f 325f 7072  on..EEC_448_2_pr
+000006a0: 6976 6174 655f 6b65 795f 6372 6561 746f  ivate_key_creato
+000006b0: 72da 0663 7265 6174 65da 0570 7269 6e74  r..create..print
+000006c0: da18 6574 6368 5f45 4543 5f34 3438 5f70  ..etch_EEC_448_p
+000006d0: 7269 7661 7465 5f6b 6579 da05 7374 6172  rivate_key..star
+000006e0: 74da 0c70 7269 7661 7465 5f73 6361 6e29  t..private_scan)
+000006f0: 08da 0573 6565 6473 da04 7365 6564 da10  ...seeds..seed..
+00000700: 7072 6976 6174 655f 6b65 795f 7061 7468  private_key_path
+00000710: da0b 7072 6976 6174 655f 6b65 79da 1470  ..private_key..p
+00000720: 7269 7661 7465 5f6b 6579 5f69 6e73 7461  rivate_key_insta
+00000730: 6e63 65da 2270 7269 7661 7465 5f6b 6579  nce."private_key
+00000740: 5f44 4552 5f68 6578 6164 6563 696d 616c  _DER_hexadecimal
+00000750: 5f73 7472 696e 67da 1b70 7269 7661 7465  _string..private
+00000760: 5f6b 6579 5f44 4552 5f62 7974 655f 7374  _key_DER_byte_st
+00000770: 7269 6e67 da15 7072 6976 6174 655f 6b65  ring..private_ke
+00000780: 795f 6672 6f6d 5f73 6361 6ea9 0072 2600  y_from_scan..r&.
+00000790: 0000 fa5d 2f68 6162 6974 6174 2f76 656e  ...]/habitat/ven
+000007a0: 7565 732f 7374 6167 6573 2f72 6563 7963  ues/stages/recyc
+000007b0: 6c69 6e67 2f6d 6978 6573 2f45 4543 5f34  ling/mixes/EEC_4
+000007c0: 3438 5f32 2f5f 7374 6174 7573 2f73 7461  48_2/_status/sta
+000007d0: 7475 735f 315f 7072 6976 6174 655f 6b65  tus_1_private_ke
+000007e0: 792f 7374 6174 7573 5f44 4552 5f31 2e70  y/status_DER_1.p
+000007f0: 79da 0763 6865 636b 5f31 0f00 0000 7340  y..check_1....s@
+00000800: 0000 0008 0108 0b02 0114 0102 ff02 0204  ................
+00000810: fe02 040e 010c 0104 0102 ff0a 0808 0108  ................
+00000820: 0108 010c 0204 0502 0102 0102 0104 fd0c  ................
+00000830: 0a06 0306 0106 ff06 0306 0102 fe04 fe0c  ................
+00000840: 0704 d372 2800 0000 7a1f 656c 6c69 7074  ...r(...z.ellipt
+00000850: 6963 2070 7269 7661 7465 206b 6579 2067  ic private key g
+00000860: 656e 6572 6174 696f 6e29 16da 075f 5f64  eneration)...__d
+00000870: 6f63 5f5f da2d 7265 6379 636c 696e 672e  oc__.-recycling.
+00000880: 6d69 7865 732e 4545 435f 3434 385f 322e  mixes.EEC_448_2.
+00000890: 7072 6976 6174 655f 6b65 792e 6372 6561  private_key.crea
+000008a0: 746f 72da 056d 6978 6573 da09 4545 435f  tor..mixes..EEC_
+000008b0: 3434 385f 3272 2100 0000 da07 6372 6561  448_2r!.....crea
+000008c0: 746f 7272 1800 0000 da2a 7265 6379 636c  torr.....*recycl
+000008d0: 696e 672e 6d69 7865 732e 4545 435f 3434  ing.mixes.EEC_44
+000008e0: 385f 322e 7072 6976 6174 655f 6b65 792e  8_2.private_key.
+000008f0: 6574 6368 da04 6574 6368 721b 0000 00da  etch..etchr.....
+00000900: 2a72 6563 7963 6c69 6e67 2e6d 6978 6573  *recycling.mixes
+00000910: 2e45 4543 5f34 3438 5f32 2e70 7269 7661  .EEC_448_2.priva
+00000920: 7465 5f6b 6579 2e73 6361 6eda 0473 6361  te_key.scan..sca
+00000930: 6e72 1d00 0000 7210 0000 00da 076f 732e  nr....r......os.
+00000940: 7061 7468 7202 0000 0072 0300 0000 7204  pathr....r....r.
+00000950: 0000 0072 1500 0000 da04 6a73 6f6e 7228  ...r......jsonr(
+00000960: 0000 00da 0663 6865 636b 7372 2600 0000  .....checksr&...
+00000970: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
+00000980: 083c 6d6f 6475 6c65 3e01 0000 0073 1600  .<module>....s..
+00000990: 0000 0401 1e04 1e01 1e01 0802 1401 0801  ................
+000009a0: 0801 0802 043f 08ff                      .....?..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/__pycache__/status_JSON_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/__pycache__/status_JSON_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2498 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,156 +1,155 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 c209 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 ba09 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d04 0200 0100 6d08 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
 00000080: 6d04 0200 0100 6d0b 5a0c 0100 6401 6402  m.....m.Z...d.d.
 00000090: 6c0d 5a0d 6401 6403 6c0e 6d0f 5a0f 6d10  l.Z.d.d.l.m.Z.m.
 000000a0: 5a10 6d11 5a11 0100 6401 6402 6c12 5a12  Z.m.Z...d.d.l.Z.
 000000b0: 6401 6402 6c13 5a13 6404 6405 8400 5a14  d.d.l.Z.d.d...Z.
-000000c0: 6406 6514 6901 5a15 6402 5300 2907 7a5b  d.e.i.Z.d.S.).z[
+000000c0: 6406 6514 6901 5a15 6402 5300 2907 7a59  d.e.i.Z.d.S.).zY
 000000d0: 0a09 7079 7468 6f6e 3320 7374 6174 7573  ..python3 status
-000000e0: 2e70 726f 632e 7079 2022 6d6f 6475 6c65  .proc.py "module
-000000f0: 732f 4545 435f 3434 385f 322f 5f73 7461  s/EEC_448_2/_sta
-00000100: 7475 732f 7374 6174 7573 5f31 5f70 7269  tus/status_1_pri
-00000110: 7661 7465 5f6b 6579 2f73 7461 7475 735f  vate_key/status_
-00000120: 4a53 4f4e 5f31 2e70 7922 0ae9 0000 0000  JSON_1.py"......
-00000130: 4e29 03da 0764 6972 6e61 6d65 da04 6a6f  N)...dirname..jo
-00000140: 696e da08 6e6f 726d 7061 7468 6300 0000  in..normpathc...
-00000150: 0000 0000 0000 0000 0008 0000 0009 0000  ................
-00000160: 0043 0000 0073 c000 0000 6700 6401 a201  .C...s....g.d...
-00000170: 7d00 7c00 4400 5d57 7d01 7400 7401 7402  }.|.D.]W}.t.t.t.
-00000180: a003 7404 a101 6a05 a006 a100 6402 8302  ..t...j.....d...
-00000190: 8301 6403 1700 7d02 7a07 7407 a008 7c02  ..d...}.z.t...|.
-000001a0: a101 0100 5700 6e09 0400 7409 7927 0100  ....W.n...t.y'..
-000001b0: 0100 0100 5900 6e01 7700 740a a00b 7c01  ....Y.n.w.t...|.
-000001c0: a101 7d03 7c03 6404 1900 7d04 7c03 6405  ..}.|.d...}.|.d.
-000001d0: 1900 7d05 7c03 6406 1900 7d06 740c a00d  ..}.|.d...}.t...
-000001e0: 7c02 740e 6a0f 6407 6405 7c03 6405 1900  |.t.j.d.d.|.d...
-000001f0: 6901 6901 6408 6409 8d02 640a a103 0100  i.i.d.d...d.....
-00000200: 7410 a00d 7c02 640a a102 7d07 7c07 6407  t...|.d...}.|.d.
-00000210: 1900 6405 1900 7c03 6405 1900 6b02 735d  ..d...|.d...k.s]
-00000220: 4a00 8201 7106 6400 5300 290b 4e29 08da  J...q.d.S.).N)..
-00000230: 7234 3938 3638 3838 6231 3133 3538 6266  r4986888b11358bf
-00000240: 3364 3534 3162 3431 6565 6135 6461 6563  3d541b41eea5daec
-00000250: 6531 6336 6566 6636 3431 3330 6134 3566  e1c6eff64130a45f
-00000260: 6338 6239 6361 3438 6633 6530 6530 3234  c8b9ca48f3e0e024
-00000270: 3633 6339 3963 3561 6564 6338 6138 3437  63c99c5aedc8a847
-00000280: 3638 3664 3636 3962 3764 3534 3763 3138  686d669b7d547c18
-00000290: 6665 3434 3866 6335 3131 3163 6138 3866  fe448fc5111ca88f
-000002a0: 3465 38da 7235 3938 3638 3838 6231 3133  4e8.r5986888b113
-000002b0: 3538 6266 3364 3534 3162 3431 6565 6135  58bf3d541b41eea5
-000002c0: 6461 6563 6531 6336 6566 6636 3431 3330  daece1c6eff64130
-000002d0: 6134 3566 6338 6239 6361 3438 6633 6530  a45fc8b9ca48f3e0
-000002e0: 6530 3234 3633 6339 3963 3561 6564 6338  e02463c99c5aedc8
-000002f0: 6138 3437 3638 3664 3636 3962 3764 3534  a847686d669b7d54
-00000300: 3763 3138 6665 3434 3866 6335 3131 3163  7c18fe448fc5111c
-00000310: 6138 3866 3465 38da 7230 3030 3030 3030  a88f4e8.r0000000
+000000e0: 2e70 726f 632e 7079 2022 6d69 7865 732f  .proc.py "mixes/
+000000f0: 4545 435f 3434 385f 322f 5f73 7461 7475  EEC_448_2/_statu
+00000100: 732f 7374 6174 7573 5f31 5f70 7269 7661  s/status_1_priva
+00000110: 7465 5f6b 6579 2f73 7461 7475 735f 4a53  te_key/status_JS
+00000120: 4f4e 5f31 2e70 7922 0ae9 0000 0000 4e29  ON_1.py"......N)
+00000130: 03da 0764 6972 6e61 6d65 da04 6a6f 696e  ...dirname..join
+00000140: da08 6e6f 726d 7061 7468 6300 0000 0000  ..normpathc.....
+00000150: 0000 0000 0000 0008 0000 0009 0000 0043  ...............C
+00000160: 0000 0073 c000 0000 6700 6401 a201 7d00  ...s....g.d...}.
+00000170: 7c00 4400 5d57 7d01 7400 7401 7402 a003  |.D.]W}.t.t.t...
+00000180: 7404 a101 6a05 a006 a100 6402 8302 8301  t...j.....d.....
+00000190: 6403 1700 7d02 7a07 7407 a008 7c02 a101  d...}.z.t...|...
+000001a0: 0100 5700 6e09 0400 7409 7927 0100 0100  ..W.n...t.y'....
+000001b0: 0100 5900 6e01 7700 740a a00b 7c01 a101  ..Y.n.w.t...|...
+000001c0: 7d03 7c03 6404 1900 7d04 7c03 6405 1900  }.|.d...}.|.d...
+000001d0: 7d05 7c03 6406 1900 7d06 740c a00d 7c02  }.|.d...}.t...|.
+000001e0: 740e 6a0f 6407 6405 7c03 6405 1900 6901  t.j.d.d.|.d...i.
+000001f0: 6901 6408 6409 8d02 640a a103 0100 7410  i.d.d...d.....t.
+00000200: a00d 7c02 640a a102 7d07 7c07 6407 1900  ..|.d...}.|.d...
+00000210: 6405 1900 7c03 6405 1900 6b02 735d 4a00  d...|.d...k.s]J.
+00000220: 8201 7106 6400 5300 290b 4e29 08da 7234  ..q.d.S.).N)..r4
+00000230: 3938 3638 3838 6231 3133 3538 6266 3364  986888b11358bf3d
+00000240: 3534 3162 3431 6565 6135 6461 6563 6531  541b41eea5daece1
+00000250: 6336 6566 6636 3431 3330 6134 3566 6338  c6eff64130a45fc8
+00000260: 6239 6361 3438 6633 6530 6530 3234 3633  b9ca48f3e0e02463
+00000270: 6339 3963 3561 6564 6338 6138 3437 3638  c99c5aedc8a84768
+00000280: 3664 3636 3962 3764 3534 3763 3138 6665  6d669b7d547c18fe
+00000290: 3434 3866 6335 3131 3163 6138 3866 3465  448fc5111ca88f4e
+000002a0: 38da 7235 3938 3638 3838 6231 3133 3538  8.r5986888b11358
+000002b0: 6266 3364 3534 3162 3431 6565 6135 6461  bf3d541b41eea5da
+000002c0: 6563 6531 6336 6566 6636 3431 3330 6134  ece1c6eff64130a4
+000002d0: 3566 6338 6239 6361 3438 6633 6530 6530  5fc8b9ca48f3e0e0
+000002e0: 3234 3633 6339 3963 3561 6564 6338 6138  2463c99c5aedc8a8
+000002f0: 3437 3638 3664 3636 3962 3764 3534 3763  47686d669b7d547c
+00000300: 3138 6665 3434 3866 6335 3131 3163 6138  18fe448fc5111ca8
+00000310: 3866 3465 38da 7230 3030 3030 3030 3030  8f4e8.r000000000
 00000320: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000330: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000340: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000350: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000360: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000370: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-00000380: 3030 3030 3030 3030 3030 30da 7266 6666  00000000000.rfff
+00000380: 3030 3030 3030 3030 30da 7266 6666 6666  000000000.rfffff
 00000390: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003a0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003b0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003c0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003d0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000003e0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-000003f0: 6666 6666 6666 6666 6666 6666 6666 66da  fffffffffffffff.
-00000400: 7231 3233 3431 3233 3431 3233 3431 3233  r123412341234123
-00000410: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000420: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000430: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000440: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000450: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000460: 3431 3233 3431 3233 3431 3233 3431 3233  4123412341234123
-00000470: 3431 32da 7230 6631 6530 6631 6530 6631  412.r0f1e0f1e0f1
-00000480: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-00000490: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-000004a0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-000004b0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-000004c0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-000004d0: 6530 6631 6530 6631 6530 6631 6530 6631  e0f1e0f1e0f1e0f1
-000004e0: 6530 6631 6530 66da 7231 3335 3739 3133  e0f1e0f.r1357913
-000004f0: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000500: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000510: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000520: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000530: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000540: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000550: 3739 3133 3537 3931 3335 37da 7232 3436  79135791357.r246
-00000560: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-00000570: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-00000580: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-00000590: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
-000005a0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
-000005b0: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
-000005c0: 3865 6632 3436 3865 6632 3436 3865 66da  8ef2468ef2468ef.
-000005d0: 1545 4543 5f34 3438 5f32 5f70 7269 7661  .EEC_448_2_priva
-000005e0: 7465 5f6b 6579 7a05 2e4a 534f 4eda 0869  te_keyz..JSON..i
-000005f0: 6e73 7461 6e63 657a 1644 4552 2068 6578  nstancez.DER hex
-00000600: 6164 6563 696d 616c 2073 7472 696e 677a  adecimal stringz
-00000610: 0f44 4552 2062 7974 6520 7374 7269 6e67  .DER byte string
-00000620: 7a0b 7072 6976 6174 6520 6b65 79e9 0400  z.private key...
-00000630: 0000 2901 da06 696e 6465 6e74 da04 4a53  ..)...indent..JS
-00000640: 4f4e 2911 7204 0000 0072 0300 0000 da07  ON).r....r......
-00000650: 7061 7468 6c69 62da 0450 6174 68da 085f  pathlib..Path.._
-00000660: 5f66 696c 655f 5fda 0670 6172 656e 74da  _file__..parent.
-00000670: 0772 6573 6f6c 7665 da02 6f73 da06 7265  .resolve..os..re
-00000680: 6d6f 7665 da09 4578 6365 7074 696f 6eda  move..Exception.
-00000690: 1d45 4543 5f34 3438 5f32 5f70 7269 7661  .EEC_448_2_priva
-000006a0: 7465 5f6b 6579 5f63 7265 6174 6f72 da06  te_key_creator..
-000006b0: 6372 6561 7465 da18 6574 6368 5f45 4543  create..etch_EEC
-000006c0: 5f34 3438 5f70 7269 7661 7465 5f6b 6579  _448_private_key
-000006d0: da05 7374 6172 74da 046a 736f 6eda 0564  ..start..json..d
-000006e0: 756d 7073 da0c 7072 6976 6174 655f 7363  umps..private_sc
-000006f0: 616e 2908 da05 7365 6564 73da 0473 6565  an)...seeds..see
-00000700: 64da 1070 7269 7661 7465 5f6b 6579 5f70  d..private_key_p
-00000710: 6174 68da 0b70 7269 7661 7465 5f6b 6579  ath..private_key
-00000720: da14 7072 6976 6174 655f 6b65 795f 696e  ..private_key_in
-00000730: 7374 616e 6365 da22 7072 6976 6174 655f  stance."private_
-00000740: 6b65 795f 4445 525f 6865 7861 6465 6369  key_DER_hexadeci
-00000750: 6d61 6c5f 7374 7269 6e67 da1b 7072 6976  mal_string..priv
-00000760: 6174 655f 6b65 795f 4445 525f 6279 7465  ate_key_DER_byte
-00000770: 5f73 7472 696e 67da 1570 7269 7661 7465  _string..private
-00000780: 5f6b 6579 5f66 726f 6d5f 7363 616e a900  _key_from_scan..
-00000790: 7229 0000 00fa 602f 6861 6269 7461 742f  r)....`/habitat/
-000007a0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
-000007b0: 6379 636c 696e 672f 6d6f 6475 6c65 732f  cycling/modules/
-000007c0: 4545 435f 3434 385f 322f 5f73 7461 7475  EEC_448_2/_statu
-000007d0: 732f 7374 6174 7573 5f31 5f70 7269 7661  s/status_1_priva
-000007e0: 7465 5f6b 6579 2f73 7461 7475 735f 4a53  te_key/status_JS
-000007f0: 4f4e 5f31 2e70 79da 0763 6865 636b 5f31  ON_1.py..check_1
-00000800: 0f00 0000 7340 0000 0008 0108 0b02 0114  ....s@..........
-00000810: 0102 ff02 0204 fe02 040e 010c 0104 0102  ................
-00000820: ff0a 0808 0108 0108 0104 0702 0104 0102  ................
-00000830: 0108 0102 ff02 ff02 0404 fc02 0504 f90c  ................
-00000840: 0e0a 0306 010a ff04 d672 2b00 0000 7a1f  .........r+...z.
-00000850: 656c 6c69 7074 6963 2070 7269 7661 7465  elliptic private
-00000860: 206b 6579 2067 656e 6572 6174 696f 6e29   key generation)
-00000870: 16da 075f 5f64 6f63 5f5f da2f 7265 6379  ...__doc__./recy
-00000880: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000890: 435f 3434 385f 322e 7072 6976 6174 655f  C_448_2.private_
-000008a0: 6b65 792e 6372 6561 746f 72da 076d 6f64  key.creator..mod
-000008b0: 756c 6573 da09 4545 435f 3434 385f 3272  ules..EEC_448_2r
-000008c0: 2400 0000 da07 6372 6561 746f 7272 1a00  $.....creatorr..
-000008d0: 0000 da2c 7265 6379 636c 696e 672e 6d6f  ...,recycling.mo
-000008e0: 6475 6c65 732e 4545 435f 3434 385f 322e  dules.EEC_448_2.
-000008f0: 7072 6976 6174 655f 6b65 792e 6574 6368  private_key.etch
-00000900: da04 6574 6368 721c 0000 00da 2c72 6563  ..etchr.....,rec
-00000910: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-00000920: 4543 5f34 3438 5f32 2e70 7269 7661 7465  EC_448_2.private
-00000930: 5f6b 6579 2e73 6361 6eda 0473 6361 6e72  _key.scan..scanr
-00000940: 2000 0000 7212 0000 00da 076f 732e 7061   ...r......os.pa
-00000950: 7468 7202 0000 0072 0300 0000 7204 0000  thr....r....r...
-00000960: 0072 1700 0000 721e 0000 0072 2b00 0000  .r....r....r+...
-00000970: da06 6368 6563 6b73 7229 0000 0072 2900  ..checksr)...r).
-00000980: 0000 7229 0000 0072 2a00 0000 da08 3c6d  ..r)...r*.....<m
-00000990: 6f64 756c 653e 0100 0000 7316 0000 0004  odule>....s.....
-000009a0: 011e 041e 011e 0108 0214 0108 0108 0108  ................
-000009b0: 0204 3f08 ff                             ..?..
+000003f0: 6666 6666 6666 6666 6666 6666 66da 7231  fffffffffffff.r1
+00000400: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000410: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000420: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000430: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000440: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000450: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000460: 3233 3431 3233 3431 3233 3431 3233 3431  2341234123412341
+00000470: 32da 7230 6631 6530 6631 6530 6631 6530  2.r0f1e0f1e0f1e0
+00000480: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+00000490: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+000004a0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+000004b0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+000004c0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+000004d0: 6631 6530 6631 6530 6631 6530 6631 6530  f1e0f1e0f1e0f1e0
+000004e0: 6631 6530 66da 7231 3335 3739 3133 3537  f1e0f.r135791357
+000004f0: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000500: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000510: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000520: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000530: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000540: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000550: 3133 3537 3931 3335 37da 7232 3436 3865  135791357.r2468e
+00000560: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+00000570: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+00000580: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+00000590: 6632 3436 3865 6632 3436 3865 6632 3436  f2468ef2468ef246
+000005a0: 3865 6632 3436 3865 6632 3436 3865 6632  8ef2468ef2468ef2
+000005b0: 3436 3865 6632 3436 3865 6632 3436 3865  468ef2468ef2468e
+000005c0: 6632 3436 3865 6632 3436 3865 66da 1545  f2468ef2468ef..E
+000005d0: 4543 5f34 3438 5f32 5f70 7269 7661 7465  EC_448_2_private
+000005e0: 5f6b 6579 7a05 2e4a 534f 4eda 0869 6e73  _keyz..JSON..ins
+000005f0: 7461 6e63 657a 1644 4552 2068 6578 6164  tancez.DER hexad
+00000600: 6563 696d 616c 2073 7472 696e 677a 0f44  ecimal stringz.D
+00000610: 4552 2062 7974 6520 7374 7269 6e67 7a0b  ER byte stringz.
+00000620: 7072 6976 6174 6520 6b65 79e9 0400 0000  private key.....
+00000630: 2901 da06 696e 6465 6e74 da04 4a53 4f4e  )...indent..JSON
+00000640: 2911 7204 0000 0072 0300 0000 da07 7061  ).r....r......pa
+00000650: 7468 6c69 62da 0450 6174 68da 085f 5f66  thlib..Path..__f
+00000660: 696c 655f 5fda 0670 6172 656e 74da 0772  ile__..parent..r
+00000670: 6573 6f6c 7665 da02 6f73 da06 7265 6d6f  esolve..os..remo
+00000680: 7665 da09 4578 6365 7074 696f 6eda 1d45  ve..Exception..E
+00000690: 4543 5f34 3438 5f32 5f70 7269 7661 7465  EC_448_2_private
+000006a0: 5f6b 6579 5f63 7265 6174 6f72 da06 6372  _key_creator..cr
+000006b0: 6561 7465 da18 6574 6368 5f45 4543 5f34  eate..etch_EEC_4
+000006c0: 3438 5f70 7269 7661 7465 5f6b 6579 da05  48_private_key..
+000006d0: 7374 6172 74da 046a 736f 6eda 0564 756d  start..json..dum
+000006e0: 7073 da0c 7072 6976 6174 655f 7363 616e  ps..private_scan
+000006f0: 2908 da05 7365 6564 73da 0473 6565 64da  )...seeds..seed.
+00000700: 1070 7269 7661 7465 5f6b 6579 5f70 6174  .private_key_pat
+00000710: 68da 0b70 7269 7661 7465 5f6b 6579 da14  h..private_key..
+00000720: 7072 6976 6174 655f 6b65 795f 696e 7374  private_key_inst
+00000730: 616e 6365 da22 7072 6976 6174 655f 6b65  ance."private_ke
+00000740: 795f 4445 525f 6865 7861 6465 6369 6d61  y_DER_hexadecima
+00000750: 6c5f 7374 7269 6e67 da1b 7072 6976 6174  l_string..privat
+00000760: 655f 6b65 795f 4445 525f 6279 7465 5f73  e_key_DER_byte_s
+00000770: 7472 696e 67da 1570 7269 7661 7465 5f6b  tring..private_k
+00000780: 6579 5f66 726f 6d5f 7363 616e a900 7229  ey_from_scan..r)
+00000790: 0000 00fa 5e2f 6861 6269 7461 742f 7665  ....^/habitat/ve
+000007a0: 6e75 6573 2f73 7461 6765 732f 7265 6379  nues/stages/recy
+000007b0: 636c 696e 672f 6d69 7865 732f 4545 435f  cling/mixes/EEC_
+000007c0: 3434 385f 322f 5f73 7461 7475 732f 7374  448_2/_status/st
+000007d0: 6174 7573 5f31 5f70 7269 7661 7465 5f6b  atus_1_private_k
+000007e0: 6579 2f73 7461 7475 735f 4a53 4f4e 5f31  ey/status_JSON_1
+000007f0: 2e70 79da 0763 6865 636b 5f31 0f00 0000  .py..check_1....
+00000800: 7340 0000 0008 0108 0b02 0114 0102 ff02  s@..............
+00000810: 0204 fe02 040e 010c 0104 0102 ff0a 0808  ................
+00000820: 0108 0108 0104 0702 0104 0102 0108 0102  ................
+00000830: ff02 ff02 0404 fc02 0504 f90c 0e0a 0306  ................
+00000840: 010a ff04 d672 2b00 0000 7a1f 656c 6c69  .....r+...z.elli
+00000850: 7074 6963 2070 7269 7661 7465 206b 6579  ptic private key
+00000860: 2067 656e 6572 6174 696f 6e29 16da 075f   generation)..._
+00000870: 5f64 6f63 5f5f da2d 7265 6379 636c 696e  _doc__.-recyclin
+00000880: 672e 6d69 7865 732e 4545 435f 3434 385f  g.mixes.EEC_448_
+00000890: 322e 7072 6976 6174 655f 6b65 792e 6372  2.private_key.cr
+000008a0: 6561 746f 72da 056d 6978 6573 da09 4545  eator..mixes..EE
+000008b0: 435f 3434 385f 3272 2400 0000 da07 6372  C_448_2r$.....cr
+000008c0: 6561 746f 7272 1a00 0000 da2a 7265 6379  eatorr.....*recy
+000008d0: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+000008e0: 3434 385f 322e 7072 6976 6174 655f 6b65  448_2.private_ke
+000008f0: 792e 6574 6368 da04 6574 6368 721c 0000  y.etch..etchr...
+00000900: 00da 2a72 6563 7963 6c69 6e67 2e6d 6978  ..*recycling.mix
+00000910: 6573 2e45 4543 5f34 3438 5f32 2e70 7269  es.EEC_448_2.pri
+00000920: 7661 7465 5f6b 6579 2e73 6361 6eda 0473  vate_key.scan..s
+00000930: 6361 6e72 2000 0000 7212 0000 00da 076f  canr ...r......o
+00000940: 732e 7061 7468 7202 0000 0072 0300 0000  s.pathr....r....
+00000950: 7204 0000 0072 1700 0000 721e 0000 0072  r....r....r....r
+00000960: 2b00 0000 da06 6368 6563 6b73 7229 0000  +.....checksr)..
+00000970: 0072 2900 0000 7229 0000 0072 2a00 0000  .r)...r)...r*...
+00000980: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
+00000990: 0000 0004 011e 041e 011e 0108 0214 0108  ................
+000009a0: 0108 0108 0204 3f08 ff                   ......?..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/status_DER_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 '''
-	python3 status.proc.py "modules/EEC_448_2/_status/status_1_private_key/status_DER_1.py"
+	python3 status.proc.py "mixes/EEC_448_2/_status/status_1_private_key/status_DER_1.py"
 '''
 
-import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
-import recycling.modules.EEC_448_2.private_key.etch as etch_EEC_448_private_key
-import recycling.modules.EEC_448_2.private_key.scan as private_scan
+import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+import recycling.mixes.EEC_448_2.private_key.etch as etch_EEC_448_private_key
+import recycling.mixes.EEC_448_2.private_key.scan as private_scan
 		
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import json
 		
 def check_1 ():
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_1_private_key/status_JSON_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 '''
-	python3 status.proc.py "modules/EEC_448_2/_status/status_1_private_key/status_JSON_1.py"
+	python3 status.proc.py "mixes/EEC_448_2/_status/status_1_private_key/status_JSON_1.py"
 '''
 
-import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
-import recycling.modules.EEC_448_2.private_key.etch as etch_EEC_448_private_key
-import recycling.modules.EEC_448_2.private_key.scan as private_scan
+import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+import recycling.mixes.EEC_448_2.private_key.etch as etch_EEC_448_private_key
+import recycling.mixes.EEC_448_2.private_key.scan as private_scan
 		
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import json
 		
 def check_1 ():
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_2_private_and_public_keys/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_2_private_and_public_keys/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 3448 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 780d 0000  o........@@fx...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 6a0d 0000  o........SQfj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d04 0200 0100 6d08 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
@@ -13,188 +13,187 @@
 000000c0: 0100 6d08 5a11 0100 6401 6402 6c12 6d02  ..m.Z...d.d.l.m.
 000000d0: 0200 0100 6d03 0200 0100 6d0e 0200 0100  ....m.....m.....
 000000e0: 6d0b 5a13 0100 6401 6402 6c14 5a14 6401  m.Z...d.d.l.Z.d.
 000000f0: 6403 6c15 6d16 5a16 6d17 5a17 6d18 5a18  d.l.m.Z.m.Z.m.Z.
 00000100: 0100 6401 6402 6c19 5a19 6401 6402 6c1a  ..d.d.l.Z.d.d.l.
 00000110: 5a1a 6404 6405 8400 5a1b 6406 6407 8400  Z.d.d...Z.d.d...
 00000120: 5a1c 6408 651c 6901 5a1d 6402 5300 2909  Z.d.e.i.Z.d.S.).
-00000130: 7a62 0a09 7079 7468 6f6e 3320 7374 6174  zb..python3 stat
-00000140: 7573 2e70 726f 632e 7079 2022 6d6f 6475  us.proc.py "modu
-00000150: 6c65 732f 4545 435f 3434 385f 322f 5f73  les/EEC_448_2/_s
-00000160: 7461 7475 732f 7374 6174 7573 5f32 5f70  tatus/status_2_p
-00000170: 7269 7661 7465 5f61 6e64 5f70 7562 6c69  rivate_and_publi
-00000180: 635f 6b65 7973 2f73 7461 7475 735f 312e  c_keys/status_1.
-00000190: 7079 220a e900 0000 004e 2903 da07 6469  py"......N)...di
-000001a0: 726e 616d 65da 046a 6f69 6eda 086e 6f72  rname..join..nor
-000001b0: 6d70 6174 6863 0100 0000 0000 0000 0000  mpathc..........
-000001c0: 0000 0200 0000 0a00 0000 4300 0000 7338  ..........C...s8
-000001d0: 0000 007a 0874 00a0 017c 00a1 0101 0057  ...z.t...|.....W
-000001e0: 0064 0053 0004 0074 0279 1b01 007d 0101  .d.S...t.y...}..
-000001f0: 007a 0757 0059 0064 007d 017e 0164 0053  .z.W.Y.d.}.~.d.S
-00000200: 0064 007d 017e 0177 0177 0029 014e 2903  .d.}.~.w.w.).N).
-00000210: da02 6f73 da06 7265 6d6f 7665 da09 4578  ..os..remove..Ex
-00000220: 6365 7074 696f 6e29 02da 0470 6174 68da  ception)...path.
-00000230: 0145 a900 720a 0000 00fa 672f 6861 6269  .E..r.....g/habi
-00000240: 7461 742f 7665 6e75 6573 2f73 7461 6765  tat/venues/stage
-00000250: 732f 7265 6379 636c 696e 672f 6d6f 6475  s/recycling/modu
-00000260: 6c65 732f 4545 435f 3434 385f 322f 5f73  les/EEC_448_2/_s
-00000270: 7461 7475 732f 7374 6174 7573 5f32 5f70  tatus/status_2_p
-00000280: 7269 7661 7465 5f61 6e64 5f70 7562 6c69  rivate_and_publi
-00000290: 635f 6b65 7973 2f73 7461 7475 735f 312e  c_keys/status_1.
-000002a0: 7079 da05 6572 6173 6513 0000 0073 0c00  py..erase....s..
-000002b0: 0000 0201 1001 0e01 0e01 0880 02ff 720c  ..............r.
-000002c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000002d0: 0900 0000 0900 0000 4300 0000 7326 0100  ........C...s&..
-000002e0: 0067 0064 01a2 017d 007c 0044 005d 8a7d  .g.d...}.|.D.].}
-000002f0: 0174 0074 0174 02a0 0374 04a1 016a 05a0  .t.t.t...t...j..
-00000300: 06a1 0064 0283 0283 0164 0317 007d 0274  ...d.....d...}.t
-00000310: 0074 0174 02a0 0374 04a1 016a 05a0 06a1  .t.t...t...j....
-00000320: 0064 0483 0283 0164 0317 007d 0374 077c  .d.....d...}.t.|
-00000330: 0283 0101 0074 077c 0383 0101 0074 08a0  .....t.|.....t..
-00000340: 097c 01a1 017d 047c 0464 0519 007d 057c  .|...}.|.d...}.|
-00000350: 0464 0619 007d 067c 0464 0719 007d 0774  .d...}.|.d...}.t
-00000360: 0aa0 0b7c 0274 0c6a 0d64 0864 067c 0464  ...|.t.j.d.d.|.d
-00000370: 0619 0069 0169 0164 0964 0a8d 0264 0ba1  ...i.i.d.d...d..
-00000380: 0301 0074 0ea0 0b7c 0264 0ba1 0264 0819  ...t...|.d...d..
-00000390: 0064 0619 007c 0464 0619 006b 0273 614a  .d...|.d...k.saJ
-000003a0: 0082 0174 0fa0 097c 05a1 017d 0874 10a0  ...t...|...}.t..
-000003b0: 0b7c 0374 0c6a 0d64 0c64 067c 0864 0619  .|.t.j.d.d.|.d..
-000003c0: 0069 0169 0164 0964 0a8d 0264 0ba1 0301  .i.i.d.d...d....
-000003d0: 0074 11a0 0b7c 0364 0ba1 0264 0c19 0064  .t...|.d...d...d
-000003e0: 0619 007c 0864 0619 006b 0273 884a 0082  ...|.d...k.s.J..
-000003f0: 0174 077c 0283 0101 0074 077c 0383 0101  .t.|.....t.|....
-00000400: 0071 0664 0053 0029 0d4e 2908 da72 3439  .q.d.S.).N)..r49
-00000410: 3836 3838 3862 3131 3335 3862 6633 6435  86888b11358bf3d5
-00000420: 3431 6234 3165 6561 3564 6165 6365 3163  41b41eea5daece1c
-00000430: 3665 6666 3634 3133 3061 3435 6663 3862  6eff64130a45fc8b
-00000440: 3963 6134 3866 3365 3065 3032 3436 3363  9ca48f3e0e02463c
-00000450: 3939 6335 6165 6463 3861 3834 3736 3836  99c5aedc8a847686
-00000460: 6436 3639 6237 6435 3437 6331 3866 6534  d669b7d547c18fe4
-00000470: 3438 6663 3531 3131 6361 3838 6634 6538  48fc5111ca88f4e8
-00000480: da72 3539 3836 3838 3862 3131 3335 3862  .r5986888b11358b
-00000490: 6633 6435 3431 6234 3165 6561 3564 6165  f3d541b41eea5dae
-000004a0: 6365 3163 3665 6666 3634 3133 3061 3435  ce1c6eff64130a45
-000004b0: 6663 3862 3963 6134 3866 3365 3065 3032  fc8b9ca48f3e0e02
-000004c0: 3436 3363 3939 6335 6165 6463 3861 3834  463c99c5aedc8a84
-000004d0: 3736 3836 6436 3639 6237 6435 3437 6331  7686d669b7d547c1
-000004e0: 3866 6534 3438 6663 3531 3131 6361 3838  8fe448fc5111ca88
-000004f0: 6634 6538 da72 3030 3030 3030 3030 3030  f4e8.r0000000000
+00000130: 7a60 0a09 7079 7468 6f6e 3320 7374 6174  z`..python3 stat
+00000140: 7573 2e70 726f 632e 7079 2022 6d69 7865  us.proc.py "mixe
+00000150: 732f 4545 435f 3434 385f 322f 5f73 7461  s/EEC_448_2/_sta
+00000160: 7475 732f 7374 6174 7573 5f32 5f70 7269  tus/status_2_pri
+00000170: 7661 7465 5f61 6e64 5f70 7562 6c69 635f  vate_and_public_
+00000180: 6b65 7973 2f73 7461 7475 735f 312e 7079  keys/status_1.py
+00000190: 220a e900 0000 004e 2903 da07 6469 726e  "......N)...dirn
+000001a0: 616d 65da 046a 6f69 6eda 086e 6f72 6d70  ame..join..normp
+000001b0: 6174 6863 0100 0000 0000 0000 0000 0000  athc............
+000001c0: 0200 0000 0a00 0000 4300 0000 7338 0000  ........C...s8..
+000001d0: 007a 0874 00a0 017c 00a1 0101 0057 0064  .z.t...|.....W.d
+000001e0: 0053 0004 0074 0279 1b01 007d 0101 007a  .S...t.y...}...z
+000001f0: 0757 0059 0064 007d 017e 0164 0053 0064  .W.Y.d.}.~.d.S.d
+00000200: 007d 017e 0177 0177 0029 014e 2903 da02  .}.~.w.w.).N)...
+00000210: 6f73 da06 7265 6d6f 7665 da09 4578 6365  os..remove..Exce
+00000220: 7074 696f 6e29 02da 0470 6174 68da 0145  ption)...path..E
+00000230: a900 720a 0000 00fa 652f 6861 6269 7461  ..r.....e/habita
+00000240: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
+00000250: 7265 6379 636c 696e 672f 6d69 7865 732f  recycling/mixes/
+00000260: 4545 435f 3434 385f 322f 5f73 7461 7475  EEC_448_2/_statu
+00000270: 732f 7374 6174 7573 5f32 5f70 7269 7661  s/status_2_priva
+00000280: 7465 5f61 6e64 5f70 7562 6c69 635f 6b65  te_and_public_ke
+00000290: 7973 2f73 7461 7475 735f 312e 7079 da05  ys/status_1.py..
+000002a0: 6572 6173 6513 0000 0073 0c00 0000 0201  erase....s......
+000002b0: 1001 0e01 0e01 0880 02ff 720c 0000 0063  ..........r....c
+000002c0: 0000 0000 0000 0000 0000 0000 0900 0000  ................
+000002d0: 0900 0000 4300 0000 7326 0100 0067 0064  ....C...s&...g.d
+000002e0: 01a2 017d 007c 0044 005d 8a7d 0174 0074  ...}.|.D.].}.t.t
+000002f0: 0174 02a0 0374 04a1 016a 05a0 06a1 0064  .t...t...j.....d
+00000300: 0283 0283 0164 0317 007d 0274 0074 0174  .....d...}.t.t.t
+00000310: 02a0 0374 04a1 016a 05a0 06a1 0064 0483  ...t...j.....d..
+00000320: 0283 0164 0317 007d 0374 077c 0283 0101  ...d...}.t.|....
+00000330: 0074 077c 0383 0101 0074 08a0 097c 01a1  .t.|.....t...|..
+00000340: 017d 047c 0464 0519 007d 057c 0464 0619  .}.|.d...}.|.d..
+00000350: 007d 067c 0464 0719 007d 0774 0aa0 0b7c  .}.|.d...}.t...|
+00000360: 0274 0c6a 0d64 0864 067c 0464 0619 0069  .t.j.d.d.|.d...i
+00000370: 0169 0164 0964 0a8d 0264 0ba1 0301 0074  .i.d.d...d.....t
+00000380: 0ea0 0b7c 0264 0ba1 0264 0819 0064 0619  ...|.d...d...d..
+00000390: 007c 0464 0619 006b 0273 614a 0082 0174  .|.d...k.saJ...t
+000003a0: 0fa0 097c 05a1 017d 0874 10a0 0b7c 0374  ...|...}.t...|.t
+000003b0: 0c6a 0d64 0c64 067c 0864 0619 0069 0169  .j.d.d.|.d...i.i
+000003c0: 0164 0964 0a8d 0264 0ba1 0301 0074 11a0  .d.d...d.....t..
+000003d0: 0b7c 0364 0ba1 0264 0c19 0064 0619 007c  .|.d...d...d...|
+000003e0: 0864 0619 006b 0273 884a 0082 0174 077c  .d...k.s.J...t.|
+000003f0: 0283 0101 0074 077c 0383 0101 0071 0664  .....t.|.....q.d
+00000400: 0053 0029 0d4e 2908 da72 3439 3836 3838  .S.).N)..r498688
+00000410: 3862 3131 3335 3862 6633 6435 3431 6234  8b11358bf3d541b4
+00000420: 3165 6561 3564 6165 6365 3163 3665 6666  1eea5daece1c6eff
+00000430: 3634 3133 3061 3435 6663 3862 3963 6134  64130a45fc8b9ca4
+00000440: 3866 3365 3065 3032 3436 3363 3939 6335  8f3e0e02463c99c5
+00000450: 6165 6463 3861 3834 3736 3836 6436 3639  aedc8a847686d669
+00000460: 6237 6435 3437 6331 3866 6534 3438 6663  b7d547c18fe448fc
+00000470: 3531 3131 6361 3838 6634 6538 da72 3539  5111ca88f4e8.r59
+00000480: 3836 3838 3862 3131 3335 3862 6633 6435  86888b11358bf3d5
+00000490: 3431 6234 3165 6561 3564 6165 6365 3163  41b41eea5daece1c
+000004a0: 3665 6666 3634 3133 3061 3435 6663 3862  6eff64130a45fc8b
+000004b0: 3963 6134 3866 3365 3065 3032 3436 3363  9ca48f3e0e02463c
+000004c0: 3939 6335 6165 6463 3861 3834 3736 3836  99c5aedc8a847686
+000004d0: 6436 3639 6237 6435 3437 6331 3866 6534  d669b7d547c18fe4
+000004e0: 3438 6663 3531 3131 6361 3838 6634 6538  48fc5111ca88f4e8
+000004f0: da72 3030 3030 3030 3030 3030 3030 3030  .r00000000000000
 00000500: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000510: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000520: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000530: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000540: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000550: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-00000560: 3030 3030 3030 3030 da72 6666 6666 6666  00000000.rffffff
+00000560: 3030 3030 da72 6666 6666 6666 6666 6666  0000.rffffffffff
 00000570: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000580: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000590: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000005a0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000005b0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000005c0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-000005d0: 6666 6666 6666 6666 6666 6666 da72 3132  ffffffffffff.r12
+000005d0: 6666 6666 6666 6666 da72 3132 3334 3132  ffffffff.r123412
 000005e0: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
 000005f0: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
 00000600: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
 00000610: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
 00000620: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
 00000630: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
-00000640: 3334 3132 3334 3132 3334 3132 3334 3132  3412341234123412
-00000650: da72 3066 3165 3066 3165 3066 3165 3066  .r0f1e0f1e0f1e0f
+00000640: 3334 3132 3334 3132 3334 3132 da72 3066  341234123412.r0f
+00000650: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 00000660: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 00000670: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 00000680: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 00000690: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 000006a0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
 000006b0: 3165 3066 3165 3066 3165 3066 3165 3066  1e0f1e0f1e0f1e0f
-000006c0: 3165 3066 da72 3133 3537 3931 3335 3739  1e0f.r1357913579
-000006d0: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-000006e0: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-000006f0: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000700: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000710: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000720: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000730: 3335 3739 3133 3537 da72 3234 3638 6566  35791357.r2468ef
-00000740: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-00000750: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-00000760: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-00000770: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-00000780: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-00000790: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-000007a0: 3234 3638 6566 3234 3638 6566 da15 4545  2468ef2468ef..EE
-000007b0: 435f 3434 385f 325f 7072 6976 6174 655f  C_448_2_private_
-000007c0: 6b65 797a 052e 4a53 4f4e da14 4545 435f  keyz..JSON..EEC_
-000007d0: 3434 385f 325f 7075 626c 6963 5f6b 6579  448_2_public_key
-000007e0: da08 696e 7374 616e 6365 7a16 4445 5220  ..instancez.DER 
-000007f0: 6865 7861 6465 6369 6d61 6c20 7374 7269  hexadecimal stri
-00000800: 6e67 7a0f 4445 5220 6279 7465 2073 7472  ngz.DER byte str
-00000810: 696e 677a 0b70 7269 7661 7465 206b 6579  ingz.private key
-00000820: e904 0000 0029 01da 0669 6e64 656e 74da  .....)...indent.
-00000830: 044a 534f 4e7a 0a70 7562 6c69 6320 6b65  .JSONz.public ke
-00000840: 7929 1272 0400 0000 7203 0000 00da 0770  y).r....r......p
-00000850: 6174 686c 6962 da04 5061 7468 da08 5f5f  athlib..Path..__
-00000860: 6669 6c65 5f5f da06 7061 7265 6e74 da07  file__..parent..
-00000870: 7265 736f 6c76 6572 0c00 0000 da1d 4545  resolver......EE
-00000880: 435f 3434 385f 325f 7072 6976 6174 655f  C_448_2_private_
-00000890: 6b65 795f 6372 6561 746f 72da 0663 7265  key_creator..cre
-000008a0: 6174 65da 1865 7463 685f 4545 435f 3434  ate..etch_EEC_44
-000008b0: 385f 7072 6976 6174 655f 6b65 79da 0573  8_private_key..s
-000008c0: 7461 7274 da04 6a73 6f6e da05 6475 6d70  tart..json..dump
-000008d0: 73da 1070 7269 7661 7465 5f6b 6579 5f73  s..private_key_s
-000008e0: 6361 6eda 1c45 4543 5f34 3438 5f32 5f70  can..EEC_448_2_p
-000008f0: 7562 6c69 635f 6b65 795f 6372 6561 746f  ublic_key_creato
-00000900: 72da 1965 7463 685f 4545 435f 3434 385f  r..etch_EEC_448_
-00000910: 325f 7075 626c 6963 5f6b 6579 da0f 7075  2_public_key..pu
-00000920: 626c 6963 5f6b 6579 5f73 6361 6e29 09da  blic_key_scan)..
-00000930: 0573 6565 6473 da04 7365 6564 da10 7072  .seeds..seed..pr
-00000940: 6976 6174 655f 6b65 795f 7061 7468 da0f  ivate_key_path..
-00000950: 7075 626c 6963 5f6b 6579 5f70 6174 68da  public_key_path.
-00000960: 0b70 7269 7661 7465 5f6b 6579 da14 7072  .private_key..pr
-00000970: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
-00000980: 6365 da22 7072 6976 6174 655f 6b65 795f  ce."private_key_
-00000990: 4445 525f 6865 7861 6465 6369 6d61 6c5f  DER_hexadecimal_
-000009a0: 7374 7269 6e67 da1b 7072 6976 6174 655f  string..private_
-000009b0: 6b65 795f 4445 525f 6279 7465 5f73 7472  key_DER_byte_str
-000009c0: 696e 67da 0a70 7562 6c69 635f 6b65 7972  ing..public_keyr
-000009d0: 0a00 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
-000009e0: 6368 6563 6b5f 3119 0000 0073 6800 0000  check_1....sh...
-000009f0: 0801 080b 0201 1401 02ff 0202 04fe 0203  ................
-00000a00: 1401 02ff 0202 04fe 0804 0801 0a07 0801  ................
-00000a10: 0801 0801 0405 0201 0401 0201 0801 02ff  ................
-00000a20: 02ff 0204 04fc 0205 04f9 120e 0601 08ff  ................
-00000a30: 0407 0201 04ff 0407 0201 0401 0201 0801  ................
-00000a40: 02ff 02ff 0204 04fc 0205 04f9 120f 0601  ................
-00000a50: 08ff 0804 0a01 04b8 7233 0000 007a 2a65  ........r3...z*e
-00000a60: 6c6c 6970 7469 6320 7075 626c 6963 2061  lliptic public a
-00000a70: 6e64 2070 7269 7661 7465 206b 6579 2067  nd private key g
-00000a80: 656e 6572 6174 696f 6e29 1eda 075f 5f64  eneration)...__d
-00000a90: 6f63 5f5f da2f 7265 6379 636c 696e 672e  oc__./recycling.
-00000aa0: 6d6f 6475 6c65 732e 4545 435f 3434 385f  modules.EEC_448_
-00000ab0: 322e 7072 6976 6174 655f 6b65 792e 6372  2.private_key.cr
-00000ac0: 6561 746f 72da 076d 6f64 756c 6573 da09  eator..modules..
-00000ad0: 4545 435f 3434 385f 3272 2e00 0000 da07  EEC_448_2r......
-00000ae0: 6372 6561 746f 7272 2000 0000 da2c 7265  creatorr ....,re
-00000af0: 6379 636c 696e 672e 6d6f 6475 6c65 732e  cycling.modules.
-00000b00: 4545 435f 3434 385f 322e 7072 6976 6174  EEC_448_2.privat
-00000b10: 655f 6b65 792e 6574 6368 da04 6574 6368  e_key.etch..etch
-00000b20: 7222 0000 00da 2c72 6563 7963 6c69 6e67  r"....,recycling
-00000b30: 2e6d 6f64 756c 6573 2e45 4543 5f34 3438  .modules.EEC_448
-00000b40: 5f32 2e70 7269 7661 7465 5f6b 6579 2e73  _2.private_key.s
-00000b50: 6361 6eda 0473 6361 6e72 2600 0000 da2e  can..scanr&.....
-00000b60: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-00000b70: 732e 4545 435f 3434 385f 322e 7075 626c  s.EEC_448_2.publ
-00000b80: 6963 5f6b 6579 2e63 7265 6174 6f72 7232  ic_key.creatorr2
-00000b90: 0000 0072 2700 0000 da2b 7265 6379 636c  ...r'....+recycl
-00000ba0: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-00000bb0: 3434 385f 322e 7075 626c 6963 5f6b 6579  448_2.public_key
-00000bc0: 2e65 7463 6872 2800 0000 da2b 7265 6379  .etchr(....+recy
-00000bd0: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000be0: 435f 3434 385f 322e 7075 626c 6963 5f6b  C_448_2.public_k
-00000bf0: 6579 2e73 6361 6e72 2900 0000 721b 0000  ey.scanr)...r...
-00000c00: 00da 076f 732e 7061 7468 7202 0000 0072  ...os.pathr....r
-00000c10: 0300 0000 7204 0000 0072 0500 0000 7224  ....r....r....r$
-00000c20: 0000 0072 0c00 0000 7233 0000 00da 0663  ...r....r3.....c
-00000c30: 6865 636b 7372 0a00 0000 720a 0000 0072  hecksr....r....r
-00000c40: 0a00 0000 720b 0000 00da 083c 6d6f 6475  ....r......<modu
-00000c50: 6c65 3e01 0000 0073 1e00 0000 0401 1e04  le>....s........
-00000c60: 1e01 1e01 1e02 1e01 1e01 0802 1401 0801  ................
-00000c70: 0801 0802 0806 0458 08ff                 .......X..
+000006c0: da72 3133 3537 3931 3335 3739 3133 3537  .r13579135791357
+000006d0: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+000006e0: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+000006f0: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000700: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000710: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000720: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000730: 3133 3537 da72 3234 3638 6566 3234 3638  1357.r2468ef2468
+00000740: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+00000750: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+00000760: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+00000770: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+00000780: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+00000790: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+000007a0: 6566 3234 3638 6566 da15 4545 435f 3434  ef2468ef..EEC_44
+000007b0: 385f 325f 7072 6976 6174 655f 6b65 797a  8_2_private_keyz
+000007c0: 052e 4a53 4f4e da14 4545 435f 3434 385f  ..JSON..EEC_448_
+000007d0: 325f 7075 626c 6963 5f6b 6579 da08 696e  2_public_key..in
+000007e0: 7374 616e 6365 7a16 4445 5220 6865 7861  stancez.DER hexa
+000007f0: 6465 6369 6d61 6c20 7374 7269 6e67 7a0f  decimal stringz.
+00000800: 4445 5220 6279 7465 2073 7472 696e 677a  DER byte stringz
+00000810: 0b70 7269 7661 7465 206b 6579 e904 0000  .private key....
+00000820: 0029 01da 0669 6e64 656e 74da 044a 534f  .)...indent..JSO
+00000830: 4e7a 0a70 7562 6c69 6320 6b65 7929 1272  Nz.public key).r
+00000840: 0400 0000 7203 0000 00da 0770 6174 686c  ....r......pathl
+00000850: 6962 da04 5061 7468 da08 5f5f 6669 6c65  ib..Path..__file
+00000860: 5f5f da06 7061 7265 6e74 da07 7265 736f  __..parent..reso
+00000870: 6c76 6572 0c00 0000 da1d 4545 435f 3434  lver......EEC_44
+00000880: 385f 325f 7072 6976 6174 655f 6b65 795f  8_2_private_key_
+00000890: 6372 6561 746f 72da 0663 7265 6174 65da  creator..create.
+000008a0: 1865 7463 685f 4545 435f 3434 385f 7072  .etch_EEC_448_pr
+000008b0: 6976 6174 655f 6b65 79da 0573 7461 7274  ivate_key..start
+000008c0: da04 6a73 6f6e da05 6475 6d70 73da 1070  ..json..dumps..p
+000008d0: 7269 7661 7465 5f6b 6579 5f73 6361 6eda  rivate_key_scan.
+000008e0: 1c45 4543 5f34 3438 5f32 5f70 7562 6c69  .EEC_448_2_publi
+000008f0: 635f 6b65 795f 6372 6561 746f 72da 1965  c_key_creator..e
+00000900: 7463 685f 4545 435f 3434 385f 325f 7075  tch_EEC_448_2_pu
+00000910: 626c 6963 5f6b 6579 da0f 7075 626c 6963  blic_key..public
+00000920: 5f6b 6579 5f73 6361 6e29 09da 0573 6565  _key_scan)...see
+00000930: 6473 da04 7365 6564 da10 7072 6976 6174  ds..seed..privat
+00000940: 655f 6b65 795f 7061 7468 da0f 7075 626c  e_key_path..publ
+00000950: 6963 5f6b 6579 5f70 6174 68da 0b70 7269  ic_key_path..pri
+00000960: 7661 7465 5f6b 6579 da14 7072 6976 6174  vate_key..privat
+00000970: 655f 6b65 795f 696e 7374 616e 6365 da22  e_key_instance."
+00000980: 7072 6976 6174 655f 6b65 795f 4445 525f  private_key_DER_
+00000990: 6865 7861 6465 6369 6d61 6c5f 7374 7269  hexadecimal_stri
+000009a0: 6e67 da1b 7072 6976 6174 655f 6b65 795f  ng..private_key_
+000009b0: 4445 525f 6279 7465 5f73 7472 696e 67da  DER_byte_string.
+000009c0: 0a70 7562 6c69 635f 6b65 7972 0a00 0000  .public_keyr....
+000009d0: 720a 0000 0072 0b00 0000 da07 6368 6563  r....r......chec
+000009e0: 6b5f 3119 0000 0073 6800 0000 0801 080b  k_1....sh.......
+000009f0: 0201 1401 02ff 0202 04fe 0203 1401 02ff  ................
+00000a00: 0202 04fe 0804 0801 0a07 0801 0801 0801  ................
+00000a10: 0405 0201 0401 0201 0801 02ff 02ff 0204  ................
+00000a20: 04fc 0205 04f9 120e 0601 08ff 0407 0201  ................
+00000a30: 04ff 0407 0201 0401 0201 0801 02ff 02ff  ................
+00000a40: 0204 04fc 0205 04f9 120f 0601 08ff 0804  ................
+00000a50: 0a01 04b8 7233 0000 007a 2a65 6c6c 6970  ....r3...z*ellip
+00000a60: 7469 6320 7075 626c 6963 2061 6e64 2070  tic public and p
+00000a70: 7269 7661 7465 206b 6579 2067 656e 6572  rivate key gener
+00000a80: 6174 696f 6e29 1eda 075f 5f64 6f63 5f5f  ation)...__doc__
+00000a90: da2d 7265 6379 636c 696e 672e 6d69 7865  .-recycling.mixe
+00000aa0: 732e 4545 435f 3434 385f 322e 7072 6976  s.EEC_448_2.priv
+00000ab0: 6174 655f 6b65 792e 6372 6561 746f 72da  ate_key.creator.
+00000ac0: 056d 6978 6573 da09 4545 435f 3434 385f  .mixes..EEC_448_
+00000ad0: 3272 2e00 0000 da07 6372 6561 746f 7272  2r......creatorr
+00000ae0: 2000 0000 da2a 7265 6379 636c 696e 672e   ....*recycling.
+00000af0: 6d69 7865 732e 4545 435f 3434 385f 322e  mixes.EEC_448_2.
+00000b00: 7072 6976 6174 655f 6b65 792e 6574 6368  private_key.etch
+00000b10: da04 6574 6368 7222 0000 00da 2a72 6563  ..etchr"....*rec
+00000b20: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000b30: 5f34 3438 5f32 2e70 7269 7661 7465 5f6b  _448_2.private_k
+00000b40: 6579 2e73 6361 6eda 0473 6361 6e72 2600  ey.scan..scanr&.
+00000b50: 0000 da2c 7265 6379 636c 696e 672e 6d69  ...,recycling.mi
+00000b60: 7865 732e 4545 435f 3434 385f 322e 7075  xes.EEC_448_2.pu
+00000b70: 626c 6963 5f6b 6579 2e63 7265 6174 6f72  blic_key.creator
+00000b80: 7232 0000 0072 2700 0000 da29 7265 6379  r2...r'....)recy
+00000b90: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+00000ba0: 3434 385f 322e 7075 626c 6963 5f6b 6579  448_2.public_key
+00000bb0: 2e65 7463 6872 2800 0000 da29 7265 6379  .etchr(....)recy
+00000bc0: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+00000bd0: 3434 385f 322e 7075 626c 6963 5f6b 6579  448_2.public_key
+00000be0: 2e73 6361 6e72 2900 0000 721b 0000 00da  .scanr)...r.....
+00000bf0: 076f 732e 7061 7468 7202 0000 0072 0300  .os.pathr....r..
+00000c00: 0000 7204 0000 0072 0500 0000 7224 0000  ..r....r....r$..
+00000c10: 0072 0c00 0000 7233 0000 00da 0663 6865  .r....r3.....che
+00000c20: 636b 7372 0a00 0000 720a 0000 0072 0a00  cksr....r....r..
+00000c30: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000c40: 3e01 0000 0073 1e00 0000 0401 1e04 1e01  >....s..........
+00000c50: 1e01 1e02 1e01 1e01 0802 1401 0801 0801  ................
+00000c60: 0802 0806 0458 08ff                      .....X..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 '''
-	python3 status.proc.py "modules/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py"
+	python3 status.proc.py "mixes/EEC_448_2/_status/status_2_private_and_public_keys/status_1.py"
 '''
 
-import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
-import recycling.modules.EEC_448_2.private_key.etch as etch_EEC_448_private_key
-import recycling.modules.EEC_448_2.private_key.scan as private_key_scan
+import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+import recycling.mixes.EEC_448_2.private_key.etch as etch_EEC_448_private_key
+import recycling.mixes.EEC_448_2.private_key.scan as private_key_scan
 
-import recycling.modules.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
-import recycling.modules.EEC_448_2.public_key.etch as etch_EEC_448_2_public_key
-import recycling.modules.EEC_448_2.public_key.scan as public_key_scan
+import recycling.mixes.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
+import recycling.mixes.EEC_448_2.public_key.etch as etch_EEC_448_2_public_key
+import recycling.mixes.EEC_448_2.public_key.scan as public_key_scan
 		
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import json
 
 def erase (path):
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_3_sign_and_verify/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 5386 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 0a15 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 f214 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d04 0200 0100 6d08 5a09 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0a 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
@@ -22,262 +22,261 @@
 00000150: 0100 6401 6402 6c1e 6d02 0200 0100 6d03  ..d.d.l.m.....m.
 00000160: 0200 0100 6d1f 0200 0100 6d20 0200 0100  ....m.....m ....
 00000170: 6d21 5a22 0100 6401 6402 6c23 5a23 6401  m!Z"..d.d.l#Z#d.
 00000180: 6403 6c24 6d25 5a25 6d26 5a26 6d27 5a27  d.l$m%Z%m&Z&m'Z'
 00000190: 0100 6401 6402 6c28 5a28 6401 6402 6c29  ..d.d.l(Z(d.d.l)
 000001a0: 5a29 6404 6405 8400 5a2a 6406 6407 8400  Z)d.d...Z*d.d...
 000001b0: 5a2b 6408 652b 6901 5a2c 6402 5300 2909  Z+d.e+i.Z,d.S.).
-000001c0: 7a5a 0a09 7079 7468 6f6e 3320 7374 6174  zZ..python3 stat
-000001d0: 7573 2e70 726f 632e 7079 2022 6d6f 6475  us.proc.py "modu
-000001e0: 6c65 732f 4545 435f 3434 385f 322f 5f73  les/EEC_448_2/_s
-000001f0: 7461 7475 732f 7374 6174 7573 5f33 5f73  tatus/status_3_s
-00000200: 6967 6e5f 616e 645f 7665 7269 6679 2f73  ign_and_verify/s
-00000210: 7461 7475 735f 312e 7079 220a e900 0000  tatus_1.py".....
-00000220: 004e 2903 da07 6469 726e 616d 65da 046a  .N)...dirname..j
-00000230: 6f69 6eda 086e 6f72 6d70 6174 6863 0100  oin..normpathc..
-00000240: 0000 0000 0000 0000 0000 0200 0000 0a00  ................
-00000250: 0000 4300 0000 7338 0000 007a 0874 00a0  ..C...s8...z.t..
-00000260: 017c 00a1 0101 0057 0064 0053 0004 0074  .|.....W.d.S...t
-00000270: 0279 1b01 007d 0101 007a 0757 0059 0064  .y...}...z.W.Y.d
-00000280: 007d 017e 0164 0053 0064 007d 017e 0177  .}.~.d.S.d.}.~.w
-00000290: 0177 0029 014e 2903 da02 6f73 da06 7265  .w.).N)...os..re
-000002a0: 6d6f 7665 da09 4578 6365 7074 696f 6e29  move..Exception)
-000002b0: 02da 0470 6174 68da 0145 a900 720a 0000  ...path..E..r...
-000002c0: 00fa 5f2f 6861 6269 7461 742f 7665 6e75  .._/habitat/venu
-000002d0: 6573 2f73 7461 6765 732f 7265 6379 636c  es/stages/recycl
-000002e0: 696e 672f 6d6f 6475 6c65 732f 4545 435f  ing/modules/EEC_
-000002f0: 3434 385f 322f 5f73 7461 7475 732f 7374  448_2/_status/st
-00000300: 6174 7573 5f33 5f73 6967 6e5f 616e 645f  atus_3_sign_and_
-00000310: 7665 7269 6679 2f73 7461 7475 735f 312e  verify/status_1.
-00000320: 7079 da05 6572 6173 651a 0000 0073 0c00  py..erase....s..
-00000330: 0000 0201 1001 0e01 0e01 0880 02ff 720c  ..............r.
-00000340: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000350: 1000 0000 0900 0000 4300 0000 73f0 0100  ........C...s...
-00000360: 0067 0064 01a2 017d 007c 0044 005d ef7d  .g.d...}.|.D.].}
-00000370: 0174 0074 0174 02a0 0374 04a1 016a 05a0  .t.t.t...t...j..
-00000380: 06a1 0064 0283 0283 0164 0317 007d 0274  ...d.....d...}.t
-00000390: 0074 0174 02a0 0374 04a1 016a 05a0 06a1  .t.t...t...j....
-000003a0: 0064 0483 0283 0164 0317 007d 0374 077c  .d.....d...}.t.|
-000003b0: 0283 0101 0074 077c 0383 0101 0074 08a0  .....t.|.....t..
-000003c0: 097c 01a1 017d 047c 0464 0519 007d 057c  .|...}.|.d...}.|
-000003d0: 0464 0619 007d 067c 0464 0719 007d 0774  .d...}.|.d...}.t
-000003e0: 0aa0 0b7c 0274 0c6a 0d64 0864 067c 0464  ...|.t.j.d.d.|.d
-000003f0: 0619 0069 0169 0164 0964 0a8d 0264 0ba1  ...i.i.d.d...d..
-00000400: 0301 0074 0ea0 0b7c 0264 0ba1 0264 0819  ...t...|.d...d..
-00000410: 0064 0619 007c 0464 0619 006b 0273 614a  .d...|.d...k.saJ
-00000420: 0082 0174 0fa0 1074 0ea0 0b7c 0264 0ba1  ...t...t...|.d..
-00000430: 0264 0819 0064 0619 00a1 0101 0074 11a0  .d...d.......t..
-00000440: 097c 05a1 017d 087c 0864 0519 007d 0974  .|...}.|.d...}.t
-00000450: 12a0 0b7c 0374 0c6a 0d64 0c64 067c 0864  ...|.t.j.d.d.|.d
-00000460: 0619 0069 0169 0164 0964 0a8d 0264 0ba1  ...i.i.d.d...d..
-00000470: 0301 0074 13a0 0b7c 0364 0ba1 0264 0c19  ...t...|.d...d..
-00000480: 0064 0619 007c 0864 0619 006b 0273 994a  .d...|.d...k.s.J
-00000490: 0082 0174 14a0 1074 13a0 0b7c 0364 0ba1  ...t...t...|.d..
-000004a0: 0264 0c19 0064 0619 00a1 0101 0074 0c6a  .d...d.......t.j
-000004b0: 0d64 0d64 0e64 0f64 109c 0264 1164 129c  .d.d.d.d...d.d..
-000004c0: 0264 139c 0264 0964 0a8d 027d 0a7c 0aa0  .d...d.d...}.|..
-000004d0: 1564 14a1 017d 0b74 166a 0b7c 057c 0b64  .d...}.t.j.|.|.d
-000004e0: 158d 027d 0c7c 0c64 1619 007d 0d74 1764  ...}.|.d...}.t.d
-000004f0: 177c 0d83 0201 0074 186a 0b7c 0974 19a0  .|.....t.j.|.t..
-00000500: 1a7c 0da1 017c 0b64 188d 037d 0e7c 0e64  .|...|.d...}.|.d
-00000510: 196b 0273 dc4a 0082 0174 186a 0b7c 0974  .k.s.J...t.j.|.t
-00000520: 19a0 1a7c 0da1 0164 1a64 188d 037d 0f7c  ...|...d.d...}.|
-00000530: 0f64 1b6b 0273 ed4a 0082 0174 077c 0283  .d.k.s.J...t.|..
-00000540: 0101 0074 077c 0383 0101 0071 0664 0053  ...t.|.....q.d.S
-00000550: 0029 1c4e 2908 da72 3439 3836 3838 3862  .).N)..r4986888b
-00000560: 3131 3335 3862 6633 6435 3431 6234 3165  11358bf3d541b41e
-00000570: 6561 3564 6165 6365 3163 3665 6666 3634  ea5daece1c6eff64
-00000580: 3133 3061 3435 6663 3862 3963 6134 3866  130a45fc8b9ca48f
-00000590: 3365 3065 3032 3436 3363 3939 6335 6165  3e0e02463c99c5ae
-000005a0: 6463 3861 3834 3736 3836 6436 3639 6237  dc8a847686d669b7
-000005b0: 6435 3437 6331 3866 6534 3438 6663 3531  d547c18fe448fc51
-000005c0: 3131 6361 3838 6634 6538 da72 3539 3836  11ca88f4e8.r5986
-000005d0: 3838 3862 3131 3335 3862 6633 6435 3431  888b11358bf3d541
-000005e0: 6234 3165 6561 3564 6165 6365 3163 3665  b41eea5daece1c6e
-000005f0: 6666 3634 3133 3061 3435 6663 3862 3963  ff64130a45fc8b9c
-00000600: 6134 3866 3365 3065 3032 3436 3363 3939  a48f3e0e02463c99
-00000610: 6335 6165 6463 3861 3834 3736 3836 6436  c5aedc8a847686d6
-00000620: 3639 6237 6435 3437 6331 3866 6534 3438  69b7d547c18fe448
-00000630: 6663 3531 3131 6361 3838 6634 6538 da72  fc5111ca88f4e8.r
+000001c0: 7a58 0a09 7079 7468 6f6e 3320 7374 6174  zX..python3 stat
+000001d0: 7573 2e70 726f 632e 7079 2022 6d69 7865  us.proc.py "mixe
+000001e0: 732f 4545 435f 3434 385f 322f 5f73 7461  s/EEC_448_2/_sta
+000001f0: 7475 732f 7374 6174 7573 5f33 5f73 6967  tus/status_3_sig
+00000200: 6e5f 616e 645f 7665 7269 6679 2f73 7461  n_and_verify/sta
+00000210: 7475 735f 312e 7079 220a e900 0000 004e  tus_1.py"......N
+00000220: 2903 da07 6469 726e 616d 65da 046a 6f69  )...dirname..joi
+00000230: 6eda 086e 6f72 6d70 6174 6863 0100 0000  n..normpathc....
+00000240: 0000 0000 0000 0000 0200 0000 0a00 0000  ................
+00000250: 4300 0000 7338 0000 007a 0874 00a0 017c  C...s8...z.t...|
+00000260: 00a1 0101 0057 0064 0053 0004 0074 0279  .....W.d.S...t.y
+00000270: 1b01 007d 0101 007a 0757 0059 0064 007d  ...}...z.W.Y.d.}
+00000280: 017e 0164 0053 0064 007d 017e 0177 0177  .~.d.S.d.}.~.w.w
+00000290: 0029 014e 2903 da02 6f73 da06 7265 6d6f  .).N)...os..remo
+000002a0: 7665 da09 4578 6365 7074 696f 6e29 02da  ve..Exception)..
+000002b0: 0470 6174 68da 0145 a900 720a 0000 00fa  .path..E..r.....
+000002c0: 5d2f 6861 6269 7461 742f 7665 6e75 6573  ]/habitat/venues
+000002d0: 2f73 7461 6765 732f 7265 6379 636c 696e  /stages/recyclin
+000002e0: 672f 6d69 7865 732f 4545 435f 3434 385f  g/mixes/EEC_448_
+000002f0: 322f 5f73 7461 7475 732f 7374 6174 7573  2/_status/status
+00000300: 5f33 5f73 6967 6e5f 616e 645f 7665 7269  _3_sign_and_veri
+00000310: 6679 2f73 7461 7475 735f 312e 7079 da05  fy/status_1.py..
+00000320: 6572 6173 651a 0000 0073 0c00 0000 0201  erase....s......
+00000330: 1001 0e01 0e01 0880 02ff 720c 0000 0063  ..........r....c
+00000340: 0000 0000 0000 0000 0000 0000 1000 0000  ................
+00000350: 0900 0000 4300 0000 73f0 0100 0067 0064  ....C...s....g.d
+00000360: 01a2 017d 007c 0044 005d ef7d 0174 0074  ...}.|.D.].}.t.t
+00000370: 0174 02a0 0374 04a1 016a 05a0 06a1 0064  .t...t...j.....d
+00000380: 0283 0283 0164 0317 007d 0274 0074 0174  .....d...}.t.t.t
+00000390: 02a0 0374 04a1 016a 05a0 06a1 0064 0483  ...t...j.....d..
+000003a0: 0283 0164 0317 007d 0374 077c 0283 0101  ...d...}.t.|....
+000003b0: 0074 077c 0383 0101 0074 08a0 097c 01a1  .t.|.....t...|..
+000003c0: 017d 047c 0464 0519 007d 057c 0464 0619  .}.|.d...}.|.d..
+000003d0: 007d 067c 0464 0719 007d 0774 0aa0 0b7c  .}.|.d...}.t...|
+000003e0: 0274 0c6a 0d64 0864 067c 0464 0619 0069  .t.j.d.d.|.d...i
+000003f0: 0169 0164 0964 0a8d 0264 0ba1 0301 0074  .i.d.d...d.....t
+00000400: 0ea0 0b7c 0264 0ba1 0264 0819 0064 0619  ...|.d...d...d..
+00000410: 007c 0464 0619 006b 0273 614a 0082 0174  .|.d...k.saJ...t
+00000420: 0fa0 1074 0ea0 0b7c 0264 0ba1 0264 0819  ...t...|.d...d..
+00000430: 0064 0619 00a1 0101 0074 11a0 097c 05a1  .d.......t...|..
+00000440: 017d 087c 0864 0519 007d 0974 12a0 0b7c  .}.|.d...}.t...|
+00000450: 0374 0c6a 0d64 0c64 067c 0864 0619 0069  .t.j.d.d.|.d...i
+00000460: 0169 0164 0964 0a8d 0264 0ba1 0301 0074  .i.d.d...d.....t
+00000470: 13a0 0b7c 0364 0ba1 0264 0c19 0064 0619  ...|.d...d...d..
+00000480: 007c 0864 0619 006b 0273 994a 0082 0174  .|.d...k.s.J...t
+00000490: 14a0 1074 13a0 0b7c 0364 0ba1 0264 0c19  ...t...|.d...d..
+000004a0: 0064 0619 00a1 0101 0074 0c6a 0d64 0d64  .d.......t.j.d.d
+000004b0: 0e64 0f64 109c 0264 1164 129c 0264 139c  .d.d...d.d...d..
+000004c0: 0264 0964 0a8d 027d 0a7c 0aa0 1564 14a1  .d.d...}.|...d..
+000004d0: 017d 0b74 166a 0b7c 057c 0b64 158d 027d  .}.t.j.|.|.d...}
+000004e0: 0c7c 0c64 1619 007d 0d74 1764 177c 0d83  .|.d...}.t.d.|..
+000004f0: 0201 0074 186a 0b7c 0974 19a0 1a7c 0da1  ...t.j.|.t...|..
+00000500: 017c 0b64 188d 037d 0e7c 0e64 196b 0273  .|.d...}.|.d.k.s
+00000510: dc4a 0082 0174 186a 0b7c 0974 19a0 1a7c  .J...t.j.|.t...|
+00000520: 0da1 0164 1a64 188d 037d 0f7c 0f64 1b6b  ...d.d...}.|.d.k
+00000530: 0273 ed4a 0082 0174 077c 0283 0101 0074  .s.J...t.|.....t
+00000540: 077c 0383 0101 0071 0664 0053 0029 1c4e  .|.....q.d.S.).N
+00000550: 2908 da72 3439 3836 3838 3862 3131 3335  )..r4986888b1135
+00000560: 3862 6633 6435 3431 6234 3165 6561 3564  8bf3d541b41eea5d
+00000570: 6165 6365 3163 3665 6666 3634 3133 3061  aece1c6eff64130a
+00000580: 3435 6663 3862 3963 6134 3866 3365 3065  45fc8b9ca48f3e0e
+00000590: 3032 3436 3363 3939 6335 6165 6463 3861  02463c99c5aedc8a
+000005a0: 3834 3736 3836 6436 3639 6237 6435 3437  847686d669b7d547
+000005b0: 6331 3866 6534 3438 6663 3531 3131 6361  c18fe448fc5111ca
+000005c0: 3838 6634 6538 da72 3539 3836 3838 3862  88f4e8.r5986888b
+000005d0: 3131 3335 3862 6633 6435 3431 6234 3165  11358bf3d541b41e
+000005e0: 6561 3564 6165 6365 3163 3665 6666 3634  ea5daece1c6eff64
+000005f0: 3133 3061 3435 6663 3862 3963 6134 3866  130a45fc8b9ca48f
+00000600: 3365 3065 3032 3436 3363 3939 6335 6165  3e0e02463c99c5ae
+00000610: 6463 3861 3834 3736 3836 6436 3639 6237  dc8a847686d669b7
+00000620: 6435 3437 6331 3866 6534 3438 6663 3531  d547c18fe448fc51
+00000630: 3131 6361 3838 6634 6538 da72 3030 3030  11ca88f4e8.r0000
 00000640: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000650: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000660: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000670: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000680: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
 00000690: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-000006a0: 3030 3030 3030 3030 3030 3030 3030 3030  0000000000000000
-000006b0: 3030 da72 6666 6666 6666 6666 6666 6666  00.rffffffffffff
+000006a0: 3030 3030 3030 3030 3030 3030 3030 da72  00000000000000.r
+000006b0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000006c0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000006d0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000006e0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 000006f0: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000700: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
 00000710: 6666 6666 6666 6666 6666 6666 6666 6666  ffffffffffffffff
-00000720: 6666 6666 6666 da72 3132 3334 3132 3334  ffffff.r12341234
+00000720: 6666 da72 3132 3334 3132 3334 3132 3334  ff.r123412341234
 00000730: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
 00000740: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
 00000750: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
 00000760: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
 00000770: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
 00000780: 3132 3334 3132 3334 3132 3334 3132 3334  1234123412341234
-00000790: 3132 3334 3132 3334 3132 da72 3066 3165  1234123412.r0f1e
+00000790: 3132 3334 3132 da72 3066 3165 3066 3165  123412.r0f1e0f1e
 000007a0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
 000007b0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
 000007c0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
 000007d0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
 000007e0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
 000007f0: 3066 3165 3066 3165 3066 3165 3066 3165  0f1e0f1e0f1e0f1e
-00000800: 3066 3165 3066 3165 3066 3165 3066 da72  0f1e0f1e0f1e0f.r
-00000810: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000820: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000830: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
-00000840: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
-00000850: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
-00000860: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
-00000870: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
-00000880: 3537 da72 3234 3638 6566 3234 3638 6566  57.r2468ef2468ef
-00000890: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-000008a0: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-000008b0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-000008c0: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
-000008d0: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
-000008e0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
-000008f0: 3234 3638 6566 da15 4545 435f 3434 385f  2468ef..EEC_448_
-00000900: 325f 7072 6976 6174 655f 6b65 797a 052e  2_private_keyz..
-00000910: 4a53 4f4e da14 4545 435f 3434 385f 325f  JSON..EEC_448_2_
-00000920: 7075 626c 6963 5f6b 6579 da08 696e 7374  public_key..inst
-00000930: 616e 6365 7a16 4445 5220 6865 7861 6465  ancez.DER hexade
-00000940: 6369 6d61 6c20 7374 7269 6e67 7a0f 4445  cimal stringz.DE
-00000950: 5220 6279 7465 2073 7472 696e 677a 0b70  R byte stringz.p
-00000960: 7269 7661 7465 206b 6579 e904 0000 0029  rivate key.....)
-00000970: 01da 0669 6e64 656e 74da 044a 534f 4e7a  ...indent..JSONz
-00000980: 0a70 7562 6c69 6320 6b65 79da 0473 656e  .public key..sen
-00000990: 64da 0945 4543 5f34 3438 5f31 da8a 3330  d..EEC_448_1..30
-000009a0: 3433 3330 3035 3036 3033 3262 3635 3731  43300506032b6571
-000009b0: 3033 3361 3030 6532 3639 3630 6138 3363  033a00e26960a83c
-000009c0: 3435 6330 6262 3836 6533 3536 6364 3732  45c0bb86e356cd72
-000009d0: 3734 3733 6539 3636 3832 6537 3663 3664  7473e96682e76c6d
-000009e0: 6430 3163 3939 3161 3665 6130 6133 3934  d01c991a6ea0a394
-000009f0: 6563 6361 3237 6234 3637 3535 3464 3733  ecca27b467554d73
-00000a00: 6532 6132 3262 3035 3432 3563 3139 3236  e2a22b05425c1926
-00000a10: 6137 6139 3262 6566 6461 3563 3139 3337  a7a92befda5c1937
-00000a20: 6436 3837 3666 3030 2902 da06 666f 726d  d6876f00)...form
-00000a30: 6174 da07 6164 6472 6573 73da 0e34 3033  at..address..403
-00000a40: 3234 3738 3933 3234 3837 3329 02da 0274  24789324873)...t
-00000a50: 6fda 0661 6d6f 756e 7429 02da 046d 6f76  o..amount)...mov
-00000a60: 65da 0666 6965 6c64 737a 0575 7466 2d38  e..fieldsz.utf-8
-00000a70: 2901 da0e 756e 7369 676e 6564 5f62 7974  )...unsigned_byt
-00000a80: 6573 7a18 7369 676e 6564 2062 7974 6573  esz.signed bytes
-00000a90: 2068 6578 6164 6563 696d 616c 7a19 7369   hexadecimalz.si
-00000aa0: 676e 6564 5f62 7974 6573 5f68 6578 6164  gned_bytes_hexad
-00000ab0: 6563 696d 616c 3a29 02da 0c73 6967 6e65  ecimal:)...signe
-00000ac0: 645f 6279 7465 7372 2500 0000 da03 7965  d_bytesr%.....ye
-00000ad0: 73f3 0000 0000 da02 6e6f 291b 7204 0000  s.......no).r...
-00000ae0: 0072 0300 0000 da07 7061 7468 6c69 62da  .r......pathlib.
-00000af0: 0450 6174 68da 085f 5f66 696c 655f 5fda  .Path..__file__.
-00000b00: 0670 6172 656e 74da 0772 6573 6f6c 7665  .parent..resolve
-00000b10: 720c 0000 00da 1d45 4543 5f34 3438 5f32  r......EEC_448_2
-00000b20: 5f70 7269 7661 7465 5f6b 6579 5f63 7265  _private_key_cre
-00000b30: 6174 6f72 da06 6372 6561 7465 da18 6574  ator..create..et
-00000b40: 6368 5f45 4543 5f34 3438 5f70 7269 7661  ch_EEC_448_priva
-00000b50: 7465 5f6b 6579 da05 7374 6172 74da 046a  te_key..start..j
-00000b60: 736f 6eda 0564 756d 7073 da10 7072 6976  son..dumps..priv
-00000b70: 6174 655f 6b65 795f 7363 616e da17 696e  ate_key_scan..in
-00000b80: 7374 616e 7469 6174 655f 7072 6976 6174  stantiate_privat
-00000b90: 655f 6b65 79da 1b66 726f 6d5f 4445 525f  e_key..from_DER_
-00000ba0: 6865 7861 6465 6369 6d61 6c5f 7374 7269  hexadecimal_stri
-00000bb0: 6e67 da1c 4545 435f 3434 385f 325f 7075  ng..EEC_448_2_pu
-00000bc0: 626c 6963 5f6b 6579 5f63 7265 6174 6f72  blic_key_creator
-00000bd0: da19 6574 6368 5f45 4543 5f34 3438 5f32  ..etch_EEC_448_2
-00000be0: 5f70 7562 6c69 635f 6b65 79da 0f70 7562  _public_key..pub
-00000bf0: 6c69 635f 6b65 795f 7363 616e da16 696e  lic_key_scan..in
-00000c00: 7374 616e 7469 6174 655f 7075 626c 6963  stantiate_public
-00000c10: 5f6b 6579 da06 656e 636f 6465 da0e 4545  _key..encode..EE
-00000c20: 435f 3434 385f 325f 7369 676e da05 7072  C_448_2_sign..pr
-00000c30: 696e 74da 0676 6572 6966 79da 1a68 6578  int..verify..hex
-00000c40: 6164 6563 696d 616c 5f74 6f5f 6279 7465  adecimal_to_byte
-00000c50: 5f73 7472 696e 67da 086d 6f64 756c 6174  _string..modulat
-00000c60: 6529 10da 0573 6565 6473 da04 7365 6564  e)...seeds..seed
-00000c70: da10 7072 6976 6174 655f 6b65 795f 7061  ..private_key_pa
-00000c80: 7468 da0f 7075 626c 6963 5f6b 6579 5f70  th..public_key_p
-00000c90: 6174 68da 0b70 7269 7661 7465 5f6b 6579  ath..private_key
-00000ca0: da14 7072 6976 6174 655f 6b65 795f 696e  ..private_key_in
-00000cb0: 7374 616e 6365 da22 7072 6976 6174 655f  stance."private_
-00000cc0: 6b65 795f 4445 525f 6865 7861 6465 6369  key_DER_hexadeci
-00000cd0: 6d61 6c5f 7374 7269 6e67 da1b 7072 6976  mal_string..priv
-00000ce0: 6174 655f 6b65 795f 4445 525f 6279 7465  ate_key_DER_byte
-00000cf0: 5f73 7472 696e 67da 0a70 7562 6c69 635f  _string..public_
-00000d00: 6b65 79da 1370 7562 6c69 635f 6b65 795f  key..public_key_
-00000d10: 696e 7374 616e 6365 da0e 756e 6963 6f64  instance..unicod
-00000d20: 655f 7374 7269 6e67 7225 0000 00da 0673  e_stringr%.....s
-00000d30: 6967 6e65 64da 1873 6967 6e65 645f 6279  igned..signed_by
-00000d40: 7465 735f 6865 7861 6465 6369 6d61 6cda  tes_hexadecimal.
-00000d50: 0e76 6572 6966 6963 6174 696f 6e5f 31da  .verification_1.
-00000d60: 0e76 6572 6966 6963 6174 696f 6e5f 3272  .verification_2r
-00000d70: 0a00 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
-00000d80: 6368 6563 6b5f 3120 0000 0073 b200 0000  check_1 ...s....
-00000d90: 0801 080b 0201 1401 02ff 0202 04fe 0203  ................
-00000da0: 1401 02ff 0202 04fe 0804 0801 0a06 0801  ................
-00000db0: 0801 0801 0405 0201 0401 0201 0801 02ff  ................
-00000dc0: 02ff 0204 04fc 0205 04f9 120e 0601 08ff  ................
-00000dd0: 0407 1201 04ff 0409 0201 04ff 0803 0405  ................
-00000de0: 0201 0401 0201 0801 02ff 02ff 0204 04fc  ................
-00000df0: 0205 04f9 120e 0601 08ff 0407 1201 04ff  ................
-00000e00: 0408 0201 0203 0201 04fe 0204 04fb 04fe  ................
-00000e10: 0209 06f7 0a0a 0402 0201 0201 06fe 0804  ................
-00000e20: 0a02 0405 0201 0802 0201 06fc 0c06 0405  ................
-00000e30: 0201 0802 0201 06fc 0c06 0804 0a01 0081  ................
-00000e40: 04f8 7251 0000 007a 2a65 6c6c 6970 7469  ..rQ...z*ellipti
-00000e50: 6320 7075 626c 6963 2061 6e64 2070 7269  c public and pri
-00000e60: 7661 7465 206b 6579 2067 656e 6572 6174  vate key generat
-00000e70: 696f 6e29 2dda 075f 5f64 6f63 5f5f da2f  ion)-..__doc__./
-00000e80: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-00000e90: 732e 4545 435f 3434 385f 322e 7072 6976  s.EEC_448_2.priv
-00000ea0: 6174 655f 6b65 792e 6372 6561 746f 72da  ate_key.creator.
-00000eb0: 076d 6f64 756c 6573 da09 4545 435f 3434  .modules..EEC_44
-00000ec0: 385f 3272 4600 0000 da07 6372 6561 746f  8_2rF.....creato
-00000ed0: 7272 2f00 0000 da2c 7265 6379 636c 696e  rr/....,recyclin
-00000ee0: 672e 6d6f 6475 6c65 732e 4545 435f 3434  g.modules.EEC_44
-00000ef0: 385f 322e 7072 6976 6174 655f 6b65 792e  8_2.private_key.
-00000f00: 6574 6368 da04 6574 6368 7231 0000 00da  etch..etchr1....
-00000f10: 2c72 6563 7963 6c69 6e67 2e6d 6f64 756c  ,recycling.modul
-00000f20: 6573 2e45 4543 5f34 3438 5f32 2e70 7269  es.EEC_448_2.pri
-00000f30: 7661 7465 5f6b 6579 2e73 6361 6eda 0473  vate_key.scan..s
-00000f40: 6361 6e72 3500 0000 da30 7265 6379 636c  canr5....0recycl
-00000f50: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-00000f60: 3434 385f 322e 7072 6976 6174 655f 6b65  448_2.private_ke
-00000f70: 792e 696e 7374 616e 6365 7217 0000 0072  y.instancer....r
-00000f80: 3600 0000 da2e 7265 6379 636c 696e 672e  6.....recycling.
-00000f90: 6d6f 6475 6c65 732e 4545 435f 3434 385f  modules.EEC_448_
-00000fa0: 322e 7075 626c 6963 5f6b 6579 2e63 7265  2.public_key.cre
-00000fb0: 6174 6f72 724a 0000 0072 3800 0000 da2b  atorrJ...r8....+
-00000fc0: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-00000fd0: 732e 4545 435f 3434 385f 322e 7075 626c  s.EEC_448_2.publ
-00000fe0: 6963 5f6b 6579 2e65 7463 6872 3900 0000  ic_key.etchr9...
-00000ff0: da2b 7265 6379 636c 696e 672e 6d6f 6475  .+recycling.modu
-00001000: 6c65 732e 4545 435f 3434 385f 322e 7075  les.EEC_448_2.pu
-00001010: 626c 6963 5f6b 6579 2e73 6361 6e72 3a00  blic_key.scanr:.
-00001020: 0000 da2f 7265 6379 636c 696e 672e 6d6f  .../recycling.mo
-00001030: 6475 6c65 732e 4545 435f 3434 385f 322e  dules.EEC_448_2.
-00001040: 7075 626c 6963 5f6b 6579 2e69 6e73 7461  public_key.insta
-00001050: 6e63 6572 3b00 0000 da20 7265 6379 636c  ncer;.... recycl
-00001060: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-00001070: 3434 385f 322e 7369 676e da04 7369 676e  448_2.sign..sign
-00001080: 723d 0000 00da 2272 6563 7963 6c69 6e67  r=...."recycling
-00001090: 2e6d 6f64 756c 6573 2e45 4543 5f34 3438  .modules.EEC_448
-000010a0: 5f32 2e76 6572 6966 7972 3f00 0000 da43  _2.verifyr?....C
-000010b0: 7265 6379 636c 696e 672e 6d6f 6475 6c65  recycling.module
-000010c0: 732e 4545 435f 3434 385f 322e 6d6f 6475  s.EEC_448_2.modu
-000010d0: 6c61 746f 7273 2e62 7974 655f 7374 7269  lators.byte_stri
-000010e0: 6e67 2e66 726f 6d5f 6865 7861 6465 6369  ng.from_hexadeci
-000010f0: 6d61 6cda 0a6d 6f64 756c 6174 6f72 73da  mal..modulators.
-00001100: 0b62 7974 655f 7374 7269 6e67 da10 6672  .byte_string..fr
-00001110: 6f6d 5f68 6578 6164 6563 696d 616c 7240  om_hexadecimalr@
-00001120: 0000 0072 2a00 0000 da07 6f73 2e70 6174  ...r*.....os.pat
-00001130: 6872 0200 0000 7203 0000 0072 0400 0000  hr....r....r....
-00001140: 7205 0000 0072 3300 0000 720c 0000 0072  r....r3...r....r
-00001150: 5100 0000 da06 6368 6563 6b73 720a 0000  Q.....checksr...
-00001160: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00001170: da08 3c6d 6f64 756c 653e 0100 0000 732a  ..<module>....s*
-00001180: 0000 0004 011e 041e 011e 011e 011e 021e  ................
-00001190: 011e 011e 0118 0218 0124 0208 0214 0108  .........$......
-000011a0: 0108 0108 0208 0600 7f04 1808 ff         .............
+00000800: 3066 3165 3066 3165 3066 da72 3133 3537  0f1e0f1e0f.r1357
+00000810: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000820: 3133 3537 3931 3335 3739 3133 3537 3931  1357913579135791
+00000830: 3335 3739 3133 3537 3931 3335 3739 3133  3579135791357913
+00000840: 3537 3931 3335 3739 3133 3537 3931 3335  5791357913579135
+00000850: 3739 3133 3537 3931 3335 3739 3133 3537  7913579135791357
+00000860: 3931 3335 3739 3133 3537 3931 3335 3739  9135791357913579
+00000870: 3133 3537 3931 3335 3739 3133 3537 da72  13579135791357.r
+00000880: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+00000890: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+000008a0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+000008b0: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+000008c0: 6566 3234 3638 6566 3234 3638 6566 3234  ef2468ef2468ef24
+000008d0: 3638 6566 3234 3638 6566 3234 3638 6566  68ef2468ef2468ef
+000008e0: 3234 3638 6566 3234 3638 6566 3234 3638  2468ef2468ef2468
+000008f0: 6566 da15 4545 435f 3434 385f 325f 7072  ef..EEC_448_2_pr
+00000900: 6976 6174 655f 6b65 797a 052e 4a53 4f4e  ivate_keyz..JSON
+00000910: da14 4545 435f 3434 385f 325f 7075 626c  ..EEC_448_2_publ
+00000920: 6963 5f6b 6579 da08 696e 7374 616e 6365  ic_key..instance
+00000930: 7a16 4445 5220 6865 7861 6465 6369 6d61  z.DER hexadecima
+00000940: 6c20 7374 7269 6e67 7a0f 4445 5220 6279  l stringz.DER by
+00000950: 7465 2073 7472 696e 677a 0b70 7269 7661  te stringz.priva
+00000960: 7465 206b 6579 e904 0000 0029 01da 0669  te key.....)...i
+00000970: 6e64 656e 74da 044a 534f 4e7a 0a70 7562  ndent..JSONz.pub
+00000980: 6c69 6320 6b65 79da 0473 656e 64da 0945  lic key..send..E
+00000990: 4543 5f34 3438 5f31 da8a 3330 3433 3330  EC_448_1..304330
+000009a0: 3035 3036 3033 3262 3635 3731 3033 3361  0506032b6571033a
+000009b0: 3030 6532 3639 3630 6138 3363 3435 6330  00e26960a83c45c0
+000009c0: 6262 3836 6533 3536 6364 3732 3734 3733  bb86e356cd727473
+000009d0: 6539 3636 3832 6537 3663 3664 6430 3163  e96682e76c6dd01c
+000009e0: 3939 3161 3665 6130 6133 3934 6563 6361  991a6ea0a394ecca
+000009f0: 3237 6234 3637 3535 3464 3733 6532 6132  27b467554d73e2a2
+00000a00: 3262 3035 3432 3563 3139 3236 6137 6139  2b05425c1926a7a9
+00000a10: 3262 6566 6461 3563 3139 3337 6436 3837  2befda5c1937d687
+00000a20: 3666 3030 2902 da06 666f 726d 6174 da07  6f00)...format..
+00000a30: 6164 6472 6573 73da 0e34 3033 3234 3738  address..4032478
+00000a40: 3933 3234 3837 3329 02da 0274 6fda 0661  9324873)...to..a
+00000a50: 6d6f 756e 7429 02da 046d 6f76 65da 0666  mount)...move..f
+00000a60: 6965 6c64 737a 0575 7466 2d38 2901 da0e  ieldsz.utf-8)...
+00000a70: 756e 7369 676e 6564 5f62 7974 6573 7a18  unsigned_bytesz.
+00000a80: 7369 676e 6564 2062 7974 6573 2068 6578  signed bytes hex
+00000a90: 6164 6563 696d 616c 7a19 7369 676e 6564  adecimalz.signed
+00000aa0: 5f62 7974 6573 5f68 6578 6164 6563 696d  _bytes_hexadecim
+00000ab0: 616c 3a29 02da 0c73 6967 6e65 645f 6279  al:)...signed_by
+00000ac0: 7465 7372 2500 0000 da03 7965 73f3 0000  tesr%.....yes...
+00000ad0: 0000 da02 6e6f 291b 7204 0000 0072 0300  ....no).r....r..
+00000ae0: 0000 da07 7061 7468 6c69 62da 0450 6174  ....pathlib..Pat
+00000af0: 68da 085f 5f66 696c 655f 5fda 0670 6172  h..__file__..par
+00000b00: 656e 74da 0772 6573 6f6c 7665 720c 0000  ent..resolver...
+00000b10: 00da 1d45 4543 5f34 3438 5f32 5f70 7269  ...EEC_448_2_pri
+00000b20: 7661 7465 5f6b 6579 5f63 7265 6174 6f72  vate_key_creator
+00000b30: da06 6372 6561 7465 da18 6574 6368 5f45  ..create..etch_E
+00000b40: 4543 5f34 3438 5f70 7269 7661 7465 5f6b  EC_448_private_k
+00000b50: 6579 da05 7374 6172 74da 046a 736f 6eda  ey..start..json.
+00000b60: 0564 756d 7073 da10 7072 6976 6174 655f  .dumps..private_
+00000b70: 6b65 795f 7363 616e da17 696e 7374 616e  key_scan..instan
+00000b80: 7469 6174 655f 7072 6976 6174 655f 6b65  tiate_private_ke
+00000b90: 79da 1b66 726f 6d5f 4445 525f 6865 7861  y..from_DER_hexa
+00000ba0: 6465 6369 6d61 6c5f 7374 7269 6e67 da1c  decimal_string..
+00000bb0: 4545 435f 3434 385f 325f 7075 626c 6963  EEC_448_2_public
+00000bc0: 5f6b 6579 5f63 7265 6174 6f72 da19 6574  _key_creator..et
+00000bd0: 6368 5f45 4543 5f34 3438 5f32 5f70 7562  ch_EEC_448_2_pub
+00000be0: 6c69 635f 6b65 79da 0f70 7562 6c69 635f  lic_key..public_
+00000bf0: 6b65 795f 7363 616e da16 696e 7374 616e  key_scan..instan
+00000c00: 7469 6174 655f 7075 626c 6963 5f6b 6579  tiate_public_key
+00000c10: da06 656e 636f 6465 da0e 4545 435f 3434  ..encode..EEC_44
+00000c20: 385f 325f 7369 676e da05 7072 696e 74da  8_2_sign..print.
+00000c30: 0676 6572 6966 79da 1a68 6578 6164 6563  .verify..hexadec
+00000c40: 696d 616c 5f74 6f5f 6279 7465 5f73 7472  imal_to_byte_str
+00000c50: 696e 67da 086d 6f64 756c 6174 6529 10da  ing..modulate)..
+00000c60: 0573 6565 6473 da04 7365 6564 da10 7072  .seeds..seed..pr
+00000c70: 6976 6174 655f 6b65 795f 7061 7468 da0f  ivate_key_path..
+00000c80: 7075 626c 6963 5f6b 6579 5f70 6174 68da  public_key_path.
+00000c90: 0b70 7269 7661 7465 5f6b 6579 da14 7072  .private_key..pr
+00000ca0: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
+00000cb0: 6365 da22 7072 6976 6174 655f 6b65 795f  ce."private_key_
+00000cc0: 4445 525f 6865 7861 6465 6369 6d61 6c5f  DER_hexadecimal_
+00000cd0: 7374 7269 6e67 da1b 7072 6976 6174 655f  string..private_
+00000ce0: 6b65 795f 4445 525f 6279 7465 5f73 7472  key_DER_byte_str
+00000cf0: 696e 67da 0a70 7562 6c69 635f 6b65 79da  ing..public_key.
+00000d00: 1370 7562 6c69 635f 6b65 795f 696e 7374  .public_key_inst
+00000d10: 616e 6365 da0e 756e 6963 6f64 655f 7374  ance..unicode_st
+00000d20: 7269 6e67 7225 0000 00da 0673 6967 6e65  ringr%.....signe
+00000d30: 64da 1873 6967 6e65 645f 6279 7465 735f  d..signed_bytes_
+00000d40: 6865 7861 6465 6369 6d61 6cda 0e76 6572  hexadecimal..ver
+00000d50: 6966 6963 6174 696f 6e5f 31da 0e76 6572  ification_1..ver
+00000d60: 6966 6963 6174 696f 6e5f 3272 0a00 0000  ification_2r....
+00000d70: 720a 0000 0072 0b00 0000 da07 6368 6563  r....r......chec
+00000d80: 6b5f 3120 0000 0073 b200 0000 0801 080b  k_1 ...s........
+00000d90: 0201 1401 02ff 0202 04fe 0203 1401 02ff  ................
+00000da0: 0202 04fe 0804 0801 0a06 0801 0801 0801  ................
+00000db0: 0405 0201 0401 0201 0801 02ff 02ff 0204  ................
+00000dc0: 04fc 0205 04f9 120e 0601 08ff 0407 1201  ................
+00000dd0: 04ff 0409 0201 04ff 0803 0405 0201 0401  ................
+00000de0: 0201 0801 02ff 02ff 0204 04fc 0205 04f9  ................
+00000df0: 120e 0601 08ff 0407 1201 04ff 0408 0201  ................
+00000e00: 0203 0201 04fe 0204 04fb 04fe 0209 06f7  ................
+00000e10: 0a0a 0402 0201 0201 06fe 0804 0a02 0405  ................
+00000e20: 0201 0802 0201 06fc 0c06 0405 0201 0802  ................
+00000e30: 0201 06fc 0c06 0804 0a01 0081 04f8 7251  ..............rQ
+00000e40: 0000 007a 2a65 6c6c 6970 7469 6320 7075  ...z*elliptic pu
+00000e50: 626c 6963 2061 6e64 2070 7269 7661 7465  blic and private
+00000e60: 206b 6579 2067 656e 6572 6174 696f 6e29   key generation)
+00000e70: 2dda 075f 5f64 6f63 5f5f da2d 7265 6379  -..__doc__.-recy
+00000e80: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+00000e90: 3434 385f 322e 7072 6976 6174 655f 6b65  448_2.private_ke
+00000ea0: 792e 6372 6561 746f 72da 056d 6978 6573  y.creator..mixes
+00000eb0: da09 4545 435f 3434 385f 3272 4600 0000  ..EEC_448_2rF...
+00000ec0: da07 6372 6561 746f 7272 2f00 0000 da2a  ..creatorr/....*
+00000ed0: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+00000ee0: 4545 435f 3434 385f 322e 7072 6976 6174  EEC_448_2.privat
+00000ef0: 655f 6b65 792e 6574 6368 da04 6574 6368  e_key.etch..etch
+00000f00: 7231 0000 00da 2a72 6563 7963 6c69 6e67  r1....*recycling
+00000f10: 2e6d 6978 6573 2e45 4543 5f34 3438 5f32  .mixes.EEC_448_2
+00000f20: 2e70 7269 7661 7465 5f6b 6579 2e73 6361  .private_key.sca
+00000f30: 6eda 0473 6361 6e72 3500 0000 da2e 7265  n..scanr5.....re
+00000f40: 6379 636c 696e 672e 6d69 7865 732e 4545  cycling.mixes.EE
+00000f50: 435f 3434 385f 322e 7072 6976 6174 655f  C_448_2.private_
+00000f60: 6b65 792e 696e 7374 616e 6365 7217 0000  key.instancer...
+00000f70: 0072 3600 0000 da2c 7265 6379 636c 696e  .r6....,recyclin
+00000f80: 672e 6d69 7865 732e 4545 435f 3434 385f  g.mixes.EEC_448_
+00000f90: 322e 7075 626c 6963 5f6b 6579 2e63 7265  2.public_key.cre
+00000fa0: 6174 6f72 724a 0000 0072 3800 0000 da29  atorrJ...r8....)
+00000fb0: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+00000fc0: 4545 435f 3434 385f 322e 7075 626c 6963  EEC_448_2.public
+00000fd0: 5f6b 6579 2e65 7463 6872 3900 0000 da29  _key.etchr9....)
+00000fe0: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+00000ff0: 4545 435f 3434 385f 322e 7075 626c 6963  EEC_448_2.public
+00001000: 5f6b 6579 2e73 6361 6e72 3a00 0000 da2d  _key.scanr:....-
+00001010: 7265 6379 636c 696e 672e 6d69 7865 732e  recycling.mixes.
+00001020: 4545 435f 3434 385f 322e 7075 626c 6963  EEC_448_2.public
+00001030: 5f6b 6579 2e69 6e73 7461 6e63 6572 3b00  _key.instancer;.
+00001040: 0000 da1e 7265 6379 636c 696e 672e 6d69  ....recycling.mi
+00001050: 7865 732e 4545 435f 3434 385f 322e 7369  xes.EEC_448_2.si
+00001060: 676e da04 7369 676e 723d 0000 00da 2072  gn..signr=.... r
+00001070: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00001080: 4543 5f34 3438 5f32 2e76 6572 6966 7972  EC_448_2.verifyr
+00001090: 3f00 0000 da41 7265 6379 636c 696e 672e  ?....Arecycling.
+000010a0: 6d69 7865 732e 4545 435f 3434 385f 322e  mixes.EEC_448_2.
+000010b0: 6d6f 6475 6c61 746f 7273 2e62 7974 655f  modulators.byte_
+000010c0: 7374 7269 6e67 2e66 726f 6d5f 6865 7861  string.from_hexa
+000010d0: 6465 6369 6d61 6cda 0a6d 6f64 756c 6174  decimal..modulat
+000010e0: 6f72 73da 0b62 7974 655f 7374 7269 6e67  ors..byte_string
+000010f0: da10 6672 6f6d 5f68 6578 6164 6563 696d  ..from_hexadecim
+00001100: 616c 7240 0000 0072 2a00 0000 da07 6f73  alr@...r*.....os
+00001110: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
+00001120: 0400 0000 7205 0000 0072 3300 0000 720c  ....r....r3...r.
+00001130: 0000 0072 5100 0000 da06 6368 6563 6b73  ...rQ.....checks
+00001140: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+00001150: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001160: 0000 732a 0000 0004 011e 041e 011e 011e  ..s*............
+00001170: 011e 021e 011e 011e 0118 0218 0124 0208  .............$..
+00001180: 0214 0108 0108 0108 0208 0600 7f04 1808  ................
+00001190: ff                                       .
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/_status/status_3_sign_and_verify/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 '''
-	python3 status.proc.py "modules/EEC_448_2/_status/status_3_sign_and_verify/status_1.py"
+	python3 status.proc.py "mixes/EEC_448_2/_status/status_3_sign_and_verify/status_1.py"
 '''
 
-import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
-import recycling.modules.EEC_448_2.private_key.etch as etch_EEC_448_private_key
-import recycling.modules.EEC_448_2.private_key.scan as private_key_scan
-import recycling.modules.EEC_448_2.private_key.instance as instantiate_private_key
+import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+import recycling.mixes.EEC_448_2.private_key.etch as etch_EEC_448_private_key
+import recycling.mixes.EEC_448_2.private_key.scan as private_key_scan
+import recycling.mixes.EEC_448_2.private_key.instance as instantiate_private_key
 	
-import recycling.modules.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
-import recycling.modules.EEC_448_2.public_key.etch as etch_EEC_448_2_public_key
-import recycling.modules.EEC_448_2.public_key.scan as public_key_scan
-import recycling.modules.EEC_448_2.public_key.instance as instantiate_public_key	
+import recycling.mixes.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
+import recycling.mixes.EEC_448_2.public_key.etch as etch_EEC_448_2_public_key
+import recycling.mixes.EEC_448_2.public_key.scan as public_key_scan
+import recycling.mixes.EEC_448_2.public_key.instance as instantiate_public_key	
 	
-import recycling.modules.EEC_448_2.sign as EEC_448_2_sign	
-import recycling.modules.EEC_448_2.verify as verify
+import recycling.mixes.EEC_448_2.sign as EEC_448_2_sign	
+import recycling.mixes.EEC_448_2.verify as verify
 
-import recycling.modules.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
+import recycling.mixes.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
 	
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import json
 
 def erase (path):
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/cryptography.py.S.HTML` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/cryptography.py.S.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/keys/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/keys/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 '''
-	import recycling.modules.EEC_448_2.keys as EEC_448_2_key_creator
+	import recycling.mixes.EEC_448_2.keys as EEC_448_2_key_creator
 	keys = EEC_448_2_key_creator.create (
 		seed = ""
 	)
 '''
 
 '''
 	{
@@ -14,16 +14,16 @@
 		},
 		"private": {
 			"hexadecimal string": private_key_DER_hexadecimal_string
 		}
 	}
 '''
 
-import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
-import recycling.modules.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
+import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+import recycling.mixes.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
 
 def create (
 	seed = ""
 ):
 	#
 	#	create private key
 	#
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/keys/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/keys/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1120 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 6004 0000  o........@@f`...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 5a04 0000  o........SQfZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 0200 0100  Z...d.d.l.m.....
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 5a06  m.....m.....m.Z.
 00000050: 0100 6401 6402 6c07 6d02 0200 0100 6d03  ..d.d.l.m.....m.
 00000060: 0200 0100 6d08 0200 0100 6d05 5a09 0100  ....m.....m.Z...
 00000070: 0903 6406 6404 6405 8401 5a0a 6402 5300  ..d.d.d...Z.d.S.
-00000080: 2907 7a79 0a09 696d 706f 7274 2072 6563  ).zy..import rec
-00000090: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-000000a0: 4543 5f34 3438 5f32 2e6b 6579 7320 6173  EC_448_2.keys as
-000000b0: 2045 4543 5f34 3438 5f32 5f6b 6579 5f63   EEC_448_2_key_c
-000000c0: 7265 6174 6f72 0a09 6b65 7973 203d 2045  reator..keys = E
-000000d0: 4543 5f34 3438 5f32 5f6b 6579 5f63 7265  EC_448_2_key_cre
-000000e0: 6174 6f72 2e63 7265 6174 6520 280a 0909  ator.create (...
-000000f0: 7365 6564 203d 2022 220a 0929 0ae9 0000  seed = ""..)....
-00000100: 0000 4eda 0063 0100 0000 0000 0000 0000  ..N..c..........
-00000110: 0000 0700 0000 0300 0000 4300 0000 7346  ..........C...sF
-00000120: 0000 0074 00a0 017c 00a1 017d 017c 0164  ...t...|...}.|.d
-00000130: 0119 007d 027c 0164 0219 007d 0374 02a0  ...}.|.d...}.t..
-00000140: 017c 02a1 017d 047c 0464 0119 007d 057c  .|...}.|.d...}.|
-00000150: 0464 0219 007d 0664 037c 0669 0164 037c  .d...}.d.|.i.d.|
-00000160: 0369 0164 049c 0253 0029 054e da08 696e  .i.d...S.).N..in
-00000170: 7374 616e 6365 7a16 4445 5220 6865 7861  stancez.DER hexa
-00000180: 6465 6369 6d61 6c20 7374 7269 6e67 7a12  decimal stringz.
-00000190: 6865 7861 6465 6369 6d61 6c20 7374 7269  hexadecimal stri
-000001a0: 6e67 2902 da06 7075 626c 6963 da07 7072  ng)...public..pr
-000001b0: 6976 6174 6529 03da 1d45 4543 5f34 3438  ivate)...EEC_448
-000001c0: 5f32 5f70 7269 7661 7465 5f6b 6579 5f63  _2_private_key_c
-000001d0: 7265 6174 6f72 da06 6372 6561 7465 da1c  reator..create..
-000001e0: 4545 435f 3434 385f 325f 7075 626c 6963  EEC_448_2_public
-000001f0: 5f6b 6579 5f63 7265 6174 6f72 2907 da04  _key_creator)...
-00000200: 7365 6564 da0b 7072 6976 6174 655f 6b65  seed..private_ke
-00000210: 79da 1470 7269 7661 7465 5f6b 6579 5f69  y..private_key_i
-00000220: 6e73 7461 6e63 65da 2270 7269 7661 7465  nstance."private
-00000230: 5f6b 6579 5f44 4552 5f68 6578 6164 6563  _key_DER_hexadec
-00000240: 696d 616c 5f73 7472 696e 67da 0a70 7562  imal_string..pub
-00000250: 6c69 635f 6b65 79da 1370 7562 6c69 635f  lic_key..public_
-00000260: 6b65 795f 696e 7374 616e 6365 da21 7075  key_instance.!pu
-00000270: 626c 6963 5f6b 6579 5f44 4552 5f68 6578  blic_key_DER_hex
-00000280: 6164 6563 696d 616c 5f73 7472 696e 67a9  adecimal_string.
-00000290: 0072 1000 0000 fa43 2f68 6162 6974 6174  .r.....C/habitat
-000002a0: 2f76 656e 7565 732f 7374 6167 6573 2f72  /venues/stages/r
-000002b0: 6563 7963 6c69 6e67 2f6d 6f64 756c 6573  ecycling/modules
-000002c0: 2f45 4543 5f34 3438 5f32 2f6b 6579 732f  /EEC_448_2/keys/
-000002d0: 5f5f 696e 6974 5f5f 2e70 7972 0700 0000  __init__.pyr....
-000002e0: 1800 0000 731a 0000 000a 0608 0108 0104  ....s...........
-000002f0: 0502 0104 ff08 0308 0104 0402 ff04 0402  ................
-00000300: ff06 fc72 0700 0000 2901 7202 0000 0029  ...r....).r....)
-00000310: 0bda 075f 5f64 6f63 5f5f da2f 7265 6379  ...__doc__./recy
-00000320: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000330: 435f 3434 385f 322e 7072 6976 6174 655f  C_448_2.private_
-00000340: 6b65 792e 6372 6561 746f 72da 076d 6f64  key.creator..mod
-00000350: 756c 6573 da09 4545 435f 3434 385f 3272  ules..EEC_448_2r
-00000360: 0a00 0000 da07 6372 6561 746f 7272 0600  ......creatorr..
-00000370: 0000 da2e 7265 6379 636c 696e 672e 6d6f  ....recycling.mo
-00000380: 6475 6c65 732e 4545 435f 3434 385f 322e  dules.EEC_448_2.
-00000390: 7075 626c 6963 5f6b 6579 2e63 7265 6174  public_key.creat
-000003a0: 6f72 720d 0000 0072 0800 0000 7207 0000  orr....r....r...
-000003b0: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
-000003c0: 7211 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000003d0: 0000 0073 0c00 0000 0402 0207 1e0b 1e01  ...s............
-000003e0: 0203 0eff                                ....
+00000080: 2907 7a77 0a09 696d 706f 7274 2072 6563  ).zw..import rec
+00000090: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+000000a0: 5f34 3438 5f32 2e6b 6579 7320 6173 2045  _448_2.keys as E
+000000b0: 4543 5f34 3438 5f32 5f6b 6579 5f63 7265  EC_448_2_key_cre
+000000c0: 6174 6f72 0a09 6b65 7973 203d 2045 4543  ator..keys = EEC
+000000d0: 5f34 3438 5f32 5f6b 6579 5f63 7265 6174  _448_2_key_creat
+000000e0: 6f72 2e63 7265 6174 6520 280a 0909 7365  or.create (...se
+000000f0: 6564 203d 2022 220a 0929 0ae9 0000 0000  ed = ""..)......
+00000100: 4eda 0063 0100 0000 0000 0000 0000 0000  N..c............
+00000110: 0700 0000 0300 0000 4300 0000 7346 0000  ........C...sF..
+00000120: 0074 00a0 017c 00a1 017d 017c 0164 0119  .t...|...}.|.d..
+00000130: 007d 027c 0164 0219 007d 0374 02a0 017c  .}.|.d...}.t...|
+00000140: 02a1 017d 047c 0464 0119 007d 057c 0464  ...}.|.d...}.|.d
+00000150: 0219 007d 0664 037c 0669 0164 037c 0369  ...}.d.|.i.d.|.i
+00000160: 0164 049c 0253 0029 054e da08 696e 7374  .d...S.).N..inst
+00000170: 616e 6365 7a16 4445 5220 6865 7861 6465  ancez.DER hexade
+00000180: 6369 6d61 6c20 7374 7269 6e67 7a12 6865  cimal stringz.he
+00000190: 7861 6465 6369 6d61 6c20 7374 7269 6e67  xadecimal string
+000001a0: 2902 da06 7075 626c 6963 da07 7072 6976  )...public..priv
+000001b0: 6174 6529 03da 1d45 4543 5f34 3438 5f32  ate)...EEC_448_2
+000001c0: 5f70 7269 7661 7465 5f6b 6579 5f63 7265  _private_key_cre
+000001d0: 6174 6f72 da06 6372 6561 7465 da1c 4545  ator..create..EE
+000001e0: 435f 3434 385f 325f 7075 626c 6963 5f6b  C_448_2_public_k
+000001f0: 6579 5f63 7265 6174 6f72 2907 da04 7365  ey_creator)...se
+00000200: 6564 da0b 7072 6976 6174 655f 6b65 79da  ed..private_key.
+00000210: 1470 7269 7661 7465 5f6b 6579 5f69 6e73  .private_key_ins
+00000220: 7461 6e63 65da 2270 7269 7661 7465 5f6b  tance."private_k
+00000230: 6579 5f44 4552 5f68 6578 6164 6563 696d  ey_DER_hexadecim
+00000240: 616c 5f73 7472 696e 67da 0a70 7562 6c69  al_string..publi
+00000250: 635f 6b65 79da 1370 7562 6c69 635f 6b65  c_key..public_ke
+00000260: 795f 696e 7374 616e 6365 da21 7075 626c  y_instance.!publ
+00000270: 6963 5f6b 6579 5f44 4552 5f68 6578 6164  ic_key_DER_hexad
+00000280: 6563 696d 616c 5f73 7472 696e 67a9 0072  ecimal_string..r
+00000290: 1000 0000 fa41 2f68 6162 6974 6174 2f76  .....A/habitat/v
+000002a0: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
+000002b0: 7963 6c69 6e67 2f6d 6978 6573 2f45 4543  ycling/mixes/EEC
+000002c0: 5f34 3438 5f32 2f6b 6579 732f 5f5f 696e  _448_2/keys/__in
+000002d0: 6974 5f5f 2e70 7972 0700 0000 1800 0000  it__.pyr........
+000002e0: 731a 0000 000a 0608 0108 0104 0502 0104  s...............
+000002f0: ff08 0308 0104 0402 ff04 0402 ff06 fc72  ...............r
+00000300: 0700 0000 2901 7202 0000 0029 0bda 075f  ....).r....)..._
+00000310: 5f64 6f63 5f5f da2d 7265 6379 636c 696e  _doc__.-recyclin
+00000320: 672e 6d69 7865 732e 4545 435f 3434 385f  g.mixes.EEC_448_
+00000330: 322e 7072 6976 6174 655f 6b65 792e 6372  2.private_key.cr
+00000340: 6561 746f 72da 056d 6978 6573 da09 4545  eator..mixes..EE
+00000350: 435f 3434 385f 3272 0a00 0000 da07 6372  C_448_2r......cr
+00000360: 6561 746f 7272 0600 0000 da2c 7265 6379  eatorr.....,recy
+00000370: 636c 696e 672e 6d69 7865 732e 4545 435f  cling.mixes.EEC_
+00000380: 3434 385f 322e 7075 626c 6963 5f6b 6579  448_2.public_key
+00000390: 2e63 7265 6174 6f72 720d 0000 0072 0800  .creatorr....r..
+000003a0: 0000 7207 0000 0072 1000 0000 7210 0000  ..r....r....r...
+000003b0: 0072 1000 0000 7211 0000 00da 083c 6d6f  .r....r......<mo
+000003c0: 6475 6c65 3e01 0000 0073 0c00 0000 0402  dule>....s......
+000003d0: 0207 1e0b 1e01 0203 0eff                 ..........
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/modulators/byte_string/__pycache__/from_hexadecimal.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/modulators/byte_string/__pycache__/from_hexadecimal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 7601 0000  o........@@fv...
+00000000: 6f0d 0d0a 0000 0000 d053 5166 7401 0000  o........SQft...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 8400 5a01 6403 5300 2904  Z.d.d...Z.d.S.).
-00000040: 7ab3 0a09 696d 706f 7274 2072 6563 7963  z...import recyc
-00000050: 6c69 6e67 2e6d 6f64 756c 6573 2e45 4543  ling.modules.EEC
-00000060: 5f34 3438 5f32 2e6d 6f64 756c 6174 6f72  _448_2.modulator
-00000070: 732e 6279 7465 5f73 7472 696e 672e 6672  s.byte_string.fr
-00000080: 6f6d 5f68 6578 6164 6563 696d 616c 2061  om_hexadecimal a
-00000090: 7320 6865 7861 6465 6369 6d61 6c5f 746f  s hexadecimal_to
-000000a0: 5f62 7974 655f 7374 7269 6e67 0a09 6279  _byte_string..by
-000000b0: 7465 5f73 7472 696e 6720 3d20 6865 7861  te_string = hexa
-000000c0: 6465 6369 6d61 6c5f 746f 5f62 7974 655f  decimal_to_byte_
-000000d0: 7374 7269 6e67 2e6d 6f64 756c 6174 6520  string.modulate 
-000000e0: 2822 3031 3233 3435 3637 3839 4142 4344  ("0123456789ABCD
-000000f0: 4546 2229 0a63 0100 0000 0000 0000 0000  EF").c..........
-00000100: 0000 0200 0000 0300 0000 4300 0000 7326  ..........C...s&
-00000110: 0000 0074 00a0 017c 00a1 017d 017c 01a0  ...t...|...}.|..
-00000120: 02a1 00a0 03a1 007c 00a0 03a1 006b 0273  .......|.....k.s
-00000130: 114a 0082 017c 0153 0029 014e 2904 da05  .J...|.S.).N)...
-00000140: 6279 7465 73da 0766 726f 6d68 6578 da03  bytes..fromhex..
-00000150: 6865 78da 0575 7070 6572 2902 da12 6865  hex..upper)...he
-00000160: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
-00000170: da0b 6279 7465 5f73 7472 696e 67a9 0072  ..byte_string..r
-00000180: 0700 0000 fa5d 2f68 6162 6974 6174 2f76  .....]/habitat/v
-00000190: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
-000001a0: 7963 6c69 6e67 2f6d 6f64 756c 6573 2f45  ycling/modules/E
-000001b0: 4543 5f34 3438 5f32 2f6d 6f64 756c 6174  EC_448_2/modulat
-000001c0: 6f72 732f 6279 7465 5f73 7472 696e 672f  ors/byte_string/
-000001d0: 6672 6f6d 5f68 6578 6164 6563 696d 616c  from_hexadecimal
-000001e0: 2e70 79da 086d 6f64 756c 6174 6508 0000  .py..modulate...
-000001f0: 0073 0a00 0000 0a01 0a03 0601 08ff 0404  .s..............
-00000200: 7209 0000 004e 2902 da07 5f5f 646f 635f  r....N)...__doc_
-00000210: 5f72 0900 0000 7207 0000 0072 0700 0000  _r....r....r....
-00000220: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
-00000230: 756c 653e 0100 0000 7304 0000 0004 020c  ule>....s.......
-00000240: 05                                       .
+00000040: 7ab1 0a09 696d 706f 7274 2072 6563 7963  z...import recyc
+00000050: 6c69 6e67 2e6d 6978 6573 2e45 4543 5f34  ling.mixes.EEC_4
+00000060: 3438 5f32 2e6d 6f64 756c 6174 6f72 732e  48_2.modulators.
+00000070: 6279 7465 5f73 7472 696e 672e 6672 6f6d  byte_string.from
+00000080: 5f68 6578 6164 6563 696d 616c 2061 7320  _hexadecimal as 
+00000090: 6865 7861 6465 6369 6d61 6c5f 746f 5f62  hexadecimal_to_b
+000000a0: 7974 655f 7374 7269 6e67 0a09 6279 7465  yte_string..byte
+000000b0: 5f73 7472 696e 6720 3d20 6865 7861 6465  _string = hexade
+000000c0: 6369 6d61 6c5f 746f 5f62 7974 655f 7374  cimal_to_byte_st
+000000d0: 7269 6e67 2e6d 6f64 756c 6174 6520 2822  ring.modulate ("
+000000e0: 3031 3233 3435 3637 3839 4142 4344 4546  0123456789ABCDEF
+000000f0: 2229 0a63 0100 0000 0000 0000 0000 0000  ").c............
+00000100: 0200 0000 0300 0000 4300 0000 7326 0000  ........C...s&..
+00000110: 0074 00a0 017c 00a1 017d 017c 01a0 02a1  .t...|...}.|....
+00000120: 00a0 03a1 007c 00a0 03a1 006b 0273 114a  .....|.....k.s.J
+00000130: 0082 017c 0153 0029 014e 2904 da05 6279  ...|.S.).N)...by
+00000140: 7465 73da 0766 726f 6d68 6578 da03 6865  tes..fromhex..he
+00000150: 78da 0575 7070 6572 2902 da12 6865 7861  x..upper)...hexa
+00000160: 6465 6369 6d61 6c5f 7374 7269 6e67 da0b  decimal_string..
+00000170: 6279 7465 5f73 7472 696e 67a9 0072 0700  byte_string..r..
+00000180: 0000 fa5b 2f68 6162 6974 6174 2f76 656e  ...[/habitat/ven
+00000190: 7565 732f 7374 6167 6573 2f72 6563 7963  ues/stages/recyc
+000001a0: 6c69 6e67 2f6d 6978 6573 2f45 4543 5f34  ling/mixes/EEC_4
+000001b0: 3438 5f32 2f6d 6f64 756c 6174 6f72 732f  48_2/modulators/
+000001c0: 6279 7465 5f73 7472 696e 672f 6672 6f6d  byte_string/from
+000001d0: 5f68 6578 6164 6563 696d 616c 2e70 79da  _hexadecimal.py.
+000001e0: 086d 6f64 756c 6174 6508 0000 0073 0a00  .modulate....s..
+000001f0: 0000 0a01 0a03 0601 08ff 0404 7209 0000  ............r...
+00000200: 004e 2902 da07 5f5f 646f 635f 5f72 0900  .N)...__doc__r..
+00000210: 0000 7207 0000 0072 0700 0000 7207 0000  ..r....r....r...
+00000220: 0072 0800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000230: 0100 0000 7304 0000 0004 020c 05         ....s........
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/BUILD.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/BUILD.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/CREATE.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/CREATE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/READ.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/READ.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/SCAN.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/creator.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/creator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1672 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 8806 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d053 5166 8606 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a02  Z.....d.d.l.m.Z.
 00000040: 0100 6401 6403 6c03 5a04 6404 6405 8400  ..d.d.l.Z.d.d...
-00000050: 5a05 6403 5300 2906 617b 0100 000a 0973  Z.d.S.).a{.....s
+00000050: 5a05 6403 5300 2906 6179 0100 000a 0973  Z.d.S.).ay.....s
 00000060: 6565 6420 3d20 2234 3938 3638 3838 6231  eed = "4986888b1
 00000070: 3133 3538 6266 3364 3534 3162 3431 6565  1358bf3d541b41ee
 00000080: 6135 6461 6563 6531 6336 6566 6636 3431  a5daece1c6eff641
 00000090: 3330 6134 3566 6338 6239 6361 3438 6633  30a45fc8b9ca48f3
 000000a0: 6530 6530 3234 3633 6339 3963 3561 6564  e0e02463c99c5aed
 000000b0: 6338 6138 3437 3638 3664 3636 3962 3764  c8a847686d669b7d
 000000c0: 3534 3763 3138 6665 3434 3866 6335 3131  547c18fe448fc511
 000000d0: 3163 6138 3866 3465 3822 0a0a 0969 6d70  1ca88f4e8"...imp
-000000e0: 6f72 7420 7265 6379 636c 696e 672e 6d6f  ort recycling.mo
-000000f0: 6475 6c65 732e 4545 435f 3434 385f 322e  dules.EEC_448_2.
-00000100: 7072 6976 6174 655f 6b65 792e 6372 6561  private_key.crea
-00000110: 746f 7220 6173 2045 4543 5f34 3438 5f32  tor as EEC_448_2
-00000120: 5f70 7269 7661 7465 5f6b 6579 5f63 7265  _private_key_cre
-00000130: 6174 6f72 0a09 4545 435f 3434 385f 325f  ator..EEC_448_2_
-00000140: 7072 6976 6174 655f 6b65 795f 6372 6561  private_key_crea
-00000150: 746f 722e 6372 6561 7465 2028 0a09 0973  tor.create (...s
-00000160: 6565 640a 0929 0a09 0a09 7072 6976 6174  eed..)....privat
-00000170: 655f 6b65 795f 696e 7374 616e 6365 203d  e_key_instance =
-00000180: 2070 7269 7661 7465 5f6b 6579 205b 2269   private_key ["i
-00000190: 6e73 7461 6e63 6522 5d0a 0970 7269 7661  nstance"]..priva
-000001a0: 7465 5f6b 6579 5f68 6578 6164 6563 696d  te_key_hexadecim
-000001b0: 616c 203d 2070 7269 7661 7465 5f6b 6579  al = private_key
-000001c0: 205b 2268 6578 6164 6563 696d 616c 2073   ["hexadecimal s
-000001d0: 7472 696e 6722 5d0a e900 0000 0029 01da  tring"]......)..
-000001e0: 0645 6363 4b65 794e 6301 0000 0000 0000  .EccKeyNc.......
-000001f0: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00000200: 0073 7e00 0000 7400 7c00 8301 6401 6b02  .s~...t.|...d.k.
-00000210: 7308 4a00 8201 7401 6402 7402 a003 7c00  s.J...t.d.t...|.
-00000220: a101 6403 8d02 7d01 7c01 6a04 6404 6405  ..d...}.|.j.d.d.
-00000230: 8d01 7d02 7c01 6a04 6406 6405 8d01 7d03  ..}.|.j.d.d...}.
-00000240: 7c02 a005 a100 a006 a100 7d04 7400 7c04  |.........}.t.|.
-00000250: 8301 6407 6b02 732f 4a00 7400 7c04 8301  ..d.k.s/J.t.|...
-00000260: 8301 8201 7402 a003 7c04 a101 7c02 6b02  ....t...|...|.k.
-00000270: 7338 4a00 8201 7c01 7c02 7c04 7c03 6408  s8J...|.|.|.|.d.
-00000280: 9c04 5300 2909 4ee9 7200 0000 da05 4564  ..S.).N.r.....Ed
-00000290: 3434 3829 02da 0563 7572 7665 da04 7365  448)...curve..se
-000002a0: 6564 da03 4445 5229 01da 0666 6f72 6d61  ed..DER)...forma
-000002b0: 74da 0350 454d e992 0000 0029 04da 0869  t..PEM.....)...i
-000002c0: 6e73 7461 6e63 657a 0f44 4552 2062 7974  nstancez.DER byt
-000002d0: 6520 7374 7269 6e67 7a16 4445 5220 6865  e stringz.DER he
-000002e0: 7861 6465 6369 6d61 6c20 7374 7269 6e67  xadecimal string
-000002f0: 7a0a 5045 4d20 7374 7269 6e67 2907 da03  z.PEM string)...
-00000300: 6c65 6e72 0200 0000 da05 6279 7465 73da  lenr......bytes.
-00000310: 0766 726f 6d68 6578 da0a 6578 706f 7274  .fromhex..export
-00000320: 5f6b 6579 da03 6865 78da 0575 7070 6572  _key..hex..upper
-00000330: 2905 7206 0000 0072 0b00 0000 da0e 4445  ).r....r......DE
-00000340: 525f 6b65 795f 7374 7269 6e67 da0e 5045  R_key_string..PE
-00000350: 4d5f 6b65 795f 7374 7269 6e67 da12 6865  M_key_string..he
-00000360: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
-00000370: a900 7215 0000 00fa 492f 6861 6269 7461  ..r.....I/habita
-00000380: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-00000390: 7265 6379 636c 696e 672f 6d6f 6475 6c65  recycling/module
-000003a0: 732f 4545 435f 3434 385f 322f 7072 6976  s/EEC_448_2/priv
-000003b0: 6174 655f 6b65 792f 6372 6561 746f 722e  ate_key/creator.
-000003c0: 7079 da06 6372 6561 7465 2200 0000 7326  py..create"...s&
-000003d0: 0000 0010 0102 0202 0108 0106 fe04 0402  ................
-000003e0: 0106 ff04 0302 0106 ff0c 0a18 0112 0102  ................
-000003f0: 0302 0202 0102 0206 fa72 1700 0000 2906  .........r....).
-00000400: da07 5f5f 646f 635f 5fda 1443 7279 7074  ..__doc__..Crypt
-00000410: 6f2e 5075 626c 6963 4b65 792e 4543 4372  o.PublicKey.ECCr
-00000420: 0200 0000 da07 6f73 2e70 6174 68da 026f  ......os.path..o
-00000430: 7372 1700 0000 7215 0000 0072 1500 0000  sr....r....r....
-00000440: 7215 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
-00000450: 756c 653e 0100 0000 730c 0000 0004 0202  ule>....s.......
-00000460: 0d02 0c0c 0308 010c 02                   .........
+000000e0: 6f72 7420 7265 6379 636c 696e 672e 6d69  ort recycling.mi
+000000f0: 7865 732e 4545 435f 3434 385f 322e 7072  xes.EEC_448_2.pr
+00000100: 6976 6174 655f 6b65 792e 6372 6561 746f  ivate_key.creato
+00000110: 7220 6173 2045 4543 5f34 3438 5f32 5f70  r as EEC_448_2_p
+00000120: 7269 7661 7465 5f6b 6579 5f63 7265 6174  rivate_key_creat
+00000130: 6f72 0a09 4545 435f 3434 385f 325f 7072  or..EEC_448_2_pr
+00000140: 6976 6174 655f 6b65 795f 6372 6561 746f  ivate_key_creato
+00000150: 722e 6372 6561 7465 2028 0a09 0973 6565  r.create (...see
+00000160: 640a 0929 0a09 0a09 7072 6976 6174 655f  d..)....private_
+00000170: 6b65 795f 696e 7374 616e 6365 203d 2070  key_instance = p
+00000180: 7269 7661 7465 5f6b 6579 205b 2269 6e73  rivate_key ["ins
+00000190: 7461 6e63 6522 5d0a 0970 7269 7661 7465  tance"]..private
+000001a0: 5f6b 6579 5f68 6578 6164 6563 696d 616c  _key_hexadecimal
+000001b0: 203d 2070 7269 7661 7465 5f6b 6579 205b   = private_key [
+000001c0: 2268 6578 6164 6563 696d 616c 2073 7472  "hexadecimal str
+000001d0: 696e 6722 5d0a e900 0000 0029 01da 0645  ing"]......)...E
+000001e0: 6363 4b65 794e 6301 0000 0000 0000 0000  ccKeyNc.........
+000001f0: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
+00000200: 7e00 0000 7400 7c00 8301 6401 6b02 7308  ~...t.|...d.k.s.
+00000210: 4a00 8201 7401 6402 7402 a003 7c00 a101  J...t.d.t...|...
+00000220: 6403 8d02 7d01 7c01 6a04 6404 6405 8d01  d...}.|.j.d.d...
+00000230: 7d02 7c01 6a04 6406 6405 8d01 7d03 7c02  }.|.j.d.d...}.|.
+00000240: a005 a100 a006 a100 7d04 7400 7c04 8301  ........}.t.|...
+00000250: 6407 6b02 732f 4a00 7400 7c04 8301 8301  d.k.s/J.t.|.....
+00000260: 8201 7402 a003 7c04 a101 7c02 6b02 7338  ..t...|...|.k.s8
+00000270: 4a00 8201 7c01 7c02 7c04 7c03 6408 9c04  J...|.|.|.|.d...
+00000280: 5300 2909 4ee9 7200 0000 da05 4564 3434  S.).N.r.....Ed44
+00000290: 3829 02da 0563 7572 7665 da04 7365 6564  8)...curve..seed
+000002a0: da03 4445 5229 01da 0666 6f72 6d61 74da  ..DER)...format.
+000002b0: 0350 454d e992 0000 0029 04da 0869 6e73  .PEM.....)...ins
+000002c0: 7461 6e63 657a 0f44 4552 2062 7974 6520  tancez.DER byte 
+000002d0: 7374 7269 6e67 7a16 4445 5220 6865 7861  stringz.DER hexa
+000002e0: 6465 6369 6d61 6c20 7374 7269 6e67 7a0a  decimal stringz.
+000002f0: 5045 4d20 7374 7269 6e67 2907 da03 6c65  PEM string)...le
+00000300: 6e72 0200 0000 da05 6279 7465 73da 0766  nr......bytes..f
+00000310: 726f 6d68 6578 da0a 6578 706f 7274 5f6b  romhex..export_k
+00000320: 6579 da03 6865 78da 0575 7070 6572 2905  ey..hex..upper).
+00000330: 7206 0000 0072 0b00 0000 da0e 4445 525f  r....r......DER_
+00000340: 6b65 795f 7374 7269 6e67 da0e 5045 4d5f  key_string..PEM_
+00000350: 6b65 795f 7374 7269 6e67 da12 6865 7861  key_string..hexa
+00000360: 6465 6369 6d61 6c5f 7374 7269 6e67 a900  decimal_string..
+00000370: 7215 0000 00fa 472f 6861 6269 7461 742f  r.....G/habitat/
+00000380: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+00000390: 6379 636c 696e 672f 6d69 7865 732f 4545  cycling/mixes/EE
+000003a0: 435f 3434 385f 322f 7072 6976 6174 655f  C_448_2/private_
+000003b0: 6b65 792f 6372 6561 746f 722e 7079 da06  key/creator.py..
+000003c0: 6372 6561 7465 2200 0000 7326 0000 0010  create"...s&....
+000003d0: 0102 0202 0108 0106 fe04 0402 0106 ff04  ................
+000003e0: 0302 0106 ff0c 0a18 0112 0102 0302 0202  ................
+000003f0: 0102 0206 fa72 1700 0000 2906 da07 5f5f  .....r....)...__
+00000400: 646f 635f 5fda 1443 7279 7074 6f2e 5075  doc__..Crypto.Pu
+00000410: 626c 6963 4b65 792e 4543 4372 0200 0000  blicKey.ECCr....
+00000420: da07 6f73 2e70 6174 68da 026f 7372 1700  ..os.path..osr..
+00000430: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000440: 0072 1600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000450: 0100 0000 730c 0000 0004 0202 0d02 0c0c  ....s...........
+00000460: 0308 010c 02                             .....
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/etch.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/etch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 650 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 8a02 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 8802 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6403 6404  Z...d.d.l.Z.d.d.
-00000040: 8400 5a02 6402 5300 2905 7a95 0a09 696d  ..Z.d.S.).z...im
+00000040: 8400 5a02 6402 5300 2905 7a93 0a09 696d  ..Z.d.S.).z...im
 00000050: 706f 7274 2072 6563 7963 6c69 6e67 2e6d  port recycling.m
-00000060: 6f64 756c 6573 2e45 4543 5f34 3438 5f32  odules.EEC_448_2
-00000070: 2e70 7269 7661 7465 5f6b 6579 2e65 7463  .private_key.etc
-00000080: 6820 6173 2065 7463 685f 4545 435f 3434  h as etch_EEC_44
-00000090: 385f 7072 6976 6174 655f 6b65 790a 0965  8_private_key..e
-000000a0: 7463 685f 4545 435f 3434 385f 7072 6976  tch_EEC_448_priv
-000000b0: 6174 655f 6b65 792e 7374 6172 7420 2870  ate_key.start (p
-000000c0: 6174 682c 2070 7269 7661 7465 5f6b 6579  ath, private_key
-000000d0: 5f73 7472 696e 672c 2022 4a53 4f4e 2229  _string, "JSON")
-000000e0: 0ae9 0000 0000 4e63 0300 0000 0000 0000  ......Nc........
-000000f0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00000100: 736a 0000 0074 006a 01a0 027c 00a1 0172  sj...t.j...|...r
-00000110: 0e74 0364 017c 009b 0064 029d 0383 0182  .t.d.|...d......
-00000120: 017c 0264 036b 0272 1874 047c 0064 0483  .|.d.k.r.t.|.d..
-00000130: 027d 036e 127c 0264 0576 0072 2274 047c  .}.n.|.d.v.r"t.|
-00000140: 0064 0683 027d 036e 0874 0364 077c 029b  .d...}.n.t.d.|..
-00000150: 0064 089d 0383 0182 017c 03a0 057c 01a1  .d.......|...|..
-00000160: 0101 007c 03a0 06a1 0001 0064 0953 0029  ...|.......d.S.)
-00000170: 0a4e 7a30 5468 6520 7061 7468 2066 6f72  .Nz0The path for
-00000180: 2074 6865 2070 7269 7661 7465 5f6b 6579   the private_key
-00000190: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-000001a0: 652e 2027 fa01 27da 0344 4552 da02 7762  e. '..'..DER..wb
-000001b0: 2903 da03 5045 4dda 0b68 6578 6164 6563  )...PEM..hexadec
-000001c0: 696d 616c da04 4a53 4f4e da01 777a 0866  imal..JSON..wz.f
-000001d0: 6f72 6d61 7420 277a 1827 2077 6173 206e  ormat 'z.' was n
-000001e0: 6f74 2061 6363 6f75 6e74 6564 2066 6f72  ot accounted for
-000001f0: 2e54 2907 da02 6f73 da04 7061 7468 da06  .T)...os..path..
-00000200: 6578 6973 7473 da09 4578 6365 7074 696f  exists..Exceptio
-00000210: 6eda 046f 7065 6eda 0577 7269 7465 da05  n..open..write..
-00000220: 636c 6f73 6529 0472 0a00 0000 da12 7072  close).r......pr
-00000230: 6976 6174 655f 6b65 795f 7374 7269 6e67  ivate_key_string
-00000240: da06 666f 726d 6174 da01 66a9 0072 1300  ..format..f..r..
-00000250: 0000 fa46 2f68 6162 6974 6174 2f76 656e  ...F/habitat/ven
-00000260: 7565 732f 7374 6167 6573 2f72 6563 7963  ues/stages/recyc
-00000270: 6c69 6e67 2f6d 6f64 756c 6573 2f45 4543  ling/modules/EEC
-00000280: 5f34 3438 5f32 2f70 7269 7661 7465 5f6b  _448_2/private_k
-00000290: 6579 2f65 7463 682e 7079 da05 7374 6172  ey/etch.py..star
-000002a0: 740d 0000 0073 1400 0000 0c05 1001 0802  t....s..........
-000002b0: 0c01 0802 0c01 1003 0a02 0801 0402 7215  ..............r.
-000002c0: 0000 0029 03da 075f 5f64 6f63 5f5f 7209  ...)...__doc__r.
-000002d0: 0000 0072 1500 0000 7213 0000 0072 1300  ...r....r....r..
-000002e0: 0000 7213 0000 0072 1400 0000 da08 3c6d  ..r....r......<m
-000002f0: 6f64 756c 653e 0100 0000 7308 0000 0004  odule>....s.....
-00000300: 0102 0508 040c 02                        .......
+00000060: 6978 6573 2e45 4543 5f34 3438 5f32 2e70  ixes.EEC_448_2.p
+00000070: 7269 7661 7465 5f6b 6579 2e65 7463 6820  rivate_key.etch 
+00000080: 6173 2065 7463 685f 4545 435f 3434 385f  as etch_EEC_448_
+00000090: 7072 6976 6174 655f 6b65 790a 0965 7463  private_key..etc
+000000a0: 685f 4545 435f 3434 385f 7072 6976 6174  h_EEC_448_privat
+000000b0: 655f 6b65 792e 7374 6172 7420 2870 6174  e_key.start (pat
+000000c0: 682c 2070 7269 7661 7465 5f6b 6579 5f73  h, private_key_s
+000000d0: 7472 696e 672c 2022 4a53 4f4e 2229 0ae9  tring, "JSON")..
+000000e0: 0000 0000 4e63 0300 0000 0000 0000 0000  ....Nc..........
+000000f0: 0000 0400 0000 0400 0000 4300 0000 736a  ..........C...sj
+00000100: 0000 0074 006a 01a0 027c 00a1 0172 0e74  ...t.j...|...r.t
+00000110: 0364 017c 009b 0064 029d 0383 0182 017c  .d.|...d.......|
+00000120: 0264 036b 0272 1874 047c 0064 0483 027d  .d.k.r.t.|.d...}
+00000130: 036e 127c 0264 0576 0072 2274 047c 0064  .n.|.d.v.r"t.|.d
+00000140: 0683 027d 036e 0874 0364 077c 029b 0064  ...}.n.t.d.|...d
+00000150: 089d 0383 0182 017c 03a0 057c 01a1 0101  .......|...|....
+00000160: 007c 03a0 06a1 0001 0064 0953 0029 0a4e  .|.......d.S.).N
+00000170: 7a30 5468 6520 7061 7468 2066 6f72 2074  z0The path for t
+00000180: 6865 2070 7269 7661 7465 5f6b 6579 2069  he private_key i
+00000190: 7320 6e6f 7420 6176 6169 6c61 626c 652e  s not available.
+000001a0: 2027 fa01 27da 0344 4552 da02 7762 2903   '..'..DER..wb).
+000001b0: da03 5045 4dda 0b68 6578 6164 6563 696d  ..PEM..hexadecim
+000001c0: 616c da04 4a53 4f4e da01 777a 0866 6f72  al..JSON..wz.for
+000001d0: 6d61 7420 277a 1827 2077 6173 206e 6f74  mat 'z.' was not
+000001e0: 2061 6363 6f75 6e74 6564 2066 6f72 2e54   accounted for.T
+000001f0: 2907 da02 6f73 da04 7061 7468 da06 6578  )...os..path..ex
+00000200: 6973 7473 da09 4578 6365 7074 696f 6eda  ists..Exception.
+00000210: 046f 7065 6eda 0577 7269 7465 da05 636c  .open..write..cl
+00000220: 6f73 6529 0472 0a00 0000 da12 7072 6976  ose).r......priv
+00000230: 6174 655f 6b65 795f 7374 7269 6e67 da06  ate_key_string..
+00000240: 666f 726d 6174 da01 66a9 0072 1300 0000  format..f..r....
+00000250: fa44 2f68 6162 6974 6174 2f76 656e 7565  .D/habitat/venue
+00000260: 732f 7374 6167 6573 2f72 6563 7963 6c69  s/stages/recycli
+00000270: 6e67 2f6d 6978 6573 2f45 4543 5f34 3438  ng/mixes/EEC_448
+00000280: 5f32 2f70 7269 7661 7465 5f6b 6579 2f65  _2/private_key/e
+00000290: 7463 682e 7079 da05 7374 6172 740d 0000  tch.py..start...
+000002a0: 0073 1400 0000 0c05 1001 0802 0c01 0802  .s..............
+000002b0: 0c01 1003 0a02 0801 0402 7215 0000 0029  ..........r....)
+000002c0: 03da 075f 5f64 6f63 5f5f 7209 0000 0072  ...__doc__r....r
+000002d0: 1500 0000 7213 0000 0072 1300 0000 7213  ....r....r....r.
+000002e0: 0000 0072 1400 0000 da08 3c6d 6f64 756c  ...r......<modul
+000002f0: 653e 0100 0000 7308 0000 0004 0102 0508  e>....s.........
+00000300: 040c 02                                  ...
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/instance.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/instance.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 958 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 be03 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 ba03 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 0200 0100  Z...d.d.l.m.....
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a07 0100 6401 6403 6c08 6d09  ..m.Z...d.d.l.m.
 00000060: 5a09 0100 6404 6405 8400 5a0a 6402 5300  Z...d.d...Z.d.S.
-00000070: 2906 7aba 0a09 696d 706f 7274 2072 6563  ).z...import rec
-00000080: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-00000090: 4543 5f34 3438 5f32 2e70 7269 7661 7465  EC_448_2.private
-000000a0: 5f6b 6579 2e69 6e73 7461 6e63 6520 6173  _key.instance as
-000000b0: 2069 6e73 7461 6e74 6961 7465 5f70 7269   instantiate_pri
-000000c0: 7661 7465 5f6b 6579 0a09 7072 6976 6174  vate_key..privat
-000000d0: 655f 6b65 795f 696e 7374 616e 6365 203d  e_key_instance =
-000000e0: 2069 6e73 7461 6e74 6961 7465 5f70 7269   instantiate_pri
-000000f0: 7661 7465 5f6b 6579 2e66 726f 6d5f 4445  vate_key.from_DE
-00000100: 525f 6865 7861 6465 6369 6d61 6c5f 7374  R_hexadecimal_st
-00000110: 7269 6e67 2028 4445 525f 6865 7861 6465  ring (DER_hexade
-00000120: 6369 6d61 6c5f 7374 7269 6e67 290a e900  cimal_string)...
-00000130: 0000 004e 2901 da03 4543 4363 0100 0000  ...N)...ECCc....
-00000140: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-00000150: 4300 0000 735c 0000 0074 006a 0174 02a0  C...s\...t.j.t..
-00000160: 037c 00a1 0164 0164 028d 027d 0109 007c  .|...d.d...}...|
-00000170: 016a 0464 0364 048d 017d 027c 02a0 05a1  .j.d.d...}.|....
-00000180: 00a0 06a1 007d 0374 077c 0383 0164 056b  .....}.t.|...d.k
-00000190: 0273 234a 0074 077c 0383 0183 0182 0174  .s#J.t.|.......t
-000001a0: 08a0 097c 03a1 017c 026b 0273 2c4a 0082  ...|...|.k.s,J..
-000001b0: 017c 0153 0029 064e da05 4564 3434 3829  .|.S.).N..Ed448)
-000001c0: 01da 0a63 7572 7665 5f6e 616d 65da 0344  ...curve_name..D
-000001d0: 4552 2901 da06 666f 726d 6174 e992 0000  ER)...format....
-000001e0: 0029 0a72 0200 0000 da0a 696d 706f 7274  .).r......import
-000001f0: 5f6b 6579 da1a 6865 7861 6465 6369 6d61  _key..hexadecima
-00000200: 6c5f 746f 5f62 7974 655f 7374 7269 6e67  l_to_byte_string
-00000210: da08 6d6f 6475 6c61 7465 da0a 6578 706f  ..modulate..expo
-00000220: 7274 5f6b 6579 da03 6865 78da 0575 7070  rt_key..hex..upp
-00000230: 6572 da03 6c65 6eda 0562 7974 6573 da07  er..len..bytes..
-00000240: 6672 6f6d 6865 7829 04da 1644 4552 5f68  fromhex)...DER_h
-00000250: 6578 6164 6563 696d 616c 5f73 7472 696e  exadecimal_strin
-00000260: 67da 0869 6e73 7461 6e63 65da 0e44 4552  g..instance..DER
-00000270: 5f6b 6579 5f73 7472 696e 67da 1268 6578  _key_string..hex
-00000280: 6164 6563 696d 616c 5f73 7472 696e 67a9  adecimal_string.
-00000290: 0072 1500 0000 fa4a 2f68 6162 6974 6174  .r.....J/habitat
-000002a0: 2f76 656e 7565 732f 7374 6167 6573 2f72  /venues/stages/r
-000002b0: 6563 7963 6c69 6e67 2f6d 6f64 756c 6573  ecycling/modules
-000002c0: 2f45 4543 5f34 3438 5f32 2f70 7269 7661  /EEC_448_2/priva
-000002d0: 7465 5f6b 6579 2f69 6e73 7461 6e63 652e  te_key/instance.
-000002e0: 7079 da1b 6672 6f6d 5f44 4552 5f68 6578  py..from_DER_hex
-000002f0: 6164 6563 696d 616c 5f73 7472 696e 6716  adecimal_string.
-00000300: 0000 0073 1800 0000 0401 0801 0201 06fe  ...s............
-00000310: 0205 0403 0201 06ff 0c03 1801 1201 0403  ................
-00000320: 7217 0000 0029 0bda 075f 5f64 6f63 5f5f  r....)...__doc__
-00000330: da43 7265 6379 636c 696e 672e 6d6f 6475  .Crecycling.modu
-00000340: 6c65 732e 4545 435f 3434 385f 322e 6d6f  les.EEC_448_2.mo
-00000350: 6475 6c61 746f 7273 2e62 7974 655f 7374  dulators.byte_st
-00000360: 7269 6e67 2e66 726f 6d5f 6865 7861 6465  ring.from_hexade
-00000370: 6369 6d61 6cda 076d 6f64 756c 6573 da09  cimal..modules..
-00000380: 4545 435f 3434 385f 32da 0a6d 6f64 756c  EEC_448_2..modul
-00000390: 6174 6f72 73da 0b62 7974 655f 7374 7269  ators..byte_stri
-000003a0: 6e67 da10 6672 6f6d 5f68 6578 6164 6563  ng..from_hexadec
-000003b0: 696d 616c 7209 0000 00da 1043 7279 7074  imalr......Crypt
-000003c0: 6f2e 5075 626c 6963 4b65 7972 0200 0000  o.PublicKeyr....
-000003d0: 7217 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000003e0: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-000003f0: 6c65 3e01 0000 0073 0a00 0000 0403 0205  le>....s........
-00000400: 2409 0c02 0c02                           $.....
+00000070: 2906 7ab8 0a09 696d 706f 7274 2072 6563  ).z...import rec
+00000080: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000090: 5f34 3438 5f32 2e70 7269 7661 7465 5f6b  _448_2.private_k
+000000a0: 6579 2e69 6e73 7461 6e63 6520 6173 2069  ey.instance as i
+000000b0: 6e73 7461 6e74 6961 7465 5f70 7269 7661  nstantiate_priva
+000000c0: 7465 5f6b 6579 0a09 7072 6976 6174 655f  te_key..private_
+000000d0: 6b65 795f 696e 7374 616e 6365 203d 2069  key_instance = i
+000000e0: 6e73 7461 6e74 6961 7465 5f70 7269 7661  nstantiate_priva
+000000f0: 7465 5f6b 6579 2e66 726f 6d5f 4445 525f  te_key.from_DER_
+00000100: 6865 7861 6465 6369 6d61 6c5f 7374 7269  hexadecimal_stri
+00000110: 6e67 2028 4445 525f 6865 7861 6465 6369  ng (DER_hexadeci
+00000120: 6d61 6c5f 7374 7269 6e67 290a e900 0000  mal_string).....
+00000130: 004e 2901 da03 4543 4363 0100 0000 0000  .N)...ECCc......
+00000140: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+00000150: 0000 735c 0000 0074 006a 0174 02a0 037c  ..s\...t.j.t...|
+00000160: 00a1 0164 0164 028d 027d 0109 007c 016a  ...d.d...}...|.j
+00000170: 0464 0364 048d 017d 027c 02a0 05a1 00a0  .d.d...}.|......
+00000180: 06a1 007d 0374 077c 0383 0164 056b 0273  ...}.t.|...d.k.s
+00000190: 234a 0074 077c 0383 0183 0182 0174 08a0  #J.t.|.......t..
+000001a0: 097c 03a1 017c 026b 0273 2c4a 0082 017c  .|...|.k.s,J...|
+000001b0: 0153 0029 064e da05 4564 3434 3829 01da  .S.).N..Ed448)..
+000001c0: 0a63 7572 7665 5f6e 616d 65da 0344 4552  .curve_name..DER
+000001d0: 2901 da06 666f 726d 6174 e992 0000 0029  )...format.....)
+000001e0: 0a72 0200 0000 da0a 696d 706f 7274 5f6b  .r......import_k
+000001f0: 6579 da1a 6865 7861 6465 6369 6d61 6c5f  ey..hexadecimal_
+00000200: 746f 5f62 7974 655f 7374 7269 6e67 da08  to_byte_string..
+00000210: 6d6f 6475 6c61 7465 da0a 6578 706f 7274  modulate..export
+00000220: 5f6b 6579 da03 6865 78da 0575 7070 6572  _key..hex..upper
+00000230: da03 6c65 6eda 0562 7974 6573 da07 6672  ..len..bytes..fr
+00000240: 6f6d 6865 7829 04da 1644 4552 5f68 6578  omhex)...DER_hex
+00000250: 6164 6563 696d 616c 5f73 7472 696e 67da  adecimal_string.
+00000260: 0869 6e73 7461 6e63 65da 0e44 4552 5f6b  .instance..DER_k
+00000270: 6579 5f73 7472 696e 67da 1268 6578 6164  ey_string..hexad
+00000280: 6563 696d 616c 5f73 7472 696e 67a9 0072  ecimal_string..r
+00000290: 1500 0000 fa48 2f68 6162 6974 6174 2f76  .....H/habitat/v
+000002a0: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
+000002b0: 7963 6c69 6e67 2f6d 6978 6573 2f45 4543  ycling/mixes/EEC
+000002c0: 5f34 3438 5f32 2f70 7269 7661 7465 5f6b  _448_2/private_k
+000002d0: 6579 2f69 6e73 7461 6e63 652e 7079 da1b  ey/instance.py..
+000002e0: 6672 6f6d 5f44 4552 5f68 6578 6164 6563  from_DER_hexadec
+000002f0: 696d 616c 5f73 7472 696e 6716 0000 0073  imal_string....s
+00000300: 1800 0000 0401 0801 0201 06fe 0205 0403  ................
+00000310: 0201 06ff 0c03 1801 1201 0403 7217 0000  ............r...
+00000320: 0029 0bda 075f 5f64 6f63 5f5f da41 7265  .)...__doc__.Are
+00000330: 6379 636c 696e 672e 6d69 7865 732e 4545  cycling.mixes.EE
+00000340: 435f 3434 385f 322e 6d6f 6475 6c61 746f  C_448_2.modulato
+00000350: 7273 2e62 7974 655f 7374 7269 6e67 2e66  rs.byte_string.f
+00000360: 726f 6d5f 6865 7861 6465 6369 6d61 6cda  rom_hexadecimal.
+00000370: 056d 6978 6573 da09 4545 435f 3434 385f  .mixes..EEC_448_
+00000380: 32da 0a6d 6f64 756c 6174 6f72 73da 0b62  2..modulators..b
+00000390: 7974 655f 7374 7269 6e67 da10 6672 6f6d  yte_string..from
+000003a0: 5f68 6578 6164 6563 696d 616c 7209 0000  _hexadecimalr...
+000003b0: 00da 1043 7279 7074 6f2e 5075 626c 6963  ...Crypto.Public
+000003c0: 4b65 7972 0200 0000 7217 0000 0072 1500  Keyr....r....r..
+000003d0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000003e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000003f0: 0a00 0000 0403 0205 2409 0c02 0c02       ........$.....
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/__pycache__/scan.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/__pycache__/scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 876 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 6c03 0000  o........@@fl...
+00000000: 6f0d 0d0a 0000 0000 d153 5166 6a03 0000  o........SQfj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6405 6406 8400 5a06 6404 5300 2907  Z.d.d...Z.d.S.).
-00000060: 7a93 0a09 696d 706f 7274 2072 6563 7963  z...import recyc
-00000070: 6c69 6e67 2e6d 6f64 756c 6573 2e45 4543  ling.modules.EEC
-00000080: 5f34 3438 5f32 2e70 7269 7661 7465 5f6b  _448_2.private_k
-00000090: 6579 2e73 6361 6e20 6173 2070 7269 7661  ey.scan as priva
-000000a0: 7465 5f6b 6579 5f73 6361 6e0a 0970 7269  te_key_scan..pri
-000000b0: 7661 7465 5f6b 6579 5f73 6361 6e20 3d20  vate_key_scan = 
-000000c0: 7072 6976 6174 655f 6b65 795f 7363 616e  private_key_scan
-000000d0: 2e73 7461 7274 2028 7061 7468 2920 5b22  .start (path) ["
-000000e0: 6865 7861 6465 6369 6d61 6c20 7374 7269  hexadecimal stri
-000000f0: 6e67 225d 0ae9 0000 0000 2901 da03 4543  ng"]......)...EC
-00000100: 4329 01da 0846 7261 6374 696f 6e4e 6302  C)...FractionNc.
-00000110: 0000 0000 0000 0000 0000 0008 0000 0008  ................
-00000120: 0000 0043 0000 0073 be00 0000 7c01 6401  ...C...s....|.d.
-00000130: 6b02 7223 7400 7c00 6402 6403 8d02 8f11  k.r#t.|.d.d.....
-00000140: 7d02 7c02 a001 a100 7d03 7402 a003 7c03  }.|.....}.t...|.
-00000150: a101 5700 0200 6400 0400 0400 8303 0100  ..W...d.........
-00000160: 5300 3100 731e 7701 0100 0100 0100 5900  S.1.s.w.......Y.
-00000170: 0100 7c01 6404 6b02 725b 7400 7c00 6405  ..|.d.k.r[t.|.d.
-00000180: 6403 8d02 8f26 7d02 7c02 a001 a100 7d04  d....&}.|.....}.
-00000190: 7404 6a05 7c04 6406 6407 8d02 7d05 7c04  t.j.|.d.d...}.|.
-000001a0: a006 a100 a007 a100 7d06 4700 6408 6409  ........}.G.d.d.
-000001b0: 8400 6409 8302 7d07 7c06 7c04 7c05 640a  ..d...}.|.|.|.d.
-000001c0: 9c03 5700 0200 6400 0400 0400 8303 0100  ..W...d.........
-000001d0: 5300 3100 7356 7701 0100 0100 0100 5900  S.1.sVw.......Y.
-000001e0: 0100 7408 640b 8301 8201 290c 4eda 044a  ..t.d.....).N..J
-000001f0: 534f 4eda 0172 2901 da04 6d6f 6465 da03  SON..r)...mode..
-00000200: 4445 52da 0272 62da 0545 6434 3438 2901  DER..rb..Ed448).
-00000210: da0a 6375 7276 655f 6e61 6d65 6300 0000  ..curve_namec...
-00000220: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00000230: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000240: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
-00000250: 7a1a 7374 6172 742e 3c6c 6f63 616c 733e  z.start.<locals>
-00000260: 2e70 7269 7661 7465 5f6b 6579 6302 0000  .private_keyc...
-00000270: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000280: 0053 0000 0073 0a00 0000 7c01 7c00 5f00  .S...s....|.|._.
-00000290: 6400 5300 2901 4e29 01da 0869 6e73 7461  d.S.).N)...insta
-000002a0: 6e63 6529 02da 0474 6869 7372 0b00 0000  nce)...thisr....
-000002b0: a900 720d 0000 00fa 462f 6861 6269 7461  ..r.....F/habita
-000002c0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-000002d0: 7265 6379 636c 696e 672f 6d6f 6475 6c65  recycling/module
-000002e0: 732f 4545 435f 3434 385f 322f 7072 6976  s/EEC_448_2/priv
-000002f0: 6174 655f 6b65 792f 7363 616e 2e70 79da  ate_key/scan.py.
-00000300: 085f 5f69 6e69 745f 5f21 0000 0073 0200  .__init__!...s..
-00000310: 0000 0a01 7a23 7374 6172 742e 3c6c 6f63  ....z#start.<loc
-00000320: 616c 733e 2e70 7269 7661 7465 5f6b 6579  als>.private_key
-00000330: 2e5f 5f69 6e69 745f 5f4e 2904 da08 5f5f  .__init__N)...__
-00000340: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000350: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000360: 720f 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000370: 0d00 0000 720e 0000 00da 0b70 7269 7661  ....r......priva
-00000380: 7465 5f6b 6579 2000 0000 7304 0000 0008  te_key ...s.....
-00000390: 000c 0172 1300 0000 2903 7a16 4445 5220  ...r....).z.DER 
-000003a0: 6865 7861 6465 6369 6d61 6c20 7374 7269  hexadecimal stri
-000003b0: 6e67 7a0f 4445 5220 6279 7465 2073 7472  ngz.DER byte str
-000003c0: 696e 6772 0b00 0000 7a03 2e2e 2e29 09da  ingr....z....)..
-000003d0: 046f 7065 6eda 0472 6561 64da 046a 736f  .open..read..jso
-000003e0: 6eda 056c 6f61 6473 7202 0000 00da 0a69  n..loadsr......i
-000003f0: 6d70 6f72 745f 6b65 79da 0368 6578 da05  mport_key..hex..
-00000400: 7570 7065 72da 0945 7863 6570 7469 6f6e  upper..Exception
-00000410: 2908 da04 7061 7468 da06 666f 726d 6174  )...path..format
-00000420: da04 6669 6c65 da0b 4a53 4f4e 5f73 7472  ..file..JSON_str
-00000430: 696e 67da 0b62 7974 655f 7374 7269 6e67  ing..byte_string
-00000440: 720b 0000 00da 1268 6578 6164 6563 696d  r......hexadecim
-00000450: 616c 5f73 7472 696e 6772 1300 0000 720d  al_stringr....r.
-00000460: 0000 0072 0d00 0000 720e 0000 00da 0573  ...r....r......s
-00000470: 7461 7274 0e00 0000 7328 0000 0008 020e  tart....s(......
-00000480: 0108 0108 0220 fd08 060e 0108 0104 0102  ..... ..........
-00000490: 0102 0106 fe0c 040e 0202 0502 0102 0104  ................
-000004a0: fd20 f408 1272 2200 0000 2907 da07 5f5f  . ...r"...)...__
-000004b0: 646f 635f 5fda 1043 7279 7074 6f2e 5075  doc__..Crypto.Pu
-000004c0: 626c 6963 4b65 7972 0200 0000 da09 6672  blicKeyr......fr
-000004d0: 6163 7469 6f6e 7372 0300 0000 7216 0000  actionsr....r...
-000004e0: 0072 2200 0000 720d 0000 0072 0d00 0000  .r"...r....r....
-000004f0: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
-00000500: 756c 653e 0100 0000 730a 0000 0004 030c  ule>....s.......
-00000510: 050c 0108 020c 02                        .......
+00000060: 7a91 0a09 696d 706f 7274 2072 6563 7963  z...import recyc
+00000070: 6c69 6e67 2e6d 6978 6573 2e45 4543 5f34  ling.mixes.EEC_4
+00000080: 3438 5f32 2e70 7269 7661 7465 5f6b 6579  48_2.private_key
+00000090: 2e73 6361 6e20 6173 2070 7269 7661 7465  .scan as private
+000000a0: 5f6b 6579 5f73 6361 6e0a 0970 7269 7661  _key_scan..priva
+000000b0: 7465 5f6b 6579 5f73 6361 6e20 3d20 7072  te_key_scan = pr
+000000c0: 6976 6174 655f 6b65 795f 7363 616e 2e73  ivate_key_scan.s
+000000d0: 7461 7274 2028 7061 7468 2920 5b22 6865  tart (path) ["he
+000000e0: 7861 6465 6369 6d61 6c20 7374 7269 6e67  xadecimal string
+000000f0: 225d 0ae9 0000 0000 2901 da03 4543 4329  "]......)...ECC)
+00000100: 01da 0846 7261 6374 696f 6e4e 6302 0000  ...FractionNc...
+00000110: 0000 0000 0000 0000 0008 0000 0008 0000  ................
+00000120: 0043 0000 0073 be00 0000 7c01 6401 6b02  .C...s....|.d.k.
+00000130: 7223 7400 7c00 6402 6403 8d02 8f11 7d02  r#t.|.d.d.....}.
+00000140: 7c02 a001 a100 7d03 7402 a003 7c03 a101  |.....}.t...|...
+00000150: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+00000160: 3100 731e 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00000170: 7c01 6404 6b02 725b 7400 7c00 6405 6403  |.d.k.r[t.|.d.d.
+00000180: 8d02 8f26 7d02 7c02 a001 a100 7d04 7404  ...&}.|.....}.t.
+00000190: 6a05 7c04 6406 6407 8d02 7d05 7c04 a006  j.|.d.d...}.|...
+000001a0: a100 a007 a100 7d06 4700 6408 6409 8400  ......}.G.d.d...
+000001b0: 6409 8302 7d07 7c06 7c04 7c05 640a 9c03  d...}.|.|.|.d...
+000001c0: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+000001d0: 3100 7356 7701 0100 0100 0100 5900 0100  1.sVw.......Y...
+000001e0: 7408 640b 8301 8201 290c 4eda 044a 534f  t.d.....).N..JSO
+000001f0: 4eda 0172 2901 da04 6d6f 6465 da03 4445  N..r)...mode..DE
+00000200: 52da 0272 62da 0545 6434 3438 2901 da0a  R..rb..Ed448)...
+00000210: 6375 7276 655f 6e61 6d65 6300 0000 0000  curve_namec.....
+00000220: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00000230: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000240: 6401 6402 8400 5a03 6403 5300 2904 7a1a  d.d...Z.d.S.).z.
+00000250: 7374 6172 742e 3c6c 6f63 616c 733e 2e70  start.<locals>.p
+00000260: 7269 7661 7465 5f6b 6579 6302 0000 0000  rivate_keyc.....
+00000270: 0000 0000 0000 0002 0000 0002 0000 0053  ...............S
+00000280: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
+00000290: 5300 2901 4e29 01da 0869 6e73 7461 6e63  S.).N)...instanc
+000002a0: 6529 02da 0474 6869 7372 0b00 0000 a900  e)...thisr......
+000002b0: 720d 0000 00fa 442f 6861 6269 7461 742f  r.....D/habitat/
+000002c0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+000002d0: 6379 636c 696e 672f 6d69 7865 732f 4545  cycling/mixes/EE
+000002e0: 435f 3434 385f 322f 7072 6976 6174 655f  C_448_2/private_
+000002f0: 6b65 792f 7363 616e 2e70 79da 085f 5f69  key/scan.py..__i
+00000300: 6e69 745f 5f21 0000 0073 0200 0000 0a01  nit__!...s......
+00000310: 7a23 7374 6172 742e 3c6c 6f63 616c 733e  z#start.<locals>
+00000320: 2e70 7269 7661 7465 5f6b 6579 2e5f 5f69  .private_key.__i
+00000330: 6e69 745f 5f4e 2904 da08 5f5f 6e61 6d65  nit__N)...__name
+00000340: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000350: 5f5f 7175 616c 6e61 6d65 5f5f 720f 0000  __qualname__r...
+00000360: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000370: 720e 0000 00da 0b70 7269 7661 7465 5f6b  r......private_k
+00000380: 6579 2000 0000 7304 0000 0008 000c 0172  ey ...s........r
+00000390: 1300 0000 2903 7a16 4445 5220 6865 7861  ....).z.DER hexa
+000003a0: 6465 6369 6d61 6c20 7374 7269 6e67 7a0f  decimal stringz.
+000003b0: 4445 5220 6279 7465 2073 7472 696e 6772  DER byte stringr
+000003c0: 0b00 0000 7a03 2e2e 2e29 09da 046f 7065  ....z....)...ope
+000003d0: 6eda 0472 6561 64da 046a 736f 6eda 056c  n..read..json..l
+000003e0: 6f61 6473 7202 0000 00da 0a69 6d70 6f72  oadsr......impor
+000003f0: 745f 6b65 79da 0368 6578 da05 7570 7065  t_key..hex..uppe
+00000400: 72da 0945 7863 6570 7469 6f6e 2908 da04  r..Exception)...
+00000410: 7061 7468 da06 666f 726d 6174 da04 6669  path..format..fi
+00000420: 6c65 da0b 4a53 4f4e 5f73 7472 696e 67da  le..JSON_string.
+00000430: 0b62 7974 655f 7374 7269 6e67 720b 0000  .byte_stringr...
+00000440: 00da 1268 6578 6164 6563 696d 616c 5f73  ...hexadecimal_s
+00000450: 7472 696e 6772 1300 0000 720d 0000 0072  tringr....r....r
+00000460: 0d00 0000 720e 0000 00da 0573 7461 7274  ....r......start
+00000470: 0e00 0000 7328 0000 0008 020e 0108 0108  ....s(..........
+00000480: 0220 fd08 060e 0108 0104 0102 0102 0106  . ..............
+00000490: fe0c 040e 0202 0502 0102 0104 fd20 f408  ............. ..
+000004a0: 1272 2200 0000 2907 da07 5f5f 646f 635f  .r"...)...__doc_
+000004b0: 5fda 1043 7279 7074 6f2e 5075 626c 6963  _..Crypto.Public
+000004c0: 4b65 7972 0200 0000 da09 6672 6163 7469  Keyr......fracti
+000004d0: 6f6e 7372 0300 0000 7216 0000 0072 2200  onsr....r....r".
+000004e0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+000004f0: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000500: 0100 0000 730a 0000 0004 030c 050c 0108  ....s...........
+00000510: 020c 02                                  ...
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/creator.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/creator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 '''
 	seed = "4986888b11358bf3d541b41eea5daece1c6eff64130a45fc8b9ca48f3e0e02463c99c5aedc8a847686d669b7d547c18fe448fc5111ca88f4e8"
 
-	import recycling.modules.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
+	import recycling.mixes.EEC_448_2.private_key.creator as EEC_448_2_private_key_creator
 	EEC_448_2_private_key_creator.create (
 		seed
 	)
 	
 	private_key_instance = private_key ["instance"]
 	private_key_hexadecimal = private_key ["hexadecimal string"]
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/etch.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/etch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 '''
-	import recycling.modules.EEC_448_2.private_key.etch as etch_EEC_448_private_key
+	import recycling.mixes.EEC_448_2.private_key.etch as etch_EEC_448_private_key
 	etch_EEC_448_private_key.start (path, private_key_string, "JSON")
 '''
 
 '''
 	{ form, save, write, compose, produce, etch }
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/instance.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 
 
 '''
-	import recycling.modules.EEC_448_2.private_key.instance as instantiate_private_key
+	import recycling.mixes.EEC_448_2.private_key.instance as instantiate_private_key
 	private_key_instance = instantiate_private_key.from_DER_hexadecimal_string (DER_hexadecimal_string)
 '''
 
 '''
 	DER_key_string = private_key_instance.export_key (
 		format = "DER"
 	)	
 	PEM_key_string = private_key_instance.export_key (
 		format = "PEM"
 	)
 '''
 
-import recycling.modules.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
+import recycling.mixes.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
 
 from Crypto.PublicKey import ECC
 
 def from_DER_hexadecimal_string (DER_hexadecimal_string):
 	instance = ECC.import_key (
 		hexadecimal_to_byte_string.modulate (DER_hexadecimal_string),
 		curve_name = "Ed448"
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/private_key/scan.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/private_key/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 '''
-	import recycling.modules.EEC_448_2.private_key.scan as private_key_scan
+	import recycling.mixes.EEC_448_2.private_key.scan as private_key_scan
 	private_key_scan = private_key_scan.start (path) ["hexadecimal string"]
 '''
 
 from Crypto.PublicKey import ECC
 from fractions import Fraction
 
 import json
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/BUILD.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/BUILD.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/CREATE.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/CREATE.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/SCAN.cpython-311.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/creator.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/creator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,90 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9505 0000  o........@@f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
-00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
-00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
-00000050: 5a05 0100 6401 6402 6c06 6d07 0200 0100  Z...d.d.l.m.....
-00000060: 6d08 0200 0100 6d09 0200 0100 6d0a 5a0b  m.....m.....m.Z.
-00000070: 0100 6405 6406 8400 5a0c 0902 6409 6407  ..d.d...Z...d.d.
-00000080: 6408 8401 5a0d 6402 5300 290a 6145 0100  d...Z.d.S.).aE..
-00000090: 000a 0923 0a09 2309 7772 6974 6520 7075  ...#..#.write pu
-000000a0: 626c 6963 206b 6579 2074 6f20 7061 7468  blic key to path
-000000b0: 0a09 230a 0969 6d70 6f72 7420 7265 6379  ..#..import recy
-000000c0: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-000000d0: 435f 3434 385f 322e 7075 626c 6963 5f6b  C_448_2.public_k
-000000e0: 6579 2e63 7265 6174 6f72 2061 7320 4545  ey.creator as EE
-000000f0: 435f 3434 385f 325f 7075 626c 6963 5f6b  C_448_2_public_k
-00000100: 6579 5f63 7265 6174 6f72 0a09 7075 626c  ey_creator..publ
-00000110: 6963 5f6b 6579 203d 2045 4543 5f34 3438  ic_key = EEC_448
-00000120: 5f32 5f70 7562 6c69 635f 6b65 795f 6372  _2_public_key_cr
-00000130: 6561 746f 722e 6372 6561 7465 2028 0a09  eator.create (..
-00000140: 0970 7269 7661 7465 5f6b 6579 5f69 6e73  .private_key_ins
-00000150: 7461 6e63 650a 0929 0a09 7075 626c 6963  tance..)..public
-00000160: 5f6b 6579 5f69 6e73 7461 6e63 6520 3d20  _key_instance = 
-00000170: 7075 626c 6963 5f6b 6579 205b 2269 6e73  public_key ["ins
-00000180: 7461 6e63 6522 5d0a 0970 7562 6c69 635f  tance"]..public_
-00000190: 6b65 795f 4445 525f 6865 7861 6465 6369  key_DER_hexadeci
-000001a0: 6d61 6c5f 7374 7269 6e67 203d 2070 7562  mal_string = pub
-000001b0: 6c69 635f 6b65 7920 5b22 4445 5220 6865  lic_key ["DER he
-000001c0: 7861 6465 6369 6d61 6c20 7374 7269 6e67  xadecimal string
-000001d0: 225d 0a09 090a e900 0000 004e 2901 da06  "].........N)...
-000001e0: 4563 634b 6579 2901 da03 4543 4363 0100  EccKey)...ECCc..
-000001f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000200: 0000 4300 0000 732e 0000 007c 00a0 00a1  ..C...s....|....
-00000210: 007d 0174 017c 0183 0164 016b 0273 0c4a  .}.t.|...d.k.s.J
-00000220: 0082 0174 02a0 037c 01a1 017c 006b 0273  ...t...|...|.k.s
-00000230: 154a 0082 017c 0153 0029 024e e98a 0000  .J...|.S.).N....
-00000240: 0029 04da 0368 6578 da03 6c65 6eda 0562  .)...hex..len..b
-00000250: 7974 6573 da07 6672 6f6d 6865 7829 02da  ytes..fromhex)..
-00000260: 1a70 7562 6c69 635f 6b65 795f 4445 525f  .public_key_DER_
-00000270: 6279 7465 5f73 7472 696e 67da 2170 7562  byte_string.!pub
-00000280: 6c69 635f 6b65 795f 4445 525f 6865 7861  lic_key_DER_hexa
-00000290: 6465 6369 6d61 6c5f 7374 7269 6e67 a900  decimal_string..
-000002a0: 720b 0000 00fa 482f 6861 6269 7461 742f  r.....H/habitat/
-000002b0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
-000002c0: 6379 636c 696e 672f 6d6f 6475 6c65 732f  cycling/modules/
-000002d0: 4545 435f 3434 385f 322f 7075 626c 6963  EEC_448_2/public
-000002e0: 5f6b 6579 2f63 7265 6174 6f72 2e70 79da  _key/creator.py.
-000002f0: 1d63 7265 6174 655f 4445 525f 6865 7861  .create_DER_hexa
-00000300: 6465 6369 6d61 6c5f 7374 7269 6e67 1c00  decimal_string..
-00000310: 0000 730c 0000 0008 0110 0108 0202 0108  ..s.............
-00000320: ff04 0472 0d00 0000 6301 0000 0000 0000  ...r....c.......
-00000330: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-00000340: 0073 3600 0000 7c00 a000 a100 7d01 7c01  .s6...|.....}.|.
-00000350: 6a01 6401 6402 8d01 7d02 7c01 6a01 6403  j.d.d...}.|.j.d.
-00000360: 6402 8d01 7d03 7402 7c02 8301 7d04 7c01  d...}.t.|...}.|.
-00000370: 7c02 7c04 7c03 6404 9c04 5300 2905 4eda  |.|.|.d...S.).N.
-00000380: 0344 4552 2901 da06 666f 726d 6174 da03  .DER)...format..
-00000390: 5045 4d29 04da 0869 6e73 7461 6e63 657a  PEM)...instancez
-000003a0: 0f44 4552 2062 7974 6520 7374 7269 6e67  .DER byte string
-000003b0: 7a16 4445 5220 6865 7861 6465 6369 6d61  z.DER hexadecima
-000003c0: 6c20 7374 7269 6e67 7a0a 5045 4d20 7374  l stringz.PEM st
-000003d0: 7269 6e67 2903 da0a 7075 626c 6963 5f6b  ring)...public_k
-000003e0: 6579 da0a 6578 706f 7274 5f6b 6579 720d  ey..export_keyr.
-000003f0: 0000 0029 05da 1470 7269 7661 7465 5f6b  ...)...private_k
-00000400: 6579 5f69 6e73 7461 6e63 65da 1370 7562  ey_instance..pub
-00000410: 6c69 635f 6b65 795f 696e 7374 616e 6365  lic_key_instance
-00000420: 7209 0000 00da 1570 7562 6c69 635f 6b65  r......public_ke
-00000430: 795f 5045 4d5f 7374 7269 6e67 720a 0000  y_PEM_stringr...
-00000440: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000450: da06 6372 6561 7465 2600 0000 731e 0000  ..create&...s...
-00000460: 0008 0304 0102 0106 ff04 0302 0106 ff02  ................
-00000470: 0402 0104 ff02 0502 0202 0102 0206 fa72  ...............r
-00000480: 1700 0000 2901 4e29 0eda 075f 5f64 6f63  ....).N)...__doc
-00000490: 5f5f da02 6f73 da14 4372 7970 746f 2e50  __..os..Crypto.P
-000004a0: 7562 6c69 634b 6579 2e45 4343 7202 0000  ublicKey.ECCr...
-000004b0: 00da 1043 7279 7074 6f2e 5075 626c 6963  ...Crypto.Public
-000004c0: 4b65 7972 0300 0000 da2c 7265 6379 636c  Keyr.....,recycl
-000004d0: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-000004e0: 3434 385f 322e 7072 6976 6174 655f 6b65  448_2.private_ke
-000004f0: 792e 7363 616e da07 6d6f 6475 6c65 73da  y.scan..modules.
-00000500: 0945 4543 5f34 3438 5f32 da0b 7072 6976  .EEC_448_2..priv
-00000510: 6174 655f 6b65 79da 0473 6361 6eda 0c70  ate_key..scan..p
-00000520: 7269 7661 7465 5f73 6361 6e72 0d00 0000  rivate_scanr....
-00000530: 7217 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000540: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00000550: 6c65 3e01 0000 0073 1200 0000 0401 020d  le>....s........
-00000560: 0805 0c02 0c01 1e02 0803 020b 0eff       ..............
+00000000: 0a27 2727 0a09 230a 0923 0977 7269 7465  .'''..#..#.write
+00000010: 2070 7562 6c69 6320 6b65 7920 746f 2070   public key to p
+00000020: 6174 680a 0923 0a09 696d 706f 7274 2072  ath..#..import r
+00000030: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00000040: 4543 5f34 3438 5f32 2e70 7562 6c69 635f  EC_448_2.public_
+00000050: 6b65 792e 6372 6561 746f 7220 6173 2045  key.creator as E
+00000060: 4543 5f34 3438 5f32 5f70 7562 6c69 635f  EC_448_2_public_
+00000070: 6b65 795f 6372 6561 746f 720a 0970 7562  key_creator..pub
+00000080: 6c69 635f 6b65 7920 3d20 4545 435f 3434  lic_key = EEC_44
+00000090: 385f 325f 7075 626c 6963 5f6b 6579 5f63  8_2_public_key_c
+000000a0: 7265 6174 6f72 2e63 7265 6174 6520 280a  reator.create (.
+000000b0: 0909 7072 6976 6174 655f 6b65 795f 696e  ..private_key_in
+000000c0: 7374 616e 6365 0a09 290a 0970 7562 6c69  stance..)..publi
+000000d0: 635f 6b65 795f 696e 7374 616e 6365 203d  c_key_instance =
+000000e0: 2070 7562 6c69 635f 6b65 7920 5b22 696e   public_key ["in
+000000f0: 7374 616e 6365 225d 0a09 7075 626c 6963  stance"]..public
+00000100: 5f6b 6579 5f44 4552 5f68 6578 6164 6563  _key_DER_hexadec
+00000110: 696d 616c 5f73 7472 696e 6720 3d20 7075  imal_string = pu
+00000120: 626c 6963 5f6b 6579 205b 2244 4552 2068  blic_key ["DER h
+00000130: 6578 6164 6563 696d 616c 2073 7472 696e  exadecimal strin
+00000140: 6722 5d0a 0909 0a27 2727 0a0a 2727 270a  g"]....'''..'''.
+00000150: 0966 6f72 6d61 743a 0a09 0944 4552 0a09  .format:...DER..
+00000160: 0950 454d 0a27 2727 0a69 6d70 6f72 7420  .PEM.'''.import 
+00000170: 6f73 0a0a 6672 6f6d 2043 7279 7074 6f2e  os..from Crypto.
+00000180: 5075 626c 6963 4b65 792e 4543 4320 696d  PublicKey.ECC im
+00000190: 706f 7274 2045 6363 4b65 790a 6672 6f6d  port EccKey.from
+000001a0: 2043 7279 7074 6f2e 5075 626c 6963 4b65   Crypto.PublicKe
+000001b0: 7920 696d 706f 7274 2045 4343 0a0a 696d  y import ECC..im
+000001c0: 706f 7274 2072 6563 7963 6c69 6e67 2e6d  port recycling.m
+000001d0: 6978 6573 2e45 4543 5f34 3438 5f32 2e70  ixes.EEC_448_2.p
+000001e0: 7269 7661 7465 5f6b 6579 2e73 6361 6e20  rivate_key.scan 
+000001f0: 6173 2070 7269 7661 7465 5f73 6361 6e0a  as private_scan.
+00000200: 0a0a 6465 6620 6372 6561 7465 5f44 4552  ..def create_DER
+00000210: 5f68 6578 6164 6563 696d 616c 5f73 7472  _hexadecimal_str
+00000220: 696e 6720 2870 7562 6c69 635f 6b65 795f  ing (public_key_
+00000230: 4445 525f 6279 7465 5f73 7472 696e 6729  DER_byte_string)
+00000240: 3a0a 0970 7562 6c69 635f 6b65 795f 4445  :..public_key_DE
+00000250: 525f 6865 7861 6465 6369 6d61 6c5f 7374  R_hexadecimal_st
+00000260: 7269 6e67 203d 2070 7562 6c69 635f 6b65  ring = public_ke
+00000270: 795f 4445 525f 6279 7465 5f73 7472 696e  y_DER_byte_strin
+00000280: 672e 6865 7820 2829 0a09 6173 7365 7274  g.hex ()..assert
+00000290: 2028 6c65 6e20 2870 7562 6c69 635f 6b65   (len (public_ke
+000002a0: 795f 4445 525f 6865 7861 6465 6369 6d61  y_DER_hexadecima
+000002b0: 6c5f 7374 7269 6e67 2920 3d3d 2031 3338  l_string) == 138
+000002c0: 290a 0961 7373 6572 7420 280a 0909 6279  )..assert (...by
+000002d0: 7465 732e 6672 6f6d 6865 7820 2870 7562  tes.fromhex (pub
+000002e0: 6c69 635f 6b65 795f 4445 525f 6865 7861  lic_key_DER_hexa
+000002f0: 6465 6369 6d61 6c5f 7374 7269 6e67 2920  decimal_string) 
+00000300: 3d3d 200a 0909 7075 626c 6963 5f6b 6579  == ...public_key
+00000310: 5f44 4552 5f62 7974 655f 7374 7269 6e67  _DER_byte_string
+00000320: 0a09 290a 090a 0972 6574 7572 6e20 7075  ..)....return pu
+00000330: 626c 6963 5f6b 6579 5f44 4552 5f68 6578  blic_key_DER_hex
+00000340: 6164 6563 696d 616c 5f73 7472 696e 670a  adecimal_string.
+00000350: 0a64 6566 2063 7265 6174 6520 280a 0970  .def create (..p
+00000360: 7269 7661 7465 5f6b 6579 5f69 6e73 7461  rivate_key_insta
+00000370: 6e63 6520 3d20 4e6f 6e65 0a29 3a09 0a09  nce = None.):...
+00000380: 7075 626c 6963 5f6b 6579 5f69 6e73 7461  public_key_insta
+00000390: 6e63 6520 3d20 7072 6976 6174 655f 6b65  nce = private_ke
+000003a0: 795f 696e 7374 616e 6365 2e70 7562 6c69  y_instance.publi
+000003b0: 635f 6b65 7920 2829 0a09 7075 626c 6963  c_key ()..public
+000003c0: 5f6b 6579 5f44 4552 5f62 7974 655f 7374  _key_DER_byte_st
+000003d0: 7269 6e67 203d 2070 7562 6c69 635f 6b65  ring = public_ke
+000003e0: 795f 696e 7374 616e 6365 2e65 7870 6f72  y_instance.expor
+000003f0: 745f 6b65 7920 280a 0909 666f 726d 6174  t_key (...format
+00000400: 203d 2022 4445 5222 0a09 290a 0970 7562   = "DER"..)..pub
+00000410: 6c69 635f 6b65 795f 5045 4d5f 7374 7269  lic_key_PEM_stri
+00000420: 6e67 203d 2070 7562 6c69 635f 6b65 795f  ng = public_key_
+00000430: 696e 7374 616e 6365 2e65 7870 6f72 745f  instance.export_
+00000440: 6b65 7920 280a 0909 666f 726d 6174 203d  key (...format =
+00000450: 2022 5045 4d22 0a09 290a 090a 0970 7562   "PEM"..)....pub
+00000460: 6c69 635f 6b65 795f 4445 525f 6865 7861  lic_key_DER_hexa
+00000470: 6465 6369 6d61 6c5f 7374 7269 6e67 203d  decimal_string =
+00000480: 2063 7265 6174 655f 4445 525f 6865 7861   create_DER_hexa
+00000490: 6465 6369 6d61 6c5f 7374 7269 6e67 2028  decimal_string (
+000004a0: 0a09 0970 7562 6c69 635f 6b65 795f 4445  ...public_key_DE
+000004b0: 525f 6279 7465 5f73 7472 696e 670a 0929  R_byte_string..)
+000004c0: 0a0a 0972 6574 7572 6e20 7b09 090a 0909  ...return {.....
+000004d0: 2269 6e73 7461 6e63 6522 3a20 7075 626c  "instance": publ
+000004e0: 6963 5f6b 6579 5f69 6e73 7461 6e63 652c  ic_key_instance,
+000004f0: 200a 0909 0a09 0922 4445 5220 6279 7465   ......"DER byte
+00000500: 2073 7472 696e 6722 3a20 7075 626c 6963   string": public
+00000510: 5f6b 6579 5f44 4552 5f62 7974 655f 7374  _key_DER_byte_st
+00000520: 7269 6e67 2c0a 0909 2244 4552 2068 6578  ring,..."DER hex
+00000530: 6164 6563 696d 616c 2073 7472 696e 6722  adecimal string"
+00000540: 3a20 7075 626c 6963 5f6b 6579 5f44 4552  : public_key_DER
+00000550: 5f68 6578 6164 6563 696d 616c 5f73 7472  _hexadecimal_str
+00000560: 696e 672c 0a09 090a 0909 2250 454d 2073  ing,......"PEM s
+00000570: 7472 696e 6722 3a20 7075 626c 6963 5f6b  tring": public_k
+00000580: 6579 5f50 454d 5f73 7472 696e 670a 097d  ey_PEM_string..}
+00000590: 0a                                       .
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/instance.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/instance.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 959 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 bf03 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 bb03 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 0200 0100  Z...d.d.l.m.....
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a07 0100 6401 6403 6c08 6d09  ..m.Z...d.d.l.m.
 00000060: 5a09 0100 6404 6405 8400 5a0a 6402 5300  Z...d.d...Z.d.S.
-00000070: 2906 7abb 0a09 696d 706f 7274 2072 6563  ).z...import rec
-00000080: 7963 6c69 6e67 2e6d 6f64 756c 6573 2e45  ycling.modules.E
-00000090: 4543 5f34 3438 5f32 2e70 7562 6c69 635f  EC_448_2.public_
-000000a0: 6b65 792e 696e 7374 616e 6365 2061 7320  key.instance as 
-000000b0: 696e 7374 616e 7469 6174 655f 7075 626c  instantiate_publ
-000000c0: 6963 5f6b 6579 0a09 7075 626c 6963 5f6b  ic_key..public_k
-000000d0: 6579 5f69 6e73 7461 6e63 6520 3d20 696e  ey_instance = in
-000000e0: 7374 616e 7469 6174 655f 7075 626c 6963  stantiate_public
-000000f0: 5f6b 6579 2e66 726f 6d5f 4445 525f 6865  _key.from_DER_he
-00000100: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
-00000110: 2028 0a09 0944 4552 5f68 6578 6164 6563   (...DER_hexadec
-00000120: 696d 616c 5f73 7472 696e 670a 0929 0ae9  imal_string..)..
-00000130: 0000 0000 4e29 01da 0345 4343 6301 0000  ....N)...ECCc...
-00000140: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000150: 0043 0000 0073 5c00 0000 7400 6a01 7402  .C...s\...t.j.t.
-00000160: a003 7c00 a101 6401 6402 8d02 7d01 0900  ..|...d.d...}...
-00000170: 7c01 6a04 6403 6404 8d01 7d02 7c02 a005  |.j.d.d...}.|...
-00000180: a100 a006 a100 7d03 7407 7c03 8301 6405  ......}.t.|...d.
-00000190: 6b02 7323 4a00 7407 7c03 8301 8301 8201  k.s#J.t.|.......
-000001a0: 7408 a009 7c03 a101 7c02 6b02 732c 4a00  t...|...|.k.s,J.
-000001b0: 8201 7c01 5300 2906 4eda 0545 6434 3438  ..|.S.).N..Ed448
-000001c0: 2901 da0a 6375 7276 655f 6e61 6d65 da03  )...curve_name..
-000001d0: 4445 5229 01da 0666 6f72 6d61 74e9 8a00  DER)...format...
-000001e0: 0000 290a 7202 0000 00da 0a69 6d70 6f72  ..).r......impor
-000001f0: 745f 6b65 79da 1a68 6578 6164 6563 696d  t_key..hexadecim
-00000200: 616c 5f74 6f5f 6279 7465 5f73 7472 696e  al_to_byte_strin
-00000210: 67da 086d 6f64 756c 6174 65da 0a65 7870  g..modulate..exp
-00000220: 6f72 745f 6b65 79da 0368 6578 da05 7570  ort_key..hex..up
-00000230: 7065 72da 036c 656e da05 6279 7465 73da  per..len..bytes.
-00000240: 0766 726f 6d68 6578 2904 da16 4445 525f  .fromhex)...DER_
-00000250: 6865 7861 6465 6369 6d61 6c5f 7374 7269  hexadecimal_stri
-00000260: 6e67 da08 696e 7374 616e 6365 da0e 4445  ng..instance..DE
-00000270: 525f 6b65 795f 7374 7269 6e67 da12 6865  R_key_string..he
-00000280: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
-00000290: a900 7215 0000 00fa 492f 6861 6269 7461  ..r.....I/habita
-000002a0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-000002b0: 7265 6379 636c 696e 672f 6d6f 6475 6c65  recycling/module
-000002c0: 732f 4545 435f 3434 385f 322f 7075 626c  s/EEC_448_2/publ
-000002d0: 6963 5f6b 6579 2f69 6e73 7461 6e63 652e  ic_key/instance.
-000002e0: 7079 da1b 6672 6f6d 5f44 4552 5f68 6578  py..from_DER_hex
-000002f0: 6164 6563 696d 616c 5f73 7472 696e 6718  adecimal_string.
-00000300: 0000 0073 1800 0000 0401 0801 0201 06fe  ...s............
-00000310: 0205 0403 0201 06ff 0c03 1801 1201 0403  ................
-00000320: 7217 0000 0029 0bda 075f 5f64 6f63 5f5f  r....)...__doc__
-00000330: da43 7265 6379 636c 696e 672e 6d6f 6475  .Crecycling.modu
-00000340: 6c65 732e 4545 435f 3434 385f 322e 6d6f  les.EEC_448_2.mo
-00000350: 6475 6c61 746f 7273 2e62 7974 655f 7374  dulators.byte_st
-00000360: 7269 6e67 2e66 726f 6d5f 6865 7861 6465  ring.from_hexade
-00000370: 6369 6d61 6cda 076d 6f64 756c 6573 da09  cimal..modules..
-00000380: 4545 435f 3434 385f 32da 0a6d 6f64 756c  EEC_448_2..modul
-00000390: 6174 6f72 73da 0b62 7974 655f 7374 7269  ators..byte_stri
-000003a0: 6e67 da10 6672 6f6d 5f68 6578 6164 6563  ng..from_hexadec
-000003b0: 696d 616c 7209 0000 00da 1043 7279 7074  imalr......Crypt
-000003c0: 6f2e 5075 626c 6963 4b65 7972 0200 0000  o.PublicKeyr....
-000003d0: 7217 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000003e0: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-000003f0: 6c65 3e01 0000 0073 0a00 0000 0403 0207  le>....s........
-00000400: 2409 0c02 0c02                           $.....
+00000070: 2906 7ab9 0a09 696d 706f 7274 2072 6563  ).z...import rec
+00000080: 7963 6c69 6e67 2e6d 6978 6573 2e45 4543  ycling.mixes.EEC
+00000090: 5f34 3438 5f32 2e70 7562 6c69 635f 6b65  _448_2.public_ke
+000000a0: 792e 696e 7374 616e 6365 2061 7320 696e  y.instance as in
+000000b0: 7374 616e 7469 6174 655f 7075 626c 6963  stantiate_public
+000000c0: 5f6b 6579 0a09 7075 626c 6963 5f6b 6579  _key..public_key
+000000d0: 5f69 6e73 7461 6e63 6520 3d20 696e 7374  _instance = inst
+000000e0: 616e 7469 6174 655f 7075 626c 6963 5f6b  antiate_public_k
+000000f0: 6579 2e66 726f 6d5f 4445 525f 6865 7861  ey.from_DER_hexa
+00000100: 6465 6369 6d61 6c5f 7374 7269 6e67 2028  decimal_string (
+00000110: 0a09 0944 4552 5f68 6578 6164 6563 696d  ...DER_hexadecim
+00000120: 616c 5f73 7472 696e 670a 0929 0ae9 0000  al_string..)....
+00000130: 0000 4e29 01da 0345 4343 6301 0000 0000  ..N)...ECCc.....
+00000140: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00000150: 0000 0073 5c00 0000 7400 6a01 7402 a003  ...s\...t.j.t...
+00000160: 7c00 a101 6401 6402 8d02 7d01 0900 7c01  |...d.d...}...|.
+00000170: 6a04 6403 6404 8d01 7d02 7c02 a005 a100  j.d.d...}.|.....
+00000180: a006 a100 7d03 7407 7c03 8301 6405 6b02  ....}.t.|...d.k.
+00000190: 7323 4a00 7407 7c03 8301 8301 8201 7408  s#J.t.|.......t.
+000001a0: a009 7c03 a101 7c02 6b02 732c 4a00 8201  ..|...|.k.s,J...
+000001b0: 7c01 5300 2906 4eda 0545 6434 3438 2901  |.S.).N..Ed448).
+000001c0: da0a 6375 7276 655f 6e61 6d65 da03 4445  ..curve_name..DE
+000001d0: 5229 01da 0666 6f72 6d61 74e9 8a00 0000  R)...format.....
+000001e0: 290a 7202 0000 00da 0a69 6d70 6f72 745f  ).r......import_
+000001f0: 6b65 79da 1a68 6578 6164 6563 696d 616c  key..hexadecimal
+00000200: 5f74 6f5f 6279 7465 5f73 7472 696e 67da  _to_byte_string.
+00000210: 086d 6f64 756c 6174 65da 0a65 7870 6f72  .modulate..expor
+00000220: 745f 6b65 79da 0368 6578 da05 7570 7065  t_key..hex..uppe
+00000230: 72da 036c 656e da05 6279 7465 73da 0766  r..len..bytes..f
+00000240: 726f 6d68 6578 2904 da16 4445 525f 6865  romhex)...DER_he
+00000250: 7861 6465 6369 6d61 6c5f 7374 7269 6e67  xadecimal_string
+00000260: da08 696e 7374 616e 6365 da0e 4445 525f  ..instance..DER_
+00000270: 6b65 795f 7374 7269 6e67 da12 6865 7861  key_string..hexa
+00000280: 6465 6369 6d61 6c5f 7374 7269 6e67 a900  decimal_string..
+00000290: 7215 0000 00fa 472f 6861 6269 7461 742f  r.....G/habitat/
+000002a0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+000002b0: 6379 636c 696e 672f 6d69 7865 732f 4545  cycling/mixes/EE
+000002c0: 435f 3434 385f 322f 7075 626c 6963 5f6b  C_448_2/public_k
+000002d0: 6579 2f69 6e73 7461 6e63 652e 7079 da1b  ey/instance.py..
+000002e0: 6672 6f6d 5f44 4552 5f68 6578 6164 6563  from_DER_hexadec
+000002f0: 696d 616c 5f73 7472 696e 6718 0000 0073  imal_string....s
+00000300: 1800 0000 0401 0801 0201 06fe 0205 0403  ................
+00000310: 0201 06ff 0c03 1801 1201 0403 7217 0000  ............r...
+00000320: 0029 0bda 075f 5f64 6f63 5f5f da41 7265  .)...__doc__.Are
+00000330: 6379 636c 696e 672e 6d69 7865 732e 4545  cycling.mixes.EE
+00000340: 435f 3434 385f 322e 6d6f 6475 6c61 746f  C_448_2.modulato
+00000350: 7273 2e62 7974 655f 7374 7269 6e67 2e66  rs.byte_string.f
+00000360: 726f 6d5f 6865 7861 6465 6369 6d61 6cda  rom_hexadecimal.
+00000370: 056d 6978 6573 da09 4545 435f 3434 385f  .mixes..EEC_448_
+00000380: 32da 0a6d 6f64 756c 6174 6f72 73da 0b62  2..modulators..b
+00000390: 7974 655f 7374 7269 6e67 da10 6672 6f6d  yte_string..from
+000003a0: 5f68 6578 6164 6563 696d 616c 7209 0000  _hexadecimalr...
+000003b0: 00da 1043 7279 7074 6f2e 5075 626c 6963  ...Crypto.Public
+000003c0: 4b65 7972 0200 0000 7217 0000 0072 1500  Keyr....r....r..
+000003d0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000003e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000003f0: 0a00 0000 0403 0207 2409 0c02 0c02       ........$.....
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/__pycache__/scan.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/__pycache__/scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 4703 0000  o........@@fG...
+00000000: 6f0d 0d0a 0000 0000 d153 5166 4503 0000  o........SQfE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6404 6405 8400 5a04 6403  d.l.Z.d.d...Z.d.
-00000050: 5300 2906 7aa3 0a09 696d 706f 7274 2072  S.).z...import r
-00000060: 6563 7963 6c69 6e67 2e6d 6f64 756c 6573  ecycling.modules
-00000070: 2e45 4543 5f34 3438 5f32 2e70 7562 6c69  .EEC_448_2.publi
-00000080: 635f 6b65 792e 7363 616e 2061 7320 7075  c_key.scan as pu
-00000090: 626c 6963 5f6b 6579 5f73 6361 6e0a 0970  blic_key_scan..p
-000000a0: 7562 6c69 635f 6b65 795f 7363 616e 2e73  ublic_key_scan.s
-000000b0: 7461 7274 2028 7075 626c 6963 5f6b 6579  tart (public_key
-000000c0: 5f70 6174 682c 2022 4a53 4f4e 2229 205b  _path, "JSON") [
-000000d0: 2270 7562 6c69 6320 6b65 7922 5d20 5b22  "public key"] ["
-000000e0: 4445 5220 6865 7861 6465 6369 6d61 6c20  DER hexadecimal 
-000000f0: 7374 7269 6e67 225d 0ae9 0000 0000 2901  string"]......).
-00000100: da03 4543 434e 6302 0000 0000 0000 0000  ..ECCNc.........
-00000110: 0000 0007 0000 0008 0000 0043 0000 0073  ...........C...s
-00000120: aa00 0000 7c01 6401 6b02 7223 7400 7c00  ....|.d.k.r#t.|.
-00000130: 6402 6403 8d02 8f11 7d02 7c02 a001 a100  d.d.....}.|.....
-00000140: 7d03 7402 a003 7c03 a101 5700 0200 6400  }.t...|...W...d.
-00000150: 0400 0400 8303 0100 5300 3100 731e 7701  ........S.1.s.w.
-00000160: 0100 0100 0100 5900 0100 7c01 6404 6b02  ......Y...|.d.k.
-00000170: 7251 7400 7c00 6405 6403 8d02 8f1c 7d02  rQt.|.d.d.....}.
-00000180: 7c02 a001 a100 7d04 7404 6a05 7c04 6406  |.....}.t.j.|.d.
-00000190: 6407 8d02 7d05 7c04 a006 a100 7d06 7c05  d...}.|.....}.|.
-000001a0: 7c04 7c06 6703 5700 0200 6400 0400 0400  |.|.g.W...d.....
-000001b0: 8303 0100 5300 3100 734c 7701 0100 0100  ....S.1.sLw.....
-000001c0: 0100 5900 0100 7407 6408 8301 8201 2909  ..Y...t.d.....).
-000001d0: 4eda 044a 534f 4eda 0172 2901 da04 6d6f  N..JSON..r)...mo
-000001e0: 6465 da03 4445 52da 0272 62da 0545 6434  de..DER..rb..Ed4
-000001f0: 3438 2901 da0a 6375 7276 655f 6e61 6d65  48)...curve_name
-00000200: da00 2908 da04 6f70 656e da04 7265 6164  ..)...open..read
-00000210: da04 6a73 6f6e da05 6c6f 6164 7372 0200  ..json..loadsr..
-00000220: 0000 da0a 696d 706f 7274 5f6b 6579 da03  ....import_key..
-00000230: 6865 78da 0945 7863 6570 7469 6f6e 2907  hex..Exception).
-00000240: da04 7061 7468 da06 666f 726d 6174 da04  ..path..format..
-00000250: 6669 6c65 da0b 4a53 4f4e 5f73 7472 696e  file..JSON_strin
-00000260: 67da 1070 7562 6c69 635f 6b65 795f 6279  g..public_key_by
-00000270: 7465 73da 0a70 7562 6c69 635f 6b65 79da  tes..public_key.
-00000280: 1170 7562 6c69 635f 6b65 795f 7374 7269  .public_key_stri
-00000290: 6e67 a900 7219 0000 00fa 452f 6861 6269  ng..r.....E/habi
-000002a0: 7461 742f 7665 6e75 6573 2f73 7461 6765  tat/venues/stage
-000002b0: 732f 7265 6379 636c 696e 672f 6d6f 6475  s/recycling/modu
-000002c0: 6c65 732f 4545 435f 3434 385f 322f 7075  les/EEC_448_2/pu
-000002d0: 626c 6963 5f6b 6579 2f73 6361 6e2e 7079  blic_key/scan.py
-000002e0: da05 7374 6172 7412 0000 0073 2600 0000  ..start....s&...
-000002f0: 0801 0e01 0801 0802 20fd 0805 0e01 0801  ........ .......
-00000300: 0402 0201 0201 06fe 0805 0203 0201 0201  ................
-00000310: 02fd 20f6 0810 721b 0000 0029 05da 075f  .. ...r....)..._
-00000320: 5f64 6f63 5f5f da10 4372 7970 746f 2e50  _doc__..Crypto.P
-00000330: 7562 6c69 634b 6579 7202 0000 0072 0d00  ublicKeyr....r..
-00000340: 0000 721b 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00000350: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
-00000360: 6475 6c65 3e01 0000 0073 0800 0000 0403  dule>....s......
-00000370: 0c0a 0802 0c02                           ......
+00000050: 5300 2906 7aa1 0a09 696d 706f 7274 2072  S.).z...import r
+00000060: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00000070: 4543 5f34 3438 5f32 2e70 7562 6c69 635f  EC_448_2.public_
+00000080: 6b65 792e 7363 616e 2061 7320 7075 626c  key.scan as publ
+00000090: 6963 5f6b 6579 5f73 6361 6e0a 0970 7562  ic_key_scan..pub
+000000a0: 6c69 635f 6b65 795f 7363 616e 2e73 7461  lic_key_scan.sta
+000000b0: 7274 2028 7075 626c 6963 5f6b 6579 5f70  rt (public_key_p
+000000c0: 6174 682c 2022 4a53 4f4e 2229 205b 2270  ath, "JSON") ["p
+000000d0: 7562 6c69 6320 6b65 7922 5d20 5b22 4445  ublic key"] ["DE
+000000e0: 5220 6865 7861 6465 6369 6d61 6c20 7374  R hexadecimal st
+000000f0: 7269 6e67 225d 0ae9 0000 0000 2901 da03  ring"]......)...
+00000100: 4543 434e 6302 0000 0000 0000 0000 0000  ECCNc...........
+00000110: 0007 0000 0008 0000 0043 0000 0073 aa00  .........C...s..
+00000120: 0000 7c01 6401 6b02 7223 7400 7c00 6402  ..|.d.k.r#t.|.d.
+00000130: 6403 8d02 8f11 7d02 7c02 a001 a100 7d03  d.....}.|.....}.
+00000140: 7402 a003 7c03 a101 5700 0200 6400 0400  t...|...W...d...
+00000150: 0400 8303 0100 5300 3100 731e 7701 0100  ......S.1.s.w...
+00000160: 0100 0100 5900 0100 7c01 6404 6b02 7251  ....Y...|.d.k.rQ
+00000170: 7400 7c00 6405 6403 8d02 8f1c 7d02 7c02  t.|.d.d.....}.|.
+00000180: a001 a100 7d04 7404 6a05 7c04 6406 6407  ....}.t.j.|.d.d.
+00000190: 8d02 7d05 7c04 a006 a100 7d06 7c05 7c04  ..}.|.....}.|.|.
+000001a0: 7c06 6703 5700 0200 6400 0400 0400 8303  |.g.W...d.......
+000001b0: 0100 5300 3100 734c 7701 0100 0100 0100  ..S.1.sLw.......
+000001c0: 5900 0100 7407 6408 8301 8201 2909 4eda  Y...t.d.....).N.
+000001d0: 044a 534f 4eda 0172 2901 da04 6d6f 6465  .JSON..r)...mode
+000001e0: da03 4445 52da 0272 62da 0545 6434 3438  ..DER..rb..Ed448
+000001f0: 2901 da0a 6375 7276 655f 6e61 6d65 da00  )...curve_name..
+00000200: 2908 da04 6f70 656e da04 7265 6164 da04  )...open..read..
+00000210: 6a73 6f6e da05 6c6f 6164 7372 0200 0000  json..loadsr....
+00000220: da0a 696d 706f 7274 5f6b 6579 da03 6865  ..import_key..he
+00000230: 78da 0945 7863 6570 7469 6f6e 2907 da04  x..Exception)...
+00000240: 7061 7468 da06 666f 726d 6174 da04 6669  path..format..fi
+00000250: 6c65 da0b 4a53 4f4e 5f73 7472 696e 67da  le..JSON_string.
+00000260: 1070 7562 6c69 635f 6b65 795f 6279 7465  .public_key_byte
+00000270: 73da 0a70 7562 6c69 635f 6b65 79da 1170  s..public_key..p
+00000280: 7562 6c69 635f 6b65 795f 7374 7269 6e67  ublic_key_string
+00000290: a900 7219 0000 00fa 432f 6861 6269 7461  ..r.....C/habita
+000002a0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
+000002b0: 7265 6379 636c 696e 672f 6d69 7865 732f  recycling/mixes/
+000002c0: 4545 435f 3434 385f 322f 7075 626c 6963  EEC_448_2/public
+000002d0: 5f6b 6579 2f73 6361 6e2e 7079 da05 7374  _key/scan.py..st
+000002e0: 6172 7412 0000 0073 2600 0000 0801 0e01  art....s&.......
+000002f0: 0801 0802 20fd 0805 0e01 0801 0402 0201  .... ...........
+00000300: 0201 06fe 0805 0203 0201 0201 02fd 20f6  .............. .
+00000310: 0810 721b 0000 0029 05da 075f 5f64 6f63  ..r....)...__doc
+00000320: 5f5f da10 4372 7970 746f 2e50 7562 6c69  __..Crypto.Publi
+00000330: 634b 6579 7202 0000 0072 0d00 0000 721b  cKeyr....r....r.
+00000340: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
+00000350: 0000 721a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000360: 3e01 0000 0073 0800 0000 0403 0c0a 0802  >....s..........
+00000370: 0c02                                     ..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/creator.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/rhythms/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,50 @@
 
+
 '''
-	#
-	#	write public key to path
-	#
-	import recycling.modules.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
-	public_key = EEC_448_2_public_key_creator.create (
-		private_key_instance
+	import recycling.mixes.EEC_448_2.rhythms as EEC_448_2_rhythm_creator
+	rhythms = EEC_448_2_rhythm_creator.create (
+		seed = ""
 	)
-	public_key_instance = public_key ["instance"]
-	public_key_DER_hexadecimal_string = public_key ["DER hexadecimal string"]
-		
 '''
 
 '''
-	format:
-		DER
-		PEM
+	{
+		"showy": {
+			"hexadecimal string": public_key_DER_hexadecimal_string,
+		},
+		"intimate": {
+			"hexadecimal string": intimate_rhythm_DER_hexadecimal_string
+		}
+	}
 '''
-import os
-
-from Crypto.PublicKey.ECC import EccKey
-from Crypto.PublicKey import ECC
-
-import recycling.modules.EEC_448_2.private_key.scan as private_scan
 
-
-def create_DER_hexadecimal_string (public_key_DER_byte_string):
-	public_key_DER_hexadecimal_string = public_key_DER_byte_string.hex ()
-	assert (len (public_key_DER_hexadecimal_string) == 138)
-	assert (
-		bytes.fromhex (public_key_DER_hexadecimal_string) == 
-		public_key_DER_byte_string
-	)
-	
-	return public_key_DER_hexadecimal_string
+import recycling.mixes.EEC_448_2.intimate_rhythm.creator as EEC_448_2_intimate_rhythm_creator
+import recycling.mixes.EEC_448_2.public_key.creator as EEC_448_2_public_key_creator
 
 def create (
-	private_key_instance = None
-):	
-	public_key_instance = private_key_instance.public_key ()
-	public_key_DER_byte_string = public_key_instance.export_key (
-		format = "DER"
-	)
-	public_key_PEM_string = public_key_instance.export_key (
-		format = "PEM"
-	)
+	seed = ""
+):
+	#
+	#	create intimate rhythm
+	#
+	intimate_rhythm = EEC_448_2_intimate_rhythm_creator.create (seed)
+	intimate_rhythm_instance = intimate_rhythm ["instance"]
+	intimate_rhythm_DER_hexadecimal_string = intimate_rhythm ["DER hexadecimal string"]
 	
-	public_key_DER_hexadecimal_string = create_DER_hexadecimal_string (
-		public_key_DER_byte_string
+	#
+	#	create showy rhythm
+	#
+	public_key = EEC_448_2_public_key_creator.create (
+		intimate_rhythm_instance
 	)
-
-	return {		
-		"instance": public_key_instance, 
-		
-		"DER byte string": public_key_DER_byte_string,
-		"DER hexadecimal string": public_key_DER_hexadecimal_string,
-		
-		"PEM string": public_key_PEM_string
-	}
+	public_key_instance = public_key ["instance"]
+	public_key_DER_hexadecimal_string = public_key ["DER hexadecimal string"]
+	
+	return {
+		"showy": {
+			"hexadecimal string": public_key_DER_hexadecimal_string,
+		},
+		"intimate": {
+			"hexadecimal string": intimate_rhythm_DER_hexadecimal_string
+		}
+	}
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/etch.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/etch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 
 
 '''
-	import recycling.modules.EEC_448_2.public_key.write as write_EEC_448_2_public_key
+	import recycling.mixes.EEC_448_2.public_key.write as write_EEC_448_2_public_key
 	write_EEC_448_2_public_key.start (
 		path,
 		public_key_string,
 		format
 	)
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/instance.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 
 
 '''
-	import recycling.modules.EEC_448_2.public_key.instance as instantiate_public_key
+	import recycling.mixes.EEC_448_2.public_key.instance as instantiate_public_key
 	public_key_instance = instantiate_public_key.from_DER_hexadecimal_string (
 		DER_hexadecimal_string
 	)
 '''
 
 '''
 	DER_key_string = private_key_instance.export_key (
 		format = "DER"
 	)	
 	PEM_key_string = private_key_instance.export_key (
 		format = "PEM"
 	)
 '''
 
-import recycling.modules.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
+import recycling.mixes.EEC_448_2.modulators.byte_string.from_hexadecimal as hexadecimal_to_byte_string
 
 from Crypto.PublicKey import ECC
 
 def from_DER_hexadecimal_string (DER_hexadecimal_string):	
 	instance = ECC.import_key (
 		hexadecimal_to_byte_string.modulate (DER_hexadecimal_string),
 		curve_name = "Ed448"
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/public_key/scan.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/public_key/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 '''
-	import recycling.modules.EEC_448_2.public_key.scan as public_key_scan
+	import recycling.mixes.EEC_448_2.public_key.scan as public_key_scan
 	public_key_scan.start (public_key_path, "JSON") ["public key"] ["DER hexadecimal string"]
 '''
 
 
 #
 #	https://pycryptodome.readthedocs.io/en/latest/src/public_key/ecc.html#Crypto.PublicKey.ECC.import_key
 #
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/sign/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/sign/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 				"address": "3043300506032b6571033a00e26960a83c45c0bb86e356cd727473e96682e76c6dd01c991a6ea0a394ecca27b467554d73e2a22b05425c1926a7a92befda5c1937d6876f00"
 			},
 			"amount": "40324789324873"
 		}
 	}, indent = 4)		
 	unsigned_bytes = unicode_string.encode ("utf-8")
 
-	import recycling.modules.EEC_448_2.sign as EEC_448_2_sign
+	import recycling.mixes.EEC_448_2.sign as EEC_448_2_sign
 	signed = EEC_448_2_sign.start (
 		private_key_instance,
 		unsigned_bytes = unsigned_bytes
 	)
 	
 	signed_bytes_hexadecimal = signed ["signed bytes hexadecimal"]
 '''
 
 from Crypto.PublicKey import ECC
 from Crypto.Signature import eddsa
 
-import recycling.modules.EEC_448_2.modulators.hexadecimal.from_byte_string as byte_string_to_hex
+import recycling.mixes.EEC_448_2.modulators.hexadecimal.from_byte_string as byte_string_to_hex
 
 def start (
 	private_key_instance = None,
 	unsigned_bytes = None
 ):
 	signer = eddsa.new (private_key_instance, 'rfc8032')
 	signed_bytes = signer.sign (unsigned_bytes)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/sign/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/sign/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1054 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 1e04 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 1a04 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 0200 0100 6d07 0200 0100 6d08 0200  m.....m.....m...
 00000060: 0100 6d09 0200 0100 6d0a 5a0b 0100 0904  ..m.....m.Z.....
 00000070: 0904 6407 6405 6406 8401 5a0c 6404 5300  ..d.d.d...Z.d.S.
-00000080: 2908 614b 0200 000a 0975 6e69 636f 6465  ).aK.....unicode
+00000080: 2908 6149 0200 000a 0975 6e69 636f 6465  ).aI.....unicode
 00000090: 5f73 7472 696e 6720 3d20 6a73 6f6e 2e64  _string = json.d
 000000a0: 756d 7073 2028 7b0a 0909 226d 6f76 6522  umps ({..."move"
 000000b0: 3a20 2273 656e 6422 2c0a 0909 2266 6965  : "send",..."fie
 000000c0: 6c64 7322 3a20 7b0a 0909 0922 746f 223a  lds": {...."to":
 000000d0: 207b 0a09 0909 0922 666f 726d 6174 223a   {....."format":
 000000e0: 2022 4545 435f 3434 385f 3122 2c0a 0909   "EEC_448_1",...
 000000f0: 0909 2261 6464 7265 7373 223a 2022 3330  .."address": "30
@@ -26,59 +26,59 @@
 00000190: 0909 0922 616d 6f75 6e74 223a 2022 3430  ..."amount": "40
 000001a0: 3332 3437 3839 3332 3438 3733 220a 0909  324789324873"...
 000001b0: 7d0a 097d 2c20 696e 6465 6e74 203d 2034  }..}, indent = 4
 000001c0: 2909 090a 0975 6e73 6967 6e65 645f 6279  )....unsigned_by
 000001d0: 7465 7320 3d20 756e 6963 6f64 655f 7374  tes = unicode_st
 000001e0: 7269 6e67 2e65 6e63 6f64 6520 2822 7574  ring.encode ("ut
 000001f0: 662d 3822 290a 0a09 696d 706f 7274 2072  f-8")...import r
-00000200: 6563 7963 6c69 6e67 2e6d 6f64 756c 6573  ecycling.modules
-00000210: 2e45 4543 5f34 3438 5f32 2e73 6967 6e20  .EEC_448_2.sign 
-00000220: 6173 2045 4543 5f34 3438 5f32 5f73 6967  as EEC_448_2_sig
-00000230: 6e0a 0973 6967 6e65 6420 3d20 4545 435f  n..signed = EEC_
-00000240: 3434 385f 325f 7369 676e 2e73 7461 7274  448_2_sign.start
-00000250: 2028 0a09 0970 7269 7661 7465 5f6b 6579   (...private_key
-00000260: 5f69 6e73 7461 6e63 652c 0a09 0975 6e73  _instance,...uns
-00000270: 6967 6e65 645f 6279 7465 7320 3d20 756e  igned_bytes = un
-00000280: 7369 676e 6564 5f62 7974 6573 0a09 290a  signed_bytes..).
-00000290: 090a 0973 6967 6e65 645f 6279 7465 735f  ...signed_bytes_
-000002a0: 6865 7861 6465 6369 6d61 6c20 3d20 7369  hexadecimal = si
-000002b0: 676e 6564 205b 2273 6967 6e65 6420 6279  gned ["signed by
-000002c0: 7465 7320 6865 7861 6465 6369 6d61 6c22  tes hexadecimal"
-000002d0: 5d0a e900 0000 0029 01da 0345 4343 2901  ]......)...ECC).
-000002e0: da05 6564 6473 614e 6302 0000 0000 0000  ..eddsaNc.......
-000002f0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
-00000300: 0073 2600 0000 7400 a001 7c00 6401 a102  .s&...t...|.d...
-00000310: 7d02 7c02 a002 7c01 a101 7d03 7c03 7403  }.|...|...}.|.t.
-00000320: a004 7c03 a101 6402 9c02 5300 2903 4eda  ..|...d...S.).N.
-00000330: 0772 6663 3830 3332 2902 7a0c 7369 676e  .rfc8032).z.sign
-00000340: 6564 2062 7974 6573 7a18 7369 676e 6564  ed bytesz.signed
-00000350: 2062 7974 6573 2068 6578 6164 6563 696d   bytes hexadecim
-00000360: 616c 2905 7203 0000 00da 036e 6577 da04  al).r......new..
-00000370: 7369 676e da12 6279 7465 5f73 7472 696e  sign..byte_strin
-00000380: 675f 746f 5f68 6578 da08 6d6f 6475 6c61  g_to_hex..modula
-00000390: 7465 2904 da14 7072 6976 6174 655f 6b65  te)...private_ke
-000003a0: 795f 696e 7374 616e 6365 da0e 756e 7369  y_instance..unsi
-000003b0: 676e 6564 5f62 7974 6573 da06 7369 676e  gned_bytes..sign
-000003c0: 6572 da0c 7369 676e 6564 5f62 7974 6573  er..signed_bytes
-000003d0: a900 720d 0000 00fa 432f 6861 6269 7461  ..r.....C/habita
-000003e0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-000003f0: 7265 6379 636c 696e 672f 6d6f 6475 6c65  recycling/module
-00000400: 732f 4545 435f 3434 385f 322f 7369 676e  s/EEC_448_2/sign
-00000410: 2f5f 5f69 6e69 745f 5f2e 7079 da05 7374  /__init__.py..st
-00000420: 6172 741e 0000 0073 0a00 0000 0c04 0a01  art....s........
-00000430: 0203 0801 06fe 720f 0000 0029 024e 4e29  ......r....).NN)
-00000440: 0dda 075f 5f64 6f63 5f5f da10 4372 7970  ...__doc__..Cryp
-00000450: 746f 2e50 7562 6c69 634b 6579 7202 0000  to.PublicKeyr...
-00000460: 00da 1043 7279 7074 6f2e 5369 676e 6174  ...Crypto.Signat
-00000470: 7572 6572 0300 0000 da43 7265 6379 636c  urer.....Crecycl
-00000480: 696e 672e 6d6f 6475 6c65 732e 4545 435f  ing.modules.EEC_
-00000490: 3434 385f 322e 6d6f 6475 6c61 746f 7273  448_2.modulators
-000004a0: 2e68 6578 6164 6563 696d 616c 2e66 726f  .hexadecimal.fro
-000004b0: 6d5f 6279 7465 5f73 7472 696e 67da 076d  m_byte_string..m
-000004c0: 6f64 756c 6573 da09 4545 435f 3434 385f  odules..EEC_448_
-000004d0: 32da 0a6d 6f64 756c 6174 6f72 73da 0b68  2..modulators..h
-000004e0: 6578 6164 6563 696d 616c da10 6672 6f6d  exadecimal..from
-000004f0: 5f62 7974 655f 7374 7269 6e67 7207 0000  _byte_stringr...
-00000500: 0072 0f00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000510: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
-00000520: 756c 653e 0100 0000 730e 0000 0004 020c  ule>....s.......
-00000530: 160c 0124 0202 0302 010e fe              ...$.......
+00000200: 6563 7963 6c69 6e67 2e6d 6978 6573 2e45  ecycling.mixes.E
+00000210: 4543 5f34 3438 5f32 2e73 6967 6e20 6173  EC_448_2.sign as
+00000220: 2045 4543 5f34 3438 5f32 5f73 6967 6e0a   EEC_448_2_sign.
+00000230: 0973 6967 6e65 6420 3d20 4545 435f 3434  .signed = EEC_44
+00000240: 385f 325f 7369 676e 2e73 7461 7274 2028  8_2_sign.start (
+00000250: 0a09 0970 7269 7661 7465 5f6b 6579 5f69  ...private_key_i
+00000260: 6e73 7461 6e63 652c 0a09 0975 6e73 6967  nstance,...unsig
+00000270: 6e65 645f 6279 7465 7320 3d20 756e 7369  ned_bytes = unsi
+00000280: 676e 6564 5f62 7974 6573 0a09 290a 090a  gned_bytes..)...
+00000290: 0973 6967 6e65 645f 6279 7465 735f 6865  .signed_bytes_he
+000002a0: 7861 6465 6369 6d61 6c20 3d20 7369 676e  xadecimal = sign
+000002b0: 6564 205b 2273 6967 6e65 6420 6279 7465  ed ["signed byte
+000002c0: 7320 6865 7861 6465 6369 6d61 6c22 5d0a  s hexadecimal"].
+000002d0: e900 0000 0029 01da 0345 4343 2901 da05  .....)...ECC)...
+000002e0: 6564 6473 614e 6302 0000 0000 0000 0000  eddsaNc.........
+000002f0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00000300: 2600 0000 7400 a001 7c00 6401 a102 7d02  &...t...|.d...}.
+00000310: 7c02 a002 7c01 a101 7d03 7c03 7403 a004  |...|...}.|.t...
+00000320: 7c03 a101 6402 9c02 5300 2903 4eda 0772  |...d...S.).N..r
+00000330: 6663 3830 3332 2902 7a0c 7369 676e 6564  fc8032).z.signed
+00000340: 2062 7974 6573 7a18 7369 676e 6564 2062   bytesz.signed b
+00000350: 7974 6573 2068 6578 6164 6563 696d 616c  ytes hexadecimal
+00000360: 2905 7203 0000 00da 036e 6577 da04 7369  ).r......new..si
+00000370: 676e da12 6279 7465 5f73 7472 696e 675f  gn..byte_string_
+00000380: 746f 5f68 6578 da08 6d6f 6475 6c61 7465  to_hex..modulate
+00000390: 2904 da14 7072 6976 6174 655f 6b65 795f  )...private_key_
+000003a0: 696e 7374 616e 6365 da0e 756e 7369 676e  instance..unsign
+000003b0: 6564 5f62 7974 6573 da06 7369 676e 6572  ed_bytes..signer
+000003c0: da0c 7369 676e 6564 5f62 7974 6573 a900  ..signed_bytes..
+000003d0: 720d 0000 00fa 412f 6861 6269 7461 742f  r.....A/habitat/
+000003e0: 7665 6e75 6573 2f73 7461 6765 732f 7265  venues/stages/re
+000003f0: 6379 636c 696e 672f 6d69 7865 732f 4545  cycling/mixes/EE
+00000400: 435f 3434 385f 322f 7369 676e 2f5f 5f69  C_448_2/sign/__i
+00000410: 6e69 745f 5f2e 7079 da05 7374 6172 741e  nit__.py..start.
+00000420: 0000 0073 0a00 0000 0c04 0a01 0203 0801  ...s............
+00000430: 06fe 720f 0000 0029 024e 4e29 0dda 075f  ..r....).NN)..._
+00000440: 5f64 6f63 5f5f da10 4372 7970 746f 2e50  _doc__..Crypto.P
+00000450: 7562 6c69 634b 6579 7202 0000 00da 1043  ublicKeyr......C
+00000460: 7279 7074 6f2e 5369 676e 6174 7572 6572  rypto.Signaturer
+00000470: 0300 0000 da41 7265 6379 636c 696e 672e  .....Arecycling.
+00000480: 6d69 7865 732e 4545 435f 3434 385f 322e  mixes.EEC_448_2.
+00000490: 6d6f 6475 6c61 746f 7273 2e68 6578 6164  modulators.hexad
+000004a0: 6563 696d 616c 2e66 726f 6d5f 6279 7465  ecimal.from_byte
+000004b0: 5f73 7472 696e 67da 056d 6978 6573 da09  _string..mixes..
+000004c0: 4545 435f 3434 385f 32da 0a6d 6f64 756c  EEC_448_2..modul
+000004d0: 6174 6f72 73da 0b68 6578 6164 6563 696d  ators..hexadecim
+000004e0: 616c da10 6672 6f6d 5f62 7974 655f 7374  al..from_byte_st
+000004f0: 7269 6e67 7207 0000 0072 0f00 0000 720d  ringr....r....r.
+00000500: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000510: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000520: 730e 0000 0004 020c 160c 0124 0202 0302  s..........$....
+00000530: 010e fe                                  ...
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/tutorial.s.HTML` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/tutorial.S.HTML`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,18 @@
 import recycling.modules.EEC_448_2.public_key.etch as etch_EEC_448_2_public_key
 		
 import pathlib
 from os.path import dirname, join, normpath
 import os
 import json	
 	
-seed = "4986888B11358BF3D541B41EEA5DAECE1C6EFF64130A45FC8B9CA48F3E0E02463C99C5AEDC8A847686D669B7D547C18FE448FC5111CA88F4E8"	
+seed = "".join ([
+	"4986888B11358BF3D541B41EEA5DAECE1C6EFF64130A45FC8B9CA48F3",
+	"E0E02463C99C5AEDC8A847686D669B7D547C18FE448FC5111CA88F4E8"	
+])
 	
 private_key_path = normpath (
 	join (pathlib.Path (__file__).parent.resolve (), "EEC_448_2_private_key")
 ) + ".JSON"
 
 public_key_path = normpath (
 	join (pathlib.Path (__file__).parent.resolve (), "EEC_448_2_public_key")
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/verify/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/verify/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 
 '''
 	{ verify, approve, validate, certify, vouch }
 '''
 
 '''
-	import recycling.modules.EEC_448_2.public_key.instance as instantiate_public_key
+	import recycling.mixes.EEC_448_2.public_key.instance as instantiate_public_key
 	public_key_instance = instantiate_public_key.from_DER_hexadecimal_string (
 		DER_hexadecimal_string
 	)
 
-	import recycling.modules.EEC_448_2.verify as verify
+	import recycling.mixes.EEC_448_2.verify as verify
 	verified = verify.start (
 		public_key_instance,
 		
 		signed_bytes = signed_bytes,
 		unsigned_bytes = unsigned_bytes
 	)
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/EEC_448_2/verify/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/EEC_448_2/verify/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 860 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 5c03 0000  o........@@f\...
+00000000: 6f0d 0d0a 0000 0000 d153 5166 5803 0000  o........SQfX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 0100 0904 0904  d.d.l.m.Z.......
 00000050: 0904 6407 6405 6406 8401 5a05 6404 5300  ..d.d.d...Z.d.S.
 00000060: 2908 7a30 0a09 7b20 7665 7269 6679 2c20  ).z0..{ verify, 
 00000070: 6170 7072 6f76 652c 2076 616c 6964 6174  approve, validat
@@ -20,23 +20,22 @@
 00000130: 7469 6f6e 3ada 026e 6f29 0572 0200 0000  tion:..no).r....
 00000140: da03 6e65 77da 0676 6572 6966 79da 0945  ..new..verify..E
 00000150: 7863 6570 7469 6f6e da05 7072 696e 7429  xception..print)
 00000160: 05da 1370 7562 6c69 635f 6b65 795f 696e  ...public_key_in
 00000170: 7374 616e 6365 da0e 756e 7369 676e 6564  stance..unsigned
 00000180: 5f62 7974 6573 da0c 7369 676e 6564 5f62  _bytes..signed_b
 00000190: 7974 6573 da08 7665 7269 6669 6572 da01  ytes..verifier..
-000001a0: 45a9 0072 1000 0000 fa45 2f68 6162 6974  E..r.....E/habit
+000001a0: 45a9 0072 1000 0000 fa43 2f68 6162 6974  E..r.....C/habit
 000001b0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-000001c0: 2f72 6563 7963 6c69 6e67 2f6d 6f64 756c  /recycling/modul
-000001d0: 6573 2f45 4543 5f34 3438 5f32 2f76 6572  es/EEC_448_2/ver
-000001e0: 6966 792f 5f5f 696e 6974 5f5f 2e70 79da  ify/__init__.py.
-000001f0: 0573 7461 7274 1900 0000 7314 0000 000c  .start....s.....
-00000200: 0602 020c 0106 010e 020a 010a 0604 0208  ................
-00000210: 8002 f772 1200 0000 2903 4e4e 4e29 06da  ...r....).NNN)..
-00000220: 075f 5f64 6f63 5f5f da10 4372 7970 746f  .__doc__..Crypto
-00000230: 2e53 6967 6e61 7475 7265 7202 0000 00da  .Signaturer.....
-00000240: 1043 7279 7074 6f2e 5075 626c 6963 4b65  .Crypto.PublicKe
-00000250: 7972 0300 0000 7212 0000 0072 1000 0000  yr....r....r....
-00000260: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000270: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
-00000280: 0000 0402 0204 0c0f 0c01 0203 0202 0201  ................
-00000290: 0efc                                     ..
+000001c0: 2f72 6563 7963 6c69 6e67 2f6d 6978 6573  /recycling/mixes
+000001d0: 2f45 4543 5f34 3438 5f32 2f76 6572 6966  /EEC_448_2/verif
+000001e0: 792f 5f5f 696e 6974 5f5f 2e70 79da 0573  y/__init__.py..s
+000001f0: 7461 7274 1900 0000 7314 0000 000c 0602  tart....s.......
+00000200: 020c 0106 010e 020a 010a 0604 0208 8002  ................
+00000210: f772 1200 0000 2903 4e4e 4e29 06da 075f  .r....).NNN)..._
+00000220: 5f64 6f63 5f5f da10 4372 7970 746f 2e53  _doc__..Crypto.S
+00000230: 6967 6e61 7475 7265 7202 0000 00da 1043  ignaturer......C
+00000240: 7279 7074 6f2e 5075 626c 6963 4b65 7972  rypto.PublicKeyr
+00000250: 0300 0000 7212 0000 0072 1000 0000 7210  ....r....r....r.
+00000260: 0000 0072 1000 0000 7211 0000 00da 083c  ...r....r......<
+00000270: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
+00000280: 0402 0204 0c0f 0c01 0203 0202 0201 0efc  ................
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/QR/__init__.py` & `recycling-1.1.0/venues/stages/recycling/mixes/QR/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/__pycache__/build.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/__pycache__/build.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1262 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 ee04 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 ec04 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a02  Z.....d.d.l.m.Z.
 00000040: 0100 6401 6403 6c03 5a04 6401 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a05 6401 6403 6c04 5a04 0904 0905 6408  Z.d.d.l.Z.....d.
-00000060: 6406 6407 8401 5a06 6403 5300 2909 615d  d.d...Z.d.S.).a]
+00000060: 6406 6407 8401 5a06 6403 5300 2909 615b  d.d...Z.d.S.).a[
 00000070: 0200 000a 0923 0a09 2309 7772 6974 6520  .....#..#.write 
 00000080: 7072 6976 6174 6520 6b65 7920 746f 2070  private key to p
 00000090: 6174 680a 0923 0a09 0a09 0a09 230a 0923  ath..#......#..#
 000000a0: 0941 4243 4445 4647 4849 4a4b 4c4d 0a09  .ABCDEFGHIJKLM..
 000000b0: 2309 4e4f 5051 5253 5455 5657 5859 5a0a  #.NOPQRSTUVWXYZ.
 000000c0: 0923 0a09 2309 4142 4344 4546 4748 494a  .#..#.ABCDEFGHIJ
 000000d0: 4b4c 4d20 4e4f 5020 2d3e 2075 7369 6e67  KLM NOP -> using
@@ -24,45 +24,45 @@
 00000170: 6134 3866 3365 3065 3032 3436 3363 3939  a48f3e0e02463c99
 00000180: 6335 6165 6463 3861 3834 3736 3836 6436  c5aedc8a847686d6
 00000190: 3639 6237 6435 3437 6331 3866 6534 3438  69b7d547c18fe448
 000001a0: 6663 3531 3131 6361 3838 6634 6538 220a  fc5111ca88f4e8".
 000001b0: 0966 6f72 6d61 7420 3d20 2250 454d 220a  .format = "PEM".
 000001c0: 0970 6174 6820 3d20 2222 0a09 0a09 696d  .path = ""....im
 000001d0: 706f 7274 2072 6563 7963 6c69 6e67 2e6d  port recycling.m
-000001e0: 6f64 756c 6573 2e45 4543 5f34 3438 5f31  odules.EEC_448_1
-000001f0: 2e70 7269 7661 7465 5f6b 6579 2e63 7265  .private_key.cre
-00000200: 6174 6f72 2061 7320 4545 435f 3434 385f  ator as EEC_448_
-00000210: 315f 7072 6976 6174 655f 6b65 795f 6372  1_private_key_cr
-00000220: 6561 746f 720a 0970 7269 7661 7465 5f6b  eator..private_k
-00000230: 6579 203d 2045 4543 5f34 3438 5f31 5f70  ey = EEC_448_1_p
-00000240: 7269 7661 7465 5f6b 6579 5f63 7265 6174  rivate_key_creat
-00000250: 6f72 2e63 7265 6174 6520 2873 6565 642c  or.create (seed,
-00000260: 2066 6f72 6d61 742c 2070 6174 6829 0a09   format, path)..
-00000270: 7072 6976 6174 655f 6b65 795f 696e 7374  private_key_inst
-00000280: 616e 6365 203d 2070 7269 7661 7465 5f6b  ance = private_k
-00000290: 6579 205b 2269 6e73 7461 6e63 6522 5d0a  ey ["instance"].
-000002a0: 0970 7269 7661 7465 5f6b 6579 5f73 7472  .private_key_str
-000002b0: 696e 6720 3d20 7072 6976 6174 655f 6b65  ing = private_ke
-000002c0: 7920 5b22 7374 7269 6e67 225d 0a09 090a  y ["string"]....
-000002d0: e900 0000 0029 01da 0645 6363 4b65 794e  .....)...EccKeyN
-000002e0: da00 da05 4564 3434 3863 0400 0000 0000  ....Ed448c......
-000002f0: 0000 0000 0000 0400 0000 0100 0000 4300  ..............C.
-00000300: 0000 730a 0000 0074 006a 017d 0364 0053  ..s....t.j.}.d.S
-00000310: 0029 014e 2902 da05 6563 6473 61da 0953  .).N)...ecdsa..S
-00000320: 4543 5032 3536 6b31 2904 da04 7365 6564  ECP256k1)...seed
-00000330: da06 666f 726d 6174 da04 7061 7468 da05  ..format..path..
-00000340: 6375 7276 65a9 0072 0b00 0000 fa50 2f68  curve..r.....P/h
-00000350: 6162 6974 6174 2f76 656e 7565 732f 7374  abitat/venues/st
-00000360: 6167 6573 2f72 6563 7963 6c69 6e67 2f6d  ages/recycling/m
-00000370: 6f64 756c 6573 2f65 6c6c 6970 7469 632f  odules/elliptic/
-00000380: 5345 4350 3235 364b 312f 7072 6976 6174  SECP256K1/privat
-00000390: 655f 6b65 792f 6275 696c 642e 7079 da06  e_key/build.py..
-000003a0: 6372 6561 7465 3400 0000 7302 0000 000a  create4...s.....
-000003b0: 0772 0d00 0000 2902 7203 0000 0072 0400  .r....).r....r..
-000003c0: 0000 2907 da07 5f5f 646f 635f 5fda 1443  ..)...__doc__..C
-000003d0: 7279 7074 6f2e 5075 626c 6963 4b65 792e  rypto.PublicKey.
-000003e0: 4543 4372 0200 0000 da07 6f73 2e70 6174  ECCr......os.pat
-000003f0: 68da 026f 7372 0500 0000 720d 0000 0072  h..osr....r....r
-00000400: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000410: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000420: 0073 1400 0000 0404 021a 020b 0c03 0801  .s..............
-00000430: 0803 0801 0206 0201 0efb                 ..........
+000001e0: 6978 6573 2e45 4543 5f34 3438 5f31 2e70  ixes.EEC_448_1.p
+000001f0: 7269 7661 7465 5f6b 6579 2e63 7265 6174  rivate_key.creat
+00000200: 6f72 2061 7320 4545 435f 3434 385f 315f  or as EEC_448_1_
+00000210: 7072 6976 6174 655f 6b65 795f 6372 6561  private_key_crea
+00000220: 746f 720a 0970 7269 7661 7465 5f6b 6579  tor..private_key
+00000230: 203d 2045 4543 5f34 3438 5f31 5f70 7269   = EEC_448_1_pri
+00000240: 7661 7465 5f6b 6579 5f63 7265 6174 6f72  vate_key_creator
+00000250: 2e63 7265 6174 6520 2873 6565 642c 2066  .create (seed, f
+00000260: 6f72 6d61 742c 2070 6174 6829 0a09 7072  ormat, path)..pr
+00000270: 6976 6174 655f 6b65 795f 696e 7374 616e  ivate_key_instan
+00000280: 6365 203d 2070 7269 7661 7465 5f6b 6579  ce = private_key
+00000290: 205b 2269 6e73 7461 6e63 6522 5d0a 0970   ["instance"]..p
+000002a0: 7269 7661 7465 5f6b 6579 5f73 7472 696e  rivate_key_strin
+000002b0: 6720 3d20 7072 6976 6174 655f 6b65 7920  g = private_key 
+000002c0: 5b22 7374 7269 6e67 225d 0a09 090a e900  ["string"]......
+000002d0: 0000 0029 01da 0645 6363 4b65 794e da00  ...)...EccKeyN..
+000002e0: da05 4564 3434 3863 0400 0000 0000 0000  ..Ed448c........
+000002f0: 0000 0000 0400 0000 0100 0000 4300 0000  ............C...
+00000300: 730a 0000 0074 006a 017d 0364 0053 0029  s....t.j.}.d.S.)
+00000310: 014e 2902 da05 6563 6473 61da 0953 4543  .N)...ecdsa..SEC
+00000320: 5032 3536 6b31 2904 da04 7365 6564 da06  P256k1)...seed..
+00000330: 666f 726d 6174 da04 7061 7468 da05 6375  format..path..cu
+00000340: 7276 65a9 0072 0b00 0000 fa4e 2f68 6162  rve..r.....N/hab
+00000350: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+00000360: 6573 2f72 6563 7963 6c69 6e67 2f6d 6978  es/recycling/mix
+00000370: 6573 2f65 6c6c 6970 7469 632f 5345 4350  es/elliptic/SECP
+00000380: 3235 364b 312f 7072 6976 6174 655f 6b65  256K1/private_ke
+00000390: 792f 6275 696c 642e 7079 da06 6372 6561  y/build.py..crea
+000003a0: 7465 3400 0000 7302 0000 000a 0772 0d00  te4...s......r..
+000003b0: 0000 2902 7203 0000 0072 0400 0000 2907  ..).r....r....).
+000003c0: da07 5f5f 646f 635f 5fda 1443 7279 7074  ..__doc__..Crypt
+000003d0: 6f2e 5075 626c 6963 4b65 792e 4543 4372  o.PublicKey.ECCr
+000003e0: 0200 0000 da07 6f73 2e70 6174 68da 026f  ......os.path..o
+000003f0: 7372 0500 0000 720d 0000 0072 0b00 0000  sr....r....r....
+00000400: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000410: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
+00000420: 0000 0404 021a 020b 0c03 0801 0803 0801  ................
+00000430: 0206 0201 0efb                           ......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/elliptic/SECP256K1/private_key/build.py` & `recycling-1.1.0/venues/stages/recycling/mixes/elliptic/SECP256K1/private_key/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	#	seed length = 114 nibbles
 	#				=  57 bytes
 	#
 	seed = "4986888b11358bf3d541b41eea5daece1c6eff64130a45fc8b9ca48f3e0e02463c99c5aedc8a847686d669b7d547c18fe448fc5111ca88f4e8"
 	format = "PEM"
 	path = ""
 	
-	import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+	import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
 	private_key = EEC_448_1_private_key_creator.create (seed, format, path)
 	private_key_instance = private_key ["instance"]
 	private_key_string = private_key ["string"]
 		
 '''
 
 '''
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/__pycache__/form.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/__pycache__/form.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 2402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,137 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 6209 0000  o........@@fb...
+00000000: 6f0d 0d0a 0000 0000 d153 5166 5a09 0000  o........SQfZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 0200 0100 6d04 0200 0100 6d05 5a06 0100  ....m.....m.Z...
 00000050: 6401 6402 6c07 6d02 0200 0100 6d03 0200  d.d.l.m.....m...
 00000060: 0100 6d08 0200 0100 6d09 5a0a 0100 6401  ..m.....m.Z...d.
 00000070: 6402 6c0b 6d02 0200 0100 6d03 0200 0100  d.l.m.....m.....
 00000080: 6d08 0200 0100 6d0c 5a0d 0100 6401 6402  m.....m.Z...d.d.
 00000090: 6c0e 5a0e 6403 6404 8400 5a0f 6405 6406  l.Z.d.d...Z.d.d.
 000000a0: 8400 5a10 0900 6900 6900 6602 6407 6408  ..Z...i.i.f.d.d.
-000000b0: 8401 5a11 6402 5300 2909 6100 0200 000a  ..Z.d.S.).a.....
+000000b0: 8401 5a11 6402 5300 2909 61fe 0100 000a  ..Z.d.S.).a.....
 000000c0: 0973 6565 6420 3d20 2234 3938 3638 3838  .seed = "4986888
 000000d0: 6231 3133 3538 6266 3364 3534 3162 3431  b11358bf3d541b41
 000000e0: 6565 6135 6461 6563 6531 6336 6566 6636  eea5daece1c6eff6
 000000f0: 3431 3330 6134 3566 6338 6239 6361 3438  4130a45fc8b9ca48
 00000100: 6633 6530 6530 3234 3633 6339 3963 3561  f3e0e02463c99c5a
 00000110: 6564 6338 6138 3437 3638 3664 3636 3962  edc8a847686d669b
 00000120: 3764 3534 3763 3138 6665 3434 3866 6335  7d547c18fe448fc5
 00000130: 3131 3163 6138 3866 3465 3822 0a0a 0969  111ca88f4e8"...i
 00000140: 6d70 6f72 7420 7265 6379 636c 696e 672e  mport recycling.
-00000150: 6d6f 6475 6c65 732e 7072 6f70 6f73 616c  modules.proposal
-00000160: 732e 6b65 7973 2e66 6f72 6d20 6173 2066  s.keys.form as f
-00000170: 6f72 6d5f 7072 6f70 6f73 616c 5f6b 6579  orm_proposal_key
-00000180: 730a 0966 6f72 6d5f 7072 6f70 6f73 616c  s..form_proposal
-00000190: 5f6b 6579 732e 736d 6f6f 7468 6c79 2028  _keys.smoothly (
-000001a0: 0a09 0923 0a09 0923 0969 6e70 7574 732c  ...#...#.inputs,
-000001b0: 2063 6f6e 7375 6d65 732c 2075 7469 6c69   consumes, utili
-000001c0: 7a65 730a 0909 230a 0909 7574 696c 697a  zes...#...utiliz
-000001d0: 6573 203d 207b 0a09 0909 2273 6565 6422  es = {...."seed"
-000001e0: 3a20 7365 6564 0a09 097d 2c0a 0909 0a09  : seed...},.....
-000001f0: 0923 0a09 0923 096f 7574 7075 7473 2c20  .#...#.outputs, 
-00000200: 7072 6f64 7563 6573 2c20 6275 696c 6473  produces, builds
-00000210: 0a09 0923 0a09 0962 7569 6c64 7320 3d20  ...#...builds = 
-00000220: 7b0a 0909 0922 7365 6564 223a 207b 0a09  {...."seed": {..
-00000230: 0909 0922 7061 7468 223a 2022 220a 0909  ..."path": ""...
-00000240: 097d 2c0a 0909 0922 7072 6976 6174 6520  .},...."private 
-00000250: 6b65 7922 3a20 7b0a 0909 0909 2266 6f72  key": {....."for
-00000260: 6d61 7422 3a20 2222 2c0a 0909 0909 2270  mat": "",....."p
-00000270: 6174 6822 3a20 2222 0a09 0909 7d2c 0a09  ath": ""....},..
-00000280: 0909 2270 7562 6c69 6320 6b65 7922 3a20  .."public key": 
-00000290: 7b0a 0909 0909 2266 6f72 6d61 7422 3a20  {....."format": 
-000002a0: 2222 2c0a 0909 0909 2270 6174 6822 3a20  "",....."path": 
-000002b0: 2222 0a09 0909 7d0a 0909 7d0a 0929 0ae9  ""....}...}..)..
-000002c0: 0000 0000 4e63 0200 0000 0000 0000 0000  ....Nc..........
-000002d0: 0000 0300 0000 0400 0000 4300 0000 f33c  ..........C....<
-000002e0: 0000 0074 006a 01a0 027c 00a1 0172 0e74  ...t.j...|...r.t
-000002f0: 0364 017c 009b 0064 029d 0383 0182 0174  .d.|...d.......t
-00000300: 047c 0064 0383 027d 027c 02a0 057c 01a1  .|.d...}.|...|..
-00000310: 0101 007c 02a0 06a1 0001 0064 0453 0029  ...|.......d.S.)
-00000320: 054e 7a30 5468 6520 7061 7468 2066 6f72  .Nz0The path for
-00000330: 2074 6865 2073 6565 645f 7374 7269 6e67   the seed_string
-00000340: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-00000350: 652e 2027 fa01 27da 0177 54a9 07da 026f  e. '..'..wT....o
-00000360: 73da 0470 6174 68da 0665 7869 7374 73da  s..path..exists.
-00000370: 0945 7863 6570 7469 6f6e da04 6f70 656e  .Exception..open
-00000380: da05 7772 6974 65da 0563 6c6f 7365 2903  ..write..close).
-00000390: 7207 0000 00da 0b73 6565 645f 7374 7269  r......seed_stri
-000003a0: 6e67 da01 66a9 0072 0f00 0000 fa3f 2f68  ng..f..r.....?/h
-000003b0: 6162 6974 6174 2f76 656e 7565 732f 7374  abitat/venues/st
-000003c0: 6167 6573 2f72 6563 7963 6c69 6e67 2f6d  ages/recycling/m
-000003d0: 6f64 756c 6573 2f70 726f 706f 7361 6c73  odules/proposals
-000003e0: 2f6b 6579 732f 666f 726d 2e70 79da 0a77  /keys/form.py..w
-000003f0: 7269 7465 5f73 6565 642d 0000 0073 0c00  rite_seed-...s..
-00000400: 0000 0c01 1001 0a03 0a01 0801 0402 7211  ..............r.
-00000410: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000420: 0300 0000 0400 0000 4300 0000 7202 0000  ........C...r...
-00000430: 0029 054e 7a3b 5468 6520 7061 7468 2066  .).Nz;The path f
-00000440: 6f72 2074 6865 2070 7562 6c69 635f 6b65  or the public_ke
-00000450: 7920 6865 7861 6465 6369 6d61 6c20 6973  y hexadecimal is
-00000460: 206e 6f74 2061 7661 696c 6162 6c65 2e20   not available. 
-00000470: 2772 0300 0000 7204 0000 0054 7205 0000  'r....r....Tr...
-00000480: 0029 0372 0700 0000 da16 7075 626c 6963  .).r......public
-00000490: 5f6b 6579 5f68 6578 6164 6563 696d 616c  _key_hexadecimal
-000004a0: 720e 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-000004b0: 1000 0000 da10 7772 6974 655f 7075 626c  ......write_publ
-000004c0: 6963 5f6b 6579 3800 0000 730c 0000 000c  ic_key8...s.....
-000004d0: 0110 010a 020a 0108 0104 0272 1300 0000  ...........r....
-000004e0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-000004f0: 0005 0000 0043 0000 0073 f200 0000 6401  .....C...s....d.
-00000500: 7c00 7600 7306 4a00 8201 6401 7c01 7600  |.v.s.J...d.|.v.
-00000510: 730c 4a00 8201 6402 7c01 6401 1900 7600  s.J...d.|.d...v.
-00000520: 7314 4a00 8201 6403 7c01 7600 731a 4a00  s.J...d.|.v.s.J.
-00000530: 8201 6404 7c01 6403 1900 7600 7322 4a00  ..d.|.d...v.s"J.
-00000540: 8201 6402 7c01 6403 1900 7600 732a 4a00  ..d.|.d...v.s*J.
-00000550: 8201 6405 7c01 7600 7330 4a00 8201 6404  ..d.|.v.s0J...d.
-00000560: 7c01 6405 1900 7600 7338 4a00 8201 6402  |.d...v.s8J...d.
-00000570: 7c01 6405 1900 7600 7340 4a00 8201 0900  |.d...v.s@J.....
-00000580: 7400 6a01 7c00 6401 1900 7c01 6403 1900  t.j.|.d...|.d...
-00000590: 6404 1900 7c01 6403 1900 6402 1900 6406  d...|.d...d...d.
-000005a0: 8d03 7d02 7c02 6407 1900 7d03 0900 7402  ..}.|.d...}...t.
-000005b0: 6a03 7c03 6408 8d01 7d04 7404 6a03 7c01  j.|.d...}.t.j.|.
-000005c0: 6405 1900 6402 1900 7c04 6409 1900 6409  d...d...|.d...d.
-000005d0: 640a 8d03 0100 7405 7c01 6401 1900 6402  d.....t.|.d...d.
-000005e0: 1900 7c00 6401 1900 8302 0100 6400 5300  ..|.d.......d.S.
-000005f0: 290b 4eda 0473 6565 6472 0700 0000 7a0b  ).N..seedr....z.
-00000600: 7072 6976 6174 6520 6b65 79da 0666 6f72  private key..for
-00000610: 6d61 747a 0a70 7562 6c69 6320 6b65 7929  matz.public key)
-00000620: 0172 0700 0000 da08 696e 7374 616e 6365  .r......instance
-00000630: 2901 da14 7072 6976 6174 655f 6b65 795f  )...private_key_
-00000640: 696e 7374 616e 6365 da0b 6865 7861 6465  instance..hexade
-00000650: 6369 6d61 6c29 0372 0700 0000 da0a 6b65  cimal).r......ke
-00000660: 795f 7374 7269 6e67 7215 0000 0029 06da  y_stringr....)..
-00000670: 1d45 4543 5f34 3438 5f31 5f70 7269 7661  .EEC_448_1_priva
-00000680: 7465 5f6b 6579 5f63 7265 6174 6f72 da06  te_key_creator..
-00000690: 6372 6561 7465 da19 666f 726d 5f45 4543  create..form_EEC
-000006a0: 5f34 3438 5f31 5f70 7562 6c69 635f 6b65  _448_1_public_ke
-000006b0: 79da 0873 6d6f 6f74 686c 79da 1a77 7269  y..smoothly..wri
-000006c0: 7465 5f45 4543 5f34 3438 5f31 5f70 7562  te_EEC_448_1_pub
-000006d0: 6c69 635f 6b65 7972 1100 0000 2905 da08  lic_keyr....)...
-000006e0: 7574 696c 697a 6573 da06 6275 696c 6473  utilizes..builds
-000006f0: da0b 7072 6976 6174 655f 6b65 7972 1700  ..private_keyr..
-00000700: 0000 da0a 7075 626c 6963 5f6b 6579 720f  ....public_keyr.
-00000710: 0000 0072 0f00 0000 7210 0000 0072 1d00  ...r....r....r..
-00000720: 0000 4800 0000 733a 0000 000c 040c 0210  ..H...s:........
-00000730: 010c 0210 0110 010c 0210 0110 0102 0204  ................
-00000740: 0306 010a 010a 0206 fc08 0602 0504 0302  ................
-00000750: 0106 ff04 030a 0106 0102 0106 fd02 070a  ................
-00000760: 0106 0108 fe72 1d00 0000 2912 da07 5f5f  .....r....)...__
-00000770: 646f 635f 5fda 2f72 6563 7963 6c69 6e67  doc__./recycling
-00000780: 2e6d 6f64 756c 6573 2e45 4543 5f34 3438  .modules.EEC_448
-00000790: 5f31 2e70 7269 7661 7465 5f6b 6579 2e63  _1.private_key.c
-000007a0: 7265 6174 6f72 da07 6d6f 6475 6c65 73da  reator..modules.
-000007b0: 0945 4543 5f34 3438 5f31 7221 0000 00da  .EEC_448_1r!....
-000007c0: 0763 7265 6174 6f72 721a 0000 00da 2b72  .creatorr.....+r
-000007d0: 6563 7963 6c69 6e67 2e6d 6f64 756c 6573  ecycling.modules
-000007e0: 2e45 4543 5f34 3438 5f31 2e70 7562 6c69  .EEC_448_1.publi
-000007f0: 635f 6b65 792e 666f 726d 7222 0000 00da  c_key.formr"....
-00000800: 0466 6f72 6d72 1c00 0000 da2c 7265 6379  .formr.....,recy
-00000810: 636c 696e 672e 6d6f 6475 6c65 732e 4545  cling.modules.EE
-00000820: 435f 3434 385f 312e 7075 626c 6963 5f6b  C_448_1.public_k
-00000830: 6579 2e77 7269 7465 720b 0000 0072 1e00  ey.writer....r..
-00000840: 0000 7206 0000 0072 1100 0000 7213 0000  ..r....r....r...
-00000850: 0072 1d00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00000860: 720f 0000 0072 1000 0000 da08 3c6d 6f64  r....r......<mod
-00000870: 756c 653e 0100 0000 7316 0000 0004 061e  ule>....s.......
-00000880: 1f1e 021e 0108 0308 0108 0b02 0a02 0702  ................
-00000890: 010e fe                                  ...
+00000150: 6d69 7865 732e 7072 6f70 6f73 616c 732e  mixes.proposals.
+00000160: 6b65 7973 2e66 6f72 6d20 6173 2066 6f72  keys.form as for
+00000170: 6d5f 7072 6f70 6f73 616c 5f6b 6579 730a  m_proposal_keys.
+00000180: 0966 6f72 6d5f 7072 6f70 6f73 616c 5f6b  .form_proposal_k
+00000190: 6579 732e 736d 6f6f 7468 6c79 2028 0a09  eys.smoothly (..
+000001a0: 0923 0a09 0923 0969 6e70 7574 732c 2063  .#...#.inputs, c
+000001b0: 6f6e 7375 6d65 732c 2075 7469 6c69 7a65  onsumes, utilize
+000001c0: 730a 0909 230a 0909 7574 696c 697a 6573  s...#...utilizes
+000001d0: 203d 207b 0a09 0909 2273 6565 6422 3a20   = {...."seed": 
+000001e0: 7365 6564 0a09 097d 2c0a 0909 0a09 0923  seed...},......#
+000001f0: 0a09 0923 096f 7574 7075 7473 2c20 7072  ...#.outputs, pr
+00000200: 6f64 7563 6573 2c20 6275 696c 6473 0a09  oduces, builds..
+00000210: 0923 0a09 0962 7569 6c64 7320 3d20 7b0a  .#...builds = {.
+00000220: 0909 0922 7365 6564 223a 207b 0a09 0909  ..."seed": {....
+00000230: 0922 7061 7468 223a 2022 220a 0909 097d  ."path": ""....}
+00000240: 2c0a 0909 0922 7072 6976 6174 6520 6b65  ,...."private ke
+00000250: 7922 3a20 7b0a 0909 0909 2266 6f72 6d61  y": {....."forma
+00000260: 7422 3a20 2222 2c0a 0909 0909 2270 6174  t": "",....."pat
+00000270: 6822 3a20 2222 0a09 0909 7d2c 0a09 0909  h": ""....},....
+00000280: 2270 7562 6c69 6320 6b65 7922 3a20 7b0a  "public key": {.
+00000290: 0909 0909 2266 6f72 6d61 7422 3a20 2222  ...."format": ""
+000002a0: 2c0a 0909 0909 2270 6174 6822 3a20 2222  ,....."path": ""
+000002b0: 0a09 0909 7d0a 0909 7d0a 0929 0ae9 0000  ....}...}..)....
+000002c0: 0000 4e63 0200 0000 0000 0000 0000 0000  ..Nc............
+000002d0: 0300 0000 0400 0000 4300 0000 f33c 0000  ........C....<..
+000002e0: 0074 006a 01a0 027c 00a1 0172 0e74 0364  .t.j...|...r.t.d
+000002f0: 017c 009b 0064 029d 0383 0182 0174 047c  .|...d.......t.|
+00000300: 0064 0383 027d 027c 02a0 057c 01a1 0101  .d...}.|...|....
+00000310: 007c 02a0 06a1 0001 0064 0453 0029 054e  .|.......d.S.).N
+00000320: 7a30 5468 6520 7061 7468 2066 6f72 2074  z0The path for t
+00000330: 6865 2073 6565 645f 7374 7269 6e67 2069  he seed_string i
+00000340: 7320 6e6f 7420 6176 6169 6c61 626c 652e  s not available.
+00000350: 2027 fa01 27da 0177 54a9 07da 026f 73da   '..'..wT....os.
+00000360: 0470 6174 68da 0665 7869 7374 73da 0945  .path..exists..E
+00000370: 7863 6570 7469 6f6e da04 6f70 656e da05  xception..open..
+00000380: 7772 6974 65da 0563 6c6f 7365 2903 7207  write..close).r.
+00000390: 0000 00da 0b73 6565 645f 7374 7269 6e67  .....seed_string
+000003a0: da01 66a9 0072 0f00 0000 fa3d 2f68 6162  ..f..r.....=/hab
+000003b0: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+000003c0: 6573 2f72 6563 7963 6c69 6e67 2f6d 6978  es/recycling/mix
+000003d0: 6573 2f70 726f 706f 7361 6c73 2f6b 6579  es/proposals/key
+000003e0: 732f 666f 726d 2e70 79da 0a77 7269 7465  s/form.py..write
+000003f0: 5f73 6565 642d 0000 0073 0c00 0000 0c01  _seed-...s......
+00000400: 1001 0a03 0a01 0801 0402 7211 0000 0063  ..........r....c
+00000410: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000420: 0400 0000 4300 0000 7202 0000 0029 054e  ....C...r....).N
+00000430: 7a3b 5468 6520 7061 7468 2066 6f72 2074  z;The path for t
+00000440: 6865 2070 7562 6c69 635f 6b65 7920 6865  he public_key he
+00000450: 7861 6465 6369 6d61 6c20 6973 206e 6f74  xadecimal is not
+00000460: 2061 7661 696c 6162 6c65 2e20 2772 0300   available. 'r..
+00000470: 0000 7204 0000 0054 7205 0000 0029 0372  ..r....Tr....).r
+00000480: 0700 0000 da16 7075 626c 6963 5f6b 6579  ......public_key
+00000490: 5f68 6578 6164 6563 696d 616c 720e 0000  _hexadecimalr...
+000004a0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000004b0: da10 7772 6974 655f 7075 626c 6963 5f6b  ..write_public_k
+000004c0: 6579 3800 0000 730c 0000 000c 0110 010a  ey8...s.........
+000004d0: 020a 0108 0104 0272 1300 0000 6302 0000  .......r....c...
+000004e0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000004f0: 0043 0000 0073 f200 0000 6401 7c00 7600  .C...s....d.|.v.
+00000500: 7306 4a00 8201 6401 7c01 7600 730c 4a00  s.J...d.|.v.s.J.
+00000510: 8201 6402 7c01 6401 1900 7600 7314 4a00  ..d.|.d...v.s.J.
+00000520: 8201 6403 7c01 7600 731a 4a00 8201 6404  ..d.|.v.s.J...d.
+00000530: 7c01 6403 1900 7600 7322 4a00 8201 6402  |.d...v.s"J...d.
+00000540: 7c01 6403 1900 7600 732a 4a00 8201 6405  |.d...v.s*J...d.
+00000550: 7c01 7600 7330 4a00 8201 6404 7c01 6405  |.v.s0J...d.|.d.
+00000560: 1900 7600 7338 4a00 8201 6402 7c01 6405  ..v.s8J...d.|.d.
+00000570: 1900 7600 7340 4a00 8201 0900 7400 6a01  ..v.s@J.....t.j.
+00000580: 7c00 6401 1900 7c01 6403 1900 6404 1900  |.d...|.d...d...
+00000590: 7c01 6403 1900 6402 1900 6406 8d03 7d02  |.d...d...d...}.
+000005a0: 7c02 6407 1900 7d03 0900 7402 6a03 7c03  |.d...}...t.j.|.
+000005b0: 6408 8d01 7d04 7404 6a03 7c01 6405 1900  d...}.t.j.|.d...
+000005c0: 6402 1900 7c04 6409 1900 6409 640a 8d03  d...|.d...d.d...
+000005d0: 0100 7405 7c01 6401 1900 6402 1900 7c00  ..t.|.d...d...|.
+000005e0: 6401 1900 8302 0100 6400 5300 290b 4eda  d.......d.S.).N.
+000005f0: 0473 6565 6472 0700 0000 7a0b 7072 6976  .seedr....z.priv
+00000600: 6174 6520 6b65 79da 0666 6f72 6d61 747a  ate key..formatz
+00000610: 0a70 7562 6c69 6320 6b65 7929 0172 0700  .public key).r..
+00000620: 0000 da08 696e 7374 616e 6365 2901 da14  ....instance)...
+00000630: 7072 6976 6174 655f 6b65 795f 696e 7374  private_key_inst
+00000640: 616e 6365 da0b 6865 7861 6465 6369 6d61  ance..hexadecima
+00000650: 6c29 0372 0700 0000 da0a 6b65 795f 7374  l).r......key_st
+00000660: 7269 6e67 7215 0000 0029 06da 1d45 4543  ringr....)...EEC
+00000670: 5f34 3438 5f31 5f70 7269 7661 7465 5f6b  _448_1_private_k
+00000680: 6579 5f63 7265 6174 6f72 da06 6372 6561  ey_creator..crea
+00000690: 7465 da19 666f 726d 5f45 4543 5f34 3438  te..form_EEC_448
+000006a0: 5f31 5f70 7562 6c69 635f 6b65 79da 0873  _1_public_key..s
+000006b0: 6d6f 6f74 686c 79da 1a77 7269 7465 5f45  moothly..write_E
+000006c0: 4543 5f34 3438 5f31 5f70 7562 6c69 635f  EC_448_1_public_
+000006d0: 6b65 7972 1100 0000 2905 da08 7574 696c  keyr....)...util
+000006e0: 697a 6573 da06 6275 696c 6473 da0b 7072  izes..builds..pr
+000006f0: 6976 6174 655f 6b65 7972 1700 0000 da0a  ivate_keyr......
+00000700: 7075 626c 6963 5f6b 6579 720f 0000 0072  public_keyr....r
+00000710: 0f00 0000 7210 0000 0072 1d00 0000 4800  ....r....r....H.
+00000720: 0000 733a 0000 000c 040c 0210 010c 0210  ..s:............
+00000730: 0110 010c 0210 0110 0102 0204 0306 010a  ................
+00000740: 010a 0206 fc08 0602 0504 0302 0106 ff04  ................
+00000750: 030a 0106 0102 0106 fd02 070a 0106 0108  ................
+00000760: fe72 1d00 0000 2912 da07 5f5f 646f 635f  .r....)...__doc_
+00000770: 5fda 2d72 6563 7963 6c69 6e67 2e6d 6978  _.-recycling.mix
+00000780: 6573 2e45 4543 5f34 3438 5f31 2e70 7269  es.EEC_448_1.pri
+00000790: 7661 7465 5f6b 6579 2e63 7265 6174 6f72  vate_key.creator
+000007a0: da05 6d69 7865 73da 0945 4543 5f34 3438  ..mixes..EEC_448
+000007b0: 5f31 7221 0000 00da 0763 7265 6174 6f72  _1r!.....creator
+000007c0: 721a 0000 00da 2972 6563 7963 6c69 6e67  r.....)recycling
+000007d0: 2e6d 6978 6573 2e45 4543 5f34 3438 5f31  .mixes.EEC_448_1
+000007e0: 2e70 7562 6c69 635f 6b65 792e 666f 726d  .public_key.form
+000007f0: 7222 0000 00da 0466 6f72 6d72 1c00 0000  r".....formr....
+00000800: da2a 7265 6379 636c 696e 672e 6d69 7865  .*recycling.mixe
+00000810: 732e 4545 435f 3434 385f 312e 7075 626c  s.EEC_448_1.publ
+00000820: 6963 5f6b 6579 2e77 7269 7465 720b 0000  ic_key.writer...
+00000830: 0072 1e00 0000 7206 0000 0072 1100 0000  .r....r....r....
+00000840: 7213 0000 0072 1d00 0000 720f 0000 0072  r....r....r....r
+00000850: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+00000860: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
+00000870: 0004 061e 1f1e 021e 0108 0308 0108 0b02  ................
+00000880: 0a02 0702 010e fe                        .......
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1175 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 9704 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 9304 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a05 6401  m.Z...d.d.l.Z.d.
 00000050: 6403 6c06 5a06 6401 6403 6c07 5a07 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c08 6d09 0200 0100 6d0a 0200 0100  d.l.m.....m.....
 00000070: 6d0b 0200 0100 6d0c 5a0d 0100 6401 6403  m.....m.Z...d.d.
 00000080: 6c0e 5a0e 6404 6405 8400 5a0f 6406 6407  l.Z.d.d...Z.d.d.
 00000090: 8400 5a10 6408 6510 6901 5a11 6403 5300  ..Z.d.e.i.Z.d.S.
-000000a0: 2909 7a4f 0a09 7079 7468 6f6e 3320 696e  ).zO..python3 in
+000000a0: 2909 7a4d 0a09 7079 7468 6f6e 3320 696e  ).zM..python3 in
 000000b0: 7375 7261 6e63 652e 7072 6f63 2e70 7920  surance.proc.py 
-000000c0: 226d 6f64 756c 6573 2f70 726f 706f 7361  "modules/proposa
-000000d0: 6c73 2f6b 6579 732f 5f73 7461 7475 732f  ls/keys/_status/
-000000e0: 315f 4445 522f 7374 6174 7573 5f31 2e70  1_DER/status_1.p
-000000f0: 7922 0ae9 0000 0000 2903 da07 6469 726e  y"......)...dirn
-00000100: 616d 65da 046a 6f69 6eda 086e 6f72 6d70  ame..join..normp
-00000110: 6174 684e 6301 0000 0000 0000 0000 0000  athNc...........
-00000120: 0001 0000 0008 0000 0043 0000 0073 2600  .........C...s&.
-00000130: 0000 7a08 7400 a001 7c00 a101 0100 5700  ..z.t...|.....W.
-00000140: 6400 5300 0400 7402 7912 0100 0100 0100  d.S...t.y.......
-00000150: 5900 6400 5300 7700 2901 4e29 03da 0673  Y.d.S.w.).N)...s
-00000160: 6875 7469 6cda 0672 6d74 7265 65da 0945  hutil..rmtree..E
-00000170: 7863 6570 7469 6f6e 2901 da0e 6469 7265  xception)...dire
-00000180: 6374 6f72 795f 7061 7468 a900 7209 0000  ctory_path..r...
-00000190: 00fa 512f 6861 6269 7461 742f 7665 6e75  ..Q/habitat/venu
-000001a0: 6573 2f73 7461 6765 732f 7265 6379 636c  es/stages/recycl
-000001b0: 696e 672f 6d6f 6475 6c65 732f 7072 6f70  ing/modules/prop
-000001c0: 6f73 616c 732f 6b65 7973 2f5f 7374 6174  osals/keys/_stat
-000001d0: 7573 2f31 5f44 4552 2f73 7461 7475 735f  us/1_DER/status_
-000001e0: 312e 7079 da0f 6572 6173 655f 6469 7265  1.py..erase_dire
-000001f0: 6374 6f72 790f 0000 0073 0a00 0000 0201  ctory....s......
-00000200: 1001 0c01 0601 02ff 720b 0000 0063 0000  ........r....c..
-00000210: 0000 0000 0000 0000 0000 0300 0000 0900  ................
-00000220: 0000 4300 0000 7380 0000 0064 017d 0074  ..C...s....d.}.t
-00000230: 00a0 0174 02a1 016a 03a0 04a1 007d 0174  ...t...j.....}.t
-00000240: 0574 067c 0164 0283 0283 017d 0274 077c  .t.|.d.....}.t.|
-00000250: 0283 0101 0074 08a0 097c 02a1 0101 0074  .....t...|.....t
-00000260: 0a6a 0b64 037c 0069 0164 0474 0574 067c  .j.d.|.i.d.t.t.|
-00000270: 0264 0583 0283 0169 0164 0674 0574 067c  .d.....i.d.t.t.|
-00000280: 0264 0783 0283 0164 089c 0264 0674 0574  .d.....d...d.t.t
-00000290: 067c 0264 0983 0283 0164 089c 0264 0a9c  .|.d.....d...d..
-000002a0: 0364 0b8d 0201 0064 0053 0029 0c4e da72  .d.....d.S.).N.r
-000002b0: 3439 3836 3838 3862 3131 3335 3862 6633  4986888b11358bf3
-000002c0: 6435 3431 6234 3165 6561 3564 6165 6365  d541b41eea5daece
-000002d0: 3163 3665 6666 3634 3133 3061 3435 6663  1c6eff64130a45fc
-000002e0: 3862 3963 6134 3866 3365 3065 3032 3436  8b9ca48f3e0e0246
-000002f0: 3363 3939 6335 6165 6463 3861 3834 3736  3c99c5aedc8a8476
-00000300: 3836 6436 3639 6237 6435 3437 6331 3866  86d669b7d547c18f
-00000310: 6534 3438 6663 3531 3131 6361 3838 6634  e448fc5111ca88f4
-00000320: 6538 da09 7465 6d70 6f72 6172 79da 0473  e8..temporary..s
-00000330: 6565 64da 0470 6174 687a 0d70 726f 706f  eed..pathz.propo
-00000340: 7361 6c2e 7365 6564 da03 4445 527a 1870  sal.seed..DERz.p
-00000350: 726f 706f 7361 6c2e 7072 6976 6174 655f  roposal.private_
-00000360: 6b65 792e 4445 5229 02da 0666 6f72 6d61  key.DER)...forma
-00000370: 7472 0f00 0000 7a17 7072 6f70 6f73 616c  tr....z.proposal
-00000380: 2e70 7562 6c69 635f 6b65 792e 4445 5229  .public_key.DER)
-00000390: 0372 0e00 0000 7a0b 7072 6976 6174 6520  .r....z.private 
-000003a0: 6b65 797a 0a70 7562 6c69 6320 6b65 7929  keyz.public key)
-000003b0: 02da 0875 7469 6c69 7a65 73da 0662 7569  ...utilizes..bui
-000003c0: 6c64 7329 0cda 0770 6174 686c 6962 da04  lds)...pathlib..
-000003d0: 5061 7468 da08 5f5f 6669 6c65 5f5f da06  Path..__file__..
-000003e0: 7061 7265 6e74 da07 7265 736f 6c76 6572  parent..resolver
-000003f0: 0400 0000 7203 0000 0072 0b00 0000 da02  ....r....r......
-00000400: 6f73 da05 6d6b 6469 72da 1266 6f72 6d5f  os..mkdir..form_
-00000410: 7072 6f70 6f73 616c 5f6b 6579 73da 0873  proposal_keys..s
-00000420: 6d6f 6f74 686c 7929 0372 0e00 0000 da0e  moothly).r......
-00000430: 7468 6973 5f64 6972 6563 746f 7279 da13  this_directory..
-00000440: 7465 6d70 6f72 6172 795f 6469 7265 6374  temporary_direct
-00000450: 6f72 7972 0900 0000 7209 0000 0072 0a00  oryr....r....r..
-00000460: 0000 da07 6368 6563 6b5f 3115 0000 0073  ....check_1....s
-00000470: 2600 0000 0401 1002 0e01 0802 0a01 0403  &...............
-00000480: 0402 02ff 0e05 02ff 0204 0c01 04fe 0205  ................
-00000490: 0c01 04fe 04f8 06fc 0416 721f 0000 007a  ..........r....z
-000004a0: 0763 6865 636b 2031 2912 da07 5f5f 646f  .check 1)...__do
-000004b0: 635f 5fda 076f 732e 7061 7468 7202 0000  c__..os.pathr...
-000004c0: 0072 0300 0000 7204 0000 0072 1400 0000  .r....r....r....
-000004d0: da03 7379 7372 1900 0000 da25 7265 6379  ..sysr.....%recy
-000004e0: 636c 696e 672e 6d6f 6475 6c65 732e 7072  cling.modules.pr
-000004f0: 6f70 6f73 616c 732e 6b65 7973 2e66 6f72  oposals.keys.for
-00000500: 6dda 076d 6f64 756c 6573 da09 7072 6f70  m..modules..prop
-00000510: 6f73 616c 73da 046b 6579 73da 0466 6f72  osals..keys..for
-00000520: 6d72 1b00 0000 7205 0000 0072 0b00 0000  mr....r....r....
-00000530: 721f 0000 00da 0663 6865 636b 7372 0900  r......checksr..
-00000540: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000550: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000560: 1600 0000 0401 1404 0801 0801 0801 1e02  ................
-00000570: 0802 0802 0806 0423 08ff                 .......#..
+000000c0: 226d 6978 6573 2f70 726f 706f 7361 6c73  "mixes/proposals
+000000d0: 2f6b 6579 732f 5f73 7461 7475 732f 315f  /keys/_status/1_
+000000e0: 4445 522f 7374 6174 7573 5f31 2e70 7922  DER/status_1.py"
+000000f0: 0ae9 0000 0000 2903 da07 6469 726e 616d  ......)...dirnam
+00000100: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
+00000110: 684e 6301 0000 0000 0000 0000 0000 0001  hNc.............
+00000120: 0000 0008 0000 0043 0000 0073 2600 0000  .......C...s&...
+00000130: 7a08 7400 a001 7c00 a101 0100 5700 6400  z.t...|.....W.d.
+00000140: 5300 0400 7402 7912 0100 0100 0100 5900  S...t.y.......Y.
+00000150: 6400 5300 7700 2901 4e29 03da 0673 6875  d.S.w.).N)...shu
+00000160: 7469 6cda 0672 6d74 7265 65da 0945 7863  til..rmtree..Exc
+00000170: 6570 7469 6f6e 2901 da0e 6469 7265 6374  eption)...direct
+00000180: 6f72 795f 7061 7468 a900 7209 0000 00fa  ory_path..r.....
+00000190: 4f2f 6861 6269 7461 742f 7665 6e75 6573  O/habitat/venues
+000001a0: 2f73 7461 6765 732f 7265 6379 636c 696e  /stages/recyclin
+000001b0: 672f 6d69 7865 732f 7072 6f70 6f73 616c  g/mixes/proposal
+000001c0: 732f 6b65 7973 2f5f 7374 6174 7573 2f31  s/keys/_status/1
+000001d0: 5f44 4552 2f73 7461 7475 735f 312e 7079  _DER/status_1.py
+000001e0: da0f 6572 6173 655f 6469 7265 6374 6f72  ..erase_director
+000001f0: 790f 0000 0073 0a00 0000 0201 1001 0c01  y....s..........
+00000200: 0601 02ff 720b 0000 0063 0000 0000 0000  ....r....c......
+00000210: 0000 0000 0000 0300 0000 0900 0000 4300  ..............C.
+00000220: 0000 7380 0000 0064 017d 0074 00a0 0174  ..s....d.}.t...t
+00000230: 02a1 016a 03a0 04a1 007d 0174 0574 067c  ...j.....}.t.t.|
+00000240: 0164 0283 0283 017d 0274 077c 0283 0101  .d.....}.t.|....
+00000250: 0074 08a0 097c 02a1 0101 0074 0a6a 0b64  .t...|.....t.j.d
+00000260: 037c 0069 0164 0474 0574 067c 0264 0583  .|.i.d.t.t.|.d..
+00000270: 0283 0169 0164 0674 0574 067c 0264 0783  ...i.d.t.t.|.d..
+00000280: 0283 0164 089c 0264 0674 0574 067c 0264  ...d...d.t.t.|.d
+00000290: 0983 0283 0164 089c 0264 0a9c 0364 0b8d  .....d...d...d..
+000002a0: 0201 0064 0053 0029 0c4e da72 3439 3836  ...d.S.).N.r4986
+000002b0: 3838 3862 3131 3335 3862 6633 6435 3431  888b11358bf3d541
+000002c0: 6234 3165 6561 3564 6165 6365 3163 3665  b41eea5daece1c6e
+000002d0: 6666 3634 3133 3061 3435 6663 3862 3963  ff64130a45fc8b9c
+000002e0: 6134 3866 3365 3065 3032 3436 3363 3939  a48f3e0e02463c99
+000002f0: 6335 6165 6463 3861 3834 3736 3836 6436  c5aedc8a847686d6
+00000300: 3639 6237 6435 3437 6331 3866 6534 3438  69b7d547c18fe448
+00000310: 6663 3531 3131 6361 3838 6634 6538 da09  fc5111ca88f4e8..
+00000320: 7465 6d70 6f72 6172 79da 0473 6565 64da  temporary..seed.
+00000330: 0470 6174 687a 0d70 726f 706f 7361 6c2e  .pathz.proposal.
+00000340: 7365 6564 da03 4445 527a 1870 726f 706f  seed..DERz.propo
+00000350: 7361 6c2e 7072 6976 6174 655f 6b65 792e  sal.private_key.
+00000360: 4445 5229 02da 0666 6f72 6d61 7472 0f00  DER)...formatr..
+00000370: 0000 7a17 7072 6f70 6f73 616c 2e70 7562  ..z.proposal.pub
+00000380: 6c69 635f 6b65 792e 4445 5229 0372 0e00  lic_key.DER).r..
+00000390: 0000 7a0b 7072 6976 6174 6520 6b65 797a  ..z.private keyz
+000003a0: 0a70 7562 6c69 6320 6b65 7929 02da 0875  .public key)...u
+000003b0: 7469 6c69 7a65 73da 0662 7569 6c64 7329  tilizes..builds)
+000003c0: 0cda 0770 6174 686c 6962 da04 5061 7468  ...pathlib..Path
+000003d0: da08 5f5f 6669 6c65 5f5f da06 7061 7265  ..__file__..pare
+000003e0: 6e74 da07 7265 736f 6c76 6572 0400 0000  nt..resolver....
+000003f0: 7203 0000 0072 0b00 0000 da02 6f73 da05  r....r......os..
+00000400: 6d6b 6469 72da 1266 6f72 6d5f 7072 6f70  mkdir..form_prop
+00000410: 6f73 616c 5f6b 6579 73da 0873 6d6f 6f74  osal_keys..smoot
+00000420: 686c 7929 0372 0e00 0000 da0e 7468 6973  hly).r......this
+00000430: 5f64 6972 6563 746f 7279 da13 7465 6d70  _directory..temp
+00000440: 6f72 6172 795f 6469 7265 6374 6f72 7972  orary_directoryr
+00000450: 0900 0000 7209 0000 0072 0a00 0000 da07  ....r....r......
+00000460: 6368 6563 6b5f 3115 0000 0073 2600 0000  check_1....s&...
+00000470: 0401 1002 0e01 0802 0a01 0403 0402 02ff  ................
+00000480: 0e05 02ff 0204 0c01 04fe 0205 0c01 04fe  ................
+00000490: 04f8 06fc 0416 721f 0000 007a 0763 6865  ......r....z.che
+000004a0: 636b 2031 2912 da07 5f5f 646f 635f 5fda  ck 1)...__doc__.
+000004b0: 076f 732e 7061 7468 7202 0000 0072 0300  .os.pathr....r..
+000004c0: 0000 7204 0000 0072 1400 0000 da03 7379  ..r....r......sy
+000004d0: 7372 1900 0000 da23 7265 6379 636c 696e  sr.....#recyclin
+000004e0: 672e 6d69 7865 732e 7072 6f70 6f73 616c  g.mixes.proposal
+000004f0: 732e 6b65 7973 2e66 6f72 6dda 056d 6978  s.keys.form..mix
+00000500: 6573 da09 7072 6f70 6f73 616c 73da 046b  es..proposals..k
+00000510: 6579 73da 0466 6f72 6d72 1b00 0000 7205  eys..formr....r.
+00000520: 0000 0072 0b00 0000 721f 0000 00da 0663  ...r....r......c
+00000530: 6865 636b 7372 0900 0000 7209 0000 0072  hecksr....r....r
+00000540: 0900 0000 720a 0000 00da 083c 6d6f 6475  ....r......<modu
+00000550: 6c65 3e01 0000 0073 1600 0000 0401 1404  le>....s........
+00000560: 0801 0801 0801 1e02 0802 0802 0806 0423  ...............#
+00000570: 08ff                                     ..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/1_DER/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/1_DER/status_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 '''
-	python3 insurance.proc.py "modules/proposals/keys/_status/1_DER/status_1.py"
+	python3 insurance.proc.py "mixes/proposals/keys/_status/1_DER/status_1.py"
 '''
 
 from os.path import dirname, join, normpath
 import pathlib
 import sys
 import os
 
-import recycling.modules.proposals.keys.form as form_proposal_keys
+import recycling.mixes.proposals.keys.form as form_proposal_keys
 
 import shutil
 
 def erase_directory (directory_path):
 	try:
 		shutil.rmtree (directory_path)
 	except Exception:
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/__pycache__/status_1.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 12 04:08:12 2024 UTC, .py size: 1208 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-00000000: 6f0d 0d0a 0000 0000 ac40 4066 b804 0000  o........@@f....
+00000000: 6f0d 0d0a 0000 0000 d153 5166 be04 0000  o........SQf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a05 6401  m.Z...d.d.l.Z.d.
 00000050: 6403 6c06 5a06 6401 6403 6c07 5a07 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c08 6d09 0200 0100 6d0a 0200 0100  d.l.m.....m.....
 00000070: 6d0b 0200 0100 6d0c 5a0d 0100 6401 6403  m.....m.Z...d.d.
 00000080: 6c0e 5a0e 6404 6405 8400 5a0f 6406 6407  l.Z.d.d...Z.d.d.
 00000090: 8400 5a10 6408 6510 6901 5a11 6403 5300  ..Z.d.e.i.Z.d.S.
-000000a0: 2909 7a62 0a09 7079 7468 6f6e 3320 696e  ).zb..python3 in
+000000a0: 2909 7a5a 0a09 7079 7468 6f6e 3320 696e  ).zZ..python3 in
 000000b0: 7375 7261 6e63 652e 7072 6f63 2e70 7920  surance.proc.py 
-000000c0: 226d 6f64 756c 6573 2f70 726f 706f 7361  "modules/proposa
-000000d0: 6c73 2f6b 6579 732f 5f73 7461 7475 732f  ls/keys/_status/
-000000e0: 315f 6865 7861 6465 6369 6d61 6c5f 7075  1_hexadecimal_pu
-000000f0: 626c 6963 5f6b 6579 2f73 7461 7475 735f  blic_key/status_
-00000100: 312e 7079 220a e900 0000 0029 03da 0764  1.py"......)...d
-00000110: 6972 6e61 6d65 da04 6a6f 696e da08 6e6f  irname..join..no
-00000120: 726d 7061 7468 4e63 0100 0000 0000 0000  rmpathNc........
-00000130: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-00000140: 7326 0000 007a 0874 00a0 017c 00a1 0101  s&...z.t...|....
-00000150: 0057 0064 0053 0004 0074 0279 1201 0001  .W.d.S...t.y....
-00000160: 0001 0059 0064 0053 0077 0029 014e 2903  ...Y.d.S.w.).N).
-00000170: da06 7368 7574 696c da06 726d 7472 6565  ..shutil..rmtree
-00000180: da09 4578 6365 7074 696f 6e29 01da 0e64  ..Exception)...d
-00000190: 6972 6563 746f 7279 5f70 6174 68a9 0072  irectory_path..r
-000001a0: 0900 0000 fa64 2f68 6162 6974 6174 2f76  .....d/habitat/v
-000001b0: 656e 7565 732f 7374 6167 6573 2f72 6563  enues/stages/rec
-000001c0: 7963 6c69 6e67 2f6d 6f64 756c 6573 2f70  ycling/modules/p
-000001d0: 726f 706f 7361 6c73 2f6b 6579 732f 5f73  roposals/keys/_s
-000001e0: 7461 7475 732f 325f 6865 7861 6465 6369  tatus/2_hexadeci
-000001f0: 6d61 6c5f 7075 626c 6963 5f6b 6579 2f73  mal_public_key/s
-00000200: 7461 7475 735f 312e 7079 da0f 6572 6173  tatus_1.py..eras
-00000210: 655f 6469 7265 6374 6f72 790f 0000 0073  e_directory....s
-00000220: 0a00 0000 0201 1001 0c01 0601 02ff 720b  ..............r.
-00000230: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000240: 0300 0000 0900 0000 4300 0000 7380 0000  ........C...s...
-00000250: 0064 017d 0074 00a0 0174 02a1 016a 03a0  .d.}.t...t...j..
-00000260: 04a1 007d 0174 0574 067c 0164 0283 0283  ...}.t.t.|.d....
-00000270: 017d 0274 077c 0283 0101 0074 08a0 097c  .}.t.|.....t...|
-00000280: 02a1 0101 0074 0a6a 0b64 037c 0069 0164  .....t.j.d.|.i.d
-00000290: 0474 0574 067c 0264 0583 0283 0169 0164  .t.t.|.d.....i.d
-000002a0: 0674 0574 067c 0264 0783 0283 0164 089c  .t.t.|.d.....d..
-000002b0: 0264 0974 0574 067c 0264 0a83 0283 0164  .d.t.t.|.d.....d
-000002c0: 089c 0264 0b9c 0364 0c8d 0201 0064 0053  ...d...d.....d.S
-000002d0: 0029 0d4e da72 3439 3836 3838 3862 3131  .).N.r4986888b11
-000002e0: 3335 3862 6633 6435 3431 6234 3165 6561  358bf3d541b41eea
-000002f0: 3564 6165 6365 3163 3665 6666 3634 3133  5daece1c6eff6413
-00000300: 3061 3435 6663 3862 3963 6134 3866 3365  0a45fc8b9ca48f3e
-00000310: 3065 3032 3436 3363 3939 6335 6165 6463  0e02463c99c5aedc
-00000320: 3861 3834 3736 3836 6436 3639 6237 6435  8a847686d669b7d5
-00000330: 3437 6331 3866 6534 3438 6663 3531 3131  47c18fe448fc5111
-00000340: 6361 3838 6634 6538 da09 7465 6d70 6f72  ca88f4e8..tempor
-00000350: 6172 79da 0473 6565 64da 0470 6174 687a  ary..seed..pathz
-00000360: 0d70 726f 706f 7361 6c2e 7365 6564 da03  .proposal.seed..
-00000370: 4445 527a 1870 726f 706f 7361 6c2e 7072  DERz.proposal.pr
-00000380: 6976 6174 655f 6b65 792e 4445 5229 02da  ivate_key.DER)..
-00000390: 0666 6f72 6d61 7472 0f00 0000 da0b 6865  .formatr......he
-000003a0: 7861 6465 6369 6d61 6c7a 1f70 726f 706f  xadecimalz.propo
-000003b0: 7361 6c2e 7075 626c 6963 5f6b 6579 2e68  sal.public_key.h
-000003c0: 6578 6164 6563 696d 616c 2903 720e 0000  exadecimal).r...
-000003d0: 007a 0b70 7269 7661 7465 206b 6579 7a0a  .z.private keyz.
-000003e0: 7075 626c 6963 206b 6579 2902 da08 7574  public key)...ut
-000003f0: 696c 697a 6573 da06 6275 696c 6473 290c  ilizes..builds).
-00000400: da07 7061 7468 6c69 62da 0450 6174 68da  ..pathlib..Path.
-00000410: 085f 5f66 696c 655f 5fda 0670 6172 656e  .__file__..paren
-00000420: 74da 0772 6573 6f6c 7665 7204 0000 0072  t..resolver....r
-00000430: 0300 0000 720b 0000 00da 026f 73da 056d  ....r......os..m
-00000440: 6b64 6972 da12 666f 726d 5f70 726f 706f  kdir..form_propo
-00000450: 7361 6c5f 6b65 7973 da08 736d 6f6f 7468  sal_keys..smooth
-00000460: 6c79 2903 720e 0000 00da 0e74 6869 735f  ly).r......this_
-00000470: 6469 7265 6374 6f72 79da 1374 656d 706f  directory..tempo
-00000480: 7261 7279 5f64 6972 6563 746f 7279 7209  rary_directoryr.
-00000490: 0000 0072 0900 0000 720a 0000 00da 0763  ...r....r......c
-000004a0: 6865 636b 5f31 1500 0000 7326 0000 0004  heck_1....s&....
-000004b0: 0110 020e 0108 020a 0104 0204 0202 ff0e  ................
-000004c0: 0502 ff02 040c 0104 fe02 050c 0104 fe04  ................
-000004d0: f806 fc04 1672 2000 0000 7a07 6368 6563  .....r ...z.chec
-000004e0: 6b20 3129 12da 075f 5f64 6f63 5f5f da07  k 1)...__doc__..
-000004f0: 6f73 2e70 6174 6872 0200 0000 7203 0000  os.pathr....r...
-00000500: 0072 0400 0000 7215 0000 00da 0373 7973  .r....r......sys
-00000510: 721a 0000 00da 2572 6563 7963 6c69 6e67  r.....%recycling
-00000520: 2e6d 6f64 756c 6573 2e70 726f 706f 7361  .modules.proposa
-00000530: 6c73 2e6b 6579 732e 666f 726d da07 6d6f  ls.keys.form..mo
-00000540: 6475 6c65 73da 0970 726f 706f 7361 6c73  dules..proposals
-00000550: da04 6b65 7973 da04 666f 726d 721c 0000  ..keys..formr...
-00000560: 0072 0500 0000 720b 0000 0072 2000 0000  .r....r....r ...
-00000570: da06 6368 6563 6b73 7209 0000 0072 0900  ..checksr....r..
-00000580: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
-00000590: 6f64 756c 653e 0100 0000 7316 0000 0004  odule>....s.....
-000005a0: 0114 0408 0108 0108 011e 0208 0208 0208  ................
-000005b0: 0604 2208 ff                             .."..
+000000c0: 226d 6978 6573 2f70 726f 706f 7361 6c73  "mixes/proposals
+000000d0: 2f6b 6579 732f 5f73 7461 7475 732f 335f  /keys/_status/3_
+000000e0: 6865 7861 6465 6369 6d61 6c5f 6b65 7973  hexadecimal_keys
+000000f0: 2f73 7461 7475 735f 312e 7079 220a e900  /status_1.py"...
+00000100: 0000 0029 03da 0764 6972 6e61 6d65 da04  ...)...dirname..
+00000110: 6a6f 696e da08 6e6f 726d 7061 7468 4e63  join..normpathNc
+00000120: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000130: 0800 0000 4300 0000 7326 0000 007a 0874  ....C...s&...z.t
+00000140: 00a0 017c 00a1 0101 0057 0064 0053 0004  ...|.....W.d.S..
+00000150: 0074 0279 1201 0001 0001 0059 0064 0053  .t.y.......Y.d.S
+00000160: 0077 0029 014e 2903 da06 7368 7574 696c  .w.).N)...shutil
+00000170: da06 726d 7472 6565 da09 4578 6365 7074  ..rmtree..Except
+00000180: 696f 6e29 01da 0e64 6972 6563 746f 7279  ion)...directory
+00000190: 5f70 6174 68a9 0072 0900 0000 fa5c 2f68  _path..r.....\/h
+000001a0: 6162 6974 6174 2f76 656e 7565 732f 7374  abitat/venues/st
+000001b0: 6167 6573 2f72 6563 7963 6c69 6e67 2f6d  ages/recycling/m
+000001c0: 6978 6573 2f70 726f 706f 7361 6c73 2f6b  ixes/proposals/k
+000001d0: 6579 732f 5f73 7461 7475 732f 335f 6865  eys/_status/3_he
+000001e0: 7861 6465 6369 6d61 6c5f 6b65 7973 2f73  xadecimal_keys/s
+000001f0: 7461 7475 735f 312e 7079 da0f 6572 6173  tatus_1.py..eras
+00000200: 655f 6469 7265 6374 6f72 790f 0000 0073  e_directory....s
+00000210: 0a00 0000 0201 1001 0c01 0601 02ff 720b  ..............r.
+00000220: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000230: 0300 0000 0900 0000 4300 0000 7380 0000  ........C...s...
+00000240: 0064 017d 0074 00a0 0174 02a1 016a 03a0  .d.}.t...t...j..
+00000250: 04a1 007d 0174 0574 067c 0164 0283 0283  ...}.t.t.|.d....
+00000260: 017d 0274 077c 0283 0101 0074 08a0 097c  .}.t.|.....t...|
+00000270: 02a1 0101 0074 0a6a 0b64 037c 0069 0164  .....t.j.d.|.i.d
+00000280: 0474 0574 067c 0264 0583 0283 0169 0164  .t.t.|.d.....i.d
+00000290: 0674 0574 067c 0264 0783 0283 0164 089c  .t.t.|.d.....d..
+000002a0: 0264 0674 0574 067c 0264 0983 0283 0164  .d.t.t.|.d.....d
+000002b0: 089c 0264 0a9c 0364 0b8d 0201 0064 0053  ...d...d.....d.S
+000002c0: 0029 0c4e da72 3439 3836 3838 3842 3131  .).N.r4986888B11
+000002d0: 3335 3842 4633 4435 3431 4234 3145 4541  358BF3D541B41EEA
+000002e0: 3544 4145 4345 3143 3645 4646 3634 3133  5DAECE1C6EFF6413
+000002f0: 3041 3435 4643 3842 3943 4134 3846 3345  0A45FC8B9CA48F3E
+00000300: 3045 3032 3436 3343 3939 4335 4145 4443  0E02463C99C5AEDC
+00000310: 3841 3834 3736 3836 4436 3639 4237 4435  8A847686D669B7D5
+00000320: 3437 4331 3846 4534 3438 4643 3531 3131  47C18FE448FC5111
+00000330: 4341 3838 4634 4538 da09 7465 6d70 6f72  CA88F4E8..tempor
+00000340: 6172 79da 0473 6565 64da 0470 6174 687a  ary..seed..pathz
+00000350: 0d70 726f 706f 7361 6c2e 7365 6564 da0b  .proposal.seed..
+00000360: 6865 7861 6465 6369 6d61 6c7a 2070 726f  hexadecimalz pro
+00000370: 706f 7361 6c2e 7072 6976 6174 655f 6b65  posal.private_ke
+00000380: 792e 6865 7861 6465 6369 6d61 6c29 02da  y.hexadecimal)..
+00000390: 0666 6f72 6d61 7472 0f00 0000 7a1f 7072  .formatr....z.pr
+000003a0: 6f70 6f73 616c 2e70 7562 6c69 635f 6b65  oposal.public_ke
+000003b0: 792e 6865 7861 6465 6369 6d61 6c29 0372  y.hexadecimal).r
+000003c0: 0e00 0000 7a0b 7072 6976 6174 6520 6b65  ....z.private ke
+000003d0: 797a 0a70 7562 6c69 6320 6b65 7929 02da  yz.public key)..
+000003e0: 0875 7469 6c69 7a65 73da 0662 7569 6c64  .utilizes..build
+000003f0: 7329 0cda 0770 6174 686c 6962 da04 5061  s)...pathlib..Pa
+00000400: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
+00000410: 7265 6e74 da07 7265 736f 6c76 6572 0400  rent..resolver..
+00000420: 0000 7203 0000 0072 0b00 0000 da02 6f73  ..r....r......os
+00000430: da05 6d6b 6469 72da 1266 6f72 6d5f 7072  ..mkdir..form_pr
+00000440: 6f70 6f73 616c 5f6b 6579 73da 0873 6d6f  oposal_keys..smo
+00000450: 6f74 686c 7929 0372 0e00 0000 da0e 7468  othly).r......th
+00000460: 6973 5f64 6972 6563 746f 7279 da13 7465  is_directory..te
+00000470: 6d70 6f72 6172 795f 6469 7265 6374 6f72  mporary_director
+00000480: 7972 0900 0000 7209 0000 0072 0a00 0000  yr....r....r....
+00000490: da07 6368 6563 6b5f 3115 0000 0073 2600  ..check_1....s&.
+000004a0: 0000 0401 1002 0e01 0802 0a01 0402 0402  ................
+000004b0: 02ff 0e05 02ff 0204 0c01 04fe 0205 0c01  ................
+000004c0: 04fe 04f8 06fc 0416 721f 0000 007a 0763  ........r....z.c
+000004d0: 6865 636b 2031 2912 da07 5f5f 646f 635f  heck 1)...__doc_
+000004e0: 5fda 076f 732e 7061 7468 7202 0000 0072  _..os.pathr....r
+000004f0: 0300 0000 7204 0000 0072 1400 0000 da03  ....r....r......
+00000500: 7379 7372 1900 0000 da23 7265 6379 636c  sysr.....#recycl
+00000510: 696e 672e 6d69 7865 732e 7072 6f70 6f73  ing.mixes.propos
+00000520: 616c 732e 6b65 7973 2e66 6f72 6dda 056d  als.keys.form..m
+00000530: 6978 6573 da09 7072 6f70 6f73 616c 73da  ixes..proposals.
+00000540: 046b 6579 73da 0466 6f72 6d72 1b00 0000  .keys..formr....
+00000550: 7205 0000 0072 0b00 0000 721f 0000 00da  r....r....r.....
+00000560: 0663 6865 636b 7372 0900 0000 7209 0000  .checksr....r...
+00000570: 0072 0900 0000 720a 0000 00da 083c 6d6f  .r....r......<mo
+00000580: 6475 6c65 3e01 0000 0073 1600 0000 0401  dule>....s......
+00000590: 1404 0801 0801 0801 1e02 0802 0802 0806  ................
+000005a0: 0422 08ff                                ."..
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/2_hexadecimal_public_key/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/2_hexadecimal_public_key/status_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 '''
-	python3 insurance.proc.py "modules/proposals/keys/_status/1_hexadecimal_public_key/status_1.py"
+	python3 insurance.proc.py "mixes/proposals/keys/_status/1_hexadecimal_public_key/status_1.py"
 '''
 
 from os.path import dirname, join, normpath
 import pathlib
 import sys
 import os
 
-import recycling.modules.proposals.keys.form as form_proposal_keys
+import recycling.mixes.proposals.keys.form as form_proposal_keys
 
 import shutil
 
 def erase_directory (directory_path):
 	try:
 		shutil.rmtree (directory_path)
 	except Exception:
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/_status/3_hexadecimal_keys/status_1.py` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 '''
-	python3 insurance.proc.py "modules/proposals/keys/_status/3_hexadecimal_keys/status_1.py"
+	python3 insurance.proc.py "mixes/proposals/keys/_status/3_hexadecimal_keys/status_1.py"
 '''
 
 from os.path import dirname, join, normpath
 import pathlib
 import sys
 import os
 
-import recycling.modules.proposals.keys.form as form_proposal_keys
+import recycling.mixes.proposals.keys.form as form_proposal_keys
 
 import shutil
 
 def erase_directory (directory_path):
 	try:
 		shutil.rmtree (directory_path)
 	except Exception:
```

### Comparing `recycling-1.0.0/venues/stages/recycling/modules/proposals/keys/form.py` & `recycling-1.1.0/venues/stages/recycling/mixes/proposals/keys/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 '''
 	seed = "4986888b11358bf3d541b41eea5daece1c6eff64130a45fc8b9ca48f3e0e02463c99c5aedc8a847686d669b7d547c18fe448fc5111ca88f4e8"
 
-	import recycling.modules.proposals.keys.form as form_proposal_keys
+	import recycling.mixes.proposals.keys.form as form_proposal_keys
 	form_proposal_keys.smoothly (
 		#
 		#	inputs, consumes, utilizes
 		#
 		utilizes = {
 			"seed": seed
 		},
@@ -31,18 +31,18 @@
 				"format": "",
 				"path": ""
 			}
 		}
 	)
 '''
 
-import recycling.modules.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
+import recycling.mixes.EEC_448_1.private_key.creator as EEC_448_1_private_key_creator
 
-import recycling.modules.EEC_448_1.public_key.form as form_EEC_448_1_public_key
-import recycling.modules.EEC_448_1.public_key.write as write_EEC_448_1_public_key
+import recycling.mixes.EEC_448_1.public_key.form as form_EEC_448_1_public_key
+import recycling.mixes.EEC_448_1.public_key.write as write_EEC_448_1_public_key
 	
 
 import os
 def write_seed (path, seed_string):
 	if (os.path.exists (path)):
 		raise Exception (f"The path for the seed_string is not available. '{ path }'");
```

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/__book/dlsdkcgl--ai-generated-8315813_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/stage/__book/dlsdkcgl--ai-generated-8315813_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/climate/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/climate/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/climate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/clique/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/clique/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/index-BizSwkP3.css` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/index-BizSwkP3.css`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/index-DIdFDc9G.js` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/index-DIdFDc9G.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/reel-DvvsKiXw.js` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/reel-DvvsKiXw.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-BPO9cr18.js` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-BPO9cr18.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-DSl6fGcC.css` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-DSl6fGcC.css`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/region-gSMgJBY7.js` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/region-gSMgJBY7.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/assets/vanilla-picker-DfFJQbG4.js` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/assets/vanilla-picker-DfFJQbG4.js`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/codesweeper--ai-generated-8311450_1920.jpg` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/codesweeper--ai-generated-8311450_1920.jpg`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/frontend/favicon.ico` & `recycling-1.1.0/venues/stages/recycling/stage/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/__init__.py` & `recycling-1.1.0/venues/stages/recycling/instrument/layer/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 
 
 '''
 
 '''
 
 
-import json
-from os.path import dirname, join, normpath
-import os
-import traceback
 
+
+
+
+#/
+#
+import recycling.instrument.layer.utilities.generate_path_inventory as generate_path_inventory
+import recycling.instrument.climate as instrument_climate
+#
+from .routes import connect_routes
+#
+#
 import rich
 from flask import Flask, request
 import flask_cors
-
-import recycling.stage.layer.utilities.generate_path_inventory as generate_path_inventory
-import recycling.stage.climate as stage_climate
-	
-from .routes import connect_routes
+#
+#
+import json
+from os.path import dirname, join, normpath
+import os
+import traceback
+#
+#\
 
 def build (
 	records = 1
 ):
-	climate = stage_climate.retrieve ()
+	climate = instrument_climate.retrieve ()
 
-	print ("starting stage flask service")
+	print ("starting instrument flask service")
 	rich.print_json (data = {
 		"variables": {
 			"frontend dist": climate ["paths"] ["frontend dist"]
 		}
 	})
 
 	app = Flask (__name__)
```

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/_clique/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/_clique/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/__pycache__/moves.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/__pycache__/moves.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/moves.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/moves.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vibe_generator.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vibe_generator.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vue/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vue/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/routes/vue/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/routes/vue/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/layer/utilities/__pycache__/generate_path_inventory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/layer/utilities/generate_path_inventory.py` & `recycling-1.1.0/venues/stages/recycling/stage/layer/utilities/generate_path_inventory.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/__init__.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/__init__.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/__pycache__/start_layer.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/__pycache__/start_layer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/__pycache__/start_mongo.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/__pycache__/start_mongo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/add_splendor.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/add_splendor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/establish_rules.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/establish_rules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce_Ehh.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/__pycache__/produce_Ehh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/add_splendor.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/add_splendor.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/establish_rules.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/establish_rules.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_1/produce_Ehh.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_1/produce_Ehh.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/establish.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/freshest.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/__pycache__/freshest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/establish.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/establish.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_index/freshest.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_index/freshest.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/__pycache__/enumerate.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/__pycache__/enumerate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/enumerate.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_insights/moves/enumerate.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/receive.cpython-310.pyc` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/scene_moves/escrow/__pycache__/receive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/start_layer.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/start_layer.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/moves/names/start_mongo.py` & `recycling-1.1.0/venues/stages/recycling/stage/moves/names/start_mongo.py`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/venues/stages/recycling/stage/stage.s.HTML` & `recycling-1.1.0/venues/stages/recycling/stage/stage.s.HTML`

 * *Files identical despite different names*

### Comparing `recycling-1.0.0/PKG-INFO` & `recycling-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: recycling
-Version: 1.0.0
+Version: 1.1.0
 Summary: The dreams that found there way to a canvas.
 License: GPL 3.0 + MongoDB SSPL
 Keywords: stories,roads,rollercoasters,motion-motions,motion-moves,motion-pictures,reels,reelity,reality,custom-support-required
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asn1crypto (>=1.5.1,<2.0.0)
 Requires-Dist: aztec-code-generator (>=0.11,<0.12)
 Requires-Dist: biotech (>=1.1.10,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: cryptography (>=42.0.7,<43.0.0)
 Requires-Dist: ecdsa (>=0.19.0,<0.20.0)
 Requires-Dist: ecpy (>=1.2.5,<2.0.0)
+Requires-Dist: fastecdsa (>=2.3.2,<3.0.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: flask-cors (>=4.0.0,<5.0.0)
 Requires-Dist: flask-openapi3 (>=3.1.0,<4.0.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: pyopenssl (>=24.1.0,<25.0.0)
 Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
@@ -32,14 +34,18 @@
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_4/apoplast
 Description-Content-Type: text/markdown
 
 
 
 
+
+
+
+
 ******
 
 Bravo!  You have received a Mercantilism Diploma in "recycling" from   
 the Simulated Parallel Science Universe Fictional Fantasy Orbital Convergence University   
 International Air and Water Embassy Naturalization Department of the Mango Planet
 (the planet that is one ellipse closer to the Sun than Earth's ellipse).
```

