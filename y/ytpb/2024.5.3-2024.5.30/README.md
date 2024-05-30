# Comparing `tmp/ytpb-2024.5.3.tar.gz` & `tmp/ytpb-2024.5.30.tar.gz`

## Comparing `ytpb-2024.5.3.tar` & `ytpb-2024.5.30.tar`

### file list

```diff
@@ -1,140 +1,190 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitattributes
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.readthedocs.yaml
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CHANGELOG.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.5.3/Makefile
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 ytpb-2024.5.3/config.toml.example
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/changelog.rst
--rw-r--r--   0        0        0    24143 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cli.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/contributing.rst
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cookbook.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/index.rst
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/quick.rst
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/reference.rst
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/why.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/index.rst
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/usage.rst
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/index.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.actions.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.cache.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.download.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.errors.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.fetchers.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.info.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.locate.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.merge.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.playback.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.representations.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.segment.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.streams.rst
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.5.3/etc/Containerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__main__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/api.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cache.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/conditional.py
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/config.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/download.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/fetchers.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/ffmpeg.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/info.py
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/locate.py
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/merge.py
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/playback.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/representations.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/segment.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/streams.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/types.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/__init__.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/capture.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/compose.py
--rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/download.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/__init__.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/common.py
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/options.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/__init__.py
--rw-r--r--   0        0        0    17114 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/capture.py
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/download.py
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/date.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/other.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/remote.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/url.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/conftest.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/helpers.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_cache.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_download.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_fetchers.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_info.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_locate.py
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_merge.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback_session.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_representations.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_segment.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_streams.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/__init__.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_compose.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_download.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/conftest.py
--rw-r--r--   0        0        0    60600 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_download_command.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/__init__.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/test_frame_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/__init__.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py
--rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/info-1695928670.json
--rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/manifest-1695928670.mpd
--rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/webpage-1695928670.html
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd_with_no_streams.out
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_dry_run_option.out
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_cut_option.out
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_refresh_mpd.out
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4
--rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4
--rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4
--rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4
--rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4
--rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i244.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_date.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_path.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_remote.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_url.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.5.3/LICENSE
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 ytpb-2024.5.3/README.rst
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 ytpb-2024.5.3/pyproject.toml
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 ytpb-2024.5.3/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ytpb-2024.5.30/.gitattributes
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.5.30/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.5.30/.readthedocs.yaml
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 ytpb-2024.5.30/CHANGELOG.md
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.5.30/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.5.30/Makefile
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 ytpb-2024.5.30/config.toml.example
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/changelog.rst
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/cli.rst
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/contributing.rst
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/cookbook.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/index.rst
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/questions.rst
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/quick.rst
+-rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/reference.rst
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/why.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/_templates/sidebarintro.html
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/index.rst
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/usage.rst
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/index.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.actions.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.cache.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.download.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.errors.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.fetchers.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.info.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.locate.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.merge.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.playback.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.representations.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.segment.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.30/docs/package/api/ytpb.streams.rst
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 ytpb-2024.5.30/etc/0001-Revert-http-Send-a-Range-header-even-when-the-offset.patch
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 ytpb-2024.5.30/etc/0002-Revert-http-Improve-handling-of-Content-Range-with-T.patch
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 ytpb-2024.5.30/etc/Containerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/__main__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/_version.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/api.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cache.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/conditional.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/download.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/fetchers.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/info.py
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/locate.py
+-rw-r--r--   0        0        0    13308 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/merge.py
+-rw-r--r--   0        0        0    24265 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/playback.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/representations.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/segment.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/streams.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/types.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/actions/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/actions/capture.py
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/actions/compose.py
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/actions/download.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/__init__.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/common.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/config.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/formats.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/options.py
+-rw-r--r--   0        0        0     8900 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/parameters.py
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/templating.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/commands/__init__.py
+-rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/commands/capture.py
+-rw-r--r--   0        0        0    25657 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/commands/download.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/commands/mpd.py
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/utils/date.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/cli/utils/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/utils/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/utils/ffmpeg.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/utils/other.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/utils/remote.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.5.30/src/ytpb/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/__init__.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/conftest.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/helpers.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_cache.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_download.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_fetchers.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_info.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_locate.py
+-rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_merge.py
+-rw-r--r--   0        0        0    11437 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_playback.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_playback_session.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_representations.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_segment.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_streams.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/actions/__init__.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/actions/test_compose.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/actions/test_download.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/conftest.py
+-rw-r--r--   0        0        0    61831 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/test_download_command.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/test_formats.py
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/test_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/capture/__init__.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/capture/test_frame_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/mpd/__init__.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/mpd/test_compose_command.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/mpd/test_refresh_command.py
+-rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/utils/test_date.py
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/cli/utils/test_path.py
+-rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/info-1695928670.json
+-rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/manifest-1695928670.mpd
+-rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/webpage-1695928670.html
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Linux.out
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Windows.out
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Darwin.out
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Linux.out
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Windows.out
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Linux.out
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Windows.out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd_with_no_streams-Darwin.out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd_with_no_streams-Linux.out
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_compose_mpd_with_no_streams-Windows.out
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_cut_option-Darwin.out
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_cut_option-Linux.out
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_cut_option-Windows.out
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Darwin.out
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Linux.out
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Windows.out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Darwin.out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Linux.out
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Windows.out
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Darwin.out
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Linux.out
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Windows.out
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Windows.out
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_dry_run_option-Darwin.out
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_dry_run_option-Linux.out
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_dry_run_option-Windows.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_cut_option-Darwin.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_cut_option-Linux.out
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_cut_option-Windows.out
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_merge_option-Darwin.out
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_merge_option-Linux.out
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_no_merge_option-Windows.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_refresh_mpd-Darwin.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_refresh_mpd-Linux.out
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/expected/test_refresh_mpd-Windows.out
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/gap-cases/gap-case-1-fixture.csv
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/gap-cases/gap-case-2-fixture.csv
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/gap-cases/gap-case-3-fixture.csv
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959120.i140.mp4
+-rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959120.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959121.i140.mp4
+-rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959121.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959122.i140.mp4
+-rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959122.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959123.i140.mp4
+-rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959123.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959203.i140.mp4
+-rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/data/segments/7959203.i244.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/utils/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/utils/test_remote.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.5.30/tests/utils/test_url.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 ytpb-2024.5.30/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.5.30/LICENSE
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 ytpb-2024.5.30/README.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 ytpb-2024.5.30/pyproject.toml
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 ytpb-2024.5.30/PKG-INFO
```

### Comparing `ytpb-2024.5.3/CHANGELOG.rst` & `ytpb-2024.5.30/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,117 @@
-Changelog
-#########
+# Changelog
 
-Versions follow `Calendar Versioning`_ with the ``YYYY.M.D`` scheme.
+Versions follow [Calendar Versioning](https://calver.org) with the `YYYY.M.D`
+scheme.
 
-.. _Calendar Versioning: https://calver.org
+## [2024.5.30]
 
-`2024.5.3`_
-***********
+- Make cutting non-default behavior and add the `-c / --cut` option
+- Start using Jinja templates for output path templates
+- Accept long option names for default option values in the config file
+- Change the format of composed MPEG-DASH MPDs from compact to full (https://github.com/xymaxim/ytpb/issues/12)
+- Remove `--from-playback` from `ytpb download`
+- Rename `-X / --dry-run` to `-x / --dry-run`
+- Rename `--segments-output-dir` to `-s / --segments-output-dir`
+
+## [2024.5.12]
+
+- Add Windows support ([#11](https://github.com/xymaxim/ytpb/issues/11))
+- Fix not cutting issue introduced in v2024.5.3
+  ([b0e4f3d](https://github.com/xymaxim/ytpb/commit/b0e4f3d10c6aad7401716f49e681bb97c2ee6d03))
+- Replace all `ffprobe` calls to `av`'s function calls
+- Move `ytpb.ffmpeg` to `ytpb.utils.ffmpeg`
+- Add CI workflows to create test expectation files, build Windows binaries,
+  publish on PyPI, and draft a GitHub release
+- Run CI tests on Linux, MacOS, and Windows
+- Start using dynamic versioning via `hatch-vcs`
+- Convert CHANGELOG from ReST to Markdown format
+- Apply patches from files in Containerfile to avoid merge conflicts
 
-- Add support for resumable downloads (`#13
-  <https://github.com/xymaxim/ytpb/pull/13>`__)
+## [2024.5.3]
+
+- Add support for resumable downloads
+  ([#13](https://github.com/xymaxim/ytpb/pull/13))
 - Change the segments output directory from the run temporary directory to a
   directory under the current working one
-- Add ``--ignore-resume``, ``-S / --keep-segments``, and
-  ``--segments-output-dir`` options
-- Change the default output path to ``<title>_<id>_<input_start_date>``
-- Rename the ``--no-cleanup`` option to ``--keep-temp``
-- Replace the ``--preview`` option with ``--preview-start`` and
-  ``--preview-end``
+- Add `--ignore-resume`, `-S / --keep-segments`, and `--segments-output-dir`
+  options
+- Change the default output path to `<title>_<id>_<input_start_date>`
+- Rename the `--no-cleanup` option to `--keep-temp`
+- Replace the `--preview` option with `--preview-start` and `--preview-end`
 
-`2024.4.20`_
-************
+## [2024.4.20]
 
 - Fix wrong frame rate values of the video-only merged files when boundary
-  segments are cut and encoded with H.264 (`e1120bf
-  <https://github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606>`__)
-- Write metadata tags with basic and rewind information to merged files (`aa7adf1
-  <https://github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba>`__)
-- Add the ``--no-metadata`` option to not write metadata tags to merged files
-
-`2024.4.12`_
-************
-
-- Add the `Python package
-  <https://ytpb.readthedocs.io/en/latest/package/index.html>`__ page with the
-  basic usage and API reference
-- Add the ``--version`` CLI option to show version number
-- Add :attr:`ytpb.representations.RepresentationInfo.type` property
-- Add :attr:`ytpb.playback.RewindInterval.duration` and
-  :attr:`~ytpb.playback.RewindInterval.sequences` properties
-- Accept Unix timestamps for moments and intervals (`b7dcbaf
-  <https://github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb>`__)
-- Add :class:`ytpb.playback.RewindTreeMap` to keep rewind history (`91fd078
-  <https://github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8>`__)
-
-Breaking changes
-================
-
-- Rename :mod:`ytpb.mpd` to :mod:`ytpb.representations`
-- Rename :mod:`ytpb.exceptions` to :mod:`ytpb.errors`
-- Rename :meth:`ytpb.playback.Playback.get_downloaded_segment` to
-  :meth:`~ytpb.playback.Playback.get_segment`
-- Rename :meth:`ytpb.representations.extract_representations_info` to
-  :meth:`~ytpb.representations.extract_representations`
-- Remove unused :meth:`ytpb.representations.strip_manifest`
+  segments are cut and encoded with H.264
+  ([e1120bf](https://github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606))
+- Write metadata tags with basic and rewind information to merged files
+  ([aa7adf1](https://github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba))
+- Add the `--no-metadata` option to not write metadata tags to merged files
+
+## [2024.4.12]
+
+- Add the [Python
+  package](https://ytpb.readthedocs.io/en/latest/package/index.html) page with
+  the basic usage and API reference
+- Add the `--version` CLI option to show version number
+- Add `ytpb.representations.RepresentationInfo.type` property
+- Add `ytpb.playback.RewindInterval.duration` and
+  `ytpb.playback.RewindInterval.sequences` properties
+- Accept Unix timestamps for moments and intervals
+  ([b7dcbaf](https://github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb))
+- Add `ytpb.playback.RewindTreeMap` to keep rewind history
+  ([91fd078](https://github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8))
+
+### Breaking changes
+
+- Rename `ytpb.mpd` to `ytpb.representations`
+- Rename `ytpb.exceptions` to `ytpb.errors`
+- Rename `ytpb.playback.Playback.get_downloaded_segment` to
+  `ytpb.playback.Playback.get_segment`
+- Rename `ytpb.representations.extract_representations_info` to
+  `ytpb.representations.extract_representations`
+- Remove unused `ytpb.representations.strip_manifest`
 
-`2024.3.27`_
-************
+## [2024.3.27]
 
 - Add Containerfile with instructions to build patched FFmpeg and MPV
 
-Breaking changes
-================
-
-- Change return value of
-  :meth:`ytpb.locate.SegmentLocator.find_sequence_by_time` to
-  :class:`~ytpb.locate.LocateResult`
+### Breaking changes
 
-`2024.3.16`_
-************
+- Change return value of `ytpb.locate.SegmentLocator.find_sequence_by_time` to
+  `ytpb.locate.LocateResult`
 
-- Add options to dump base (``--dump-base-urls``) and segment
-  (``--dump-segment-urls``) URLs to the ``download`` command (`#10
-  <https://github.com/xymaxim/ytpb/pull/10>`__)
-- Add the `Cookbook`_ documentation page
+## [2024.3.16]
 
-.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
+- Add options to dump base (`--dump-base-urls`) and segment
+  (`--dump-segment-urls`) URLs to the `download` command
+  ([#10](https://github.com/xymaxim/ytpb/pull/10))
+- Add the [Cookbook](https://ytpb.readthedocs.io/en/latest/cookbook.html)
+  documentation page
 
-`2024.3.13`_
-************
+## [2024.3.13]
 
 - Add the config.toml.example file
-- Add ability to use `custom aliases`_ in format specs
-- Add `aliases`_ for itags (``@<itag>``) as `dynamic aliases`_
+- Add ability to use [custom
+  aliases](https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases)
+  in format specs
+- Add [aliases](https://ytpb.readthedocs.io/en/latest/reference.html#itags) for
+  itags (`@<itag>`) as [dynamic
+  aliases](https://ytpb.readthedocs.io/en/latest/reference.html#aliases)
 - Fix allowing empty representations in the CLI commands
 
-.. _custom aliases: https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases
-.. _aliases: https://ytpb.readthedocs.io/en/latest/reference.html#itags
-.. _dynamic aliases: https://ytpb.readthedocs.io/en/latest/reference.html#aliases
-
-`2024.3.9`_
-***********
+## [2024.3.9]
 
 - Add the CHANGELOG file and documentation page
-- Change the first segment locating step: don't limit it to two jumps (`#8
-  <https://github.com/xymaxim/ytpb/pull/8>`__)
+- Change the first segment locating step: don\'t limit it to two jumps
+  ([#8](https://github.com/xymaxim/ytpb/pull/8))
 
-.. _2024.5.3: https://github.com/xymaxim/ytpb/compare/v2024.4.20..v2024.5.3
-.. _2024.4.20: https://github.com/xymaxim/ytpb/compare/v2024.4.12..v2024.4.20
-.. _2024.4.12: https://github.com/xymaxim/ytpb/compare/v2024.3.27..v2024.4.12
-.. _2024.3.27: https://github.com/xymaxim/ytpb/compare/v2024.3.16..v2024.3.27
-.. _2024.3.16: https://github.com/xymaxim/ytpb/compare/v2024.3.13..v2024.3.16
-.. _2024.3.13: https://github.com/xymaxim/ytpb/compare/v2024.3.9..v2024.3.13
-.. _2024.3.9: https://github.com/xymaxim/ytpb/compare/v2024.3.7..v2024.3.9
+[Unreleased]: https://github.com/xymaxim/ytpb/compare/v2024.5.12..HEAD
+[2024.5.12]: https://github.com/xymaxim/ytpb/compare/v2024.5.3..v2024.5.12
+[2024.5.3]: https://github.com/xymaxim/ytpb/compare/v2024.4.20..v2024.5.3
+[2024.4.20]: https://github.com/xymaxim/ytpb/compare/v2024.4.12..v2024.4.20
+[2024.4.12]: https://github.com/xymaxim/ytpb/compare/v2024.3.27..v2024.4.12
+[2024.3.27]: https://github.com/xymaxim/ytpb/compare/v2024.3.16..v2024.3.27
+[2024.3.16]: https://github.com/xymaxim/ytpb/compare/v2024.3.13..v2024.3.16
+[2024.3.13]: https://github.com/xymaxim/ytpb/compare/v2024.3.9..v2024.3.13
+[2024.3.9]: https://github.com/xymaxim/ytpb/compare/v2024.3.7..v2024.3.9
```

#### html2text {}

```diff
@@ -1,56 +1,68 @@
-Changelog ######### Versions follow `Calendar Versioning`_ with the
-``YYYY.M.D`` scheme. .. _Calendar Versioning: https://calver.org `2024.5.3`_
-*********** - Add support for resumable downloads (`#13
-github.com/xymaxim/ytpb/pull/13>`__) - Change the segments output directory
-from the run temporary directory to a directory under the current working one -
-Add ``--ignore-resume``, ``-S / --keep-segments``, and ``--segments-output-
-dir`` options - Change the default output path to ``
-_`` - Rename the ``--no-cleanup`` option to ``--keep-temp`` - Replace the ``--
-preview`` option with ``--preview-start`` and ``--preview-end`` `2024.4.20`_
-************ - Fix wrong frame rate values of the video-only merged files when
-boundary segments are cut and encoded with H.264 (`e1120bf
-github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606>`__) -
-Write metadata tags with basic and rewind information to merged files (`aa7adf1
-github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba>`__) -
-Add the ``--no-metadata`` option to not write metadata tags to merged files
-`2024.4.12`_ ************ - Add the `Python package
-ytpb.readthedocs.io/en/latest/package/index.html>`__ page with the basic usage
-and API reference - Add the ``--version`` CLI option to show version number -
-Add :attr:`ytpb.representations.RepresentationInfo.type` property - Add :attr:
-`ytpb.playback.RewindInterval.duration` and :attr:
-`~ytpb.playback.RewindInterval.sequences` properties - Accept Unix timestamps
-for moments and intervals (`b7dcbaf
-github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb>`__) -
-Add :class:`ytpb.playback.RewindTreeMap` to keep rewind history (`91fd078
-github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8>`__)
-Breaking changes ================ - Rename :mod:`ytpb.mpd` to :mod:
-`ytpb.representations` - Rename :mod:`ytpb.exceptions` to :mod:`ytpb.errors` -
-Rename :meth:`ytpb.playback.Playback.get_downloaded_segment` to :meth:
-`~ytpb.playback.Playback.get_segment` - Rename :meth:
-`ytpb.representations.extract_representations_info` to :meth:
-`~ytpb.representations.extract_representations` - Remove unused :meth:
-`ytpb.representations.strip_manifest` `2024.3.27`_ ************ - Add
-Containerfile with instructions to build patched FFmpeg and MPV Breaking
-changes ================ - Change return value of :meth:
-`ytpb.locate.SegmentLocator.find_sequence_by_time` to :class:
-`~ytpb.locate.LocateResult` `2024.3.16`_ ************ - Add options to dump
-base (``--dump-base-urls``) and segment (``--dump-segment-urls``) URLs to the
-``download`` command (`#10
-github.com/xymaxim/ytpb/pull/10>`__) - Add the `Cookbook`_ documentation page
-.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html `2024.3.13`_
-************ - Add the config.toml.example file - Add ability to use `custom
-aliases`_ in format specs - Add `aliases`_ for itags (``@``) as `dynamic
-aliases`_ - Fix allowing empty representations in the CLI commands .. _custom
-aliases: https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases ..
-_aliases: https://ytpb.readthedocs.io/en/latest/reference.html#itags ..
-_dynamic aliases: https://ytpb.readthedocs.io/en/latest/reference.html#aliases
-`2024.3.9`_ *********** - Add the CHANGELOG file and documentation page -
-Change the first segment locating step: don't limit it to two jumps (`#8
-github.com/xymaxim/ytpb/pull/8>`__) .. _2024.5.3: https://github.com/xymaxim/
-ytpb/compare/v2024.4.20..v2024.5.3 .. _2024.4.20: https://github.com/xymaxim/
-ytpb/compare/v2024.4.12..v2024.4.20 .. _2024.4.12: https://github.com/xymaxim/
-ytpb/compare/v2024.3.27..v2024.4.12 .. _2024.3.27: https://github.com/xymaxim/
-ytpb/compare/v2024.3.16..v2024.3.27 .. _2024.3.16: https://github.com/xymaxim/
-ytpb/compare/v2024.3.13..v2024.3.16 .. _2024.3.13: https://github.com/xymaxim/
-ytpb/compare/v2024.3.9..v2024.3.13 .. _2024.3.9: https://github.com/xymaxim/
-ytpb/compare/v2024.3.7..v2024.3.9
+# Changelog Versions follow [Calendar Versioning](https://calver.org) with the
+`YYYY.M.D` scheme. ## [2024.5.30] - Make cutting non-default behavior and add
+the `-c / --cut` option - Start using Jinja templates for output path templates
+- Accept long option names for default option values in the config file -
+Change the format of composed MPEG-DASH MPDs from compact to full (https://
+github.com/xymaxim/ytpb/issues/12) - Remove `--from-playback` from `ytpb
+download` - Rename `-X / --dry-run` to `-x / --dry-run` - Rename `--segments-
+output-dir` to `-s / --segments-output-dir` ## [2024.5.12] - Add Windows
+support ([#11](https://github.com/xymaxim/ytpb/issues/11)) - Fix not cutting
+issue introduced in v2024.5.3 ([b0e4f3d](https://github.com/xymaxim/ytpb/
+commit/b0e4f3d10c6aad7401716f49e681bb97c2ee6d03)) - Replace all `ffprobe` calls
+to `av`'s function calls - Move `ytpb.ffmpeg` to `ytpb.utils.ffmpeg` - Add CI
+workflows to create test expectation files, build Windows binaries, publish on
+PyPI, and draft a GitHub release - Run CI tests on Linux, MacOS, and Windows -
+Start using dynamic versioning via `hatch-vcs` - Convert CHANGELOG from ReST to
+Markdown format - Apply patches from files in Containerfile to avoid merge
+conflicts ## [2024.5.3] - Add support for resumable downloads ([#13](https://
+github.com/xymaxim/ytpb/pull/13)) - Change the segments output directory from
+the run temporary directory to a directory under the current working one - Add
+`--ignore-resume`, `-S / --keep-segments`, and `--segments-output-dir` options
+- Change the default output path to `
+_` - Rename the `--no-cleanup` option to `--keep-temp` - Replace the `--
+preview` option with `--preview-start` and `--preview-end` ## [2024.4.20] - Fix
+wrong frame rate values of the video-only merged files when boundary segments
+are cut and encoded with H.264 ([e1120bf](https://github.com/xymaxim/ytpb/
+commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606)) - Write metadata tags with
+basic and rewind information to merged files ([aa7adf1](https://github.com/
+xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba)) - Add the `--no-
+metadata` option to not write metadata tags to merged files ## [2024.4.12] -
+Add the [Python package](https://ytpb.readthedocs.io/en/latest/package/
+index.html) page with the basic usage and API reference - Add the `--version`
+CLI option to show version number - Add
+`ytpb.representations.RepresentationInfo.type` property - Add
+`ytpb.playback.RewindInterval.duration` and
+`ytpb.playback.RewindInterval.sequences` properties - Accept Unix timestamps
+for moments and intervals ([b7dcbaf](https://github.com/xymaxim/ytpb/commit/
+b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb)) - Add `ytpb.playback.RewindTreeMap`
+to keep rewind history ([91fd078](https://github.com/xymaxim/ytpb/commit/
+91fd078caf37f31fee167e0c2a20a38aa2badcd8)) ### Breaking changes - Rename
+`ytpb.mpd` to `ytpb.representations` - Rename `ytpb.exceptions` to
+`ytpb.errors` - Rename `ytpb.playback.Playback.get_downloaded_segment` to
+`ytpb.playback.Playback.get_segment` - Rename
+`ytpb.representations.extract_representations_info` to
+`ytpb.representations.extract_representations` - Remove unused
+`ytpb.representations.strip_manifest` ## [2024.3.27] - Add Containerfile with
+instructions to build patched FFmpeg and MPV ### Breaking changes - Change
+return value of `ytpb.locate.SegmentLocator.find_sequence_by_time` to
+`ytpb.locate.LocateResult` ## [2024.3.16] - Add options to dump base (`--dump-
+base-urls`) and segment (`--dump-segment-urls`) URLs to the `download` command
+([#10](https://github.com/xymaxim/ytpb/pull/10)) - Add the [Cookbook](https://
+ytpb.readthedocs.io/en/latest/cookbook.html) documentation page ## [2024.3.13]
+- Add the config.toml.example file - Add ability to use [custom aliases](https:
+//ytpb.readthedocs.io/en/latest/reference.html#custom-aliases) in format specs
+- Add [aliases](https://ytpb.readthedocs.io/en/latest/reference.html#itags) for
+itags (`@`) as [dynamic aliases](https://ytpb.readthedocs.io/en/latest/
+reference.html#aliases) - Fix allowing empty representations in the CLI
+commands ## [2024.3.9] - Add the CHANGELOG file and documentation page - Change
+the first segment locating step: don\'t limit it to two jumps ([#8](https://
+github.com/xymaxim/ytpb/pull/8)) [Unreleased]: https://github.com/xymaxim/ytpb/
+compare/v2024.5.12..HEAD [2024.5.12]: https://github.com/xymaxim/ytpb/compare/
+v2024.5.3..v2024.5.12 [2024.5.3]: https://github.com/xymaxim/ytpb/compare/
+v2024.4.20..v2024.5.3 [2024.4.20]: https://github.com/xymaxim/ytpb/compare/
+v2024.4.12..v2024.4.20 [2024.4.12]: https://github.com/xymaxim/ytpb/compare/
+v2024.3.27..v2024.4.12 [2024.3.27]: https://github.com/xymaxim/ytpb/compare/
+v2024.3.16..v2024.3.27 [2024.3.16]: https://github.com/xymaxim/ytpb/compare/
+v2024.3.13..v2024.3.16 [2024.3.13]: https://github.com/xymaxim/ytpb/compare/
+v2024.3.9..v2024.3.13 [2024.3.9]: https://github.com/xymaxim/ytpb/compare/
+v2024.3.7..v2024.3.9
```

### Comparing `ytpb-2024.5.3/CONTRIBUTING.rst` & `ytpb-2024.5.30/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/docs/cli.rst` & `ytpb-2024.5.30/docs/cli.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Command line application
 ########################
 
 This section describes using the Ytpb command line application: from an overview
 and usage of commands to configuring and advanced use cases.
 
 .. contents:: Contents
-   :depth: 2
+   :depth: 3
    :backlinks: top
    :local:
 
 Overview
 ********
 
 Synopsis
@@ -193,25 +193,14 @@
 
 where ``<timestamp> = "@"<epoch-seconds>``:
 
 The date and time interval can also be specified with Unix timestamps as: ::
 
    $ ytpb download -i @1704190800/@1704190830 ...
 
-*'Now' keyword*
-^^^^^^^^^^^^^^^
-
-* ``-i/--interval <start>/now``
-
-To refer to the current moment, the end part accepts the ``now`` keyword: ::
-
-  $ ytpb download -i 20240102T1020+00/now ...
-
-(To be exact, it refers to the last available media segment.)
-
 B. Using duration
 -----------------
 
 * ``-i/--interval <start>/<duration>`` or
 
 * ``-i/--interval <duration>/<end>``,
 
@@ -228,17 +217,66 @@
 
   # Specified by a start and a duration
   $ ytpb download -i 2024-01-02T10:20:00+00/PT30S ...
 
   # Specified by a duration and an end
   $ ytpb download -i PT30S/2024-01-02T10:20:30+00 ...
 
+C. Using sequence numbers
+-------------------------
+
+* ``-i/--interval <sequence-number>/<sequence-number>``
+
+Besides dates, you can specify the sequence number (positive, starting from 0)
+of an MPEG-DASH `media segment
+<https://dashif-documents.azurewebsites.net/Guidelines-TimingModel/master/Guidelines-TimingModel.html#media-segment/>`_
+to refer to a specific point in a live stream. Usually, sequence numbers are
+used when a segment has already been previously determined.
+
+For example, an interval from the beginning to segment 100: ::
+
+  $ ytpb download -i 0/100 ...
+
+Sequence numbers can also be combined with other types: ::
+
+  $ ytpb download -i 0/2024-01-02T10:20:30+00 ...
+  $ ytpb download -i 0/PT30S ...
+  $ ytpb download -i 0/now ...
+
+D. Using keywords
+-----------------
+
+*'Earliest' keyword*
+^^^^^^^^^^^^^^^^^^^^
+
+* ``-i/--interval earliest/<end>``
+
+To refer to the earliest available moment, the start part accepts the ``earliest``
+keyword::
+
+  $ ytpb download -i earliest/PT30S ...
+
+It could refer to the beginning of a stream (e.g., the very first media segment)
+or the earliest available segment if a stream lasts longer than the time
+available to rewind.
+
+*'Now' keyword*
+^^^^^^^^^^^^^^^
+
+* ``-i/--interval <start>/now``
+
+To refer to the current moment, the end part accepts the ``now`` keyword: ::
+
+  $ ytpb download -i 20240102T1020+00/now ...
+
+To be exact, it refers to the last available media segment.
+
 .. _Preview mode:
 
-C. Preview mode
+E. Preview mode
 ---------------
 
 * ``--interval <start>/<end> --preview-start``
 * ``--interval <start>/<end> --preview-end``
 * ``--interval <start>/.. --preview-start``
 * ``--interval ../<end> --preview-end``
 
@@ -258,305 +296,151 @@
 
 By default, the output preview duration varies from 10 to 10 + one segment
 duration seconds. The imprecision is due to the reliance on the full-length,
 uncut end segment (to reduce merging time). The minimal preview duration value
 can be changed via the ``general.preview_duration`` field in the ``config.toml``
 file.
 
-D. Using sequence numbers
--------------------------
-
-* ``-i/--interval <sequence-number>/<sequence-number>``
-
-Besides dates, you can specify the sequence number (positive, starting from 0)
-of an MPEG-DASH `media segment
-<https://dashif-documents.azurewebsites.net/Guidelines-TimingModel/master/Guidelines-TimingModel.html#media-segment/>`_
-to refer to a specific point in a live stream. Usually, sequence numbers are
-used when a segment has already been previously determined.
-
-For example, an interval from the beginning to segment 100: ::
-
-  $ ytpb download -i 0/100 ...
-
-Sequence numbers can also be combined with other types: ::
-
-  $ ytpb download -i 0/2024-01-02T10:20:30+00 ...
-  $ ytpb download -i 0/PT30S ...
-  $ ytpb download -i 0/now ...
-
 Compatibility table
 -------------------
 
 .. table:: **Table:** Interval parts compatibility
 
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   |                           | Date and time | Time | Duration | Replacing components | Sequence number | 'Now', '..' |
-   |                           | / Timestamp   |      |          |                      |                 |             |
-   +===========================+===============+======+==========+======================+=================+=============+
-   | Date and time / Timestamp |       Y       |  Y   |    Y     |          Y           |        Y        |      Y      |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Time                      |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Duration                  |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Replacing components      |       Y       | *N*  |   *N*    |         *N*          |       *N*       |     *N*     |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Sequence number           |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | 'Now', '..'               |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
-   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   |                           | Date and time | Time | Duration | Replacing components | Sequence number | 'Earliest' | 'Now', '..' |
+   |                           | / Timestamp   |      |          |                      |                 |            |             |
+   +===========================+===============+======+==========+======================+=================+============+=============+
+   | Date and time / Timestamp |       Y       |  Y   |    Y     |          Y           |        Y        |      Y     |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | Time                      |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y     |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | Duration                  |       Y       |  Y   |   *N*    |         *N*          |        Y        |      Y     |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | Replacing components      |       Y       | *N*  |   *N*    |         *N*          |       *N*       |     *N*    |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | Sequence number           |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y     |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | 'Earliest'                |       Y       |  Y   |    Y     |         *N*          |        Y        |     *N*    |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
+   | 'Now', '..'               |       Y       |  Y   |   *N*    |         *N*          |        Y        |      Y     |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+------------+-------------+
 
 Specifying formats
 ==================
 
 Now let's look at the ``-af/--audio-format(s)`` and ``-vf/--video-format(s)``
-options. It accepts *format spec* string, a query expression used to select the
-desired formats (MPEG-DASH `representations
+options. They accept the *format spec* string, a query expression used to select
+the desired formats (MPEG-DASH `representations
 <https://dashif-documents.azurewebsites.net/Guidelines-TimingModel/master/Guidelines-TimingModel.html#representations/>`_,
-to be exact).
-
-Representations describe different versions of the content and are
-characterized by attributes, such as itags (format codes), resolutions, used
+to be exact), which are characterized by the itag values, qualities, used
 codecs, etc.
 
-See :ref:`reference:Format spec` for more information on format specs: their
-grammar, aliases, and functions.
-
-Some examples
--------------
+See :ref:`reference:Format spec` for the grammar, aliases, and functions.
 
-*Conditional expressions and lookup attributes*
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Conditionals and lookup attributes
+----------------------------------
 
-The ``itag`` values as format codes uniquely determine representations. For
-example, providing the format spec in the form of a conditional expression as
-below gives us a very specific audio stream: ::
+The itag values as format codes uniquely determine representations. For example,
+providing a format spec in the form of a conditional expression as below gives
+us a very specific audio stream:
 
-  $ ytpb download -af 'itag eq 140' ...
+.. code:: sh
 
-Or, with the following logical condition, one of two video streams: ::
+   $ ytpb download -af 'itag = 140' -vf none ...
 
-  $ ytpb download -vf 'itag eq 271 or itag eq 248' ...
-
-The specific audio and video ``itag`` values for a live stream can be seen in
-the *Stats for nerds* popup in the browser. To show all available DASH-specific
+The audio and video itag values for a playing live stream can be seen in the
+*Stats for nerds* popup in the browser. To show all available MPEG DASH-specific
 formats, running the `yt-dlp <https://github.com/yt-dlp/yt-dlp/>`_ program is
-helpful: ::
+helpful::
 
   $ yt-dlp --live-from-start -F <STREAM>
 
-Here are some other examples of format specs with lookup attributes (see
-:ref:`reference:Attributes`) and a function: ::
+Here are other examples using other lookup :ref:`attributes
+<reference:Attributes>` and logical conditions:
 
-  $ ytpb download -vf 'best(format eq mp4 and [frame_rate eq 60 or frame_rate eq 30])' ...
-  $ ytpb mpd compose -vf 'format eq webm and height le 1080 and frame_rate eq 30' ...
+.. code:: sh
 
+   $ ytpb download -vf 'best(format = mp4 and frame_rate = 30)' ...
+   $ ytpb mpd compose -vf 'codecs = vp9 and [height = 1080 or height = 720]' ...
 
-Note that the ``download`` command requires the query result to be
-non-ambiguous, with one representation per query.
+(Note that all commands except ``mpd compose`` require query results to be
+non-ambiguous, with one representation per query. This is where the ``best()``
+function can be used to limit query results.)
 
-*Using aliases*
-^^^^^^^^^^^^^^^
+*Using format spec aliases*
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-:ref:`reference:Aliases` allow defining a part or whole format spec for
-different cases and make expressions much shorter. For example: ::
+:ref:`reference:Aliases` allow defining and use of a named condition (or
+conditions) and make expressions much shorter and easier to understand. For
+example, using the built-in aliases:
 
-  $ ytpb download -vf 'best(@mp4 and @30fps)' ...
+.. code:: sh
 
-.. _Default format values:
+   $ ytpb download -vf 'best(@mp4 and @30fps)' ...
 
-Default values
---------------
+.. _Default format values:
 
-The format specs can be provided using the following ways (in order of
-increasing priority): (a) using the default, built-in option values, (b) parsing
-custom, user-defined :ref:`configuration <Configuring>` file, ``config.toml``, and (c) via ``-af/--audio-format(s)`` and
-``-vf/--video-format(s)`` options.
+Default option values
+---------------------
 
-The default option values are as follows:
+The command options can be ommited and the default, built-in values listed below
+will be used. As part of :ref:`Configuring`, they can be overriden.
 
 .. code:: TOML
 
-	  [options.download]
-	  audio_format = "@140"
-	  video_format = "best(@mp4 and <=1080p and @30fps)"
-
-          [options.capture.frame]
-	  video_format = "best(@mp4 and @30fps)"
-
-          [options.capture.timelapse]
-	  video_format = "best(@mp4 and @30fps)"
-
-	  [options.mpd.compose]
-	  audio_formats = "@140"
-	  video_formats = "@webm and [@720p or @1080p] and @30fps"
+   [options.download]
+   audio_format = "itag = 140"
+   video_format = "best(@avc1 and @<=1080p and @30fps)"
+
+   [options.capture.frame]
+   video_format = "best(@30fps)"
+
+   [options.capture.timelapse]
+   video_format = "best(@30fps)"
+
+   [options.mpd.compose]
+   audio_formats = "itag = 140"
+   video_formats = "@vp9 and [@1080p or @720p] and @30fps"
 
 Specifying output name
 ======================
 
-There are two options to change the output naming: (a) specify a full output
-path, (b) provide a template output path (both without extension). The extension
-will be automatically determined during the merging step.
-
-Specify values directly via the ``-o / --output`` option::
-
-  $ ytpb download -o '<title>_<input_start_date>' ... && ls
-  $ Stream-Title_20240102T102000+00.mp4
-
-Or set default option values in the ``config.toml`` file::
-
-  [options.download]
-  output = <title>_<input_start_date>
-
-See :ref:`reference:Output name context` for the available template variables.
-
-Formatting titles
------------------
-
-Titles can be formatted to adapt them for the output name: set maximum length,
-normalize characters, change case, etc.
-
-See the corresponding ``[output.title]`` section in ``config.toml``.
-
-*Available styles*
-^^^^^^^^^^^^^^^^^^
-
-Two styles are available: ``original`` and ``custom``.
-
-.. collapse:: Click here for details on available styles...
-
-   Let's consider the following titles as original:
-
-   1. FRANCE 24 – EN DIRECT – Info et actualités internationales en continu 24h/24
-   2. 【LIVE】新宿駅前の様子 Shinjuku, Tokyo JAPAN【ライブカメラ】 | TBS NEWS DIG
-
-   .. raw:: html
-
-            <h6><code>original</code></h6>
-
-   An original title with unallowed symbols replaced. Allows Unicode characters.
-
-   .. code:: TOML
-
-             [output.title]
-             style = "original"
-
-   1. ``FRANCE 24 – EN DIRECT – Info et actualités internationales en continu 24h-24``
-   2. ``【LIVE】新宿駅前の様子 Shinjuku, Tokyo JAPAN【ライブカメラ】 | TBS NEWS DIG``
-
-   .. raw:: html
+By default, merged files are saved in the current working directory with
+names composed of the adjusted title, video ID and formatted input start
+date::
 
-      <h6><code>custom</code></h6>
+  $ ytpb download -i PT30S/20240102T102030+00 abcdefgh123 && ls
+  Stream-title_abcdefgh123_20240102T102000+00.mkv
 
-   Format an original title with settings from the ``[output.title.custom]``
-   section: reduce length, convert to ASCII-only characters, make
-   POSIX-compatible, make lowercase.
+There are several ways to change the output naming: (a) provide a full output
+path or (b) provide a template output path (c) change the default corresponding
+configuration value. All are without extension: the extension will be
+automatically determined during the merging step.
 
-   *Shortening titles*. For example, to shorten the title length (by truncating at
-   word boundaries) and keep Unicode characters, the following settings:
+(A) Provide a full value directly via the ``-o / --output`` option::
 
-   .. code:: TOML
+      $ ytpb download -o output/path ... && ls output/*
+      output/path.mkv
 
-             [output.title]
-             style = "custom"
+(B) Provide a template value via the ``-o / --output`` option::
 
-             [output.title.custom]
-             max_length = 30
-             characters = "unicode"
+      $ ytpb download -o '{{ title|adjust }}_{{ input_start_date|isodate }}' ... && ls
+      Stream-title_20240102T102000+00.mkv
 
-   will produce:
+    See :ref:`Templating` for templating and available variables.
 
-   1. ``FRANCE 24 — EN DIRECT — Info et actualités``
-   2. ``【LIVE】新宿駅前の様子 Shinjuku, Tokyo``
+(C) Change the default option value in the ``config.toml`` file:
 
-   *Converting to ASCII-only*. To convert all characters to ASCII-only, the following:
+    .. code:: TOML
 
-   .. code:: TOML
+       [options.download]
+       output = "{{ title|adjust }}_{{ input_start_date|isodate }}"
 
-             [output.title.custom]
-             characters = "ascii"
-
-   will produce:
-
-   1. ``FRANCE 24 -- EN DIRECT -- Info et actualites internationales en continu 24h-24``
-   2. ``[(LIVE)] Xin Su Yi Qian noYang Zi Shinjuku, Tokyo JAPAN[(raibukamera)] | TBS NEWS DIG``
-
-   *Making POSIX-compliant*. To make the output filename POSIX-compliant and
-   lowercase it, the following:
-
-   .. code:: TOML
-
-             [output.title.custom]
-             max_length = 50
-             separator = "-"
-             characters = "posix"
-             lowercase = true
-
-   will produce:
-
-   1. ``france-24--en-direct--info-et-actualites-internationales-en-continu-24h-24``
-   2. ``live-xin-su-yi-qian-noyang-zi-shinjuku-tokyo-japan-raibukamera-tbs-news-dig``
-
-Formatting dates
-----------------
-
-The date formatting can be changed via the ``output.date.styles`` field in the
-``config.toml`` file. The default set of styles (``"basic,reduced,hh"``)
-corresponds to the basic representation with the reduced precision. Some other
-examples:
-
-.. code:: TOML
-
-	  [output.date]
-	  # 2024-01-02T10:20:00+00:00
-	  styles = "extended,complete,hhmm"
-
-	  # 20240102T102000+00
-	  styles = "basic,complete,hh"
-
-	  # 20240102T1020Z
-          # 20240102T1220+02
-	  styles = "basic,reduced,z"
-
-Writing metadata tags
-=====================
-
-*Related command:* ``ytpb download``
-
-By default, metadata tags will be added to an output excerpt file. Use the
-``--no-metadata`` option to disable it.
-
-.. table:: Metadata tags overview
-
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | Tag                       | Description                   |                   Example                   |
-   +===========================+===============================+=============================================+
-   | ``title``                 | Video's title                 | Stream Title                                |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``author``                | Video's channel name          | Author or Channel Name                      |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``comment``               | YouTube video URL             | https://www.youtube.com/watch?v=abcdefgh123 |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``input_start_time``      | Input start time              | 1700000000.000000                           |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``input_end_time``        | Input end time                | 1700000030.000000                           |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``actual_start_time``     | Actual start time             | 1700000000.000000                           |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``actual_start_time``     | Actual end time               | 1700000030.000000                           |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``start_sequence_number`` | Start segment sequence number | 0                                           |
-   +---------------------------+-------------------------------+---------------------------------------------+
-   | ``end_sequence_number``   | End segment sequence number   | 1001                                        |
-   +---------------------------+-------------------------------+---------------------------------------------+
-
-The input and actual time values (represented as seconds since the epoch) are
-expected to be different in only two cases: if the boundary (start and end)
-points fall in gaps or the ``--no-cut`` option is requested. In the opposite
-cases, after accurate cut, they're supposed to be identical.
+       [options.capture.frame]
+       ...
 
 Saving segment files
 ====================
 
 *Related command:* ``ytpb download``
 
 After merging downloaded segment files to make an excerpt, the segments will be
@@ -566,21 +450,24 @@
 --keep-segments`` option::
 
   $ ytpb download ... -S <STREAM>
   ...
   Success! Saved to 'Stream-Title_abcdefgh123_20240102T102030+00.mkv'.
   ~ Segments are kept in 'Stream-Title_abcdefgh123_20240102T102030+00'.
 
-The download destination can be changed via ``--segments-output-dir``::
+The download destination can be changed via ``-s / --segments-output-dir``::
 
   $ ytpb download ... -S --segments-output-dir segments <STREAM>
   ...
   Success! Saved to 'Stream-Title_abcdefgh123_20240102T102030+00.mkv'.
   ~ Segments are kept in 'segments'.
 
+Of course, the later option can be used without ``-S``, for example, to download
+segments (will be deleted after merging) to another drive.
+
 *Second*, download only segment files without merging them::
 
   $ ytpb download ... --no-merge <STREAM>
   ...
   Success! Segments saved to 'Stream-Title_abcdefgh123_20240102T102030+00'.
 
 Resuming unfinished downloads
@@ -600,51 +487,64 @@
 
 .. _Configuring:
 
 Configuring
 ***********
 
 The configuration provides the way to set up default values of the command
-options and change other settings via configuration files. It's optional, and
-the default, built-in settings are used.
+options and change other settings via configuration files. It's optional and the
+default, built-in settings are used otherwise.
 
 By default, the ``config.toml`` file is looked up under the ``~/.config/ytpb``
-directory (or in ``$XDG_CONFIG_HOME`` if set). Also, the ``--config`` option can
-be used to override the default file location. The priority of applying the
-settings is following: default settings < the ``config.toml`` file under the
-default directory < a file provided via the ``--config`` option < commands
-options.
+directory (or ``$XDG_CONFIG_HOME``) if you're on Unix or under platform-specific
+system directories if you're on `macOS
+<https://platformdirs.readthedocs.io/en/latest/api.html#platformdirs.macos.MacOS.site_data_dir>`__
+or `Windows
+<https://platformdirs.readthedocs.io/en/latest/api.html#platformdirs.windows.Windows.site_data_dir>`__. Also,
+the ``--config`` option can be used to override the default file location.
+
+The priority of applying settings is the following, from lowest to highest:
+
+1. Default, built-in settings.
+2. The ``config.toml`` file under the default directory.
+3. A file specified via the ``--config`` option.
+4. User-provided command options.
 
 See `config.toml.example`_ for the available fields and their descriptions.
 
 .. _config.toml.example: https://github.com/xymaxim/ytpb/blob/main/config.toml.example
 
 Advanced usage
 **************
 
-Merging without cutting
-=======================
+Writing metadata tags
+=====================
+
+*Related command:* ``ytpb download``
+
+By default, metadata tags will be added to an output excerpt file. Use the
+``--no-metadata`` option to disable it.
+
+.. rubric:: Metadata tags overview
 
-The boundary segments are cutted to exact times during the merging step to
-make an excerpt. It may take some time to re-encode boundary segments. If you
-don't need exact precision, it could be practical to omit cutting via the
-``--no-cut`` option. In this case the accuracy will be slightly reduced, which
-will depend on the constant segment duration (or type of `live-streaming latency
-<https://support.google.com/youtube/answer/7444635?hl=en>`_): in the worst case,
-the error will be 1 (for ultra-low latency), 2 (low latency), or 5 (normal
-latency) seconds.
+.. autoclass:: ytpb.cli.commands.download.MetadataTagsContext
+   :no-index:
 
-::
+The input and actual date values are expected to be different in only two cases:
+(a) if the boundary (start and end) points fall in gaps or (b) the ``--cut``
+option is not requested (default). In the opposite cases, after accurate cut,
+they're supposed to be identical.
 
-   $ ytpb download ... --no-cut <STREAM>
+The dates can be represented as seconds since the epoch via the configuration
+value: ``output.metadata.dates = unix``.
 
 Running without downloading
 ===========================
 
-There is a dry run mode (``-X / --dry-run``) to run without downloading. It
+There is a dry run mode (``-x / --dry-run``) to run without downloading. It
 could be useful if you are not interested in having an output excerpt file: for
 example, you want to locate the rewind interval or debug just the first steps
 (by combining a dry run mode with the ``--debug`` global option).
 
 For example, just to locate start and end moments, use::
 
   $ ytpb download ... --dry-run <STREAM>
```

### Comparing `ytpb-2024.5.3/docs/cookbook.rst` & `ytpb-2024.5.30/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/docs/quick.rst` & `ytpb-2024.5.30/docs/quick.rst`

 * *Files 12% similar despite different names*

```diff
@@ -24,32 +24,42 @@
 :ref:`cli:Specifying rewind interval`). For example, it would be handy to locate
 the desired moments first by previewing them and only after download a full
 excerpt. To run downloading in the :ref:`preview mode <Preview mode>`, use the
 ``-ps / --preview-start`` or ``-ps / --preview-end`` options::
 
   $ ytpb download -i 2024-01-02T10:20:00+00/PT30S -ps <STREAM>
 
+Note that the duration of an output excerpt :ref:`may be a bit longer <Why is
+the duration longer>` because the merging of media segments is done without
+cutting. You can use the ``-c / --cut`` option to frame-accurately cut an
+excerpt, but this will require additional disk space almost equal to the size of
+an excerpt.
+
 Check also out how to `download
 <https://ytpb.readthedocs.io/en/latest/cookbook.html#download-segments-with-curl>`__
 media segments with an external downloader.
 
 Compose and play
 ****************
 
 If you want to play an excerpt without downloading it, you can compose a static
 MPEG-DASH manifest (MPD) file: ::
 
-  $ ytpb mpd compose -i 2024-01-02T10:20:00+00/PT30S <STREAM> && ls
+  $ ytpb mpd compose -i 2024-01-02T10:20:00+00/PT1H <STREAM> && ls
   $ Stream-Title_20240102T102000+00.mpd
 
 By default, a manifest will contain a 128k AAC audio track and 720p (or better)
 30 fps VP9 video channels.
 
-Next, you can play a composed manifest in a player that supports MPEG-DASH (for
-example, with `mpv <https://mpv.io/>`__):
+Next, you can play a composed manifest in a player that supports MPEG-DASH. For
+example, with `VLC <https://www.videolan.org/vlc/>`__::
+
+  $ vlc Stream-Title_20240102T102000+00.mpd
+
+Or with `mpv <https://mpv.io/>`__:
 
   *Note:* Requires a custom mpv build. See `#4
   <https://github.com/xymaxim/ytpb/issues/4>`__ for details.
 
 ::
 
   $ mpv Stream-Title_20240102T102000+00.mpd
```

### Comparing `ytpb-2024.5.3/docs/why.rst` & `ytpb-2024.5.30/docs/why.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/docs/package/index.rst` & `ytpb-2024.5.30/docs/package/index.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/docs/package/usage.rst` & `ytpb-2024.5.30/docs/package/usage.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/etc/Containerfile` & `ytpb-2024.5.30/etc/Containerfile`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 
 RUN apk --no-cache add build-base git coreutils autoconf automake cmake \
   nasm yasm meson ninja-build libtool ffmpeg-dev mpv-dev libxxhash libdovi \
   libunwind-dev libplacebo-dev glslang-dev elfutils-dev mesa-dev \
   freetype-dev fribidi harfbuzz-dev mujs lua5.2-dev luajit rubberband uchardet \
   alsa-lib jack libpulse libvpx-dev x264-dev gnutls-dev xrandr
 
+# See https://github.com/mpv-player/mpv-build/pull/203.
 RUN ln -sf /usr/lib/ninja-build/bin/ninja /usr/bin/ninja
 
 WORKDIR ${BUILDDIR}
 RUN git clone https://github.com/mpv-player/mpv-build .
 
 RUN ./update
 
 WORKDIR ${BUILDDIR}/ffmpeg
+COPY *.patch .
 RUN <<EOF
-git revert --no-commit c122831
-git revert --no-commit 0dd1ff6
+git apply 0001-Revert-http-Send-a-Range-header-even-when-the-offset.patch
+git apply 0002-Revert-http-Improve-handling-of-Content-Range-with-T.patch
 EOF
 
 WORKDIR ${BUILDDIR}
 RUN printf "%s\n" --enable-gnutls --enable-libx264 --enable-libvpx \
   --enable-libxml2 --enable-demuxer=dash > ffmpeg_options
 
 # Stage 2. Build FFmpeg and mpv.
```

### Comparing `ytpb-2024.5.3/src/ytpb/api.py` & `ytpb-2024.5.30/src/ytpb/api.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/cache.py` & `ytpb-2024.5.30/src/ytpb/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             path.unlink()
 
         if _check_item_is_expired(latest_item_path.name):
             logger.debug("Found expired cached item: %s", latest_item_path)
             latest_item_path.unlink()
             item = None
         else:
-            with open(latest_item_path) as f:
+            with open(latest_item_path, encoding="utf-8") as f:
                 item = json.load(f)
             logger.debug("Found unexpired cached item: %s", latest_item_path)
 
     return item
 
 
 def write_to_cache(
@@ -71,15 +71,15 @@
         cache_directory: A cached items location.
     """
     cache_directory.mkdir(parents=True, exist_ok=True)
     if old_item_paths := _find_cached_item_paths(key, cache_directory):
         for path in old_item_paths:
             path.unlink()
     new_item_path = cache_directory / f"{expires_at}~{key}"
-    with open(new_item_path, "w") as f:
+    with open(new_item_path, "w", encoding="utf-8") as f:
         json.dump(item, f)
     logger.debug("New cache item has been created: %s", new_item_path)
 
 
 def remove_expired_cache_items(cache_directory: Path) -> None:
     """Removes expired cache items."""
     for path in sorted(cache_directory.glob("*~*")):
```

### Comparing `ytpb-2024.5.3/src/ytpb/conditional.py` & `ytpb-2024.5.30/src/ytpb/conditional.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,23 @@
 import re
 from typing import Any, Callable
 
 import pycond as pc
-
 import structlog
 
-from ytpb.config import ALIAS_EXPAND_FUNCTIONS, ALL_ALIASES
 from ytpb.errors import QueryError
 from ytpb.types import AudioOrVideoStream
 
 logger = structlog.get_logger(__name__)
 
-ALIAS_RE = re.compile(r"@([\w<>=-]+)(?!\s)?")
 FORMAT_SPEC_RE = re.compile(
     r"^(?:(?P<function>[\w\-]+)\((?P<expr>[^\(\)]+)\)|(?P<just_expr>[^\(\)]+))$"
 )
 
-
-def _expand_aliases(expression: str, aliases: dict[str, str]) -> str:
-    for f in ALIAS_EXPAND_FUNCTIONS:
-        expression = f(expression)
-
-    all_aliases = ALL_ALIASES | aliases
-    for matched in ALIAS_RE.finditer(expression):
-        alias_with_symbol = matched.group()
-        alias = matched.group(1)
-        try:
-            aliased_value = all_aliases[alias]
-            expression = expression.replace(alias_with_symbol, aliased_value)
-        except KeyError:
-            raise QueryError(
-                f"Unknown alias in format spec: '{alias_with_symbol}'"
-            ) from None
-    return expression
+pc.ops_use_symbolic_and_txt(allow_single_eq=True)
 
 
 def treat_none_as_false(operator_function: Callable, a: Any, b: Any) -> bool:
     if a is None:
         return False
     else:
         return operator_function(a, b)
@@ -56,18 +37,14 @@
             )
         attribute_value = getattr(state, attribute)
     except AttributeError as e:
         raise QueryError(f"Unknown attribute in format spec: '{attribute}'") from e
     return attribute_value, target
 
 
-def make_filter_from_expression(expression: str, aliases: dict[str, str] | None = None):
-    if ALIAS_RE.search(expression):
-        expression = _expand_aliases(expression, aliases or {})
-        logger.debug(f"Expression with alias(es) expanded as '{expression}'")
-    output = pc.make_filter(
+def make_filter_from_expression(expression: str):
+    return pc.make_filter(
         expression,
         autoconv_lookups=True,
         lookup=custom_lookup,
         ops_thru=treat_none_as_false,
     )
-    return output
```

### Comparing `ytpb-2024.5.3/src/ytpb/download.py` & `ytpb-2024.5.30/src/ytpb/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/errors.py` & `ytpb-2024.5.30/src/ytpb/errors.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/fetchers.py` & `ytpb-2024.5.30/src/ytpb/fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/info.py` & `ytpb-2024.5.30/src/ytpb/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from enum import auto, StrEnum
 from typing import Any
 
 from lxml import etree
 
 from ytpb.errors import InfoExtractError
+from ytpb.utils.other import normalize_info_string
 
 
 class BroadcastStatus(StrEnum):
     """Represents a live broadcast status."""
 
     #: A broadcast is live.
     ACTIVE = auto()
@@ -23,20 +24,28 @@
     NONE = auto()
 
 
 @dataclass
 class YouTubeVideoInfo:
     """Represents information about a video."""
 
+    #: Youtube video URL.
     url: str
+    #: Video's title.
     title: str
+    #: Video's author (channel's name).
     author: str
+    #: Video' broadcast status.
     status: BroadcastStatus
     dash_manifest_url: str | None = None
 
+    def __post_init__(self):
+        self.title = normalize_info_string(self.title)
+        self.author = normalize_info_string(self.author)
+
 
 class LeftNotFetched:
     pass
 
 
 #: A sentinel object for a value that is intentionally not fetched.
 LEFT_NOT_FETCHED = LeftNotFetched()
```

### Comparing `ytpb-2024.5.3/src/ytpb/locate.py` & `ytpb-2024.5.30/src/ytpb/locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/merge.py` & `ytpb-2024.5.30/src/ytpb/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 import functools
 import os
 import shlex
 from pathlib import Path
 from typing import Any
 
-from ytpb import ffmpeg
+import av
+
+from ytpb.utils import ffmpeg
 
 __all__ = ("merge_segments", "mux_and_cut_boundary_segment")
 
 
 DEFAULT_VIDEO_ENCODING_SETTINGS = {
     "h264": "libx264 -crf 18",
     "vp9": "libvpx-vp9 -crf 31 -b:v 0",
@@ -61,17 +63,17 @@
 
     if not {"cut_at_start", "cut_at_end"} > cut_kwargs.keys():
         raise ValueError(
             "only cut_at_start or cut_at_end keyword argument is accepted in cut_kwargs"
         )
 
     if video_segment_path and video_codec is None:
-        video_codec = ffmpeg.ffprobe_show_entries(
-            video_segment_path, "stream=codec_name"
-        )
+        with av.open(video_segment_path) as container:
+            video_av_stream = container.streams.get({"video": 0})[0]
+            video_codec = video_av_stream.codec_context.name
 
     ffmpeg_input_options = []
     ffmpeg_codecs_options = []
 
     should_cut = bool(
         cut_kwargs.get("cut_at_start", 0) or cut_kwargs.get("cut_at_end", 0)
     )
@@ -95,15 +97,15 @@
             else:
                 try:
                     ffmpeg_codecs_options += ["-c:v"] + shlex.split(
                         DEFAULT_VIDEO_ENCODING_SETTINGS[video_codec]
                     )
                 except KeyError:
                     raise ValueError(
-                        "No encoding settings are availabe for"
+                        "No encoding settings are availabe for "
                         f"'{video_codec}' video codec"
                     )
 
         if audio_segment_path:
             ffmpeg_input_options += prepare_ffmpeg_input_options(
                 audio_segment_path, **cut_kwargs
             )
@@ -241,17 +243,17 @@
         start_video_segment_path = get_nth_or_none(video_segment_paths, 0)
 
         end_audio_segment_path = get_nth_or_none(audio_segment_paths, -1)
         end_video_segment_path = get_nth_or_none(video_segment_paths, -1)
 
         video_codec: str | None = None
         if video_segment_paths:
-            video_codec = ffmpeg.ffprobe_show_entries(
-                video_segment_paths[0], "stream=codec_name"
-            )
+            with av.open(video_segment_paths[0]) as container:
+                video_av_stream = container.streams.get({"video": 0})[0]
+                video_codec = video_av_stream.codec_context.name
 
         if num_of_segments == 1:
             segment_trimmed_path = Path(temp_directory, "a.a" + output_extension)
             mux_and_cut_boundary_segment(
                 start_audio_segment_path,
                 start_video_segment_path,
                 segment_trimmed_path,
```

### Comparing `ytpb-2024.5.3/src/ytpb/playback.py` & `ytpb-2024.5.30/src/ytpb/playback.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 import operator
 import re
 import tempfile
 from dataclasses import asdict, dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Iterable, Self, TypeGuard
+from typing import Iterable, Self, TypedDict, TypeGuard, Unpack
 from urllib.parse import parse_qs, urlparse
 
 import requests
 import structlog
 from platformdirs import user_cache_path
 
 from ytpb.cache import read_from_cache, write_to_cache
-from ytpb.config import USER_AGENT
 from ytpb.download import (
     compose_default_segment_filename,
     download_segment,
     SegmentOutputFilename,
 )
 from ytpb.errors import (
     BaseUrlExpiredError,
@@ -171,15 +170,14 @@
     max_retries: int = 3
 
     def __init__(self, playback: "Playback" = None, **kwargs):
         super().__init__(**kwargs)
 
         self.playback = playback
         self.hooks["response"].append(self._handle_http_errors)
-        self.headers["User-Agent"] = USER_AGENT
 
     def set_playback(self, playback):
         self.playback = playback
 
     def _handle_403_error(self, request: requests.Request) -> None:
         old_corresponding_stream = next(
             iter(
@@ -228,42 +226,55 @@
         else:
             raise MaxRetryError(
                 f"Maximum number of retries exceeded with URL: {request.url}",
                 response,
             )
 
 
+class _PlaybackOptions(TypedDict, total=False):
+    user_agent: str
+
+
 class Playback:
     """The playback for live streams."""
 
     def __init__(
         self,
         video_url: str,
         session: requests.Session | None = None,
         fetcher: InfoFetcher | None = None,
         write_to_cache: bool = False,
-    ):
+        **kwargs: Unpack[_PlaybackOptions],
+    ) -> None:
         """Constructs a playback.
 
         To work with a playback, fetch the essential information afterwards::
 
             playback = Playback(video_url)
             playback.fetch_and_set_essential()
 
         Args:
             video_url: A video URL.
             session: An instance of :class:`requests.Session`.
             fetcher: A fetcher used to gather the video information and streams.
             write_to_cache: Whether to write to cache.
+
+        Keyword Args:
+            user_agent: The HTTP User-Agent string used for requests. Note that
+              this value has priority over the value from ``session``
+              headers.
         """
         self.video_url = video_url
-        self.session = session or PlaybackSession(self)
         self.fetcher = fetcher or YtpbInfoFetcher(video_url)
         self._need_to_cache = write_to_cache
 
+        self.session = session or PlaybackSession(self)
+        if user_agent := kwargs.get("user_agent"):
+            self.session.headers["User-Agent"] = user_agent
+
         self._info: YouTubeVideoInfo | LeftNotFetched | None = None
         self._streams: SetOfStreams | None = None
         self._temp_directory: Path | None = None
         self._cache_directory: Path | None = None
 
         self.rewind_history = RewindTreeMap()
 
@@ -287,15 +298,15 @@
     @classmethod
     def from_manifest(
         cls,
         manifest_path: Path,
         fetch_video_info: bool = True,
         **kwargs,
     ) -> "Playback":
-        with open(manifest_path, "r") as f:
+        with open(manifest_path, "r", encoding="utf-8") as f:
             list_of_streams = extract_representations(f.read())
             streams = Streams(list_of_streams)
 
         some_base_url = next(iter(streams)).base_url
         video_url = build_video_url_from_base_url(some_base_url)
 
         if not check_base_url_is_expired(some_base_url):
@@ -451,15 +462,15 @@
             SegmentOutputFilename | None
         ) = compose_default_segment_filename,
         force_download: bool = False,
     ) -> Path:
         """Downloads a segment.
 
         Examples:
-            Download a segment to a file, and read it::
+            Download a segment to a file and read it::
 
                 from ytpb.segment import Segment
                 downloaded_path = playback.download_segment(
                     0, playback.streams.get_by_itag("140")
                 )
                 segment = Segment.from_file(downloaded_path)
```

### Comparing `ytpb-2024.5.3/src/ytpb/representations.py` & `ytpb-2024.5.30/src/ytpb/representations.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 @dataclass(frozen=True)
 class VideoQuality:
     """Represents a video quality (height and frame rate).
 
     Examples:
         The class supports comparison operations. For example: ::
 
-          >>> VideoQuality("720p") == VideoQuality("720p30")
-          True
-          >>> VideoQuality("720p") > VideoQuality("720p60")
+          >>> VideoQuality(720) == VideoQuality(720, 30)
           True
+          >>> VideoQuality(720) > VideoQuality(720, 60)
+          False
     """
 
     height: int
     frame_rate: float
 
     @classmethod
     def from_string(cls, value: str) -> "VideoQuality":
@@ -62,52 +62,66 @@
             return False
 
 
 @dataclass(frozen=True, slots=True)
 class RepresentationInfo:
     """Represents common attributes of audio and video representations."""
 
+    #: itag value, e.g. '140', '247'.
     itag: str
+    #: MIME type, e.g. 'audio/mp4', 'video/webm'.
     mime_type: str
+    #: Codec name, e.g. 'mp4', 'vp9'.
     codecs: str
+    #: Segment base URL.
     base_url: str
 
     @property
     def type(self) -> str:
-        """An alias for a MIME type."""
+        """An alias for a MIME type, e.g. 'audio', 'video'."""
         return self.mime_type.split("/")[0]
 
     @property
     def format(self) -> str:
-        """An alias for a MIME subtype."""
+        """An alias for a MIME subtype, e.g. 'mp4', 'webm'."""
         return self.mime_type.split("/")[1]
 
     def __repr__(self):
         return f"{type(self).__name__}(itag={self.itag})"
 
 
 @dataclass(frozen=True, repr=False)
 class AudioRepresentationInfo(RepresentationInfo):
     """Represents attributes of audio representations."""
 
+    #: Sampling rate (in Hz).
     audio_sampling_rate: int
 
 
 @dataclass(frozen=True, repr=False)
 class VideoRepresentationInfo(RepresentationInfo):
     """Represents attributes of video representations."""
 
+    #: Width of frame.
     width: int
+    #: Height of frame.
     height: int
+    #: Frame per second (FPS).
     frame_rate: int
 
     @property
     def quality(self) -> VideoQuality:
+        """Quality string (resolution and FPS), e.g. '720p', '1080p60'."""
         return VideoQuality(self.height, self.frame_rate)
 
+    @property
+    def fps(self) -> int:
+        """An alias for ``frame_rate``."""
+        return self.frame_rate
+
 
 def _eval_local_xpath(element: etree.Element, node: str) -> list[etree.Element]:
     return element.xpath(".//*[local-name() = $node]", node=node)
 
 
 def extract_representations(manifest_content: str) -> list[RepresentationInfo]:
     """Extracts representations from a manifest.
```

### Comparing `ytpb-2024.5.3/src/ytpb/segment.py` & `ytpb-2024.5.30/src/ytpb/segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
     All timestamp and time-related values are in seconds.
     """
 
     sequence_number: SegmentSequence
     ingestion_walltime: Timestamp
     ingestion_uncertainty: float
-    stream_duration: float
-    max_dvr_duration: float
     target_duration: float
     first_frame_time: Timestamp
     first_frame_uncertainty: float
+    stream_duration: float = None
+    max_dvr_duration: float = None
     streamable: str | None = None
     encoding_alias: str | None = None
 
 
 @dataclass
 class Segment:
     """A media segment."""
@@ -99,15 +99,20 @@
 
         Args:
             content: Full or partial segment byte content.
 
         Returns:
             A parsed segment metadata.
         """
-        optional_fields = ("Streamable", "Encoding-Alias")
+        optional_fields = (
+            "Encoding-Alias",
+            "Streamable",
+            "Stream-Duration-Us",
+            "Max-Dvr-Duration-Us",
+        )
 
         def _search_for_metadata_field(
             name: str, content: bytes, optional: bool = False
         ) -> bytes | None:
             if matched := re.search(rf"{name}:\s(.+)\r\n".encode(), content):
                 value = matched.group(1)
             else:
@@ -145,14 +150,11 @@
                 name_as_key = name.removesuffix("-Us").lower().replace("-", "_")
                 parsed_metadata_fields[name_as_key] = value
 
         return SegmentMetadata(**parsed_metadata_fields)
 
     def get_actual_duration(self) -> float:
         """Gets the actual segment duration in seconds."""
-        with av.open(str(self.local_path)) as container:
+        with av.open(self.local_path) as container:
             first_packet, *_, last_packet = list(container.demux())[:-1]
-            end_timestamp = last_packet.pts + last_packet.duration
-            duration = (end_timestamp - first_packet.pts) * float(
-                first_packet.time_base
-            )
-            return duration
+        end_pts = last_packet.pts + last_packet.duration
+        return float((end_pts - first_packet.pts) * first_packet.time_base)
```

### Comparing `ytpb-2024.5.3/src/ytpb/streams.py` & `ytpb-2024.5.30/src/ytpb/streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,29 +98,22 @@
     ) -> list[AudioOrVideoStream]:
         """Queries streams by a format spec.
 
         Notes:
             Check for attributes is strict. This means that the following code
             will fail with :class:`.QueryError` because audio streams don't have
             the ``height`` attribute::
-              audio_streams.query("height eq 1080")
 
-        Examples:
-            Query streams of a specific media format using aliases::
-
-              playback.streams.query(
-                  "@webm", aliases={"webm": "format eq webm"}
-              )
+                audio_streams.query("height eq 1080")
 
         References:
             https://ytpb.readthedocs.io/en/latest/reference.html#format-spec
 
         Args:
-            format_spec: A format spec. May contains aliases.
-            aliases: A dictionary of aliases.
+            format_spec: A format spec.
 
         Returns:
             A list of queried streams.
 
         Raises:
             QueryError: If failed to query streams with the given format spec.
         """
@@ -135,15 +128,15 @@
             if function_name := matched.group("function"):
                 expression = matched.group("expr")
             else:
                 expression = matched.group("just_expr")
         else:
             raise QueryError(f"Format spec is invalid: {format_spec}")
 
-        expression_filter = make_filter_from_expression(expression, aliases)
+        expression_filter = make_filter_from_expression(expression)
         queried: list[AudioOrVideoStream] = list(
             filter(expression_filter, self._elements)
         )
         if queried:
             if function_name:
                 try:
                     queried = [functions_map[function_name](queried)]
```

### Comparing `ytpb-2024.5.3/src/ytpb/types.py` & `ytpb-2024.5.30/src/ytpb/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Protocol, TypeAlias
 
-from ytpb.config import AddressableChainMap
 from ytpb.representations import AudioRepresentationInfo, VideoRepresentationInfo
 
 
 class RelativeSegmentSequence(int): ...
 
 
 Timestamp: TypeAlias = float
@@ -18,16 +17,14 @@
 PointInStream: TypeAlias = AbsolutePointInStream | RelativePointInStream
 
 AudioStream: TypeAlias = AudioRepresentationInfo
 VideoStream: TypeAlias = VideoRepresentationInfo
 AudioOrVideoStream: TypeAlias = AudioStream | VideoStream
 SetOfStreams: TypeAlias = "Streams[AudioOrVideoStream]"
 
-ConfigMap: TypeAlias = AddressableChainMap
-
 
 class AddressableMappingProtocol(Protocol):
     def traverse(self, address: str, default: Any, delimiter: str) -> Any: ...
 
 
 @dataclass
 class DateInterval:
```

### Comparing `ytpb-2024.5.3/src/ytpb/actions/capture.py` & `ytpb-2024.5.30/src/ytpb/actions/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/actions/compose.py` & `ytpb-2024.5.30/src/ytpb/actions/compose.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
             "media": "sq/$Number$",
             "startNumber": str(rewind_interval.start.sequence),
             "duration": str(int(segment_duration_s) * int(S_TO_MS)),
             "timescale": "1000",
         }
     )
 
-    for element in period_element.findall(".//AdaptationSet", namespaces=NS):
-        element.insert(0, copy.deepcopy(segment_template_element))
+    for element in period_element.findall(".//Representation", namespaces=NS):
+        element.insert(1, copy.deepcopy(segment_template_element))
 
     output = etree.tostring(
         etree.ElementTree(mpd_element),
         xml_declaration=True,
         encoding="UTF-8",
         pretty_print=True,
     )
@@ -168,16 +168,16 @@
     )
 
     segment_duration_ms = int(rewind_metadata.target_duration * S_TO_MS)
     segment_template_element.append(
         E("SegmentTimeline", E("S", d=str(segment_duration_ms), r="-1"))
     )
 
-    for element in period_element.findall(".//AdaptationSet", namespaces=NS):
-        element.insert(0, copy.deepcopy(segment_template_element))
+    for element in period_element.findall(".//Representation", namespaces=NS):
+        element.insert(1, copy.deepcopy(segment_template_element))
 
     output = etree.tostring(
         etree.ElementTree(mpd_element),
         xml_declaration=True,
         encoding="UTF-8",
         pretty_print=True,
     )
```

### Comparing `ytpb-2024.5.3/src/ytpb/actions/download.py` & `ytpb-2024.5.30/src/ytpb/actions/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/cli/__init__.py` & `ytpb-2024.5.30/src/ytpb/cli/options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,151 @@
-import atexit
-import logging
-import os
-import re
-import sys
-from copy import deepcopy
-from dataclasses import dataclass, field
 from datetime import datetime, timezone
-from fileinput import FileInput
 from pathlib import Path
-from typing import Any, cast, TextIO
+from textwrap import fill
+from typing import Callable
 
 import click
-import cloup
-import structlog
-import toml
-
-from ytpb.cli.commands.capture import capture_group
-from ytpb.cli.commands.download import download_command
-from ytpb.cli.commands.mpd import mpd_group
-
-from ytpb.cli.common import suppress_output
-from ytpb.cli.options import config_options, logging_options
-from ytpb.config import (
-    ALL_ALIASES,
-    DEFAULT_CONFIG,
-    get_default_config_path,
-    load_config_from_file,
-    setup_logging,
-    update_nested_dict,
+from cloup.constraints import constraint, mutually_exclusive
+from jinja2 import TemplateSyntaxError
+from jinja2.meta import find_undeclared_variables
+from PIL import Image
+
+from ytpb.cli import parameters
+from ytpb.cli.common import EARLIEST_DATE_TIMEDELTA
+from ytpb.cli.templating import check_is_template
+
+
+def validate_output_path(template_context_class) -> Callable[..., Path]:
+    def wrapper(ctx: click.Context, param: click.Option, value: Path) -> Path:
+        if check_is_template(str(value)):
+            try:
+                parsed = ctx.obj.jinja_environment.parse(str(value))
+            except TemplateSyntaxError as exc:
+                raise click.BadParameter(
+                    f"Bad template syntax, line {exc.lineno}: {exc}"
+                )
+            undeclared_variables = find_undeclared_variables(parsed)
+            context_variables = set(template_context_class.__annotations__.keys())
+            if not undeclared_variables.issubset(context_variables):
+                unknown_variables = undeclared_variables - context_variables
+                raise click.BadParameter(
+                    "Unknown template variable(s) found: {}.".format(
+                        str(unknown_variables).strip("{}")
+                    )
+                )
+        return value
+
+    return wrapper
+
+
+def validate_image_output_path(template_context_class) -> Callable[..., Path]:
+    def wrapper(ctx: click.Context, param: click.Option, value: Path) -> Path:
+        if not value.suffix:
+            raise click.BadParameter("Image extension must be provided.")
+
+        extensions = Image.registered_extensions()
+        allowed_extensions = {ext for ext, f in extensions.items() if f in Image.SAVE}
+        if value.suffix not in allowed_extensions:
+            tip = fill(
+                "Choose one of: {}".format(", ".join(sorted(allowed_extensions)))
+            )
+            raise click.BadParameter(
+                f"Format '{value.suffix}' is not supported.\n\n{tip}"
+            )
+
+        return validate_output_path(template_context_class)(ctx, param, value)
+
+    return wrapper
+
+
+def validate_start_date_not_too_far(
+    ctx: click.Context, param: click.Option, value: datetime | str
+) -> datetime | str:
+    if isinstance(value, datetime):
+        now = datetime.now(timezone.utc).astimezone(value.tzinfo)
+        earliest_date = now - EARLIEST_DATE_TIMEDELTA
+        if value <= earliest_date:
+            raise click.BadParameter(
+                "Start date is beyond the limit of 7 days. "
+                "The earliest date is {}.".format(
+                    earliest_date.isoformat(timespec="minutes")
+                )
+            )
+    return value
+
+
+interval_option = click.option(
+    "-i",
+    "--interval",
+    metavar="INTERVAL",
+    type=parameters.RewindIntervalParamType(),
+    help="Time or segment interval.",
+    required=True,
 )
-from ytpb.types import ConfigMap
 
-logger = structlog.get_logger(__name__)
 
+def config_options(f):
+    f = click.option(
+        "-C",
+        "--config",
+        "config_path",
+        help="Specifies a path to a configuration file.",
+        type=click.Path(path_type=Path),
+        is_eager=True,
+    )(f)
 
-@dataclass
-class ReportStreamWrapper:
-    stream: TextIO
-    file: TextIO
-
-    def write(self, message: str) -> None:
-        self.stream.write(message)
-        self.file.write(message)
-
-    def __getattr__(self, attr: str) -> Any:
-        return getattr(self.stream, attr)
-
-
-@dataclass
-class ContextObject:
-    """This object is referenced as `ctx.obj`."""
-
-    config: ConfigMap = field(default_factory=lambda: ConfigMap(DEFAULT_CONFIG))
-    original_stdout: TextIO = field(default_factory=lambda: sys.stdout)
-
-
-def load_config_into_context(ctx: click.Context, path: Path) -> dict:
-    try:
-        config_dict = load_config_from_file(path)
-    except FileNotFoundError as e:
-        raise click.FileError(
-            filename=path,
-            hint=str(e),
-        )
-    except toml.TomlDecodeError as e:
-        raise click.FileError(
-            filename=path,
-            hint=f"Could not load configuration file.\n{e}",
-        )
-
-    ctx.ensure_object(ContextObject)
-    ctx.obj.config = ctx.obj.config.new_child(config_dict)
-
-    default_map_from_config = ctx.obj.config["options"]
-    ctx.default_map = update_nested_dict(ctx.default_map, default_map_from_config)
-
-    try:
-        ALL_ALIASES.update(ctx.obj.config["general"]["aliases"])
-    except KeyError:
-        pass
-
-
-@cloup.group(invoke_without_command=True)
-@cloup.option_group(
-    "Global options",
-    config_options,
-    logging_options,
-    click.option(
-        "-q",
-        "--quiet",
-        help="Supress all normal output.",
+    f = click.option(
+        "--no-config",
+        help="Do not load any configuration files.",
         default=False,
         is_flag=True,
         is_eager=True,
-    ),
+    )(f)
+
+    return f
+
+
+def cache_options(f):
+    f = click.option(
+        "--force-update-cache",
+        help="Force to update cache.",
+        is_flag=True,
+    )(f)
+
+    f = click.option(
+        "--no-cache",
+        help="Do not use cache.",
+        is_flag=True,
+    )(f)
+
+    f = constraint(mutually_exclusive, ["no_cache", "force_update_cache"])(f)
+
+    return f
+
+
+def logging_options(f):
+    f = click.option(
+        "--report",
+        help="Dump all output to a file. It implies --debug.",
+        is_flag=True,
+        is_eager=True,
+    )(f)
+
+    f = click.option(
+        "--debug",
+        "debug",
+        help="Enable verbose output for debugging.",
+        is_flag=True,
+        is_eager=True,
+    )(f)
+
+    return f
+
+
+yt_dlp_option = click.option(
+    "-Y", "--yt-dlp", is_flag=True, help="Use yt-dlp to extract info."
 )
-@click.version_option(None, "-V", "--version", message="%(version)s")
-@click.pass_context
-def base_cli(
-    ctx: click.Context,
-    config_path: Path,
-    no_config: bool,
-    debug: bool,
-    report: bool,
-    quiet: bool,
-) -> None:
-    if ctx.invoked_subcommand is None:
-        click.echo(ctx.get_help())
-        ctx.exit()
-
-    ctx.ensure_object(ContextObject)
-    ctx.default_map = ctx.obj.config["options"]
-
-    if quiet:
-        suppress_output()
-
-    if report:
-        debug = True
-        os.environ["NO_COLOR"] = "1"
-
-        timestamp = datetime.now(tz=timezone.utc).strftime("%Y%m%d-%H%M%S")
-        report_handle = open(Path.cwd() / f"ytpb-{timestamp}.log", "a")
-        sys.stdout = cast(
-            TextIO, ReportStreamWrapper(ctx.obj.original_stdout, report_handle)
-        )
-        sys.stderr = cast(TextIO, ReportStreamWrapper(sys.stderr, report_handle))
-
-        @atexit.register
-        def sanitize_report_file() -> None:
-            report_handle.close()
-            with FileInput(report_handle.name, inplace=True) as fi:
-                for line in fi:
-                    print(re.sub("/ip/([\w.:]+)/", "/ip/0.0.0.0/", line), end="")
-
-    setup_logging(logging.DEBUG if debug else logging.WARNING)
-
-    if not no_config:
-        if config_path:
-            logger.info("Using configuration from '%s' via --config", config_path)
-            load_config_into_context(ctx, config_path)
-        else:
-            default_config_path = get_default_config_path()
-            if default_config_path.exists():
-                logger.info("Using configuration from '%s'", default_config_path)
-                load_config_into_context(ctx, default_config_path)
-    else:
-        if config_path:
-            raise click.UsageError("Conflicting --config and --no-config options given")
-
-
-cli = deepcopy(base_cli)
-
-cli.help = "A playback for YouTube live streams"
-cli.section(
-    "Top-level commands",
-    download_command,
-    capture_group,
-    mpd_group,
+
+
+keep_temp_option = click.option(
+    "--keep-temp", is_flag=True, help="Keep temporary files."
 )
```

### Comparing `ytpb-2024.5.3/src/ytpb/cli/common.py` & `ytpb-2024.5.30/src/ytpb/cli/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,88 +4,36 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import click
 import cloup
 import structlog
 
+from ytpb.cli.utils.date import format_timedelta, round_date
+
 from ytpb.errors import (
     BadCommandArgument,
-    BaseUrlExpiredError,
     BroadcastStatusError,
     CachedItemNotFoundError,
+    MaxRetryError,
     QueryError,
+    SegmentDownloadError,
 )
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
 from ytpb.info import BroadcastStatus
 from ytpb.playback import Playback, RewindInterval
-from ytpb.types import DateInterval, SetOfStreams
-from ytpb.utils.date import format_timedelta, round_date
+from ytpb.types import DateInterval, SegmentSequence, SetOfStreams
 from ytpb.utils.url import extract_parameter_from_url, normalize_video_url
 
 logger = structlog.getLogger(__name__)
 
-
 CONSOLE_TEXT_WIDTH = 80
 EARLIEST_DATE_TIMEDELTA = timedelta(days=6, hours=23)
 
 
-def get_parameter_by_name(name: str, ctx: click.Context) -> click.Parameter:
-    return next((p for p in ctx.command.params if p.name == name), None)
-
-
-def create_playback(ctx: click.Context) -> Playback:
-    stream_url = ctx.params["stream_url"]
-
-    if ctx.params["yt_dlp"]:
-        fetcher = YoutubeDLInfoFetcher(stream_url)
-    else:
-        fetcher = YtpbInfoFetcher(stream_url)
-
-    try:
-        if from_manifest := ctx.params.get("from_manifest"):
-            try:
-                click.echo("Run playback from manifest file")
-                playback = Playback.from_manifest(from_manifest, fetcher=fetcher)
-            except BaseUrlExpiredError:
-                click.echo("Oh no, the manifest has been expired, exit.", err=True)
-                sys.exit(1)
-        else:
-            click.echo(f"Run playback for {stream_url}")
-            click.echo("(<<) Collecting info about the video...")
-
-            force_update_cache = ctx.params.get("force_update_cache", False)
-            need_read_cache = not (
-                ctx.params.get("no_cache", True) or force_update_cache
-            )
-            if need_read_cache:
-                try:
-                    playback = Playback.from_cache(stream_url, fetcher=fetcher)
-                except CachedItemNotFoundError:
-                    logger.debug("Could not find unexpired cached item for the video")
-                    playback = Playback.from_url(
-                        stream_url, fetcher=fetcher, write_to_cache=True
-                    )
-            else:
-                playback = Playback.from_url(
-                    stream_url, fetcher=fetcher, write_to_cache=force_update_cache
-                )
-    except BroadcastStatusError as e:
-        match e.status:
-            case BroadcastStatus.NONE:
-                click.echo("It's seems that the video is not a live stream", err=True)
-            case BroadcastStatus.COMPLETED:
-                click.echo("Stream was live, but now it's finished", err=True)
-        sys.exit(1)
-
-    click.echo(f"Stream '{playback.info.title}' is alive!")
-
-    return playback
-
-
 def normalize_stream_url(ctx: click.Context, param: click.Argument, value: str) -> str:
     try:
         return normalize_video_url(value)
     except BadCommandArgument as e:
         raise click.BadParameter(str(e))
 
 
@@ -93,14 +41,32 @@
     "stream_url",
     metavar="STREAM",
     help="Stream URL or video ID.",
     callback=normalize_stream_url,
 )
 
 
+def suppress_output() -> None:
+    sys.stdout = open(os.devnull, "w")
+
+
+def echo_notice(message: str) -> None:
+    click.echo(f"~ {message}")
+
+
+def get_parameter_by_name(name: str, ctx: click.Context) -> click.Parameter:
+    return next((p for p in ctx.command.params if p.name == name), None)
+
+
+def resolve_output_path(output_path: Path) -> Path:
+    resolved_path = Path(output_path).expanduser().resolve()
+    resolved_path.parent.mkdir(parents=True, exist_ok=True)
+    return resolved_path
+
+
 def prepare_line_for_summary_info(
     date: datetime,
     input_actual_timedelta: timedelta,
     use_ms_precision: bool = False,
 ) -> str:
     if not use_ms_precision:
         date = round_date(date)
@@ -147,14 +113,53 @@
     click.echo(
         "  Actual end: {}, seq. {}".format(
             end_time_info_line, rewind_interval.end.sequence
         )
     )
 
 
+def create_playback(ctx: click.Context) -> Playback:
+    stream_url = ctx.params["stream_url"]
+
+    if ctx.params["yt_dlp"]:
+        fetcher = YoutubeDLInfoFetcher(stream_url)
+    else:
+        fetcher = YtpbInfoFetcher(stream_url)
+
+    try:
+        click.echo(f"Run playback for {stream_url}")
+        click.echo("(<<) Collecting info about the video...")
+
+        force_update_cache = ctx.params.get("force_update_cache", False)
+        need_read_cache = not (ctx.params.get("no_cache", True) or force_update_cache)
+        if need_read_cache:
+            try:
+                playback = Playback.from_cache(stream_url, fetcher=fetcher)
+            except CachedItemNotFoundError:
+                logger.debug("Could not find unexpired cached item for the video")
+                playback = Playback.from_url(
+                    stream_url, fetcher=fetcher, write_to_cache=True
+                )
+        else:
+            playback = Playback.from_url(
+                stream_url, fetcher=fetcher, write_to_cache=force_update_cache
+            )
+    except BroadcastStatusError as e:
+        match e.status:
+            case BroadcastStatus.NONE:
+                click.echo("It's seems that the video is not a live stream", err=True)
+            case BroadcastStatus.COMPLETED:
+                click.echo("Stream was live, but now it's finished", err=True)
+        sys.exit(1)
+
+    click.echo(f"Stream '{playback.info.title}' is alive!")
+
+    return playback
+
+
 def query_streams_or_exit(
     streams: SetOfStreams,
     format_spec: str,
     param: str | None = None,
     allow_empty: bool = False,
     allow_many: bool = True,
 ) -> SetOfStreams:
@@ -216,19 +221,61 @@
             "Sequence number is ahead or equal to the current one: "
             f"{sequence} >= {current_sequence}"
         )
         param = get_parameter_by_name(param_name, ctx)
         raise click.BadParameter(message, ctx, param)
 
 
-def resolve_output_path(output_path: Path) -> Path:
-    resolved_path = Path(output_path).expanduser().resolve()
-    resolved_path.parent.mkdir(parents=True, exist_ok=True)
-    return resolved_path
-
-
-def suppress_output() -> None:
-    sys.stdout = open(os.devnull, "w")
+def find_earliest_sequence(
+    playback: Playback, head_sequence: SegmentSequence, head_date: datetime
+) -> SegmentSequence:
+    """Finds the earliest available segment sequence number.
+
+    Note that the function returns not the most earliest available sequence
+    number, but the safe one, which is close to the 7-days availability limit
+    (or potentially to the lower limit if a stream is stored less, for example,
+    5 days, if such a thing occurs).
+    """
+    some_stream = next(iter(playback.streams))
+    segment_duration = float(extract_parameter_from_url("dur", some_stream.base_url))
+
+    target_date = head_date - EARLIEST_DATE_TIMEDELTA
+    logger.info("Start finding the earliest segment", limit=target_date)
+
+    jump_to_left = int(EARLIEST_DATE_TIMEDELTA.total_seconds() // segment_duration)
+    left_sequence = head_sequence - jump_to_left
+    right_sequence = head_sequence - jump_to_left // 2
+    if left_sequence < 0:
+        logger.debug("Found beginning segment to be the earliest")
+        return 0
+
+    search_domain = range(left_sequence, right_sequence + 1)
+    logger.debug("Set search domain", left=left_sequence, right=right_sequence)
+
+    def _check_ahead_target(sequence: SegmentSequence, target_date: datetime) -> bool:
+        try:
+            segment = playback.get_segment(sequence, some_stream)
+        except (SegmentDownloadError, MaxRetryError):
+            timedelta_to_target = None
+            result = False
+        else:
+            timedelta_to_target = segment.ingestion_start_date - target_date
+            if timedelta_to_target > timedelta(0):
+                result = True
+            else:
+                result = False
+        logger.debug("Bisect step", sequence=sequence, timedelta=timedelta_to_target)
+        return result
+
+    low, high = 0, len(search_domain)
+    while low < high:
+        middle = (low + high) // 2
+        candidate_sequence = search_domain[middle]
+        if _check_ahead_target(candidate_sequence, target_date):
+            high = middle
+        else:
+            low = middle + 1
 
+    result = search_domain[low]
+    logger.debug("Found the earliest segment", sequence=result)
 
-def echo_notice(message: str) -> None:
-    click.echo(f"~ {message}")
+    return result
```

### Comparing `ytpb-2024.5.3/src/ytpb/cli/parameters.py` & `ytpb-2024.5.30/src/ytpb/cli/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 from enum import auto, StrEnum
 from typing import Literal, NamedTuple
 
 import click
 import structlog
 from timedelta_isoformat import timedelta as isotimedelta
 
-from ytpb import types
+from ytpb.cli.formats import ALIAS_RE as FORMAT_ALIAS_RE, expand_aliases
+from ytpb.cli.utils.date import ensure_date_aware
+
 from ytpb.conditional import FORMAT_SPEC_RE
-from ytpb.types import SegmentSequence
-from ytpb.utils.date import ensure_date_aware
+
+from ytpb.types import AbsolutePointInStream, SegmentSequence
 
 logger = structlog.get_logger(__name__)
 
 
 class PointInStreamParamType(click.ParamType):
     def __init__(self, allowed_literals: list[str] = None):
         if allowed_literals:
             self.allowed_literals = allowed_literals
         else:
             self.allowed_literals = []
 
-    def convert(self, value: str, param, ctx) -> types.AbsolutePointInStream | str:
+    def convert(self, value: str, param, ctx) -> AbsolutePointInStream | str:
         match value:
             # Allowed literals
             case literal if value in self.allowed_literals:
                 output = literal
             # Time of today
             case x if x[0] == "T" or (":" in x and "-" not in x):
                 parsed_time = time.fromisoformat(x)
@@ -111,15 +113,15 @@
             # Date and time
             case x if "T" in x:
                 output = datetime.fromisoformat(x)
             # Unix timestamp
             case x if x.startswith("@"):
                 timestamp = float(x.lstrip("@"))
                 output = datetime.fromtimestamp(timestamp, timezone.utc)
-            case "now" | ".." as x:
+            case "earliest" | "now" | ".." as x:
                 output = x
             case _:
                 raise click.BadParameter(f"Incorrectly formatted part: {part}")
 
         return output
 
     def convert(
@@ -144,26 +146,32 @@
         match parsed_start, parsed_end:
             # Two durations
             case [timedelta(), timedelta()]:
                 raise click.BadParameter("Two durations are ambiguous.")
             # Two '..' keywords
             case ["..", ".."]:
                 raise click.BadParameter("Two '..' are ambiguous.")
+            # Anything and 'earliest'
+            case [_, "earliest" as x]:
+                raise click.BadParameter(
+                    f"Keyword '{x}' is only allowed for the start part."
+                )
+            # 'Now' and anything
             case ["now" as x, _]:
                 raise click.BadParameter(
                     f"Keyword '{x}' is only allowed for the end part."
                 )
             # Duration and '..'
             case [timedelta(), ".."] | ["..", timedelta()]:
                 raise click.BadParameter(
                     "Keyword '..' is not compatible with duration."
                 )
             # Anything compatible and 'now' or '..'
-            case [int() | datetime() | timedelta(), "now" | ".."] | [
-                "..",
+            case [int() | datetime() | timedelta() | "earliest", "now" | ".."] | [
+                ".." | "earliest",
                 int() | datetime() | timedelta(),
             ]:
                 start = parsed_start
                 end = parsed_end
             # Replacing components and date and time
             case (str(), datetime()) | (datetime(), str()):
                 if isinstance(parsed_start, str):
@@ -178,15 +186,16 @@
                     "Replacement components are only compatible with date and time."
                 )
             # Remaining and compatible
             case [_, _]:
                 start = parsed_start
                 end = parsed_end
 
-        if type(start) == type(end) and start >= end:
+        both_same_type = type(start) == type(end)
+        if both_same_type and not isinstance(start, str) and start >= end:
             raise click.BadParameter(
                 f"Start is ahead or equal to end: {start} >= {end}"
             )
 
         return start, end
 
 
@@ -198,19 +207,28 @@
 class FormatSpecParamType(click.ParamType):
     def __init__(self, format_spec_type: FormatSpecType):
         self.format_spec_type = format_spec_type
 
     def convert(
         self, value: str, param: click.Parameter, ctx: click.Context
     ) -> str | None:
-        if value in ("", "none"):
-            output = None
-        else:
-            guard_condition = f"mime_type contains {self.format_spec_type.value}"
-            if matched := FORMAT_SPEC_RE.match(value):
-                if matched.group("function"):
-                    replace_with = f"{guard_condition} and [{matched.group('expr')}]"
-                    output = value.replace(matched.group("expr"), replace_with)
-                else:
-                    output = f"{guard_condition} and [{value}]"
+        if value == "" or value == "none":
+            return None
+
+        output = value
+        if FORMAT_ALIAS_RE.search(output):
+            alias_substitutions = ctx.obj.config.traverse("general.aliases")
+            unaliased_value = expand_aliases(output, alias_substitutions)
+            logger.debug(
+                f"Format spec expression '{value}' expanded as '{unaliased_value}'"
+            )
+            output = unaliased_value
+
+        guard_condition = f"mime_type contains {self.format_spec_type.value}"
+        if matched := FORMAT_SPEC_RE.match(output):
+            if matched.group("function"):
+                replace_with = f"{guard_condition} and [{matched.group('expr')}]"
+                output = output.replace(matched.group("expr"), replace_with)
+            else:
+                output = f"{guard_condition} and [{output}]"
 
         return output
```

### Comparing `ytpb-2024.5.3/src/ytpb/cli/commands/capture.py` & `ytpb-2024.5.30/src/ytpb/cli/commands/capture.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     TaskProgressColumn,
     TextColumn,
     TimeRemainingColumn,
 )
 from timedelta_isoformat import timedelta as isotimedelta
 
 from ytpb.actions.capture import capture_frames, extract_frame_as_image
-from ytpb.cli.commands.download import render_download_output_path_context
 from ytpb.cli.common import (
     create_playback,
     echo_notice,
     get_parameter_by_name,
     prepare_line_for_summary_info,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
@@ -41,79 +40,45 @@
 )
 from ytpb.cli.parameters import (
     FormatSpecParamType,
     FormatSpecType,
     InputRewindInterval,
     PointInStreamParamType,
 )
+from ytpb.cli.templating import (
+    check_is_template,
+    IntervalOutputPathContext,
+    MinimalOutputPathContext,
+    render_template,
+    VideoStreamOutputPathContext,
+)
+from ytpb.cli.utils.date import DurationFormatPattern, format_duration
+from ytpb.cli.utils.path import sanitize_for_filename
 from ytpb.errors import QueryError, SegmentDownloadError, SequenceLocatingError
 from ytpb.locate import SegmentLocator
 from ytpb.segment import Segment
-from ytpb.types import (
-    AbsolutePointInStream,
-    AddressableMappingProtocol,
-    DateInterval,
-    SegmentSequence,
-)
-from ytpb.utils.date import DurationFormatPattern, format_duration, ISO8601DateFormatter
+from ytpb.types import AbsolutePointInStream, DateInterval, SegmentSequence
 from ytpb.utils.other import resolve_relativity_in_interval
-from ytpb.utils.path import (
-    expand_template_output_path,
-    IntervalOutputPathContext,
-    MinimalOutputPathContext,
-    OUTPUT_PATH_PLACEHOLDER_RE,
-    OutputPathContextRenderer,
-    render_minimal_output_path_context,
-)
 from ytpb.utils.remote import request_reference_sequence
 
 logger = structlog.get_logger(__name__)
 
 
-class CaptureOutputPathContext(MinimalOutputPathContext):
+class CaptureOutputPathContext(MinimalOutputPathContext, VideoStreamOutputPathContext):
+    #: Date the frame was captured.
     moment_date: datetime
 
 
-class TimelapseOutputPathContext(MinimalOutputPathContext, IntervalOutputPathContext):
+class TimelapseOutputPathContext(
+    MinimalOutputPathContext, VideoStreamOutputPathContext, IntervalOutputPathContext
+):
+    #: Interval at wich frames are captured.
     every: timedelta
 
 
-def render_capture_output_path_context(
-    context: CaptureOutputPathContext,
-    config_settings: AddressableMappingProtocol,
-) -> CaptureOutputPathContext:
-    output = context
-    for variable in CaptureOutputPathContext.__annotations__.keys():
-        match variable:
-            case "moment_date" as x:
-                date_formatter = ISO8601DateFormatter()
-                output[x] = OutputPathContextRenderer.render_date(
-                    context[x], date_formatter, config_settings
-                )
-
-    output.update(render_minimal_output_path_context(context, config_settings))
-
-    return output
-
-
-def render_timelapse_output_path_context(
-    context: TimelapseOutputPathContext,
-    config_settings: AddressableMappingProtocol,
-) -> TimelapseOutputPathContext:
-    output = context
-    for variable in TimelapseOutputPathContext.__annotations__.keys():
-        match variable:
-            case "every" as x:
-                output[x] = isotimedelta.isoformat(context[x]).replace("P", "E")
-
-    output.update(render_download_output_path_context(context, config_settings))
-
-    return output
-
-
 def convert_every_option_to_timedelta(
     ctx: click.Context, param: click.Option, value: str
 ) -> timedelta:
     try:
         output = isotimedelta.fromisoformat(f"PT{value}")
     except ValueError:
         raise click.BadParameter(
@@ -123,15 +88,15 @@
 
 
 def print_timelapse_summary_info(
     dates: list[datetime], end_date: datetime, every: timedelta
 ) -> None:
     click.echo(
         "Every {} a time-lapse frame will be captured:".format(
-            format_duration(every, DurationFormatPattern.IN_SENTENCE)
+            format_duration(every, DurationFormatPattern.SENTENCE)
         )
     )
 
     def _format_datetime(x):
         return email.utils.format_datetime(x).split(", ")[1]
 
     click.echo("{:>12}: {} / S".format("Frame 1", _format_datetime(dates[0])))
@@ -266,25 +231,25 @@
         "Actual moment: {}, seq. {}".format(
             actual_moment_info_line, moment_segment.sequence
         )
     )
 
     # Absolute output path of an image with extension.
     final_output_path: Path
-    if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
+    if check_is_template(str(output_path)):
         template_context: CaptureOutputPathContext = {
             "id": playback.video_id,
-            "title": playback.info.title,
+            "title": sanitize_for_filename(playback.info.title),
+            "video_stream": reference_stream,
             "moment_date": requested_moment_date,
         }
-        final_output_path = expand_template_output_path(
+        final_output_path = render_template(
             output_path,
+            ctx.obj.jinja_environment,
             template_context,
-            render_capture_output_path_context,
-            ctx.obj.config,
         )
     else:
         final_output_path = output_path
     final_output_path = resolve_output_path(final_output_path)
 
     image = extract_frame_as_image(moment_segment, requested_moment_date)
     image.save(final_output_path, quality=80)
@@ -452,31 +417,32 @@
         echo_notice("Preview mode enabled, only first 3 frames will be taken.")
         dates_to_capture = dates_to_capture[:3]
 
     click.echo()
 
     # Absolute output path of images with a numeric pattern.
     final_output_path: Path
-    if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
+    if check_is_template(str(output_path)):
         input_timezone = requested_date_interval.start.tzinfo
         template_context: TimelapseOutputPathContext = {
             "id": playback.video_id,
-            "title": playback.info.title,
+            "title": sanitize_for_filename(playback.info.title),
+            "audio_stream": None,
+            "video_stream": reference_stream,
             "input_start_date": requested_date_interval.start,
             "input_end_date": requested_date_interval.end,
             "actual_start_date": actual_date_interval.start.astimezone(input_timezone),
             "actual_end_date": actual_date_interval.end.astimezone(input_timezone),
             "duration": requested_end_date - requested_start_date,
             "every": every,
         }
-        final_output_path = expand_template_output_path(
+        final_output_path = render_template(
             output_path,
+            ctx.obj.jinja_environment,
             template_context,
-            render_timelapse_output_path_context,
-            ctx.obj.config,
         )
     else:
         final_output_path = output_path
     final_output_path = resolve_output_path(final_output_path)
 
     click.echo("(<<) Capturing frames as images:")
```

### Comparing `ytpb-2024.5.3/src/ytpb/cli/commands/download.py` & `ytpb-2024.5.30/src/ytpb/cli/commands/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import pickle
 import shutil
 import sys
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from functools import partial
 from pathlib import Path
+from typing import Any, Callable, TypedDict
 
 import click
 import cloup
 import structlog
 from cloup.constraints import constraint, mutually_exclusive, require_any
 
 from ytpb import actions
 from ytpb.cli.common import (
     create_playback,
     echo_notice,
+    find_earliest_sequence,
     get_parameter_by_name,
     print_summary_info,
     query_streams_or_exit,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
     resolve_output_path,
     stream_argument,
@@ -27,46 +29,72 @@
     cache_options,
     interval_option,
     keep_temp_option,
     validate_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import FormatSpecParamType, FormatSpecType, InputRewindInterval
+from ytpb.cli.templating import (
+    AudioStreamOutputPathContext,
+    check_is_template,
+    IntervalOutputPathContext,
+    MinimalOutputPathContext,
+    render_template,
+    VideoStreamOutputPathContext,
+)
+from ytpb.cli.utils.path import (
+    remove_directories_between,
+    sanitize_for_filename,
+    try_get_relative_path,
+)
 from ytpb.download import compose_default_segment_filename
 from ytpb.errors import SequenceLocatingError
 from ytpb.merge import merge_segments
 from ytpb.types import (
-    AddressableMappingProtocol,
     AudioOrVideoStream,
     DateInterval,
     RelativeSegmentSequence,
     SegmentSequence,
 )
 from ytpb.utils.other import resolve_relativity_in_interval
-from ytpb.utils.path import (
-    expand_template_output_path,
-    IntervalOutputPathContext,
-    MinimalOutputPathContext,
-    OUTPUT_PATH_PLACEHOLDER_RE,
-    remove_directories_between,
-    render_interval_output_path_context,
-    render_minimal_output_path_context,
-    try_get_relative_path,
-)
 from ytpb.utils.remote import request_reference_sequence
 from ytpb.utils.url import build_segment_url, extract_parameter_from_url
 
 logger = structlog.get_logger(__name__)
 
 
 class DownloadOutputPathContext(
-    MinimalOutputPathContext, IntervalOutputPathContext
+    MinimalOutputPathContext,
+    AudioStreamOutputPathContext,
+    VideoStreamOutputPathContext,
+    IntervalOutputPathContext,
 ): ...
 
 
+class MetadataTagsContext(TypedDict):
+    #: Video's title.
+    title: str
+    #: Video's author (channel's name).
+    author: str
+    #: YouTube video URL as a comment.
+    comment: str
+    #: Input start date.
+    input_start_date: str
+    #: Input end date.
+    input_end_date: str
+    #: Actual start date.
+    actual_start_date: str
+    #: Actual end date.
+    actual_end_date: str
+    #: Start segment sequence number.
+    start_segment: str
+    #: End segment sequence number.
+    end_segment: str
+
+
 def compose_resume_filename(
     video_id: str, streams: list[AudioOrVideoStream | None]
 ) -> str:
     for i, arg in enumerate(sys.argv):
         if arg in ("--interval", "-i"):
             interval_option_value = sys.argv[i + 1]
             break
@@ -77,24 +105,14 @@
     interval_part = interval_part.replace("/", "-")
 
     itag_part = "".join([stream.itag for stream in streams if stream])
 
     return f"{video_id}-{interval_part}-{itag_part}.resume"
 
 
-def render_download_output_path_context(
-    context: DownloadOutputPathContext,
-    config_settings: AddressableMappingProtocol,
-) -> DownloadOutputPathContext:
-    output = context
-    output.update(render_minimal_output_path_context(context, config_settings))
-    output.update(render_interval_output_path_context(context, config_settings))
-    return output
-
-
 @cloup.command("download", short_help="Download excerpts.", help="Download an excerpt.")
 @cloup.option_group(
     "Input options",
     interval_option,
     cloup.option(
         "-af",
         "--audio-format",
@@ -130,14 +148,19 @@
         help="Print base URLs and exit.",
     ),
     cloup.option(
         "--dump-segment-urls",
         is_flag=True,
         help="Print segment URLs and exit.",
     ),
+    cloup.option(
+        "--dump-rewind-interval",
+        is_flag=True,
+        help="Print segments rewind interval and exit.",
+    ),
 )
 @cloup.option_group(
     "Output options",
     cloup.option(
         "-o",
         "--output",
         "output_path",
@@ -145,36 +168,32 @@
         help="Output path (without extension).",
         callback=validate_output_path(DownloadOutputPathContext),
     ),
     cloup.option(
         "-S", "--keep-segments", is_flag=True, help="Keep downloaded segments."
     ),
     cloup.option(
+        "-s",
         "--segments-output-dir",
         "segments_output_dir_option",
         type=click.Path(path_type=Path),
         help="Location where to download segments to.",
     ),
+    cloup.option(
+        "-c", "--cut", is_flag=True, help="Accurately cut an excerpt at boundaries."
+    ),
     cloup.option("--no-metadata", is_flag=True, help="Do not write metadata tags."),
-    cloup.option("--no-cut", is_flag=True, help="Do not perform excerpt cutting."),
     cloup.option(
         "--no-merge",
         is_flag=True,
         help="Only download segments, without merging.",
     ),
 )
 @click.option(
-    "-m",
-    "--from-manifest",
-    metavar="PATH",
-    type=click.Path(path_type=Path),
-    help="Path to a MPEG-DASH manifest.",
-)
-@click.option(
-    "-X",
+    "-x",
     "--dry-run",
     is_flag=True,
     help="Run without downloading.",
 )
 @yt_dlp_option
 @click.option(
     "--ignore-resume", is_flag=True, help="Avoid resuming unfinished download."
@@ -190,30 +209,30 @@
     interval: InputRewindInterval,
     audio_format: str,
     video_format: str,
     preview_start: bool,
     preview_end: bool,
     dump_base_urls: bool,
     dump_segment_urls: bool,
+    dump_rewind_interval: bool,
     output_path: Path,
     keep_segments: bool,
     segments_output_dir_option: Path,
+    cut: bool,
     no_metadata: bool,
-    no_cut: bool,
     no_merge: bool,
-    from_manifest: Path,
     dry_run: bool,
     yt_dlp: bool,
     ignore_resume: bool,
     no_cache: bool,
     force_update_cache: bool,
     keep_temp: bool,
     stream_url: str,
 ) -> int:
-    if dump_base_urls or dump_segment_urls:
+    if dump_base_urls or dump_segment_urls or dump_rewind_interval:
         suppress_output()
 
     if no_merge:
         keep_segments = True
 
     playback = create_playback(ctx)
 
@@ -269,14 +288,18 @@
 
     reference_stream = video_stream or audio_stream
     reference_base_url = reference_stream.base_url
     head_sequence = request_reference_sequence(reference_base_url, playback.session)
 
     requested_start, requested_end = resolve_relativity_in_interval(*interval)
 
+    if requested_start == "earliest":
+        head_date = datetime.now(timezone.utc)
+        requested_start = find_earliest_sequence(playback, head_sequence, head_date)
+
     if isinstance(requested_start, SegmentSequence):
         raise_for_too_far_sequence(
             requested_start, head_sequence, reference_base_url, ctx, "interval"
         )
         raise_for_sequence_ahead_of_current(
             requested_start, head_sequence, ctx, "interval"
         )
@@ -361,14 +384,23 @@
         build_dump_url = lambda base_url: build_segment_url(base_url, range_part)
         if audio_format:
             click.echo(build_dump_url(audio_stream.base_url), ctx.obj.original_stdout)
         if video_format:
             click.echo(build_dump_url(video_stream.base_url), ctx.obj.original_stdout)
         sys.exit()
 
+    if dump_rewind_interval:
+        click.echo(
+            "{start}-{end}".format(
+                start=rewind_interval.start.sequence, end=rewind_interval.end.sequence
+            ),
+            ctx.obj.original_stdout,
+        )
+        sys.exit()
+
     # if preview_mode and interval[1] != "..":
     if preview_mode:
         echo_notice(
             "Preview mode enabled, interval {} is ignored.".format(
                 "end" if preview_start else "start"
             )
         )
@@ -399,17 +431,17 @@
     requested_date_interval = DateInterval(requested_start_date, requested_end_date)
     actual_date_interval = DateInterval(
         start_segment.ingestion_start_date,
         end_segment.ingestion_end_date,
     )
 
     cut_kwargs: dict[str, float] = {}
-    if not no_cut:
-        cut_at_start = rewind_interval.start.cut_at if preview_start else 0
-        cut_at_end = rewind_interval.end.cut_at if preview_end else 0
+    if cut:
+        cut_at_start = 0 if preview_start else rewind_interval.start.cut_at
+        cut_at_end = 0 if preview_end else rewind_interval.end.cut_at
         cut_kwargs.update(
             {
                 "cut_at_start": cut_at_start,
                 "cut_at_end": cut_at_end,
             }
         )
         actual_date_interval = DateInterval(
@@ -426,34 +458,35 @@
         final_output_path: Path
 
         if preview_mode:
             default_output_path = ctx.obj.config.traverse(
                 "options.download.output_path"
             )
             if str(output_path) == default_output_path:
-                output_path = "<title>_<id>_preview"
+                output_path = Path("{{ title|adjust }}_{{ id }}_preview")
 
-        if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
+        if check_is_template(str(output_path)):
             input_timezone = requested_date_interval.start.tzinfo
             template_context: DownloadOutputPathContext = {
                 "id": playback.video_id,
-                "title": playback.info.title,
+                "title": sanitize_for_filename(playback.info.title),
+                "audio_stream": audio_stream,
+                "video_stream": video_stream,
                 "input_start_date": requested_date_interval.start,
                 "input_end_date": requested_date_interval.end,
-                "actual_start_date": actual_date_interval.start.astimezone(
-                    input_timezone
+                "actual_start_date": (
+                    actual_date_interval.start.astimezone(input_timezone)
                 ),
                 "actual_end_date": actual_date_interval.end.astimezone(input_timezone),
                 "duration": requested_end_date - requested_start_date,
             }
-            final_output_path = expand_template_output_path(
+            final_output_path = render_template(
                 output_path,
+                ctx.obj.jinja_environment,
                 template_context,
-                render_download_output_path_context,
-                ctx.obj.config,
             )
         else:
             final_output_path = output_path
         final_output_path = resolve_output_path(final_output_path)
 
         if preview_mode:
             segments_output_directory = playback.get_temp_directory()
@@ -579,49 +612,67 @@
             if video_stream:
                 audio_and_video_segment_paths[1] = [
                     segments_output_directory
                     / compose_default_segment_filename(sequence, video_stream.base_url)
                     for sequence in rewind_interval.sequences
                 ]
 
-            if no_cut:
-                click.echo("2. Merging segments (no cut requested)... ", nl=False)
+            if cut:
+                click.echo("2. Merging segments (cut requested)... ", nl=False)
             else:
                 click.echo("2. Merging segments (may take a while)... ", nl=False)
 
-            metadata_tags: dict[str, str] = {}
+            metadata_tags: dict[str, Any] = {}
             if not no_metadata:
-                convert_timestamp_to_string = lambda timestamp: f"{timestamp:.6f}"
-                metadata_tags = {
+
+                def _convert_date_to_isostring(date: datetime) -> str:
+                    iso_date = date.astimezone(timezone.utc)
+                    return iso_date.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+
+                metadata_date_converter: Callable[[datetime], str]
+                match ctx.obj.config.traverse("output.metadata.dates"):
+                    case "unix":
+                        metadata_date_converter = lambda d: f"{d.timestamp():.6f}"
+                    case "iso":
+                        metadata_date_converter = _convert_date_to_isostring
+                    case _ as value:
+                        click.echo()
+                        logger.warning(
+                            f"Unknown 'output.metadata.dates = {value}' config value, "
+                            "fallback to 'iso'"
+                        )
+                        metadata_date_converter = _convert_date_to_isostring
+
+                metadata_context: MetadataTagsContext = {
                     "title": playback.info.title,
                     "author": playback.info.author,
                     "comment": playback.video_url,
-                    "actual_start_time": convert_timestamp_to_string(
-                        actual_date_interval.start.timestamp()
+                    "input_start_date": metadata_date_converter(
+                        requested_date_interval.start
                     ),
-                    "actual_end_time": convert_timestamp_to_string(
-                        actual_date_interval.end.timestamp()
+                    "input_end_date": metadata_date_converter(
+                        requested_date_interval.end
                     ),
-                    "input_start_time": convert_timestamp_to_string(
-                        requested_date_interval.start.timestamp()
+                    "actual_start_date": metadata_date_converter(
+                        actual_date_interval.start
                     ),
-                    "input_end_time": convert_timestamp_to_string(
-                        requested_date_interval.end.timestamp()
+                    "actual_end_date": metadata_date_converter(
+                        actual_date_interval.end
                     ),
-                    "start_sequence_number": rewind_interval.start.sequence,
-                    "end_sequence_number": rewind_interval.end.sequence,
+                    "start_segment": str(rewind_interval.start.sequence),
+                    "end_segment": str(rewind_interval.end.sequence),
                 }
 
             merged_path = merge_segments(
                 audio_and_video_segment_paths[0],
                 audio_and_video_segment_paths[1],
                 output_directory=final_output_path.parent,
                 output_stem=final_output_path.name,
                 temp_directory=playback.get_temp_directory(),
-                metadata_tags=metadata_tags,
+                metadata_tags=metadata_context,
                 **cut_kwargs,
             )
 
             click.echo("done.\n")
             click.echo(f"Success! Saved to '{try_get_relative_path(merged_path)}'.")
 
             if keep_segments and not preview_mode:
@@ -651,15 +702,15 @@
                 for path in paths:
                     path.unlink()
         except OSError:
             logger.warning("Could not remove segment: %s", path)
         try:
             if need_to_remove_segments_directory:
                 logger.debug(
-                    "Remove created segments directory: %s",
+                    "Remove segments directory: %s",
                     segments_directory_to_remove,
                 )
                 remove_directories_between(
                     segments_directory_to_remove, segments_output_directory
                 )
         except OSError:
             logger.warning(
```

### Comparing `ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py` & `ytpb-2024.5.30/src/ytpb/cli/commands/mpd.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from cloup.constraints import constraint, require_any
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from ytpb import types
 from ytpb.actions.compose import compose_static_mpd, refresh_mpd
-from ytpb.cli.commands.download import (
-    DownloadOutputPathContext,
-    render_download_output_path_context,
-)
 from ytpb.cli.common import (
     CONSOLE_TEXT_WIDTH,
     create_playback,
     print_summary_info,
     query_streams_or_exit,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
@@ -29,32 +25,37 @@
 from ytpb.cli.options import (
     cache_options,
     interval_option,
     validate_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import FormatSpecParamType, FormatSpecType
+from ytpb.cli.templating import (
+    check_is_template,
+    IntervalOutputPathContext,
+    MinimalOutputPathContext,
+    render_template,
+)
+from ytpb.cli.utils.date import express_timedelta_in_words
+from ytpb.cli.utils.path import sanitize_for_filename
 from ytpb.errors import BroadcastStatusError
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
 from ytpb.info import BroadcastStatus
 from ytpb.playback import Playback
 from ytpb.representations import extract_representations
 from ytpb.streams import Streams
 from ytpb.types import DateInterval, SegmentSequence
-from ytpb.utils.date import express_timedelta_in_words
 from ytpb.utils.other import resolve_relativity_in_interval
-from ytpb.utils.path import expand_template_output_path, OUTPUT_PATH_PLACEHOLDER_RE
 from ytpb.utils.remote import request_reference_sequence
 from ytpb.utils.url import build_video_url_from_base_url, extract_parameter_from_url
 
 logger = structlog.get_logger(__name__)
 
 
-MpdOutputPathContext = DownloadOutputPathContext
-render_mpd_output_path_context = render_download_output_path_context
+class MPDOutputPathContext(MinimalOutputPathContext, IntervalOutputPathContext): ...
 
 
 def print_audio_table(console, streams, **table_kwargs):
     table = Table(title="(Audio)", **table_kwargs)
     for name in ("itag", "Format", "Codec", "Sampling"):
         if name == "itag":
             table.add_column(" " + name, ratio=0.2, justify="center")
@@ -106,15 +107,15 @@
 )
 @click.option(
     "-o",
     "--output",
     "output_path",
     type=click.Path(path_type=Path),
     help="Output path (with extension).",
-    callback=validate_output_path(MpdOutputPathContext),
+    callback=validate_output_path(MPDOutputPathContext),
 )
 @yt_dlp_option
 @cache_options
 @stream_argument
 @constraint(require_any, ["audio_formats", "video_formats"])
 @click.pass_context
 def compose_command(
@@ -225,40 +226,39 @@
     )
 
     print_summary_info(requested_date_interval, actual_date_interval, rewind_interval)
     click.echo()
 
     # Absolute output path of a manifest with extension.
     final_output_path: Path
-    if OUTPUT_PATH_PLACEHOLDER_RE.search(str(output_path)):
+    if check_is_template(str(output_path)):
         input_timezone = requested_date_interval.start.tzinfo
-        template_context: MpdOutputPathContext = {
+        template_context: MPDOutputPathContext = {
             "id": playback.video_id,
-            "title": playback.info.title,
+            "title": sanitize_for_filename(playback.info.title),
             "input_start_date": requested_date_interval.start,
             "input_end_date": requested_date_interval.end,
             "actual_start_date": actual_date_interval.start.astimezone(input_timezone),
             "actual_end_date": actual_date_interval.end.astimezone(input_timezone),
             "duration": requested_end_date - requested_start_date,
         }
-        final_output_path = expand_template_output_path(
+        final_output_path = render_template(
             output_path,
+            ctx.obj.jinja_environment,
             template_context,
-            render_mpd_output_path_context,
-            ctx.obj.config,
         )
     else:
         final_output_path = output_path
     final_output_path = resolve_output_path(final_output_path)
 
     click.echo("(<<) Composing MPEG-DASH manifest...")
     streams = Streams(queried_audio_streams + queried_video_streams)
     composed_manifest = compose_static_mpd(playback, rewind_interval, streams)
 
-    with open(final_output_path, "w") as f:
+    with open(final_output_path, "w", encoding="utf-8") as f:
         f.write(composed_manifest)
 
     try:
         saved_to_path_value = f"{final_output_path.relative_to(Path.cwd())}"
     except ValueError:
         saved_to_path_value = final_output_path
 
@@ -292,15 +292,15 @@
     except BroadcastStatusError as e:
         match e.status:
             case BroadcastStatus.COMPLETED:
                 click.echo("Stream was live, but now it's finished", err=True)
         sys.exit(1)
 
     refreshed = refresh_mpd(manifest_content, playback.streams)
-    with open(manifest, "w") as f:
+    with open(manifest, "w", encoding="utf-8") as f:
         f.write(refreshed)
 
     some_base_url = next(iter(playback.streams)).base_url
     expires_at_time = int(extract_parameter_from_url("expire", some_base_url))
     expires_at_date = datetime.fromtimestamp(expires_at_time)
     expires_in = express_timedelta_in_words(expires_at_date - datetime.now())
```

### Comparing `ytpb-2024.5.3/src/ytpb/utils/date.py` & `ytpb-2024.5.30/src/ytpb/cli/utils/date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,86 @@
 import enum
 import math
+import os
 import re
 import string
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, time, timedelta
 from typing import Any, Literal
 
 
 @dataclass
-class ISO8601DateStyleParameters:
+class ISODateStyleParameters:
     format: Literal["basic", "extended"] = "basic"
     precision: Literal["reduced", "complete"] = "complete"
     offset_format: Literal["hh", "hhmm"] = "hh"
     fractional_component: Literal["sec"] | None = None
     fraction_delimiter: Literal[".", ","] = "."
     use_z_for_utc: bool = False
 
 
+class DurationFormatPattern(enum.Enum):
+    HMS = "[%-Hh][%-Mm][%-Ss]"
+    ISO = "PT[%-HH][%-MM][%-SS]"
+    NUMERIC = "%H:%M:%S"
+    SENTENCE = "[%-H h ][%-M m ][%-S s]"
+
+
+class ISODateFormatter(string.Formatter):
+    """A variant of `string.Formatter` that format dates in ISO 8601
+    format.
+
+    This extends the format specification for `datetime` objects with
+    the following, ISO-8601 related, styles: 'basic', 'extended', 'reduced',
+    'complete', 'hh', 'hhmm', and 'z'.
+    """
+
+    def convert_field(self, value: Any, conversion: str | None) -> Any:
+        if isinstance(value, datetime):
+            if conversion == "t":
+                return int(value.timestamp())
+        return value
+
+    def format_field(self, value: Any, format_spec: str) -> Any:
+        known_styles = ("basic", "extended", "reduced", "complete", "hh", "hhmm", "z")
+        if isinstance(value, datetime):
+            match format_spec:
+                case spec if set(spec.split(",")).issubset(known_styles):
+                    style_parameters = build_style_parameters_from_spec(spec)
+                    output = format_iso_datetime(value, style_parameters)  # type: ignore
+                case "":
+                    output = format_iso_datetime(value)
+        else:
+            output = super().format_field(value, format_spec)
+
+        return output
+
+
 def ensure_date_aware(date: datetime) -> datetime:
     """Ensure a date is timezone aware."""
     if date.tzinfo is None:
         local_tzinfo = date.astimezone().tzinfo
         return date.replace(tzinfo=local_tzinfo)
     else:
         return date
 
 
 def format_iso_datetime(
     date: datetime,
-    style: ISO8601DateStyleParameters | None = None,
+    style: ISODateStyleParameters | None = None,
 ) -> str:
-    """Format `datetime` objects after ISO 8601. Supports complete and reduced
-    date and time representations in basic and extended formats.
+    """Format `datetime` objects after ISO 8601.
 
-    Complete:
-    - [year]["-"][month]["-"][day]["T"][hour][min][sec]
+    Supports complete and reduced date and time representations in basic and
+    extended formats.
     """
 
     if style is None:
-        style = ISO8601DateStyleParameters()
+        style = ISODateStyleParameters()
 
     plain_offset = date.strftime("%z")
     if plain_offset == "":
         raise ValueError("datetime object should be timezone aware")
 
     match style.precision:
         case "reduced":
@@ -92,30 +129,27 @@
         output = f"{date_string}{offset}"
     else:
         output = f"{date_string}{offset}"
 
     return output
 
 
-class DurationFormatPattern(enum.Enum):
-    NUMERIC = "%H:%M%:%S"
-    ISO8601 = "PT[%-HH][%-MM][%-SS]"
-    IN_SENTENCE = "[%-H h ][%-M m ][%-S s]"
-
-
 def format_duration(duration: timedelta, pattern: DurationFormatPattern) -> str:
     total_seconds = math.floor(duration.total_seconds() + 0.5)
     total_minutes, ss = divmod(total_seconds, 60)
     hh, mm = divmod(total_minutes, 60)
-
-    output = pattern.value
     time_object = time(hh, mm, ss)
 
-    optional_parts_re = r"\[(?P<part>(?P<fmt>%-?[HMS]).*?)\]"
-    for matched in re.finditer(optional_parts_re, pattern.value):
+    pattern_value = pattern.value
+    if os.name == "nt":
+        pattern_value = pattern_value.replace("%-", "%#")
+
+    output = pattern_value
+    optional_parts_re = r"\[(?P<part>(?P<fmt>%[-#]?[HMS]).*?)\]"
+    for matched in re.finditer(optional_parts_re, pattern_value):
         if int(time_object.strftime(matched.group("fmt"))) == 0:
             output = output.replace(matched.group(0), "")
         else:
             formatted_part = time_object.strftime(matched.group("part"))
             output = output.replace(matched.group(0), formatted_part)
 
     output = time_object.strftime(output).rstrip(" ")
@@ -180,29 +214,29 @@
         output = "a moment"
 
     return output
 
 
 def build_style_parameters_from_spec(
     style_spec: str,
-) -> ISO8601DateStyleParameters | None:
+) -> ISODateStyleParameters | None:
     if not style_spec:
         return None
 
     style_parameters = {}
     input_styles = set([x.strip() for x in style_spec.split(",")])
 
     if "z" in input_styles:
         style_parameters["use_z_for_utc"] = True
         input_styles.remove("z")
 
     conflicting_styles_map: dict[str, str] = {}
     parameters_to_check = ["format", "precision", "offset_format"]
     for field_name in parameters_to_check:
-        field = ISO8601DateStyleParameters.__dataclass_fields__[field_name]
+        field = ISODateStyleParameters.__dataclass_fields__[field_name]
         conflicting_styles_map[field_name] = field.type.__args__
 
     for input_style in input_styles:
         for parameter, parameter_styles in conflicting_styles_map.items():
             if input_style in parameter_styles:
                 if already_set_style := style_parameters.get(parameter, None):
                     conflicted_styles = sorted([already_set_style, input_style])
@@ -213,29 +247,8 @@
                 else:
                     style_parameters[parameter] = input_style
                     break
 
     if unknown_styles := input_styles ^ set(style_parameters.values()):
         warnings.warn(f"Ignoring unknown style(s): {', '.join(sorted(unknown_styles))}")
 
-    return ISO8601DateStyleParameters(**style_parameters)
-
-
-class ISO8601DateFormatter(string.Formatter):
-    """A variant of `string.Formatter` that format dates in ISO 8601
-    format.
-
-    This extends the format specification for `datetime` objects with
-    the following, ISO-8601 related, styles: 'basic', 'extended', 'reduced',
-    'complete', 'hh', 'hhmm', and 'z'.
-    """
-
-    def format_field(self, value: Any, format_spec: str) -> str:
-        if isinstance(value, datetime):
-            if not format_spec:
-                return format_iso_datetime(value)
-            style_parameters = build_style_parameters_from_spec(format_spec)
-            output = format_iso_datetime(value, style_parameters)  # type: ignore
-        else:
-            output = super().format_field(value, format_spec)
-
-        return output
+    return ISODateStyleParameters(**style_parameters)
```

### Comparing `ytpb-2024.5.3/src/ytpb/utils/remote.py` & `ytpb-2024.5.30/src/ytpb/utils/remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/src/ytpb/utils/url.py` & `ytpb-2024.5.30/src/ytpb/utils/url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/conftest.py` & `ytpb-2024.5.30/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
-import os
 import re
 import tempfile
 from dataclasses import asdict
 from pathlib import Path
 from typing import Callable
 from unittest.mock import Mock, patch
 
+import platformdirs
 import pytest
 import responses
 from pytest_socket import disable_socket
 
 from ytpb.info import BroadcastStatus, YouTubeVideoInfo
 from ytpb.playback import InfoFetcher, Playback
 from ytpb.segment import Segment
@@ -35,47 +35,53 @@
 @pytest.fixture
 def mocked_responses() -> responses.RequestsMock:
     with responses.RequestsMock() as responses_mock:
         yield responses_mock
 
 
 @pytest.fixture(autouse=True)
-def set_enviromental_variables(
+def monkeypatch_directories(
     monkeypatch: pytest.MonkeyPatch, tmp_path: Path, run_temp_directory: Path
 ):
-    monkeypatch.setenv("XDG_CONFIG_HOME", str(tmp_path / "config"))
-    monkeypatch.setenv("XDG_CACHE_HOME", str(tmp_path / "cache"))
+    monkeypatch.setattr(
+        "platformdirs.user_config_path", Mock(return_value=tmp_path / "config")
+    )
+    monkeypatch.setattr(
+        "platformdirs.user_cache_path", Mock(return_value=tmp_path / "cache")
+    )
     monkeypatch.setattr(
         "ytpb.playback.Playback.get_temp_directory",
         Mock(return_value=run_temp_directory),
     )
 
 
 @pytest.fixture()
 def cache_directory() -> Path:
-    cache_directory_path = Path(os.environ["XDG_CACHE_HOME"])
+    cache_directory_path = platformdirs.user_cache_path()
     cache_directory_path.mkdir(parents=True)
     return cache_directory_path
 
 
 @pytest.fixture()
 def create_cache_file(
     monkeypatch: pytest.MonkeyPatch,
     video_id: str,
     active_live_video_info: YouTubeVideoInfo,
     streams_in_list: list[AudioOrVideoStream],
     tmp_path: Path,
 ) -> None:
-    test_cache_directory = Path(os.environ["XDG_CACHE_HOME"]) / "ytpb"
+    test_cache_directory = platformdirs.user_cache_path() / "ytpb"
     test_cache_directory.mkdir(parents=True)
 
     some_base_url = streams_in_list[0].base_url
     expired_at = int(some_base_url.split("/expire/")[1].split("/")[0])
 
-    with open(test_cache_directory / f"{expired_at}~{video_id}", "w") as f:
+    with open(
+        test_cache_directory / f"{expired_at}~{video_id}", "w", encoding="utf-8"
+    ) as f:
         test_cached_item = {
             "info": asdict(active_live_video_info),
             "streams": [asdict(stream) for stream in streams_in_list],
         }
         json.dump(test_cached_item, f)
 
 
@@ -208,15 +214,15 @@
 @pytest.fixture()
 def video_base_url() -> str:
     return "https://rr5---sn-25ge7nzr.googlevideo.com/videoplayback/expire/1695928670/ei/_nwVZYXhAqbQvdIPjKmqgAM/ip/0.0.0.0/id/kHwmzef842g.2/itag/244/source/yt_live_broadcast/requiressl/yes/spc/UWF9fy2D4rPPhPMeyQnmxgP0Yhyaohs/vprv/1/playlist_type/DVR/ratebypass/yes/mime/video%2Fwebm/live/1/gir/yes/noclen/1/dur/2.000/keepalive/yes/fexp/24007246/beids/24350017/sparams/expire,ei,ip,id,itag,source,requiressl,spc,vprv,playlist_type,ratebypass,mime,live,gir,noclen,dur/sig/AOq0QJ8wRgIhAJBYRElUjO7WhY5_gsjtj0aUbXbyb9Z_Yjo7JeecnqrzAiEAkzwV4SYIFponf7BddjJ5hscSZr8hbPBSx09Qffev9AA%3D/initcwndbps/623750/mh/XB/mm/44/mn/sn-25ge7nzr/ms/lva/mt/1695906793/mv/m/mvi/5/pl/38/lsparams/initcwndbps,mh,mm,mn,ms,mv,mvi,pl/lsig/AG3C_xAwRQIhAP_FmY_xO0cSx-hk2oibYFE1AHaCvDHeYyMXXUEuBNeVAiARmaf6MprHE-eEJJx3Ai59WyTOSt8INUUWhA7MSoEO2w%3D%3D/"
 
 
 @pytest.fixture()
 def youtube_dl_info() -> dict:
-    with open(TEST_DATA_PATH / "info-1695928670.json") as f:
+    with open(TEST_DATA_PATH / "info-1695928670.json", encoding="utf-8") as f:
         return json.load(f)
 
 
 @pytest.fixture()
 def streams_in_list(youtube_dl_info: dict) -> list[AudioOrVideoStream]:
     list_of_streams: list[AudioOrVideoStream] = []
     for f in youtube_dl_info["formats"]:
```

### Comparing `ytpb-2024.5.3/tests/helpers.py` & `ytpb-2024.5.30/tests/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import timezone
 from pathlib import Path
 
+import av
 import pytest
 
-from ytpb.ffmpeg import ffprobe_show_entries
 
+def assert_number_of_streams(file_path: Path, expected: int):
+    with av.open(file_path) as container:
+        assert len(container.streams) == expected
 
-def assert_number_of_streams(filepath: Path, expected: int):
-    assert ffprobe_show_entries(filepath, "format=nb_streams") == str(expected)
 
+def assert_approx_duration(file_path: Path, expected: float, abs: float = 2.2e-2):
+    with av.open(file_path) as container:
+        actual = container.duration / 1e6
 
-def assert_approx_duration(filepath: Path, expected: float, abs: float = 2.2e-2):
-    actual = float(ffprobe_show_entries(filepath, "format=duration"))
     approx_expected = pytest.approx(expected, abs=abs)
     if actual != approx_expected:
         raise AssertionError(
             "Durations are not almost equal\n"
             f" - expected: {approx_expected}\n"
             f" + actual: {actual}"
         )
```

### Comparing `ytpb-2024.5.3/tests/test_cache.py` & `ytpb-2024.5.30/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/test_download.py` & `ytpb-2024.5.30/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/test_fetchers.py` & `ytpb-2024.5.30/tests/test_fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/test_locate.py` & `ytpb-2024.5.30/tests/test_locate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import csv
 from pathlib import Path
 from typing import NamedTuple
 
 import pytest
 
-from conftest import TEST_DATA_PATH
-
 from ytpb.locate import SegmentLocator, SequenceMetadataPair
 from ytpb.segment import Segment, SegmentMetadata
 from ytpb.types import SegmentSequence
 
+from tests.conftest import TEST_DATA_PATH
+
 
 def read_gap_case_fixture_data(path: Path) -> dict:
     class Row(NamedTuple):
         sequence: str
         ingestion_walltime_ms: str
         duration_s: str
 
     data = {}
-    with open(path) as f:
+    with open(path, encoding="utf-8") as f:
         reader = csv.reader(f, delimiter=",")
         next(reader)
         for fields in reader:
             row = Row(*fields)
             data[int(row.sequence)] = (
                 float(row.ingestion_walltime_ms) / 1e6,
                 float(row.duration_s),
@@ -154,20 +154,25 @@
 
     def test_E3(self):
         sequence, _, falls_in_gap, _ = self.ssl.find_sequence_by_time(
             1679763611.742391, end=True
         )
         assert (7947334, True) == (sequence, falls_in_gap)
 
-    @pytest.mark.xfail
+    @pytest.mark.xfail(
+        reason=(
+            "Overestimated due to large actual duration of segment 7947335 "
+            "(the difference > TIME_DIFF_TOLERANCE; see issue #5)"
+        )
+    )
     def test_S4(self):
         sequence, _, falls_in_gap, _ = self.ssl.find_sequence_by_time(
             1679763626.506922, end=True
         )
-        assert (7947335, True) == (sequence, falls_in_gap)
+        assert (7947335, False) == (sequence, falls_in_gap)
 
 
 class TestGapCase3(BaseGapCase):
     fixture_data_path = f"{TEST_DATA_PATH}/gap-cases/gap-case-3-fixture.csv"
     reference_sequence = 7958122
 
     def test_S1(self):
```

### Comparing `ytpb-2024.5.3/tests/test_merge.py` & `ytpb-2024.5.30/tests/test_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from pathlib import Path
 
 import pytest
 
-from conftest import TEST_DATA_PATH
-
-from helpers import assert_approx_duration, assert_number_of_streams
 from ytpb.merge import merge_segments
 
+from tests.conftest import TEST_DATA_PATH
+from tests.helpers import assert_approx_duration, assert_number_of_streams
+
 SEGMENT_BASE_PATH = Path(TEST_DATA_PATH) / "segments"
 
 
 def setup_function():
     os.environ["YTPB_VP9_ENCODING_SETTINGS"] = (
         "libvpx-vp9 -crf 63 -b:v 0 -deadline realtime -cpu-used 8 -row-mt 1 -s 1x1"
     )
```

### Comparing `ytpb-2024.5.3/tests/test_playback.py` & `ytpb-2024.5.30/tests/test_playback.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,32 +16,28 @@
 from pathlib import Path
 from typing import Callable
 from urllib.parse import urljoin
 
 import pytest
 import responses
 
-from conftest import TEST_DATA_PATH
 from freezegun import freeze_time
 
 from ytpb.errors import (
     BaseUrlExpiredError,
     CachedItemNotFoundError,
     SequenceLocatingError,
 )
 from ytpb.fetchers import YtpbInfoFetcher
 from ytpb.info import YouTubeVideoInfo
 from ytpb.playback import Playback, RewindInterval, RewindMoment
 from ytpb.streams import AudioOrVideoStream
-from ytpb.types import (
-    AbsolutePointInStream,
-    RelativePointInStream,
-    RelativeSegmentSequence,
-    SegmentSequence,
-)
+from ytpb.types import RelativeSegmentSequence, SegmentSequence
+
+from .conftest import TEST_DATA_PATH
 
 
 @pytest.fixture
 def fake_stream(audio_base_url: str) -> "FakeStream":
     @dataclass
     class FakeStream:
         base_url: str
@@ -296,19 +292,21 @@
     streams_in_list: list[AudioOrVideoStream],
     video_id: str,
     stream_url: str,
     tmp_path: Path,
 ):
     # Given:
     test_cache_directory = Playback.get_cache_directory()
-    test_cache_directory.mkdir(parents=True)
+    test_cache_directory.mkdir(parents=True, exist_ok=True)
 
     frozen_time = datetime.fromisoformat("2123-09-28T17:00:00+00:00").timestamp()
     expired_at = int(frozen_time - 10)
-    with open(test_cache_directory / f"{expired_at}~{video_id}", "w") as f:
+    with open(
+        test_cache_directory / f"{expired_at}~{video_id}", "w", encoding="utf-8"
+    ) as f:
         test_cache = {
             "info": asdict(active_live_video_info),
             "streams": [asdict(stream) for stream in streams_in_list],
         }
         json.dump(test_cache, f)
 
     # When:
```

### Comparing `ytpb-2024.5.3/tests/test_playback_session.py` & `ytpb-2024.5.30/tests/test_playback_session.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/test_representations.py` & `ytpb-2024.5.30/tests/test_representations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import re
-
-from conftest import TEST_DATA_PATH
-from lxml import etree
-
 from ytpb import representations
 
+from .conftest import TEST_DATA_PATH
+
 
 def test_representation_properties(audio_base_url):
     representation = representations.AudioRepresentationInfo(
         itag="140",
         codecs="mp4a.40.2",
         mime_type="audio/mp4",
         base_url=audio_base_url,
```

### Comparing `ytpb-2024.5.3/tests/test_segment.py` & `ytpb-2024.5.30/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/test_streams.py` & `ytpb-2024.5.30/tests/test_streams.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,26 +48,14 @@
 )
 def test_invalid_query(format_spec: str, streams_in_list: list[AudioOrVideoStream]):
     with pytest.raises(QueryError) as exc_info:
         Streams(streams_in_list).query(format_spec)
     assert "Format spec is invalid" in str(exc_info.value)
 
 
-def test_query_with_alias(streams_in_list: list[AudioOrVideoStream]):
-    streams = Streams(streams_in_list)
-    assert streams.query("itag eq 244 and @webm") == [streams.get_by_itag("244")]
-
-
-def test_query_with_unknown_alias(streams_in_list: list[AudioOrVideoStream]):
-    with pytest.raises(QueryError) as exc_info:
-        streams = Streams(streams_in_list)
-        streams.query("@unknown")
-    assert "Unknown alias" in str(exc_info.value)
-
-
 def test_query_with_function(streams_in_list: list[AudioOrVideoStream]):
     streams = Streams(streams_in_list)
     assert streams.query("best(format eq webm)") == [streams.get_by_itag("271")]
 
 
 def test_union(streams_in_list: list[AudioOrVideoStream]):
     a, b, *_ = streams_in_list
```

### Comparing `ytpb-2024.5.3/tests/test_types.py` & `ytpb-2024.5.30/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/actions/test_compose.py` & `ytpb-2024.5.30/tests/actions/test_compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import asdict, dataclass
 from difflib import unified_diff
 
 import freezegun
 import pytest
 from freezegun import freeze_time
 
-from helpers import patched_freezgun_astimezone
-
 from ytpb.actions.compose import compose_dynamic_mpd, compose_static_mpd, refresh_mpd
 from ytpb.errors import YtpbError
 from ytpb.playback import Playback
 from ytpb.segment import SegmentMetadata
 from ytpb.streams import Streams
 from ytpb.types import AudioOrVideoStream, AudioStream, VideoStream
 
+from tests.helpers import patched_freezgun_astimezone
+
 freezegun.api.FakeDatetime.astimezone = patched_freezgun_astimezone
 
 
 @dataclass
 class FakeRewindMoment:
     sequence: int
 
@@ -35,23 +35,23 @@
 <MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:DASH:schema:MPD:2011" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-main:2011" type="static" mediaPresentationDuration="PT66S">
   <ProgramInformation>
     <Title>Webcam Zürich HB</Title>
     <Source>https://www.youtube.com/watch?v=kHwmzef842g</Source>
   </ProgramInformation>
   <Period duration="PT66S">
     <AdaptationSet id="0" mimeType="audio/mp4" subsegmentAlignment="true">
-      <SegmentTemplate media="sq/$Number$" startNumber="7959120" duration="2000" timescale="1000"/>
       <Representation id="140" codecs="mp4a.40.2" startWithSAP="1" audioSamplingRate="44100">
         <BaseURL>{audio_base_url}</BaseURL>
+        <SegmentTemplate media="sq/$Number$" startNumber="7959120" duration="2000" timescale="1000"/>
       </Representation>
     </AdaptationSet>
     <AdaptationSet id="1" mimeType="video/webm" subsegmentAlignment="true">
-      <SegmentTemplate media="sq/$Number$" startNumber="7959120" duration="2000" timescale="1000"/>
       <Representation id="244" codecs="vp9" startWithSAP="1" width="854" height="480" maxPlayoutRate="1" frameRate="30">
         <BaseURL>{video_base_url}</BaseURL>
+        <SegmentTemplate media="sq/$Number$" startNumber="7959120" duration="2000" timescale="1000"/>
       </Representation>
     </AdaptationSet>
   </Period>
 </MPD>
 """
 
 
@@ -62,31 +62,31 @@
 <MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:DASH:schema:MPD:2011" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" type="dynamic" availabilityStartTime="2023-03-25T23:33:54.491+00:00">
   <ProgramInformation>
     <Title>Webcam Zürich HB</Title>
     <Source>https://www.youtube.com/watch?v=kHwmzef842g</Source>
   </ProgramInformation>
   <Period start="PT15917833.539S">
     <AdaptationSet id="0" mimeType="audio/mp4" subsegmentAlignment="true">
-      <SegmentTemplate media="sq/$Number$" startNumber="7959120" timescale="1000">
-        <SegmentTimeline>
-          <S d="2000" r="-1"/>
-        </SegmentTimeline>
-      </SegmentTemplate>
       <Representation id="140" codecs="mp4a.40.2" startWithSAP="1" audioSamplingRate="44100">
         <BaseURL>{audio_base_url}</BaseURL>
+        <SegmentTemplate media="sq/$Number$" startNumber="7959120" timescale="1000">
+          <SegmentTimeline>
+            <S d="2000" r="-1"/>
+          </SegmentTimeline>
+        </SegmentTemplate>
       </Representation>
     </AdaptationSet>
     <AdaptationSet id="1" mimeType="video/webm" subsegmentAlignment="true">
-      <SegmentTemplate media="sq/$Number$" startNumber="7959120" timescale="1000">
-        <SegmentTimeline>
-          <S d="2000" r="-1"/>
-        </SegmentTimeline>
-      </SegmentTemplate>
       <Representation id="244" codecs="vp9" startWithSAP="1" width="854" height="480" maxPlayoutRate="1" frameRate="30">
         <BaseURL>{video_base_url}</BaseURL>
+        <SegmentTemplate media="sq/$Number$" startNumber="7959120" timescale="1000">
+          <SegmentTimeline>
+            <S d="2000" r="-1"/>
+          </SegmentTimeline>
+        </SegmentTemplate>
       </Representation>
     </AdaptationSet>
   </Period>
 </MPD>
 """
 
 
@@ -167,18 +167,18 @@
     )
     assert actual_diff == [
         "--- \n",
         "+++ \n",
         "@@ -2 +2 @@\n",
         "-<!--This file is created with ytpb, and expires at 2023-09-28T21:17:50+02:00-->\n",
         "+<!--This file is created with ytpb, and expires at 2023-09-28T21:23:20+02:00-->\n",
-        "@@ -12 +12 @@\n",
+        "@@ -11 +11 @@\n",
         "-        <BaseURL>https://rr5---sn-25ge7nzr.googlevideo.com/videoplayback/expire/1695928670/ei/_nwVZYXhAqbQvdIPjKmqgAM/ip/0.0.0.0/id/kHwmzef842g.2/itag/140/source/yt_live_broadcast/requiressl/yes/spc/UWF9fy2D4rPPhPMeyQnmxgP0Yhyaohs/vprv/1/playlist_type/DVR/ratebypass/yes/mime/audio%2Fmp4/live/1/gir/yes/noclen/1/dur/2.000/keepalive/yes/fexp/24007246/beids/24350017/sparams/expire,ei,ip,id,itag,source,requiressl,spc,vprv,playlist_type,ratebypass,mime,live,gir,noclen,dur/sig/AOq0QJ8wRAIgANge9FK8aJnP8nDX_HCd9LixBc1iiZueVKgR1eWAi4ACIE5wyoXt2JUnPjHbh6xp8ZJhy1j9ScEgHiBAO_2xH3h9/initcwndbps/623750/mh/XB/mm/44/mn/sn-25ge7nzr/ms/lva/mt/1695906793/mv/m/mvi/5/pl/38/lsparams/initcwndbps,mh,mm,mn,ms,mv,mvi,pl/lsig/AG3C_xAwRQIhAM6lQ9DNT724pGLtqWR01mXgxu_67Ing2nzPBj4ffCT8AiAYnVuWcAosv-DKUGO2bNSq5ptYGJhRCdlYo8E3-6HKOA%3D%3D/</BaseURL>\n",
         "+        <BaseURL>https://test/expire/1695929000/</BaseURL>\n",
-        "@@ -18 +18 @@\n",
+        "@@ -17 +17 @@\n",
         "-        <BaseURL>https://rr5---sn-25ge7nzr.googlevideo.com/videoplayback/expire/1695928670/ei/_nwVZYXhAqbQvdIPjKmqgAM/ip/0.0.0.0/id/kHwmzef842g.2/itag/244/source/yt_live_broadcast/requiressl/yes/spc/UWF9fy2D4rPPhPMeyQnmxgP0Yhyaohs/vprv/1/playlist_type/DVR/ratebypass/yes/mime/video%2Fwebm/live/1/gir/yes/noclen/1/dur/2.000/keepalive/yes/fexp/24007246/beids/24350017/sparams/expire,ei,ip,id,itag,source,requiressl,spc,vprv,playlist_type,ratebypass,mime,live,gir,noclen,dur/sig/AOq0QJ8wRgIhAJBYRElUjO7WhY5_gsjtj0aUbXbyb9Z_Yjo7JeecnqrzAiEAkzwV4SYIFponf7BddjJ5hscSZr8hbPBSx09Qffev9AA%3D/initcwndbps/623750/mh/XB/mm/44/mn/sn-25ge7nzr/ms/lva/mt/1695906793/mv/m/mvi/5/pl/38/lsparams/initcwndbps,mh,mm,mn,ms,mv,mvi,pl/lsig/AG3C_xAwRQIhAP_FmY_xO0cSx-hk2oibYFE1AHaCvDHeYyMXXUEuBNeVAiARmaf6MprHE-eEJJx3Ai59WyTOSt8INUUWhA7MSoEO2w%3D%3D/</BaseURL>\n",
         "+        <BaseURL>https://test/expire/1695929000/</BaseURL>\n",
     ]
 
 
 def test_refresh_mpd_with_mismatched_streams(
     streams_in_list: list[AudioOrVideoStream], testing_static_mpd: str
```

### Comparing `ytpb-2024.5.3/tests/actions/test_download.py` & `ytpb-2024.5.30/tests/actions/test_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import os
 from dataclasses import dataclass
-from datetime import datetime
 from pathlib import Path
 from typing import Callable
 from urllib.parse import urljoin
 
-import responses
-
-from helpers import assert_approx_duration
-
 from ytpb import actions
 from ytpb.playback import Playback, RewindInterval
 
+from tests.helpers import assert_approx_duration
+
 
 @dataclass
 class FakeRewindMoment:
     sequence: int
     cut_at: float = 0
```

### Comparing `ytpb-2024.5.3/tests/cli/conftest.py` & `ytpb-2024.5.30/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/cli/test_download_command.py` & `ytpb-2024.5.30/tests/cli/test_download_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import glob
 import os
 import pickle
-import re
+import platform
 import shutil
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
+import av
 import click
+
+import platformdirs
 import pytest
 import responses
 import toml
 
-from conftest import TEST_DATA_PATH
 from freezegun import freeze_time
-from helpers import assert_approx_duration
 
-from ytpb.config import DEFAULT_CONFIG
-from ytpb.ffmpeg import ffprobe_show_entries
+from ytpb.cli.config import DEFAULT_CONFIG
 from ytpb.playback import RewindInterval, RewindMoment
 
+from tests.conftest import TEST_DATA_PATH
+from tests.helpers import assert_approx_duration
+
 
 @pytest.mark.parametrize(
     "interval,output_subpath",
     [
         # Segments and corresponding ingestion start dates:
         #             7959120       21       22
         #                  |        |        |
@@ -36,14 +39,15 @@
         ("2023-03-25T23:33:55+00/2023-03-25T23:33:57+00", "233355+00.mp4"),
         ("2023-03-25T23:33:55+00/PT3S", "233355+00.mp4"),
         ("2023-03-25T23:33:55+00/7959121", "233355+00.mp4"),
         ("PT3S/7959121", "233355+00.mp4"),
         ("PT3S/2023-03-25T23:33:58+00", "233355+00.mp4"),
     ],
 )
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_download_within_interval(
     interval: str,
     output_subpath: str,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -76,16 +80,16 @@
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    assert result.output == expected_out
     assert result.exit_code == 0
+    assert result.output == expected_out
     assert glob.glob(str(tmp_path / f"*{output_subpath}"))
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_providing_start_and_end_equals_now(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
@@ -182,15 +186,15 @@
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
     assert result.exit_code == 0
-    if not ".." in interval:
+    if ".." not in interval:
         assert "~ Preview mode enabled, interval end is ignored." in result.output
     assert os.path.exists(tmp_path / "Webcam-Zurich-HB_kHwmzef842g_preview.mp4")
 
 
 @pytest.mark.parametrize(
     "interval",
     [
@@ -342,14 +346,15 @@
     assert os.path.exists(run_temp_directory / "7959121.i140.mp4")
 
 
 @pytest.mark.parametrize(
     "audio_format,video_format",
     [("itag eq 140", "itag eq 244"), ("itag eq 140", "none"), ("none", "itag eq 244")],
 )
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_download_audio_and_or_video(
     audio_format: str | None,
     video_format: str | None,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -371,15 +376,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 audio_format,
                 "-vf",
                 video_format,
                 stream_url,
@@ -430,15 +434,15 @@
 
     # Then:
     assert result.exit_code == 0
     assert os.path.exists(tmp_path / "test" / "merged.mp4")
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_download_to_custom_relative_path(
+def test_download_to_user_relative_path(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
@@ -470,27 +474,16 @@
         )
 
     # Then:
     assert result.exit_code == 0
     assert os.path.exists(tmp_path / "test" / "merged.mp4")
 
 
-@pytest.mark.parametrize(
-    "output_path,expected",
-    [
-        (
-            "<title>_<input_start_date>_<duration>",
-            "Webcam-Zurich-HB_20230325T233354+00_PT4S.mp4",
-        ),
-    ],
-)
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_download_to_template_output_path(
-    output_path: str,
-    expected: str,
+def test_download_to_user_template_output_path(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
@@ -512,22 +505,22 @@
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 "-o",
-                output_path,
+                "{{ id }}",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    assert expected == str(next(tmp_path.glob("*.mp4")).name)
+    assert "kHwmzef842g.mp4" == str(next(tmp_path.glob("*.mp4")).name)
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_keep_temp_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -566,14 +559,15 @@
     assert result.exit_code == 0
     assert os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     )
     assert os.path.exists(run_temp_directory / "7959120.i140.mp4")
 
 
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_merge_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
@@ -605,21 +599,22 @@
                 "--no-merge",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
+    assert expected_out == result.output
     assert not os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     )
     assert not os.path.exists(run_temp_directory)
-    assert expected_out == result.output
 
 
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_dry_run_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
@@ -658,16 +653,17 @@
     assert result.output == expected_out
     assert not os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
     )
     assert not os.path.exists(run_temp_directory)
 
 
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_no_cut_option(
+def test_cut_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
@@ -690,26 +686,25 @@
                 "--no-cache",
                 "--interval",
                 "2023-03-25T23:33:55+00/2023-03-25T23:33:58+00",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
-                "--no-cut",
+                "--cut",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
+    assert result.output == expected_out
     expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
     assert os.path.exists(expected_path)
-    assert_approx_duration(expected_path, 4.0)
-
-    assert result.output == expected_out
+    assert_approx_duration(expected_path, 3.0, abs=4.2e-2)
 
 
 @freeze_time("2023-09-28T17:00:00+00:00")
 def test_from_cache(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -729,15 +724,14 @@
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 stream_url,
@@ -769,15 +763,14 @@
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 stream_url,
@@ -813,15 +806,14 @@
 ) -> None:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
-                "--no-cut",
                 "--no-cache",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 audio_format,
                 "-vf",
                 video_format,
@@ -853,15 +845,14 @@
     with patch("ytpb.cli.common.YoutubeDLInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--yt-dlp",
-                "--no-cut",
                 "--no-cache",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
@@ -896,21 +887,21 @@
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
     config = {
         "options": {
             "download": {
-                "audio_format": "NON-SENS",
+                "audio-format": "NON-SENS",
             }
         }
     }
-    config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w") as f:
+    with config_path.open("w", encoding="utf-8") as f:
         toml.dump(config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -947,32 +938,32 @@
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
     default_config = {
         "options": {
             "download": {
-                "audio_format": "NON-SENS",
+                "audio-format": "NON-SENS",
             }
         }
     }
-    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    default_config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w") as f:
+    with default_config_path.open("w", encoding="utf-8") as f:
         toml.dump(default_config, f)
 
     test_config = {
         "options": {
             "download": {
-                "audio_format": "itag eq 140",
+                "audio-format": "itag eq 140",
             }
         }
     }
-    test_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "test-config.toml"
-    with test_config_path.open("w") as f:
+    test_config_path = platformdirs.user_config_path() / "test-config.toml"
+    with test_config_path.open("w", encoding="utf-8") as f:
         toml.dump(test_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -1006,22 +997,22 @@
     default_config = {
         "options": {
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
-    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    default_config_path = platformdirs.user_config_path() / "ytpb" / "config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w") as f:
+    with default_config_path.open("w", encoding="utf-8") as f:
         toml.dump(default_config, f)
 
-    test_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "test-config.toml"
+    test_config_path = platformdirs.user_config_path() / "ytpb" / "test-config.toml"
 
-    # When:
+    # Then:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.FileError) as exc_info:
             ytpb_cli_invoke(
                 [
                     "--config",
                     test_config_path,
@@ -1033,16 +1024,14 @@
                     "none",
                     stream_url,
                 ],
                 catch_exceptions=False,
                 standalone_mode=False,
             )
 
-    assert str(test_config_path) in str(exc_info)
-
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_config_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
@@ -1061,17 +1050,17 @@
     default_config = {
         "options": {
             "download": {
                 "interval": "7959120/7959121",
             }
         }
     }
-    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    default_config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w") as f:
+    with default_config_path.open("w", encoding="utf-8") as f:
         toml.dump(default_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.MissingParameter) as exc_info:
             ytpb_cli_invoke(
@@ -1108,17 +1097,17 @@
     default_config = {
         "options": {
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
-    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    default_config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w") as f:
+    with default_config_path.open("w", encoding="utf-8") as f:
         toml.dump(default_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.UsageError) as exc_info:
             ytpb_cli_invoke(
@@ -1160,15 +1149,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 video_id,
@@ -1200,39 +1188,32 @@
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_custom_aliases(
+def test_custom_alias(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
-    tmp_path: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
-    custom_config = {
-        "general": {
-            "aliases": {
-                "custom-alias": "itag eq 140",
-            }
-        }
-    }
-    config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    custom_config = {"general": {"aliases": {"custom": "itag eq 140"}}}
+    config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w") as f:
+    with config_path.open("w", encoding="utf-8") as f:
         toml.dump(custom_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -1242,54 +1223,15 @@
                 "--dry-run",
                 "--no-cache",
                 "--interval",
                 "7959120/7959121",
                 "-vf",
                 "none",
                 "-af",
-                "@custom-alias",
-                stream_url,
-            ],
-        )
-
-    # Then:
-    assert result.exit_code == 0
-
-
-@freeze_time("2023-03-26T00:00:00+00:00")
-def test_dynamic_aliases(
-    ytpb_cli_invoke: Callable,
-    add_responses_callback_for_reference_base_url: Callable,
-    add_responses_callback_for_segment_urls: Callable,
-    fake_info_fetcher: MagicMock,
-    stream_url: str,
-    audio_base_url: str,
-    tmp_path: Path,
-) -> None:
-    # Given:
-    add_responses_callback_for_reference_base_url()
-    add_responses_callback_for_segment_urls(
-        urljoin(audio_base_url, r"sq/\w+"),
-    )
-
-    # When:
-    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
-        mock_fetcher.return_value = fake_info_fetcher
-        result = ytpb_cli_invoke(
-            [
-                "--no-config",
-                "download",
-                "--dry-run",
-                "--no-cache",
-                "--interval",
-                "7959120/7959121",
-                "-vf",
-                "none",
-                "-af",
-                "@140",
+                "@custom",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
 
@@ -1314,15 +1256,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--dry-run",
-                "--no-cut",
                 "--no-cache",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 audio_format,
                 "-vf",
                 video_format,
@@ -1487,23 +1428,59 @@
     assert result.output == (
         f"{audio_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
         f"{video_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
     )
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_metadata_tags_with_cutting(
+def test_dump_rewind_interval_option(
+    add_responses_callback_for_reference_base_url,
+    add_responses_callback_for_segment_urls,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                "--dump-rewind-interval",
+                stream_url,
+            ],
+        )
+
+    assert result.exit_code == 0
+    assert result.output == "7959120-7959121\n"
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_metadata_tags_without_cutting_and_iso_dates(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1524,40 +1501,38 @@
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    format_tags = ffprobe_show_entries(
-        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
-        "format_tags",
-        "default",
-    )
-    assert "TAG:title=Webcam Zürich HB" in format_tags
-    assert "TAG:author=David Gubler" in format_tags
-    assert f"TAG:comment={stream_url}" in format_tags
-    assert "TAG:input_start_time=1679787235.000000" in format_tags
-    assert "TAG:input_end_time=1679787237.000000" in format_tags
-    assert "TAG:actual_start_time=1679787235.000000" in format_tags
-    assert "TAG:actual_end_time=1679787237.000000" in format_tags
-    assert "TAG:start_sequence_number=7959120" in format_tags
-    assert "TAG:end_sequence_number=7959121" in format_tags
+    output_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
+    with av.open(output_path) as container:
+        metadata_tags = container.metadata
+
+    assert metadata_tags["title"] == "Webcam Zürich HB"
+    assert metadata_tags["author"] == "David Gubler"
+    assert metadata_tags["comment"] == stream_url
+    assert metadata_tags["input_start_date"] == "2023-03-25T23:33:55.000000Z"
+    assert metadata_tags["input_end_date"] == "2023-03-25T23:33:57.000000Z"
+    assert metadata_tags["actual_start_date"] == "2023-03-25T23:33:54.491176Z"
+    assert metadata_tags["actual_end_date"] == "2023-03-25T23:33:58.486826Z"
+    assert metadata_tags["start_segment"] == "7959120"
+    assert metadata_tags["end_segment"] == "7959121"
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
-def test_metadata_tags_without_cutting(
+def test_metadata_tags_with_cutting_and_iso_dates(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1565,55 +1540,114 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
+                "--cut",
                 "--interval",
                 "2023-03-25T23:33:55+00/2023-03-25T23:33:57+00",
-                "--no-cut",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    format_tags = ffprobe_show_entries(
-        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
-        "format_tags",
-        "default",
-    )
-    assert "TAG:title=Webcam Zürich HB" in format_tags
-    assert "TAG:author=David Gubler" in format_tags
-    assert f"TAG:comment={stream_url}" in format_tags
-    assert "TAG:input_start_time=1679787235.000000" in format_tags
-    assert "TAG:input_end_time=1679787237.000000" in format_tags
-    assert "TAG:actual_start_time=1679787234.491176" in format_tags
-    assert "TAG:actual_end_time=1679787238.486826" in format_tags
-    assert "TAG:start_sequence_number=7959120" in format_tags
-    assert "TAG:end_sequence_number=7959121" in format_tags
+    output_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
+    with av.open(output_path) as container:
+        metadata_tags = container.metadata
+
+    assert metadata_tags["title"] == "Webcam Zürich HB"
+    assert metadata_tags["author"] == "David Gubler"
+    assert metadata_tags["comment"] == stream_url
+    assert metadata_tags["input_start_date"] == "2023-03-25T23:33:55.000000Z"
+    assert metadata_tags["input_end_date"] == "2023-03-25T23:33:57.000000Z"
+    assert metadata_tags["actual_start_date"] == "2023-03-25T23:33:55.000000Z"
+    assert metadata_tags["actual_end_date"] == "2023-03-25T23:33:57.000000Z"
+    assert metadata_tags["start_segment"] == "7959120"
+    assert metadata_tags["end_segment"] == "7959121"
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_metadata_tags_without_cutting_and_unix_timestamps(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    custom_config = {
+        "output": {
+            "metadata": {
+                "dates": "unix",
+            }
+        }
+    }
+    config_path = platformdirs.user_config_path() / "ytpb/config.toml"
+    config_path.parent.mkdir(parents=True)
+    with config_path.open("w", encoding="utf-8") as f:
+        toml.dump(custom_config, f)
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "download",
+                "--no-cache",
+                "--interval",
+                "2023-03-25T23:33:55+00/2023-03-25T23:33:57+00",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    output_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
+    with av.open(output_path) as container:
+        metadata_tags = container.metadata
+
+    assert metadata_tags["title"] == "Webcam Zürich HB"
+    assert metadata_tags["author"] == "David Gubler"
+    assert metadata_tags["comment"] == stream_url
+    assert metadata_tags["input_start_date"] == "1679787235.000000"
+    assert metadata_tags["input_end_date"] == "1679787237.000000"
+    assert metadata_tags["actual_start_date"] == "1679787234.491176"
+    assert metadata_tags["actual_end_date"] == "1679787238.486826"
+    assert metadata_tags["start_segment"] == "7959120"
+    assert metadata_tags["end_segment"] == "7959121"
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_resume_downloading(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1652,15 +1686,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/2023-03-25T23:33:59+00",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 video_id,
@@ -1681,20 +1714,18 @@
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_keep_segments(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1702,15 +1733,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--keep-segments",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
@@ -1728,20 +1758,18 @@
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_remove_default_segments_output_directory(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1749,15 +1777,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 video_id,
@@ -1775,20 +1802,18 @@
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_remove_created_segments_output_directory(
     segments_output_dir_option: str,
     monkeypatch: pytest.MonkeyPatch,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     sub_tmp_path = tmp_path / "sub"
     sub_tmp_path.mkdir()
     monkeypatch.chdir(sub_tmp_path)
 
     segments_output_directory = sub_tmp_path / segments_output_dir_option
@@ -1802,15 +1827,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 "--segments-output-dir",
@@ -1829,20 +1853,18 @@
         assert not os.path.exists(segments_output_directory.parent)
 
 
 def test_remove_only_rewound_segments(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1854,15 +1876,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 video_id,
@@ -1878,20 +1899,18 @@
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_do_not_remove_existing_directory(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1902,15 +1921,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
                 "--segments-output-dir",
@@ -1928,20 +1946,18 @@
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_ignore_resume_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1949,15 +1965,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--ignore-resume",
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "none",
@@ -1972,20 +1987,18 @@
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_ignore_resume_option_after_unfinished_run(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
-    mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
-    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -2023,15 +2036,14 @@
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
                 "--no-config",
                 "download",
                 "--no-cache",
-                "--no-cut",
                 "--ignore-resume",
                 "--segments-output-dir",
                 "segments",
                 "--keep-segments",
                 "--interval",
                 "7959120/7959122",
                 "-af",
```

### Comparing `ytpb-2024.5.3/tests/cli/test_parameters.py` & `ytpb-2024.5.30/tests/cli/test_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,16 @@
         (
             "@1704190800/@1704190830.123",
             (
                 datetime(2024, 1, 2, 10, 20, 0, tzinfo=timezone.utc),
                 datetime(2024, 1, 2, 10, 20, 30, 123000, tzinfo=timezone.utc),
             ),
         ),
+        ("earliest/100", ("earliest", 100)),
+        ("earliest/..", ("earliest", "..")),
     ],
 )
 def test_rewind_interval(value: str, expected):
     assert expected == RewindIntervalParamType().convert(value, None, None)
 
 
 @pytest.mark.parametrize(
@@ -145,14 +147,16 @@
 
 
 @pytest.mark.parametrize(
     "value,invalid_part",
     [
         ("20240102T102070+00/PT30M", "20240102T102070+00"),
         ("20240102T102030+00/PT30", "PT30"),
+        ("100/earliest", "'earliest'"),
+        ("now/100", "'now'"),
     ],
 )
 def test_invalid_rewind_interval(value: str, invalid_part: str):
     with pytest.raises(click.BadParameter) as exc_info:
         RewindIntervalParamType().convert(value, None, None)
     assert invalid_part in str(exc_info.value)
 
@@ -162,13 +166,14 @@
     [
         ("PT10M/PT20M", "Two durations"),
         ("../..", "Two '..'"),
         ("PT1H/..", "Keyword '..'"),
         ("../PT1H", "Keyword '..'"),
         ("2024Y/PT1H", "Replacement components"),
         ("2024Y/..", "Replacement components"),
+        ("earliest/2024Y", "Replacement components"),
     ],
 )
 def test_non_compatible_interval_parts(interval: str, error: str):
     with pytest.raises(click.BadParameter) as exc_info:
         RewindIntervalParamType().convert(interval, None, None)
     assert error in str(exc_info.value)
```

### Comparing `ytpb-2024.5.3/tests/cli/capture/test_frame_command.py` & `ytpb-2024.5.30/tests/cli/capture/test_frame_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
 import av
 import click
 import pytest
 
-from conftest import TEST_DATA_PATH
 from freezegun import freeze_time
 from PIL import Image
 
+from tests.conftest import TEST_DATA_PATH
+
 IMAGE_SAVE_SETTINGS = {"format": "jpeg", "quality": 80}
 
 
 def assert_two_images(
     actual_image_path: Path,
     segment_path: Path,
     expected_frame: int,
```

### Comparing `ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py` & `ytpb-2024.5.30/tests/cli/mpd/test_compose_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
+import platform
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
+import platformdirs
 import pytest
-
 import toml
 from freezegun import freeze_time
 
 
 @pytest.mark.parametrize(
     "audio_formats,video_formats",
     [
         ("itag eq 140", "itag eq 243 or itag eq 244"),
         ("itag eq 140", "none"),
         ("none", "itag eq 243 or itag eq 244"),
     ],
 )
+@pytest.mark.expect_suffix(platform.system())
 def test_compose_mpd(
     audio_formats,
     video_formats,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
@@ -49,14 +51,15 @@
                 stream_url,
             ],
         )
     assert result.exit_code == 0
     assert result.output == expected_out
 
 
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_compose_mpd_with_no_streams(
     ytpb_cli_invoke: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     video_id: str,
     audio_base_url: str,
@@ -136,22 +139,22 @@
         r"https://.+\.googlevideo\.com/videoplayback/.+/sq/\w+"
     )
 
     config = {
         "options": {
             "mpd": {
                 "compose": {
-                    "audio_formats": "NON-SENS",
+                    "audio-formats": "NON-SENS",
                 }
             }
         }
     }
-    config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    config_path = platformdirs.user_config_path() / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w") as f:
+    with config_path.open("w", encoding="utf-8") as f:
         toml.dump(config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -165,18 +168,19 @@
                 "-vf",
                 "itag eq 243",
                 stream_url,
             ],
         )
 
     # Then:
+    print(result.output)
     assert result.exit_code == 0
 
 
-def test_compose_to_custom_output_path(
+def test_compose_to_user_output_path(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     tmp_path: Path,
 ):
@@ -203,15 +207,15 @@
             ],
             catch_exceptions=False,
         )
     assert result.exit_code == 0
     assert os.path.exists("manifest.xml")
 
 
-def test_compose_to_custom_template_output_path(
+def test_compose_to_user_template_output_path(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     video_id: str,
     tmp_path: Path,
@@ -230,14 +234,14 @@
                 "--interval",
                 "7959120/7959121",
                 "-af",
                 "itag eq 140",
                 "-vf",
                 "itag eq 243",
                 "-o",
-                "<id>.xml",
+                "{{ id }}.xml",
                 stream_url,
             ],
             catch_exceptions=False,
         )
     assert result.exit_code == 0
     assert os.path.exists(f"{video_id}.xml")
```

### Comparing `ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py` & `ytpb-2024.5.30/tests/cli/mpd/test_refresh_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # ruff: noqa: E501
 
 import copy
+import platform
 from dataclasses import asdict
 from difflib import unified_diff
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 
 import freezegun
-
 import pytest
 from freezegun import freeze_time
 
-from helpers import patched_freezgun_astimezone
-
 from ytpb.info import YouTubeVideoInfo
 from ytpb.playback import Playback
 from ytpb.streams import Streams
 from ytpb.types import AudioOrVideoStream, AudioStream, VideoStream
 
+from tests.helpers import patched_freezgun_astimezone
+
 freezegun.api.FakeDatetime.astimezone = patched_freezgun_astimezone
 
 
 @pytest.fixture()
 def dash_manifest(audio_base_url: str, video_base_url: str) -> str:
     return f"""<?xml version='1.0' encoding='UTF-8'?>
 <!--This file is created with ytpb, and expires at 2023-08-16T04:24:48+02:00-->
@@ -41,14 +41,15 @@
       </Representation>
     </AdaptationSet>
   </Period>
 </MPD>
 """
 
 
+@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-08-16T02:30:00+02:00", tz_offset=2)
 def test_refresh_mpd(
     ytpb_cli_invoke: Callable,
     mock_fetch_and_set_essential: MagicMock,
     streams_in_list: list[AudioOrVideoStream],
     active_live_video_info: YouTubeVideoInfo,
     stream_url: str,
@@ -57,15 +58,15 @@
     video_base_url: str,
     dash_manifest: str,
     tmp_path: Path,
     expected_out,
 ) -> None:
     # Given:
     manifest_path = tmp_path / "manifest.mpd"
-    with open(manifest_path, "w") as f:
+    with open(manifest_path, "w", encoding="utf-8") as f:
         f.write(dash_manifest)
 
     # When:
     def mock_essential(obj: Playback, *args, **kwargs):
         updated_streams = copy.deepcopy(streams_in_list)
         for i, stream in enumerate(updated_streams):
             stream_as_dict = asdict(stream)
@@ -82,15 +83,15 @@
     ):
         result = ytpb_cli_invoke(["mpd", "refresh", str(manifest_path)])
 
     # Then:
     assert result.exit_code == 0
     assert result.output == expected_out
 
-    with open(manifest_path) as f:
+    with open(manifest_path, encoding="utf-8") as f:
         refreshed_manifest = f.read()
 
     actual_diff = list(
         unified_diff(
             dash_manifest.splitlines(keepends=True),
             refreshed_manifest.splitlines(keepends=True),
             n=0,
```

### Comparing `ytpb-2024.5.3/tests/data/info-1695928670.json` & `ytpb-2024.5.30/tests/data/info-1695928670.json`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/manifest-1695928670.mpd` & `ytpb-2024.5.30/tests/data/manifest-1695928670.mpd`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/webpage-1695928670.html` & `ytpb-2024.5.30/tests/data/webpage-1695928670.html`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out` & `ytpb-2024.5.30/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Darwin.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.5.30/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out` & `ytpb-2024.5.30/tests/data/expected/test_cut_option-Darwin.out`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
-These representations will be downloaded:
+This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+2. Merging segments (cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mkv'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out` & `ytpb-2024.5.30/tests/data/expected/test_cut_option-Linux.out`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+2. Merging segments (cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out` & `ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Darwin.out`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
+   - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
-   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+   - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
+2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Linux.out`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Darwin.out`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Linux.out`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Darwin.out`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000 (+00:01), seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Linux.out`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000 (+00:01), seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Darwin.out`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000 (+00:01), seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Darwin.out`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000 (-00:01), seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.5.30/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Linux.out`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000 (-00:01), seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
```

### Comparing `ytpb-2024.5.3/tests/data/expected/test_no_cut_option.out` & `ytpb-2024.5.30/tests/data/expected/test_no_cut_option-Darwin.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out` & `ytpb-2024.5.30/tests/data/expected/test_no_merge_option-Darwin.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv` & `ytpb-2024.5.30/tests/data/gap-cases/gap-case-1-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv` & `ytpb-2024.5.30/tests/data/gap-cases/gap-case-2-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv` & `ytpb-2024.5.30/tests/data/gap-cases/gap-case-3-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4` & `ytpb-2024.5.30/tests/data/segments/7959120.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959120.i244.webm` & `ytpb-2024.5.30/tests/data/segments/7959120.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4` & `ytpb-2024.5.30/tests/data/segments/7959121.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959121.i244.webm` & `ytpb-2024.5.30/tests/data/segments/7959121.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4` & `ytpb-2024.5.30/tests/data/segments/7959122.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959122.i244.webm` & `ytpb-2024.5.30/tests/data/segments/7959122.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4` & `ytpb-2024.5.30/tests/data/segments/7959123.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959123.i244.webm` & `ytpb-2024.5.30/tests/data/segments/7959123.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4` & `ytpb-2024.5.30/tests/data/segments/7959203.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/data/segments/7959203.i244.webm` & `ytpb-2024.5.30/tests/data/segments/7959203.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/utils/test_date.py` & `ytpb-2024.5.30/tests/cli/utils/test_date.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import datetime, timedelta, timezone
 
 import pytest
 
-from ytpb.utils.date import (
+from ytpb.cli.utils.date import (
     build_style_parameters_from_spec,
     DurationFormatPattern,
     express_timedelta_in_words,
     format_duration,
     format_iso_datetime,
     format_timedelta,
-    ISO8601DateStyleParameters,
+    ISODateStyleParameters,
 )
 
 
 class TestFormatDatetime:
     @pytest.mark.parametrize(
         "date,expected",
         [
@@ -22,15 +22,15 @@
             ("2023-08-09T10:20:30+01:00", "2023-08-09T10:20:30+01"),
             ("2023-08-09T10:00:00.123+01:00", "2023-08-09T10:00:00+01"),
         ],
     )
     def test_extended_format_and_complete_precision(self, date, expected):
         assert expected == format_iso_datetime(
             datetime.fromisoformat(date),
-            ISO8601DateStyleParameters(format="extended", precision="complete"),
+            ISODateStyleParameters(format="extended", precision="complete"),
         )
 
     @pytest.mark.parametrize(
         "date,expected",
         [
             ("2023-08-09T00+01:00", "2023-08-09T00+01"),
             ("2023-08-09T10+01:00", "2023-08-09T10+01"),
@@ -38,114 +38,189 @@
             ("2023-08-09T10:20:30+01:00", "2023-08-09T10:20:30+01"),
             ("2023-08-09T10:00:00.123+01:00", "2023-08-09T10:00:00+01"),
         ],
     )
     def test_extended_format_and_reduced_precision(self, date, expected):
         assert expected == format_iso_datetime(
             datetime.fromisoformat(date),
-            ISO8601DateStyleParameters(format="extended", precision="reduced"),
+            ISODateStyleParameters(format="extended", precision="reduced"),
         )
 
     @pytest.mark.parametrize(
         "date,expected",
         [
             ("2023-08-09T10+01:00", "20230809T100000+01"),
             ("2023-08-09T10:20+01:00", "20230809T102000+01"),
             ("2023-08-09T10:20:30+01:00", "20230809T102030+01"),
             ("2023-08-09T10:00:00.123+01:00", "20230809T100000+01"),
         ],
     )
     def test_basic_format_and_complete_precision(self, date, expected):
         assert expected == format_iso_datetime(
             datetime.fromisoformat(date),
-            ISO8601DateStyleParameters(format="basic", precision="complete"),
+            ISODateStyleParameters(format="basic", precision="complete"),
         )
 
     @pytest.mark.parametrize(
         "date,expected",
         [
             ("2023-08-09T10+01:00", "20230809T10+01"),
             ("2023-08-09T10:20+01:00", "20230809T1020+01"),
             ("2023-08-09T10:20:30+01:00", "20230809T102030+01"),
             ("2023-08-09T10:00:00.123+01:00", "20230809T100000+01"),
         ],
     )
     def test_basic_format_and_reduced_precision(self, date, expected):
         assert expected == format_iso_datetime(
             datetime.fromisoformat(date),
-            ISO8601DateStyleParameters(format="basic", precision="reduced"),
+            ISODateStyleParameters(format="basic", precision="reduced"),
         )
 
     @pytest.mark.parametrize(
         "basic_or_extended,offset_format,expected",
         [
             ("basic", "hh", "20230809T102030+01"),
             ("basic", "hhmm", "20230809T102030+0100"),
             ("extended", "hh", "2023-08-09T10:20:30+01"),
             ("extended", "hhmm", "2023-08-09T10:20:30+01:00"),
         ],
     )
     def test_utc_offset_formats(self, basic_or_extended, offset_format, expected):
         assert expected == format_iso_datetime(
             datetime.fromisoformat("2023-08-09T10:20:30+01:00"),
-            ISO8601DateStyleParameters(
+            ISODateStyleParameters(
                 format=basic_or_extended, offset_format=offset_format
             ),
         )
 
     def test_use_z_for_utc(self):
         assert "20230809T102030Z" == format_iso_datetime(
             datetime.fromisoformat("2023-08-09T10:20:30+00:00"),
-            ISO8601DateStyleParameters(use_z_for_utc=True),
+            ISODateStyleParameters(use_z_for_utc=True),
         )
         assert "20230809T102030+01" == format_iso_datetime(
             datetime.fromisoformat("2023-08-09T10:20:30+01:00"),
-            ISO8601DateStyleParameters(use_z_for_utc=True),
+            ISODateStyleParameters(use_z_for_utc=True),
         )
         assert "20230809T102030+00" == format_iso_datetime(
             datetime.fromisoformat("2023-08-09T10:20:30+00:00"),
-            ISO8601DateStyleParameters(use_z_for_utc=False),
+            ISODateStyleParameters(use_z_for_utc=False),
         )
 
     def test_raise_with_naive_datetime(self):
         with pytest.raises(ValueError):
             format_iso_datetime(
                 datetime.now(),
             )
 
     def test_raise_with_invalid_argument(self):
         with pytest.raises(ValueError):
             format_iso_datetime(
-                datetime.now(timezone.utc), ISO8601DateStyleParameters(format="invalid")
+                datetime.now(timezone.utc), ISODateStyleParameters(format="invalid")
             )
         with pytest.raises(ValueError):
             format_iso_datetime(
                 datetime.now(timezone.utc),
-                ISO8601DateStyleParameters(precision="invalid"),
+                ISODateStyleParameters(precision="invalid"),
             )
         with pytest.raises(ValueError):
             format_iso_datetime(
                 datetime.now(timezone.utc),
-                ISO8601DateStyleParameters(offset_format="invalid"),
+                ISODateStyleParameters(offset_format="invalid"),
             )
 
 
-@pytest.mark.parametrize(
-    "delta,expected",
-    [
-        (timedelta(hours=1), "PT1H"),
-        (timedelta(hours=1, minutes=2), "PT1H2M"),
-        (timedelta(hours=1, minutes=2, seconds=3), "PT1H2M3S"),
-        (timedelta(hours=0, minutes=2, seconds=3), "PT2M3S"),
-        (timedelta(hours=0, minutes=0, seconds=3), "PT3S"),
-        (timedelta(hours=1, minutes=0, seconds=3), "PT1H3S"),
-    ],
-)
-def test_format_duration(delta, expected: str):
-    assert expected == format_duration(delta, DurationFormatPattern.ISO8601)
+class TestFormatDuration:
+    @pytest.mark.parametrize(
+        "duration,expected",
+        [
+            (timedelta(hours=1), "PT1H"),
+            (timedelta(hours=1, minutes=2), "PT1H2M"),
+            (
+                timedelta(hours=1, minutes=2, seconds=30),
+                "PT1H2M30S",
+            ),
+            (timedelta(hours=0, minutes=2, seconds=30), "PT2M30S"),
+            (
+                timedelta(hours=0, minutes=0, seconds=30),
+                "PT30S",
+            ),
+            (timedelta(hours=0, minutes=0, seconds=30.123), "PT30S"),
+            (timedelta(hours=1, minutes=0, seconds=30), "PT1H30S"),
+            (timedelta(seconds=123), "PT2M3S"),
+        ],
+    )
+    def test_iso_pattern(self, duration: timedelta, expected: str):
+        assert expected == format_duration(duration, DurationFormatPattern.ISO)
+
+    @pytest.mark.parametrize(
+        "duration,expected",
+        [
+            (timedelta(hours=1), "01:00:00"),
+            (timedelta(hours=1, minutes=2), "01:02:00"),
+            (
+                timedelta(hours=1, minutes=2, seconds=30),
+                "01:02:30",
+            ),
+            (timedelta(hours=0, minutes=2, seconds=30), "00:02:30"),
+            (
+                timedelta(hours=0, minutes=0, seconds=30),
+                "00:00:30",
+            ),
+            (timedelta(hours=0, minutes=0, seconds=30.123), "00:00:30"),
+            (timedelta(hours=1, minutes=0, seconds=30), "01:00:30"),
+            (timedelta(seconds=123), "00:02:03"),
+        ],
+    )
+    def test_numeric_pattern(self, duration: timedelta, expected: str):
+        assert expected == format_duration(duration, DurationFormatPattern.NUMERIC)
+
+    @pytest.mark.parametrize(
+        "duration,expected",
+        [
+            (timedelta(hours=1), "1 h"),
+            (timedelta(hours=1, minutes=2), "1 h 2 m"),
+            (
+                timedelta(hours=1, minutes=2, seconds=30),
+                "1 h 2 m 30 s",
+            ),
+            (timedelta(hours=0, minutes=2, seconds=30), "2 m 30 s"),
+            (
+                timedelta(hours=0, minutes=0, seconds=30),
+                "30 s",
+            ),
+            (timedelta(hours=0, minutes=0, seconds=30.123), "30 s"),
+            (timedelta(hours=1, minutes=0, seconds=30), "1 h 30 s"),
+            (timedelta(seconds=123), "2 m 3 s"),
+        ],
+    )
+    def test_sentence_pattern(self, duration: timedelta, expected: str):
+        assert expected == format_duration(duration, DurationFormatPattern.SENTENCE)
+
+    @pytest.mark.parametrize(
+        "duration,expected",
+        [
+            (timedelta(hours=1), "1h"),
+            (timedelta(hours=1, minutes=2), "1h2m"),
+            (
+                timedelta(hours=1, minutes=2, seconds=30),
+                "1h2m30s",
+            ),
+            (timedelta(hours=0, minutes=2, seconds=30), "2m30s"),
+            (
+                timedelta(hours=0, minutes=0, seconds=30),
+                "30s",
+            ),
+            (timedelta(hours=0, minutes=0, seconds=30.123), "30s"),
+            (timedelta(hours=1, minutes=0, seconds=30), "1h30s"),
+            (timedelta(seconds=123), "2m3s"),
+        ],
+    )
+    def test_hms_pattern(self, duration: timedelta, expected: str):
+        assert expected == format_duration(duration, DurationFormatPattern.HMS)
 
 
 @pytest.mark.parametrize(
     "delta,expected",
     [
         (timedelta(hours=1), "an hour"),
         (timedelta(hours=1, minutes=14), "an hour"),
@@ -192,22 +267,22 @@
 def test_format_timedelta_with_ms_precision(duration, expected):
     result = format_timedelta(duration, use_ms_precision=True)
     assert result == expected
 
 
 class TestBuildStyleParametersFromSpec:
     def test_parse_single_date_style(self):
-        expected = ISO8601DateStyleParameters(
+        expected = ISODateStyleParameters(
             format="extended",
         )
         assert expected == build_style_parameters_from_spec("extended")
 
     @pytest.mark.parametrize("spec", ["extended,complete", "extended, complete"])
     def test_parse_date_styles(self, spec):
-        expected = ISO8601DateStyleParameters(
+        expected = ISODateStyleParameters(
             format="extended",
             precision="complete",
         )
         assert expected == build_style_parameters_from_spec(spec)
 
     def test_mutually_exlusive_styles(self):
         with pytest.raises(ValueError) as exc_info:
```

### Comparing `ytpb-2024.5.3/tests/utils/test_remote.py` & `ytpb-2024.5.30/tests/utils/test_remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/tests/utils/test_url.py` & `ytpb-2024.5.30/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/.gitignore` & `ytpb-2024.5.30/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+notebooks/out/
 notebooks/shared/*
 !notebooks/shared/.gitkeep
-notebooks/out/
+
+src/ytpb/_version.py
+
+pyrightconfig.json
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `ytpb-2024.5.3/LICENSE` & `ytpb-2024.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.3/README.rst` & `ytpb-2024.5.30/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -58,40 +58,57 @@
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
 Installation
 ************
 
-Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
+Ytpb requires Python 3.11 or higher and has been `tested
+<https://github.com/xymaxim/ytpb/actions/workflows/ci.yml>`__ on Linux, macOS,
+and Windows. Also, it needs the recent version of `FFmpeg
+<https://ffmpeg.org/download.html>`__ to be installed.
+
+Installing from PyPI
+====================
+
+When you have all required dependencies, you can install Ytpb via `pipx
 <https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
 To upgrade to the newer version, do::
 
   $ pipx upgrade ytpb
 
+Windows binaries
+================
+
+For Windows, pre-built binaries are available: check `releases
+<https://github.com/xymaxim/ytpb/releases>`__ on GitHub. Make sure to `add
+<https://www.wikihow.com/Install-FFmpeg-on-Windows>`__ the ``ffmpeg.exe`` file
+to your system path or place it in the folder next to the Ytpb binary. Now
+you're ready to use Ytpb in Terminal: type commands, not double-click.
+
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
-provides some general aspects and terms. `Cookbook`_ contains some useful
-examples. See `Changelog`_ for the history of releases. Have any issues,
-suggestions, or want to contribute code? `Contributing`_ tells how to
+provides some general aspects and terms. See `Questions`_ for answers to the
+most anticipated questions. `Cookbook`_ contains some useful examples.  Have any
+issues, suggestions, or want to contribute code? `Contributing`_ tells how to
 participate in the project.
 
 .. _Why Ytpb?: https://ytpb.readthedocs.io/en/latest/why.html
 .. _Quick start: https://ytpb.readthedocs.io/en/latest/quick.html
 .. _Command line application: https://ytpb.readthedocs.io/en/latest/cli.html
 .. _Reference: https://ytpb.readthedocs.io/en/latest/reference.html
+.. _Questions: https://ytpb.readthedocs.io/en/latest/questions.html
 .. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
-.. _Changelog: https://ytpb.readthedocs.io/en/latest/changelog.html
 
 Similar projects
 ****************
 
 - `Kethsar/ytarchive <https://github.com/Kethsar/ytarchive>`__ — archive streams from the start
 - `rytsikau/ee.Yrewind <https://github.com/rytsikau/ee.Yrewind>`__ — rewind and save streams
 - `yt-dlp/yt-dlp#6498 <https://github.com/yt-dlp/yt-dlp/pull/6498>`__ — brings rewind range selection to yt-dlp
```

### Comparing `ytpb-2024.5.3/pyproject.toml` & `ytpb-2024.5.30/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,77 +2,89 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb"
 description = "A playback for YouTube live streams"
 readme = "README.rst"
-version = "2024.5.3"
+dynamic = ["version"]
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 dependencies = [
-    "av>=11.0.0",
+    "av>=12.0.0",
     "click>=8.1.7",
-    "cloup>=3.0.4",
-    "lxml>=5.0.0",
+    "cloup>=3.0.5",
+    "Jinja2>=3.1.4",
+    "lxml>=5.2.2",
     "pathvalidate>=3.2.0",
-    "pillow>=10.2.0",
-    "platformdirs>=4.1.0",
+    "pillow>=10.3.0",
+    "platformdirs>=4.2.2",
     "pycond>=20230212",
     "python-mpv-jsonipc>=1.2.0",
-    "requests>=2.31.0",
+    "requests>=2.32.0",
     "rich>=13.7.0",
-    "structlog>=23.3.0",
+    "structlog>=24.2.0",
     "timedelta_isoformat>=0.6.2.11",
     "toml>=0.10.2",
-    "unidecode>=1.3.7",
-    "yt_dlp>=2023.12.30",
+    "unidecode>=1.3.8",
+    "yt_dlp>=2024.05.27",
 ]
 
 [project.optional-dependencies]
 test = [
-    "freezegun>=1.4.0",
-    "pytest>=7.4.4",
+    "freezegun>=1.5.1",
+    "pytest>=8.2.1",
     "pytest-matcher==2.0.1",
-    "pytest-socket>=0.6.0",
-    "responses>=0.24.1"
+    "pytest-socket>=0.7.0",
+    "responses>=0.25.0"
 ]
 dev = [
     "ytpb[test]",
     "pre-commit",
 ]
 docs = [
-    "sphinx==7.2.6",
+    "sphinx==7.3.7",
     "sphinx-toolbox==3.5.0",
+    "myst-parser==3.0.1",
 ]
 
 [project.urls]
 Source = "https://github.com/xymaxim/ytpb"
 Documentation = "https://ytpb.readthedocs.io"
 
 [project.scripts]
 ytpb = "ytpb.__main__:main"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.version.raw-options]
+version_scheme = "calver-by-date"
+local_scheme = "dirty-tag"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/ytpb/_version.py"
+
 [tool.hatch.build.targets.sdist]
 exclude = [
    "/.github",
    "/notebooks",
 ]
 
 [tool.black]
 line-length = 88
 
 [tool.pytest.ini_options]
 pm-patterns-base-dir = "tests/data/expected/"
-pm-pattern-file-fmt = "{fn}{callspec}"
+pm-pattern-file-fmt = "{fn}{callspec}{suffix}"
```

### Comparing `ytpb-2024.5.3/PKG-INFO` & `ytpb-2024.5.30/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ytpb
-Version: 2024.5.3
+Version: 2024.5.30
 Summary: A playback for YouTube live streams
 Project-URL: Source, https://github.com/xymaxim/ytpb
 Project-URL: Documentation, https://ytpb.readthedocs.io
 Author: Maxim Stolyarchuk
 License: MIT License
         
         Copyright (c) 2024 Maxim Stolyarchuk
@@ -30,46 +30,48 @@
 Keywords: youtube
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
-Requires-Dist: av>=11.0.0
+Requires-Dist: av>=12.0.0
 Requires-Dist: click>=8.1.7
-Requires-Dist: cloup>=3.0.4
-Requires-Dist: lxml>=5.0.0
+Requires-Dist: cloup>=3.0.5
+Requires-Dist: jinja2>=3.1.4
+Requires-Dist: lxml>=5.2.2
 Requires-Dist: pathvalidate>=3.2.0
-Requires-Dist: pillow>=10.2.0
-Requires-Dist: platformdirs>=4.1.0
+Requires-Dist: pillow>=10.3.0
+Requires-Dist: platformdirs>=4.2.2
 Requires-Dist: pycond>=20230212
 Requires-Dist: python-mpv-jsonipc>=1.2.0
-Requires-Dist: requests>=2.31.0
+Requires-Dist: requests>=2.32.0
 Requires-Dist: rich>=13.7.0
-Requires-Dist: structlog>=23.3.0
+Requires-Dist: structlog>=24.2.0
 Requires-Dist: timedelta-isoformat>=0.6.2.11
 Requires-Dist: toml>=0.10.2
-Requires-Dist: unidecode>=1.3.7
-Requires-Dist: yt-dlp>=2023.12.30
+Requires-Dist: unidecode>=1.3.8
+Requires-Dist: yt-dlp>=2024.05.27
 Provides-Extra: dev
-Requires-Dist: freezegun>=1.4.0; extra == 'dev'
+Requires-Dist: freezegun>=1.5.1; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest-matcher==2.0.1; extra == 'dev'
-Requires-Dist: pytest-socket>=0.6.0; extra == 'dev'
-Requires-Dist: pytest>=7.4.4; extra == 'dev'
-Requires-Dist: responses>=0.24.1; extra == 'dev'
+Requires-Dist: pytest-socket>=0.7.0; extra == 'dev'
+Requires-Dist: pytest>=8.2.1; extra == 'dev'
+Requires-Dist: responses>=0.25.0; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: myst-parser==3.0.1; extra == 'docs'
 Requires-Dist: sphinx-toolbox==3.5.0; extra == 'docs'
-Requires-Dist: sphinx==7.2.6; extra == 'docs'
+Requires-Dist: sphinx==7.3.7; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: freezegun>=1.4.0; extra == 'test'
+Requires-Dist: freezegun>=1.5.1; extra == 'test'
 Requires-Dist: pytest-matcher==2.0.1; extra == 'test'
-Requires-Dist: pytest-socket>=0.6.0; extra == 'test'
-Requires-Dist: pytest>=7.4.4; extra == 'test'
-Requires-Dist: responses>=0.24.1; extra == 'test'
+Requires-Dist: pytest-socket>=0.7.0; extra == 'test'
+Requires-Dist: pytest>=8.2.1; extra == 'test'
+Requires-Dist: responses>=0.25.0; extra == 'test'
 Description-Content-Type: text/x-rst
 
 Ytpb
 ####
 
 A playback for YouTube live streams.
 
@@ -128,40 +130,57 @@
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
 Installation
 ************
 
-Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
+Ytpb requires Python 3.11 or higher and has been `tested
+<https://github.com/xymaxim/ytpb/actions/workflows/ci.yml>`__ on Linux, macOS,
+and Windows. Also, it needs the recent version of `FFmpeg
+<https://ffmpeg.org/download.html>`__ to be installed.
+
+Installing from PyPI
+====================
+
+When you have all required dependencies, you can install Ytpb via `pipx
 <https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
 To upgrade to the newer version, do::
 
   $ pipx upgrade ytpb
 
+Windows binaries
+================
+
+For Windows, pre-built binaries are available: check `releases
+<https://github.com/xymaxim/ytpb/releases>`__ on GitHub. Make sure to `add
+<https://www.wikihow.com/Install-FFmpeg-on-Windows>`__ the ``ffmpeg.exe`` file
+to your system path or place it in the folder next to the Ytpb binary. Now
+you're ready to use Ytpb in Terminal: type commands, not double-click.
+
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
-provides some general aspects and terms. `Cookbook`_ contains some useful
-examples. See `Changelog`_ for the history of releases. Have any issues,
-suggestions, or want to contribute code? `Contributing`_ tells how to
+provides some general aspects and terms. See `Questions`_ for answers to the
+most anticipated questions. `Cookbook`_ contains some useful examples.  Have any
+issues, suggestions, or want to contribute code? `Contributing`_ tells how to
 participate in the project.
 
 .. _Why Ytpb?: https://ytpb.readthedocs.io/en/latest/why.html
 .. _Quick start: https://ytpb.readthedocs.io/en/latest/quick.html
 .. _Command line application: https://ytpb.readthedocs.io/en/latest/cli.html
 .. _Reference: https://ytpb.readthedocs.io/en/latest/reference.html
+.. _Questions: https://ytpb.readthedocs.io/en/latest/questions.html
 .. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
-.. _Changelog: https://ytpb.readthedocs.io/en/latest/changelog.html
 
 Similar projects
 ****************
 
 - `Kethsar/ytarchive <https://github.com/Kethsar/ytarchive>`__ — archive streams from the start
 - `rytsikau/ee.Yrewind <https://github.com/rytsikau/ee.Yrewind>`__ — rewind and save streams
 - `yt-dlp/yt-dlp#6498 <https://github.com/yt-dlp/yt-dlp/pull/6498>`__ — brings rewind range selection to yt-dlp
```

