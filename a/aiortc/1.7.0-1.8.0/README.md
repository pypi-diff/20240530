# Comparing `tmp/aiortc-1.7.0.tar.gz` & `tmp/aiortc-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiortc-1.7.0.tar", last modified: Thu Jan 25 10:15:07 2024, max compression
+gzip compressed data, was "aiortc-1.8.0.tar", last modified: Mon Mar 11 23:26:20 2024, max compression
```

## Comparing `aiortc-1.7.0.tar` & `aiortc-1.8.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.845567 aiortc-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-25 10:14:59.000000 aiortc-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-25 10:14:59.000000 aiortc-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-01-25 10:15:07.845567 aiortc-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-25 10:14:59.000000 aiortc-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.821567 aiortc-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-25 10:14:59.000000 aiortc-1.7.0/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.817567 aiortc-1.7.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.821567 aiortc-1.7.0/examples/datachannel-cli/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-cli/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.821567 aiortc-1.7.0/examples/datachannel-filexfer/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-filexfer/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-filexfer/filexfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.821567 aiortc-1.7.0/examples/datachannel-vpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-vpn/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-vpn/tuntap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/datachannel-vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.821567 aiortc-1.7.0/examples/janus/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/janus/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/janus/janus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.825567 aiortc-1.7.0/examples/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/server/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)  1173624 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/server/demo-instruct.wav
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/server/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.825567 aiortc-1.7.0/examples/videostream-cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/videostream-cli/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/videostream-cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.825567 aiortc-1.7.0/examples/webcam/
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/webcam/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/webcam/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-01-25 10:14:59.000000 aiortc-1.7.0/examples/webcam/webcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-25 10:14:59.000000 aiortc-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 10:15:07.845567 aiortc-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-25 10:14:59.000000 aiortc-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.817567 aiortc-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.825567 aiortc-1.7.0/src/_cffi_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/_cffi_src/build_opus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/_cffi_src/build_vpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.829567 aiortc-1.7.0/src/aiortc/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/clock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.829567 aiortc-1.7.0/src/aiortc/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/_opus.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/_vpx.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/g711.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/h264.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/opus.py
--rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/codecs/vpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.833567 aiortc-1.7.0/src/aiortc/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/contrib/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/contrib/signaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/jitterbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/mediastreams.py
--rw-r--r--   0 runner    (1001) docker     (127)    20679 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcdatachannel.py
--rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcdtlstransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcicetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    48106 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcpeerconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcrtpparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    20729 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcrtpreceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcrtpsender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcrtptransceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    60760 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcsctptransport.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtcsessiondescription.py
--rw-r--r--   0 runner    (1001) docker     (127)    24732 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/rtp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/sdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-25 10:14:59.000000 aiortc-1.7.0/src/aiortc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.841567 aiortc-1.7.0/src/aiortc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-01-25 10:15:07.000000 aiortc-1.7.0/src/aiortc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-01-25 10:15:07.000000 aiortc-1.7.0/src/aiortc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 10:15:07.000000 aiortc-1.7.0/src/aiortc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-25 10:15:07.000000 aiortc-1.7.0/src/aiortc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-25 10:15:07.000000 aiortc-1.7.0/src/aiortc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:15:07.841567 aiortc-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/h264_0000.bin
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/h264_0001.bin
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/h264_0002.bin
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/h264_0003.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_bye.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_bye_invalid.bin
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_bye_no_sources.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_bye_padding.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_psfb_invalid.bin
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_psfb_pli.bin
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_rr.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_rr_invalid.bin
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_rtpfb.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_rtpfb_invalid.bin
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_sdes.bin
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_sdes_item_truncated.bin
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_sdes_source_truncated.bin
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_sr.bin
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtcp_sr_invalid.bin
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp.bin
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp_dtmf.bin
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp_only_padding.bin
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp_only_padding_with_header_extensions.bin
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp_with_csrc.bin
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/rtp_with_sdes_mid.bin
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_abort.bin
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_cookie_echo.bin
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_data.bin
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_data_padding.bin
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_error.bin
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_forward_tsn.bin
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_heartbeat.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_init.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_init_bad_verification.bin
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_reconfig_add_out.bin
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_reconfig_reset_out.bin
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_reconfig_response.bin
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_sack.bin
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/sctp_shutdown.bin
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25185 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_contrib_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_contrib_signaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_g711.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_h264.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_jitterbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_mediastreams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_opus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_ortc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31734 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19439 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcdtlstransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcicetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)   183370 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcpeerconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18849 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcrtpreceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcrtpsender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcrtptransceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    92649 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcsctptransport.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtcsessiondescription.py
--rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_rtp.py
--rw-r--r--   0 runner    (1001) docker     (127)    76647 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_sdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/test_vpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-25 10:14:59.000000 aiortc-1.7.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.274492 aiortc-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-11 23:26:12.000000 aiortc-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-11 23:26:12.000000 aiortc-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-11 23:26:20.274492 aiortc-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-11 23:26:12.000000 aiortc-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.250491 aiortc-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-11 23:26:12.000000 aiortc-1.8.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.246491 aiortc-1.8.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.250491 aiortc-1.8.0/examples/datachannel-cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-cli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.250491 aiortc-1.8.0/examples/datachannel-filexfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-filexfer/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-filexfer/filexfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.250491 aiortc-1.8.0/examples/datachannel-vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-vpn/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-vpn/tuntap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/datachannel-vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.250491 aiortc-1.8.0/examples/janus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/janus/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/janus/janus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.254491 aiortc-1.8.0/examples/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/server/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)  1173624 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/server/demo-instruct.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/server/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.254491 aiortc-1.8.0/examples/videostream-cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/videostream-cli/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/videostream-cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.254491 aiortc-1.8.0/examples/webcam/
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/webcam/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/webcam/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-03-11 23:26:12.000000 aiortc-1.8.0/examples/webcam/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-11 23:26:12.000000 aiortc-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 23:26:20.274492 aiortc-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-11 23:26:12.000000 aiortc-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.246491 aiortc-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.254491 aiortc-1.8.0/src/_cffi_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/_cffi_src/build_opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/_cffi_src/build_vpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.258492 aiortc-1.8.0/src/aiortc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/clock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.262492 aiortc-1.8.0/src/aiortc/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/_opus.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/_vpx.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/g711.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/h264.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/codecs/vpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.262492 aiortc-1.8.0/src/aiortc/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/contrib/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/contrib/signaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/jitterbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/mediastreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20679 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcdatachannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcdtlstransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcicetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48562 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcpeerconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcrtpparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcrtpreceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcrtpsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcrtptransceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60760 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcsctptransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtcsessiondescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24732 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/rtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/sdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-11 23:26:12.000000 aiortc-1.8.0/src/aiortc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.274492 aiortc-1.8.0/src/aiortc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-11 23:26:20.000000 aiortc-1.8.0/src/aiortc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-03-11 23:26:20.000000 aiortc-1.8.0/src/aiortc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 23:26:20.000000 aiortc-1.8.0/src/aiortc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-11 23:26:20.000000 aiortc-1.8.0/src/aiortc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 23:26:20.000000 aiortc-1.8.0/src/aiortc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:20.274492 aiortc-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/h264_0000.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/h264_0001.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/h264_0002.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/h264_0003.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_bye.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_bye_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_bye_no_sources.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_bye_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_psfb_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_psfb_pli.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_rr.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_rr_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_rtpfb.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_rtpfb_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_sdes.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_sdes_item_truncated.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_sdes_source_truncated.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_sr.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtcp_sr_invalid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp_dtmf.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp_only_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp_only_padding_with_header_extensions.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp_with_csrc.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/rtp_with_sdes_mid.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_abort.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_cookie_echo.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_data.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_data_padding.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_error.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_forward_tsn.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_heartbeat.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_init.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_init_bad_verification.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_reconfig_add_out.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_reconfig_reset_out.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_reconfig_response.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_sack.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/sctp_shutdown.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25185 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_contrib_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_contrib_signaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_g711.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_h264.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_jitterbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_mediastreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_opus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_ortc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31734 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19439 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcdtlstransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcicetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181301 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcpeerconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcrtpreceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcrtpsender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcrtptransceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92649 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcsctptransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtcsessiondescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26490 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_rtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76647 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_sdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/test_vpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-11 23:26:12.000000 aiortc-1.8.0/tests/utils.py
```

### Comparing `aiortc-1.7.0/LICENSE` & `aiortc-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/PKG-INFO` & `aiortc-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiortc
-Version: 1.7.0
+Version: 1.8.0
 Summary: An implementation of WebRTC and ORTC
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/aiortc/aiortc
 Project-URL: changelog, https://aiortc.readthedocs.io/en/stable/changelog.html
 Project-URL: documentation, https://aiortc.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiortc-1.7.0/README.rst` & `aiortc-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/Makefile` & `aiortc-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/api.rst` & `aiortc-1.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/changelog.rst` & `aiortc-1.8.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Changelog
 =========
 
 .. currentmodule:: aiortc
 
+1.8.0
+-----
+
+* Only send / receive RTP according to :attr:`RTCRtpTransceiver.currentDirection`.
+* Close the :class:`RTCPeerConnection` if all DTLS transports are closed.
+* Free the encoder as soon as the :class:`RTCRtpSender` stops to save memory.
+* Modernise JavaScript in `server` and `webcam` examples.
+
 1.7.0
 -----
 
  * Add support for GCM based SRTP protection profiles.
  * Reduce supported DTLS cipher list to avoid Client Hello fragmentation.
  * Fix `utcnow()` deprecation warning on Python 3.12.
 
 1.6.0
 -----
 
  * Build wheels using `Py_LIMITED_ABI` to make them compatible with future Python versions.
  * Build wheels using opus 1.4 and vpx 1.13.1.
  * Use unique IDs for audio and video header extensions.
- * Allow :class:`aiortc.contrib.media.MediaRecorder` to record audio from pulse.
+ * Allow :class:`~aiortc.contrib.media.MediaRecorder` to record audio from pulse.
 
 1.5.0
 -----
 
  * Make H.264 send a full picture when picture loss occurs.
  * Fix TURN over TCP by updating `aioice` to 0.9.0.
  * Make use of the `ifaddr` package instead of the unmaintained `netifaces` package.
 
 1.4.0
 -----
 
  * Build wheels for Python 3.11.
- * Allow :class:`aiortc.contrib.media.MediaPlayer` to send media without transcoding.
- * Allow :class:`aiortc.contrib.media.MediaPlayer` to specify a timeout when opening media.
- * Make :class:`aiortc.RTCSctpTransport` transmit packets sooner to reduce datachannel latency.
- * Refactor :class:`aiortc.RTCDtlsTransport` to use PyOpenSSL.
- * Make :class:`aiortc.RTCPeerConnection` log sent and received SDP when using verbose logging.
+ * Allow :class:`~aiortc.contrib.media.MediaPlayer` to send media without transcoding.
+ * Allow :class:`~aiortc.contrib.media.MediaPlayer` to specify a timeout when opening media.
+ * Make :class:`RTCSctpTransport` transmit packets sooner to reduce datachannel latency.
+ * Refactor :class:`RTCDtlsTransport` to use PyOpenSSL.
+ * Make :class:`RTCPeerConnection` log sent and received SDP when using verbose logging.
 
 1.3.2
 -----
 
  * Limit size of NACK reports to avoid excessive packet size.
  * Improve H.264 codec matching.
- * Determine video size from first frame received by :class:`aiortc.contrib.media.MediaRecorder`.
+ * Determine video size from first frame received by :class:`~aiortc.contrib.media.MediaRecorder`.
  * Fix a deprecation warning when using `av` >= 9.1.0.
  * Tolerate STUN URLs containing a `protocol` querystring argument.
 
 1.3.1
 -----
 
  * Build wheels for aarch64 on Linux.
- * Adapt :class:`aiortc.contrib.media.MediaPlayer` for PyAV 9.x.
+ * Adapt :class:`~aiortc.contrib.media.MediaPlayer` for PyAV 9.x.
  * Ensure H.264 produces B-frames by resetting picture type.
 
 1.3.0
 -----
 
  * Build wheels for Python 3.10 and for arm64 on Mac.
  * Build wheels against `libvpx` 1.10.
- * Add support for looping in :class:`aiortc.contrib.media.MediaPlayer`.
- * Add unbuffered option to :class:`aiortc.contrib.media.MediaRelay`.
+ * Add support for looping in :class:`~aiortc.contrib.media.MediaPlayer`.
+ * Add unbuffered option to :class:`~aiortc.contrib.media.MediaRelay`.
  * Calculate audio energy and send in RTP header extension.
  * Fix a race condition in RTP sender/receiver shutdown.
  * Improve performance of H.264 bitstream splitting code.
  * Update imports for `pyee` version 9.x.
  * Fully switch to `google-crc32c` instead of `crc32`.
  * Drop support for Python 3.6.
  * Remove `apprtc` code as the service is no longer publicly hosted.
@@ -77,15 +85,15 @@
 -----
 
  * Fix jitter buffer to avoid severe picture corruption under packet loss and
    send Picture Loss Indication (PLI) when needed.
  * Make H.264 encoder honour the bitrate from the bandwidth estimator.
  * Add support for hardware-accelerated H.264 encoding on Raspberry Pi 4 using
    the `h264_omx` codec.
- * Add :class:`aiortc.contrib.media.MediaRelay` class to allow sending media
+ * Add :class:`~aiortc.contrib.media.MediaRelay` class to allow sending media
    tracks to multiple consumers.
 
 1.1.2
 -----
 
  * Add :attr:`RTCPeerConnection.connectionState` property.
  * Correctly detect RTCIceTransport `"failed"` state.
@@ -245,21 +253,21 @@
 ....
 
   * Call SSL_CTX_set_ecdh_auto for OpenSSL 1.0.2.
 
 Media
 .....
 
-  * Correctly route REMB packets to the :class:`aiortc.RTCRtpSender`.
+  * Correctly route REMB packets to the :class:`RTCRtpSender`.
 
 Examples
 ........
 
-  * :class:`aiortc.contrib.media.MediaPlayer` : release resources (e.g. webcam) when the player stops.
-  * :class:`aiortc.contrib.signaling.ApprtcSignaling` : make AppRTC signaling available for more examples.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : release resources (e.g. webcam) when the player stops.
+  * :class:`~aiortc.contrib.signaling.ApprtcSignaling` : make AppRTC signaling available for more examples.
   * `datachannel-cli` : make uvloop optional.
   * `videostream-cli` : animate the flag with a wave effect.
   * `webcam` : explicitly set frame rate to 30 fps for webcams.
 
 0.9.20
 ------
 
@@ -272,15 +280,15 @@
 .............
 
   * Fix documentation build by installing `crc32c` instead of `crcmod`.
 
 Examples
 ........
 
-  * :class:`aiortc.contrib.media.MediaPlayer` : skip frames with no presentation timestamp (pts).
+  * :class:`~aiortc.contrib.media.MediaPlayer` : skip frames with no presentation timestamp (pts).
 
 0.9.19
 ------
 
 Data channels
 .............
 
@@ -450,15 +458,15 @@
     reduces the response time.
   * Adjust package requirements to accept PyAV < 7.0.0.
 
 Examples
 ........
 
   * `webcam` : force Chrome to use "unified-plan" semantics to enabled `addTransceiver`.
-  * :class:`aiortc.contrib.media.MediaPlayer` : don't sleep at all when playing from webcam.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : don't sleep at all when playing from webcam.
     This eliminates the constant one-second lag in the `webcam` demo.
 
 0.9.9
 -----
 
 .. warning::
 
@@ -471,21 +479,21 @@
   * Use a jitter buffer for incoming audio.
   * Add :meth:`RTCPeerConnection.addTransceiver` method.
   * Add :attr:`RTCRtpTransceiver.direction` to manage transceiver direction.
 
 Examples
 ........
 
-  * `apprtc` : demonstrate the use of :class:`aiortc.contrib.media.MediaPlayer`
-    and :class:`aiortc.contrib.media.MediaRecorder`.
+  * `apprtc` : demonstrate the use of :class:`~aiortc.contrib.media.MediaPlayer`
+    and :class:`~aiortc.contrib.media.MediaRecorder`.
   * `webcam` : new examples illustrating sending video from a webcam to a browser.
-  * :class:`aiortc.contrib.media.MediaPlayer` : don't sleep if a frame lacks timing information.
-  * :class:`aiortc.contrib.media.MediaPlayer` : remove `start()` and `stop()` methods.
-  * :class:`aiortc.contrib.media.MediaRecorder` : use `libx264` for encoding.
-  * :class:`aiortc.contrib.media.MediaRecorder` : make `start()` and `stop()` coroutines.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : don't sleep if a frame lacks timing information.
+  * :class:`~aiortc.contrib.media.MediaPlayer` : remove `start()` and `stop()` methods.
+  * :class:`~aiortc.contrib.media.MediaRecorder` : use `libx264` for encoding.
+  * :class:`~aiortc.contrib.media.MediaRecorder` : make `start()` and `stop()` coroutines.
 
 0.9.8
 -----
 
 Media
 .....
 
@@ -500,17 +508,17 @@
 
   * Add the :meth:`RTCPeerConnection.getStats()` coroutine to retrieve statistics.
   * Add initial :class:`RTCTransportStats` to report transport statistics.
 
 Examples
 ........
 
-  * Add new :class:`aiortc.contrib.media.MediaPlayer` class to read audio / video from a file.
-  * Add new :class:`aiortc.contrib.media.MediaRecorder` class to write audio / video to a file.
-  * Add new :class:`aiortc.contrib.media.MediaBlackhole` class to discard audio / video.
+  * Add new :class:`~aiortc.contrib.media.MediaPlayer` class to read audio / video from a file.
+  * Add new :class:`~aiortc.contrib.media.MediaRecorder` class to write audio / video to a file.
+  * Add new :class:`~aiortc.contrib.media.MediaBlackhole` class to discard audio / video.
 
 0.9.7
 -----
 
 Media
 .....
 
@@ -686,21 +694,21 @@
 ...............
 
   * Add :meth:`RTCPeerConnection.addIceCandidate()` method to handle trickled ICE candidates.
 
 Media
 .....
 
-  * Make stop() methods of :class:`aiortc.RTCRtpReceiver`, :class:`aiortc.RTCRtpSender`
+  * Make stop() methods of :class:`RTCRtpReceiver`, :class:`RTCRtpSender`
     and :class:`RTCRtpTransceiver` coroutines to enable clean shutdown.
 
 Data channels
 .............
 
-  * Clean up :class:`aiortc.RTCDataChannel` shutdown sequence.
+  * Clean up :class:`RTCDataChannel` shutdown sequence.
 
   * Support receiving an SCTP `RE-CONFIG` to raise number of inbound streams.
 
 Examples
 ........
 
   * `server`:
@@ -728,19 +736,19 @@
   * Add `BUNDLE` support to use a single ICE/DTLS transport for multiple media.
 
   * Move media encoding / decoding off the main thread.
 
 Data channels
 .............
 
-  * Use SCTP `ABORT` instead of `SHUTDOWN` when stopping :class:`aiortc.RTCSctpTransport`.
+  * Use SCTP `ABORT` instead of `SHUTDOWN` when stopping :class:`RTCSctpTransport`.
 
   * Advertise support for SCTP `RE-CONFIG` extension.
 
-  * Make :class:`aiortc.RTCDataChannel` emit `open` and `close` events.
+  * Make :class:`RTCDataChannel` emit `open` and `close` events.
 
 Examples
 ........
 
   * Add an example of how to connect to appr.tc.
 
   * Capture audio frames to a WAV file in server example.
```

### Comparing `aiortc-1.7.0/docs/conf.py` & `aiortc-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/contributing.rst` & `aiortc-1.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/helpers.rst` & `aiortc-1.8.0/docs/helpers.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/docs/index.rst` & `aiortc-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-cli/README.rst` & `aiortc-1.8.0/examples/datachannel-cli/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-cli/cli.py` & `aiortc-1.8.0/examples/datachannel-cli/cli.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-filexfer/README.rst` & `aiortc-1.8.0/examples/datachannel-filexfer/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-filexfer/filexfer.py` & `aiortc-1.8.0/examples/datachannel-filexfer/filexfer.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-vpn/README.rst` & `aiortc-1.8.0/examples/datachannel-vpn/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-vpn/tuntap.py` & `aiortc-1.8.0/examples/datachannel-vpn/tuntap.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/datachannel-vpn/vpn.py` & `aiortc-1.8.0/examples/datachannel-vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/janus/README.rst` & `aiortc-1.8.0/examples/janus/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/janus/janus.py` & `aiortc-1.8.0/examples/janus/janus.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/server/README.rst` & `aiortc-1.8.0/examples/server/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/server/demo-instruct.wav` & `aiortc-1.8.0/examples/server/demo-instruct.wav`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/server/index.html` & `aiortc-1.8.0/examples/server/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 <head>
     <meta charset="UTF-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>WebRTC demo</title>
     <style>
     button {
@@ -37,24 +38,30 @@
         <option value='{"ordered": false, "maxRetransmits": 0}'>Unordered, no retransmissions</option>
         <option value='{"ordered": false, "maxPacketLifetime": 500}'>Unordered, 500ms lifetime</option>
     </select>
 </div>
 <div class="option">
     <input id="use-audio" checked="checked" type="checkbox"/>
     <label for="use-audio">Use audio</label>
+    <select id="audio-input">
+        <option value="" selected>Default device</option>
+    </select>
     <select id="audio-codec">
         <option value="default" selected>Default codecs</option>
         <option value="opus/48000/2">Opus</option>
         <option value="PCMU/8000">PCMU</option>
         <option value="PCMA/8000">PCMA</option>
     </select>
 </div>
 <div class="option">
     <input id="use-video" type="checkbox"/>
     <label for="use-video">Use video</label>
+    <select id="video-input">
+        <option value="" selected>Default device</option>
+    </select>
     <select id="video-resolution">
         <option value="" selected>Default resolution</option>
         <option value="320x240">320x240</option>
         <option value="640x480">640x480</option>
         <option value="960x540">960x540</option>
         <option value="1280x720">1280x720</option>
     </select>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ********** OOppttiioonnss **********
 Use datachannel[One of: Ordered, reliable/Unordered, no retransmissions/
 Unordered, 500ms lifetime]
-Use audio[One of: Default codecs/Opus/PCMU/PCMA]
-??Use video[One of: Default resolution/320x240/640x480/960x540/1280x720][One of:
-No transform/Edge detection/Cartoon effect/Rotate][One of: Default codecs/VP8/
-H264]
+Use audio[One of: Default device][One of: Default codecs/Opus/PCMU/PCMA]
+??Use video[One of: Default device][One of: Default resolution/320x240/640x480/
+960x540/1280x720][One of: No transform/Edge detection/Cartoon effect/Rotate]
+[One of: Default codecs/VP8/H264]
 ??Use STUN server
 Start Stop
 ********** SSttaattee **********
 ICE gathering state:
 ICE connection state:
 Signaling state:
 ********** MMeeddiiaa **********
```

### Comparing `aiortc-1.7.0/examples/server/server.py` & `aiortc-1.8.0/examples/server/server.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/videostream-cli/README.rst` & `aiortc-1.8.0/examples/videostream-cli/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/videostream-cli/cli.py` & `aiortc-1.8.0/examples/videostream-cli/cli.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/webcam/README.rst` & `aiortc-1.8.0/examples/webcam/README.rst`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/examples/webcam/index.html` & `aiortc-1.8.0/examples/webcam/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 <head>
     <meta charset="UTF-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>WebRTC webcam</title>
     <style>
     button {
```

### Comparing `aiortc-1.7.0/examples/webcam/webcam.py` & `aiortc-1.8.0/examples/webcam/webcam.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/pyproject.toml` & `aiortc-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 disallow_untyped_decorators = true
 ignore_missing_imports = true
 mypy_path = "stubs"
 strict_optional = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "W",  # pycodestyle
     "I",  # isort
 ]
```

### Comparing `aiortc-1.7.0/src/_cffi_src/build_opus.py` & `aiortc-1.8.0/src/_cffi_src/build_opus.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/_cffi_src/build_vpx.py` & `aiortc-1.8.0/src/_cffi_src/build_vpx.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/__init__.py` & `aiortc-1.8.0/src/aiortc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,14 @@
     RTCOutboundRtpStreamStats,
     RTCRemoteInboundRtpStreamStats,
     RTCRemoteOutboundRtpStreamStats,
     RTCStatsReport,
     RTCTransportStats,
 )
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 # Disable PyAV's logging framework as it can lead to thread deadlocks.
 av.logging.restore_default_callback()
 
 # Set default logging handler to avoid "No handler found" warnings.
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `aiortc-1.7.0/src/aiortc/clock.py` & `aiortc-1.8.0/src/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/__init__.py` & `aiortc-1.8.0/src/aiortc/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/base.py` & `aiortc-1.8.0/src/aiortc/codecs/base.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/g711.py` & `aiortc-1.8.0/src/aiortc/codecs/g711.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/h264.py` & `aiortc-1.8.0/src/aiortc/codecs/h264.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/opus.py` & `aiortc-1.8.0/src/aiortc/codecs/opus.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/codecs/vpx.py` & `aiortc-1.8.0/src/aiortc/codecs/vpx.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/contrib/media.py` & `aiortc-1.8.0/src/aiortc/contrib/media.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/contrib/signaling.py` & `aiortc-1.8.0/src/aiortc/contrib/signaling.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/events.py` & `aiortc-1.8.0/src/aiortc/events.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/jitterbuffer.py` & `aiortc-1.8.0/src/aiortc/jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/mediastreams.py` & `aiortc-1.8.0/src/aiortc/mediastreams.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rate.py` & `aiortc-1.8.0/src/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcconfiguration.py` & `aiortc-1.8.0/src/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcdatachannel.py` & `aiortc-1.8.0/src/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcdtlstransport.py` & `aiortc-1.8.0/src/aiortc/rtcdtlstransport.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcicetransport.py` & `aiortc-1.8.0/src/aiortc/rtcicetransport.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcpeerconnection.py` & `aiortc-1.8.0/src/aiortc/rtcpeerconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,18 +307,19 @@
         self.__sctp_mline_index: Optional[int] = None
         self._sctpLegacySdp = True
         self.__sctpRemotePort: Optional[int] = None
         self.__sctpRemoteCaps = None
         self.__stream_id = str(uuid.uuid4())
         self.__transceivers: List[RTCRtpTransceiver] = []
 
+        self.__closeTask: Optional[asyncio.Task] = None
         self.__connectionState = "new"
         self.__iceConnectionState = "new"
         self.__iceGatheringState = "new"
-        self.__isClosed = False
+        self.__isClosed: Optional[asyncio.Future[bool]] = None
         self.__signalingState = "stable"
 
         self.__currentLocalDescription: Optional[sdp.SessionDescription] = None
         self.__currentRemoteDescription: Optional[sdp.SessionDescription] = None
         self.__pendingLocalDescription: Optional[sdp.SessionDescription] = None
         self.__pendingRemoteDescription: Optional[sdp.SessionDescription] = None
 
@@ -475,16 +476,17 @@
         )
 
     async def close(self):
         """
         Terminate the ICE agent, ending ICE processing and streams.
         """
         if self.__isClosed:
+            await self.__isClosed
             return
-        self.__isClosed = True
+        self.__isClosed = asyncio.Future()
         self.__setSignalingState("closed")
 
         # stop senders / receivers
         for transceiver in self.__transceivers:
             await transceiver.stop()
         if self.__sctp:
             await self.__sctp.stop()
@@ -502,14 +504,16 @@
         self.__updateIceConnectionState()
         self.__updateConnectionState()
 
         # no more events will be emitted, so remove all event listeners
         # to facilitate garbage collection.
         self.remove_all_listeners()
 
+        self.__isClosed.set_result(True)
+
     async def createAnswer(self):
         """
         Create an SDP answer to an offer received from a remote peer during
         the offer/answer negotiation of a WebRTC connection.
 
         :rtype: :class:`RTCSessionDescription`
         """
@@ -781,15 +785,15 @@
                     transceiver._transport._set_role(media.dtls.role)
                 elif media.kind == "application":
                     self.__sctp.transport._set_role(media.dtls.role)
 
         # configure direction
         for t in self.__transceivers:
             if description.type in ["answer", "pranswer"]:
-                t._currentDirection = and_direction(t.direction, t._offerDirection)
+                t._setCurrentDirection(and_direction(t.direction, t._offerDirection))
 
         # gather candidates
         await self.__gather()
         for i, media in enumerate(description.media):
             if media.kind in ["audio", "video"]:
                 transceiver = self.__getTransceiverByMLineIndex(i)
                 add_transport_description(media, transceiver._transport)
@@ -863,15 +867,15 @@
                 transceiver._headerExtensions = find_common_header_extensions(
                     HEADER_EXTENSIONS[media.kind], media.rtp.headerExtensions
                 )
 
                 # configure direction
                 direction = reverse_direction(media.direction)
                 if description.type in ["answer", "pranswer"]:
-                    transceiver._currentDirection = direction
+                    transceiver._setCurrentDirection(direction)
                 else:
                     transceiver._offerDirection = direction
 
                 # create remote stream track
                 if (
                     direction in ["recvonly", "sendrecv"]
                     and not transceiver.receiver.track
@@ -1173,14 +1177,22 @@
 
         # update state
         if state != self.__connectionState:
             self.__log_debug("connectionState %s -> %s", self.__connectionState, state)
             self.__connectionState = state
             self.emit("connectionstatechange")
 
+        # if all DTLS connections are closed, initiate a shutdown
+        if (
+            not self.__isClosed
+            and self.__closeTask is None
+            and dtlsStates == set(["closed"])
+        ):
+            self.__closeTask = asyncio.ensure_future(self.close())
+
     def __updateIceConnectionState(self) -> None:
         # compute new state
         # NOTE: we do not have "connected" or "disconnected" states
         states = set(map(lambda x: x.state, self.__iceTransports))
         if self.__isClosed:
             state = "closed"
         elif "failed" in states:
```

### Comparing `aiortc-1.7.0/src/aiortc/rtcrtpparameters.py` & `aiortc-1.8.0/src/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtcrtpreceiver.py` & `aiortc-1.8.0/src/aiortc/rtcrtpreceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,15 @@
     :param transport: An :class:`RTCDtlsTransport`.
     """
 
     def __init__(self, kind: str, transport: RTCDtlsTransport) -> None:
         if transport.state == "closed":
             raise InvalidStateError
 
+        self._enabled = True
         self.__active_ssrc: Dict[int, datetime.datetime] = {}
         self.__codecs: Dict[int, RTCRtpCodecParameters] = {}
         self.__decoder_queue: queue.Queue = queue.Queue()
         self.__decoder_thread: Optional[threading.Thread] = None
         self.__kind = kind
         if kind == "audio":
             self.__jitter_buffer = JitterBuffer(capacity=16, prefetch=4)
@@ -446,14 +447,18 @@
 
     async def _handle_rtp_packet(self, packet: RtpPacket, arrival_time_ms: int) -> None:
         """
         Handle an incoming RTP packet.
         """
         self.__log_debug("< %s", packet)
 
+        # If the receiver is disabled, discard the packet.
+        if not self._enabled:
+            return
+
         # feed bitrate estimator
         if self.__remote_bitrate_estimator is not None:
             if packet.extensions.abs_send_time is not None:
                 remb = self.__remote_bitrate_estimator.add(
                     abs_send_time=packet.extensions.abs_send_time,
                     arrival_time_ms=arrival_time_ms,
                     payload_size=len(packet.payload) + packet.padding_size,
```

### Comparing `aiortc-1.7.0/src/aiortc/rtcrtpsender.py` & `aiortc-1.8.0/src/aiortc/rtcrtpsender.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             self.__kind = trackOrKind
             self.replaceTrack(None)
         self.__cname: Optional[str] = None
         self._ssrc = random32()
         self._rtx_ssrc = random32()
         # FIXME: how should this be initialised?
         self._stream_id = str(uuid.uuid4())
+        self._enabled = True
         self.__encoder: Optional[Encoder] = None
         self.__force_keyframe = False
         self.__loop = asyncio.get_event_loop()
         self.__mid: Optional[str] = None
         self.__rtp_exited = asyncio.Event()
         self.__rtp_header_extensions_map = rtp.HeaderExtensionsMap()
         self.__rtp_started = asyncio.Event()
@@ -264,14 +265,21 @@
                         self.__encoder.target_bitrate = bitrate
             except ValueError:
                 pass
 
     async def _next_encoded_frame(self, codec: RTCRtpCodecParameters):
         # get [Frame|Packet]
         data = await self.__track.recv()
+
+        # If the sender is disabled, drop the frame instead of encoding it.
+        # We still want to read from the track in order to avoid frames
+        # accumulating in memory.
+        if not self._enabled:
+            return None
+
         audio_level = None
 
         if self.__encoder is None:
             self.__encoder = get_encoder(codec)
 
         if isinstance(data, Frame):
             # encode frame
@@ -321,15 +329,20 @@
         timestamp_origin = random32()
         try:
             while True:
                 if not self.__track:
                     await asyncio.sleep(0.02)
                     continue
 
+                # Fetch the next encoded frame. This can be `None` if the sender
+                # is disabled, in which case we just continue the loop.
                 enc_frame = await self._next_encoded_frame(codec)
+                if enc_frame is None:
+                    continue
+
                 timestamp = uint32_add(timestamp_origin, enc_frame.timestamp)
 
                 for i, payload in enumerate(enc_frame.payloads):
                     packet = RtpPacket(
                         payload_type=codec.payloadType,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
@@ -344,17 +357,17 @@
                     ) & 0x00FFFFFF
                     packet.extensions.mid = self.__mid
                     if enc_frame.audio_level is not None:
                         packet.extensions.audio_level = (False, -enc_frame.audio_level)
 
                     # send packet
                     self.__log_debug("> %s", packet)
-                    self.__rtp_history[
-                        packet.sequence_number % RTP_HISTORY_SIZE
-                    ] = packet
+                    self.__rtp_history[packet.sequence_number % RTP_HISTORY_SIZE] = (
+                        packet
+                    )
                     packet_bytes = packet.serialize(self.__rtp_header_extensions_map)
                     await self.transport._send_rtp(packet_bytes)
 
                     self.__ntp_timestamp = clock.current_ntp_time()
                     self.__rtp_timestamp = packet.timestamp
                     self.__octet_count += len(payload)
                     self.__packet_count += 1
@@ -367,14 +380,18 @@
             self.__log_warning(traceback.format_exc())
 
         # stop track
         if self.__track:
             self.__track.stop()
             self.__track = None
 
+        # release encoder
+        if self.__encoder:
+            del self.__encoder
+
         self.__log_debug("- RTP finished")
         self.__rtp_exited.set()
 
     async def _run_rtcp(self) -> None:
         self.__log_debug("- RTCP started")
         self.__rtcp_started.set()
```

### Comparing `aiortc-1.7.0/src/aiortc/rtcrtptransceiver.py` & `aiortc-1.8.0/src/aiortc/rtcrtptransceiver.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     def __init__(
         self,
         kind: str,
         receiver: RTCRtpReceiver,
         sender: RTCRtpSender,
         direction: str = "sendrecv",
     ):
+        self.__currentDirection: Optional[str] = None
         self.__direction = direction
         self.__kind = kind
         self.__mid: Optional[str] = None
         self.__mline_index: Optional[int] = None
         self.__receiver = receiver
         self.__sender = sender
         self.__stopped = False
 
-        self._currentDirection: Optional[str] = None
         self._offerDirection: Optional[str] = None
         self._preferred_codecs: List[RTCRtpCodecCapability] = []
         self._transport: RTCDtlsTransport = None
 
         # FIXME: this is only used by RTCPeerConnection
         self._bundled = False
         self._codecs: List[RTCRtpCodecParameters] = []
@@ -50,15 +50,15 @@
     @property
     def currentDirection(self) -> Optional[str]:
         """
         The currently negotiated direction of the transceiver.
 
         One of `'sendrecv'`, `'sendonly'`, `'recvonly'`, `'inactive'` or `None`.
         """
-        return self._currentDirection
+        return self.__currentDirection
 
     @property
     def direction(self) -> str:
         """
         The preferred direction of the transceiver, which will be used in
         :meth:`RTCPeerConnection.createOffer` and
         :meth:`RTCPeerConnection.createAnswer`.
@@ -126,14 +126,30 @@
         """
         Permanently stops the :class:`RTCRtpTransceiver`.
         """
         await self.__receiver.stop()
         await self.__sender.stop()
         self.__stopped = True
 
+    def _setCurrentDirection(self, direction: str) -> None:
+        self.__currentDirection = direction
+
+        if direction == "sendrecv":
+            self.__sender._enabled = True
+            self.__receiver._enabled = True
+        elif direction == "sendonly":
+            self.__sender._enabled = True
+            self.__receiver._enabled = False
+        elif direction == "recvonly":
+            self.__sender._enabled = False
+            self.__receiver._enabled = True
+        elif direction == "inactive":
+            self.__sender._enabled = False
+            self.__receiver._enabled = False
+
     def _set_mid(self, mid: str) -> None:
         self.__mid = mid
 
     def _get_mline_index(self) -> Optional[int]:
         return self.__mline_index
 
     def _set_mline_index(self, idx: int) -> None:
```

### Comparing `aiortc-1.7.0/src/aiortc/rtcsctptransport.py` & `aiortc-1.8.0/src/aiortc/rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/rtp.py` & `aiortc-1.8.0/src/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/sdp.py` & `aiortc-1.8.0/src/aiortc/sdp.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/stats.py` & `aiortc-1.8.0/src/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc/utils.py` & `aiortc-1.8.0/src/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/src/aiortc.egg-info/PKG-INFO` & `aiortc-1.8.0/src/aiortc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiortc
-Version: 1.7.0
+Version: 1.8.0
 Summary: An implementation of WebRTC and ORTC
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/aiortc/aiortc
 Project-URL: changelog, https://aiortc.readthedocs.io/en/stable/changelog.html
 Project-URL: documentation, https://aiortc.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiortc-1.7.0/src/aiortc.egg-info/SOURCES.txt` & `aiortc-1.8.0/src/aiortc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/codecs.py` & `aiortc-1.8.0/tests/codecs.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/h264_0001.bin` & `aiortc-1.8.0/tests/h264_0001.bin`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/h264_0002.bin` & `aiortc-1.8.0/tests/h264_0002.bin`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/h264_0003.bin` & `aiortc-1.8.0/tests/h264_0003.bin`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_clock.py` & `aiortc-1.8.0/tests/test_clock.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_contrib_media.py` & `aiortc-1.8.0/tests/test_contrib_media.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_contrib_signaling.py` & `aiortc-1.8.0/tests/test_contrib_signaling.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_g711.py` & `aiortc-1.8.0/tests/test_g711.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_h264.py` & `aiortc-1.8.0/tests/test_h264.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,43 +209,43 @@
     def test_split_bitstream(self):
         # No start code
         packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x00"))
         self.assertEqual(packages, [])
 
         # 3-byte start code
         packages = list(
-            H264Encoder._split_bitstream(b"\x00\x00\x01\xFF\x00\x00\x01\xFB")
+            H264Encoder._split_bitstream(b"\x00\x00\x01\xff\x00\x00\x01\xfb")
         )
-        self.assertEqual(packages, [b"\xFF", b"\xFB"])
+        self.assertEqual(packages, [b"\xff", b"\xfb"])
 
         # 4-byte start code
         packages = list(
-            H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xFF\x00\x00\x00\x01\xFB")
+            H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xff\x00\x00\x00\x01\xfb")
         )
-        self.assertEqual(packages, [b"\xFF", b"\xFB"])
+        self.assertEqual(packages, [b"\xff", b"\xfb"])
 
         # Multiple bytes in a packet
         packages = list(
             H264Encoder._split_bitstream(
-                b"\x00\x00\x00\x01\xFF\xAB\xCD\x00\x00\x00\x01\xFB"
+                b"\x00\x00\x00\x01\xff\xab\xcd\x00\x00\x00\x01\xfb"
             )
         )
-        self.assertEqual(packages, [b"\xFF\xAB\xCD", b"\xFB"])
+        self.assertEqual(packages, [b"\xff\xab\xcd", b"\xfb"])
 
         # Skip leading 0s
-        packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xFF"))
-        self.assertEqual(packages, [b"\xFF"])
+        packages = list(H264Encoder._split_bitstream(b"\x00\x00\x00\x01\xff"))
+        self.assertEqual(packages, [b"\xff"])
 
         # Both leading and trailing 0s
         packages = list(
             H264Encoder._split_bitstream(
-                b"\x00\x00\x00\x00\x00\x00\x01\xFF\x00\x00\x00\x00\x00"
+                b"\x00\x00\x00\x00\x00\x00\x01\xff\x00\x00\x00\x00\x00"
             )
         )
-        self.assertEqual(packages, [b"\xFF\x00\x00\x00\x00\x00"])
+        self.assertEqual(packages, [b"\xff\x00\x00\x00\x00\x00"])
 
     def test_packetize_one_small(self):
         packages = [bytes([0xFF, 0xFF])]
         packetize_packages = H264Encoder._packetize(packages)
         self.assertListEqual(packages, packetize_packages)
 
         packages = [bytes([0xFF]) * 1300]
```

### Comparing `aiortc-1.7.0/tests/test_jitterbuffer.py` & `aiortc-1.8.0/tests/test_jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_mediastreams.py` & `aiortc-1.8.0/tests/test_mediastreams.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_opus.py` & `aiortc-1.8.0/tests/test_opus.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_ortc.py` & `aiortc-1.8.0/tests/test_ortc.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rate.py` & `aiortc-1.8.0/tests/test_rate.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rtcdtlstransport.py` & `aiortc-1.8.0/tests/test_rtcdtlstransport.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rtcicetransport.py` & `aiortc-1.8.0/tests/test_rtcicetransport.py`

 * *Files 7% similar despite different names*

```diff
@@ -258,23 +258,29 @@
             [RTCIceServer(urls="stun:stun.l.google.com:19302")],
         )
 
 
 class RTCIceTransportTest(TestCase):
     def setUp(self):
         # save timers
+        self.consent_failures = aioice.ice.CONSENT_FAILURES
+        self.consent_interval = aioice.ice.CONSENT_INTERVAL
         self.retry_max = aioice.stun.RETRY_MAX
         self.retry_rto = aioice.stun.RETRY_RTO
 
         # shorten timers to run tests faster
+        aioice.ice.CONSENT_FAILURES = 1
+        aioice.ice.CONSENT_INTERVAL = 1
         aioice.stun.RETRY_MAX = 1
         aioice.stun.RETRY_RTO = 0.1
 
     def tearDown(self):
         # restore timers
+        aioice.ice.CONSENT_FAILURES = self.consent_failures
+        aioice.ice.CONSENT_INTERVAL = self.consent_interval
         aioice.stun.RETRY_MAX = self.retry_max
         aioice.stun.RETRY_RTO = self.retry_rto
 
     @asynctest
     async def test_construct(self):
         gatherer = RTCIceGatherer()
         connection = RTCIceTransport(gatherer)
@@ -354,14 +360,50 @@
 
         # cleanup
         await asyncio.gather(transport_1.stop(), transport_2.stop())
         self.assertEqual(transport_1.state, "closed")
         self.assertEqual(transport_2.state, "closed")
 
     @asynctest
+    async def test_connect_then_consent_expires(self):
+        gatherer_1 = RTCIceGatherer()
+        transport_1 = RTCIceTransport(gatherer_1)
+
+        gatherer_2 = RTCIceGatherer()
+        transport_2 = RTCIceTransport(gatherer_2)
+
+        # gather candidates
+        await asyncio.gather(gatherer_1.gather(), gatherer_2.gather())
+        for candidate in gatherer_2.getLocalCandidates():
+            await transport_1.addRemoteCandidate(candidate)
+        for candidate in gatherer_1.getLocalCandidates():
+            await transport_2.addRemoteCandidate(candidate)
+        self.assertEqual(transport_1.state, "new")
+        self.assertEqual(transport_2.state, "new")
+
+        # connect
+        await asyncio.gather(
+            transport_1.start(gatherer_2.getLocalParameters()),
+            transport_2.start(gatherer_1.getLocalParameters()),
+        )
+        self.assertEqual(transport_1.state, "completed")
+        self.assertEqual(transport_2.state, "completed")
+
+        # close one side
+        await transport_1.stop()
+        self.assertEqual(transport_1.state, "closed")
+
+        # wait for consent to expire
+        await asyncio.sleep(2)
+
+        # close other side
+        await transport_2.stop()
+        self.assertEqual(transport_2.state, "closed")
+
+    @asynctest
     async def test_connect_when_closed(self):
         gatherer = RTCIceGatherer()
         transport = RTCIceTransport(gatherer)
 
         # stop transport
         await transport.stop()
         self.assertEqual(transport.state, "closed")
```

### Comparing `aiortc-1.7.0/tests/test_rtcpeerconnection.py` & `aiortc-1.8.0/tests/test_rtcpeerconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,19 @@
         transport = transceivers[0].receiver.transport
         for i in range(1, len(transceivers)):
             self.assertEqual(transceivers[i].receiver.transport, transport)
             self.assertEqual(transceivers[i].sender.transport, transport)
         if pc.sctp:
             self.assertEqual(pc.sctp.transport, transport)
 
+    def assertClosed(self, pc):
+        self.assertEqual(pc.connectionState, "closed")
+        self.assertEqual(pc.iceConnectionState, "closed")
+        self.assertEqual(pc.signalingState, "closed")
+
     async def assertDataChannelOpen(self, dc):
         await self.sleepWhile(lambda: dc.readyState == "connecting")
         self.assertEqual(dc.readyState, "open")
 
     async def assertIceChecking(self, pc):
         await self.sleepWhile(lambda: pc.iceConnectionState == "new")
         self.assertEqual(pc.iceConnectionState, "checking")
@@ -549,29 +554,23 @@
         total = 0.0
         while f() and total < max_sleep:
             await asyncio.sleep(sleep)
             total += sleep
 
     def setUp(self):
         # save timers
-        self.consent_failures = aioice.ice.CONSENT_FAILURES
-        self.consent_interval = aioice.ice.CONSENT_INTERVAL
         self.retry_max = aioice.stun.RETRY_MAX
         self.retry_rto = aioice.stun.RETRY_RTO
 
         # shorten timers to run tests faster
-        aioice.ice.CONSENT_FAILURES = 1
-        aioice.ice.CONSENT_INTERVAL = 1
         aioice.stun.RETRY_MAX = 1
         aioice.stun.RETRY_RTO = 0.1
 
     def tearDown(self):
         # restore timers
-        aioice.ice.CONSENT_FAILURES = self.consent_failures
-        aioice.ice.CONSENT_INTERVAL = self.consent_interval
         aioice.stun.RETRY_MAX = self.retry_max
         aioice.stun.RETRY_RTO = self.retry_rto
 
     @asynctest
     async def test_addIceCandidate_no_sdpMid_or_sdpMLineIndex(self):
         pc = RTCPeerConnection()
         with self.assertRaises(ValueError) as cm:
@@ -898,16 +897,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1029,16 +1028,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1090,24 +1089,20 @@
 
         # handle answer
         await pc1.setRemoteDescription(pc2.localDescription)
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
-        # close one side
+        # close one side, which causes the other to shutdown
         await pc1.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-
-        # wait for consent to expire
-        await asyncio.sleep(2)
+        await asyncio.sleep(1)
 
-        # close other side
-        await pc2.close()
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1117,20 +1112,18 @@
         )
         self.assertEqual(
             pc1_states["signalingState"],
             ["stable", "have-local-offer", "stable", "closed"],
         )
 
         self.assertEqual(
-            pc2_states["connectionState"],
-            ["new", "connecting", "connected", "failed", "closed"],
+            pc2_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
-            pc2_states["iceConnectionState"],
-            ["new", "checking", "completed", "failed", "closed"],
+            pc2_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
         )
         self.assertEqual(
             pc2_states["iceGatheringState"], ["new", "gathering", "complete"]
         )
         self.assertEqual(
             pc2_states["signalingState"],
             ["stable", "have-remote-offer", "stable", "closed"],
@@ -1245,16 +1238,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1352,16 +1345,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1456,16 +1449,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1561,16 +1554,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1665,16 +1658,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1767,16 +1760,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1870,16 +1863,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -1972,16 +1965,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2072,16 +2065,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2187,16 +2180,16 @@
         if stop_tracks:
             player.audio.stop()
             player.video.stop()
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2298,16 +2291,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2404,16 +2397,16 @@
         await done.wait()
         self.assertEqual(pc1.iceConnectionState, "closed")
         self.assertEqual(pc2.iceConnectionState, "failed")
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(pc1_states["connectionState"], ["new", "closed"])
         self.assertEqual(pc1_states["iceConnectionState"], ["new", "closed"])
         self.assertEqual(
             pc1_states["iceGatheringState"], ["new", "gathering", "complete"]
         )
@@ -2544,16 +2537,16 @@
         # check a single transport is used
         self.assertBundled(pc1)
         self.assertBundled(pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"],
             ["new", "connecting", "connected", "connecting", "connected", "closed"],
         )
         self.assertEqual(
@@ -2685,16 +2678,16 @@
                 "transport",
             ],
         )
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2793,16 +2786,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -2899,16 +2892,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3011,16 +3004,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3120,16 +3113,16 @@
 
         # check outcome
         await self.assertIceCompleted(pc1, pc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3182,16 +3175,16 @@
         await self.assertIceCompleted(pc1, pc2)
         self.assertEqual(dc1.readyState, "closed")
         await self.assertDataChannelOpen(dc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     @asynctest
     async def test_connect_datachannel_negotiated_and_close_immediately(self):
         pc1 = RTCPeerConnection()
         pc2 = RTCPeerConnection()
 
         # create two negotiated data channels
@@ -3215,16 +3208,16 @@
         await self.assertIceCompleted(pc1, pc2)
         self.assertEqual(dc1.readyState, "closed")
         await self.assertDataChannelOpen(dc2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     @asynctest
     async def test_connect_datachannel_legacy_sdp(self):
         pc1 = RTCPeerConnection()
         pc1._sctpLegacySdp = True
         pc1_data_messages = []
         pc1_states = track_states(pc1)
@@ -3354,16 +3347,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3516,16 +3509,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3673,16 +3666,16 @@
 
         # close data channels
         await self.closeDataChannel(dc1)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -3744,16 +3737,16 @@
         dc4 = pc1.createDataChannel("chat4")
         await self.assertDataChannelOpen(dc4)
         self.assertEqual(dc4.id, 3)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
     def test_create_datachannel_with_maxpacketlifetime_and_maxretransmits(self):
         pc = RTCPeerConnection()
         with self.assertRaises(ValueError) as cm:
             pc.createDataChannel("chat", maxPacketLifeTime=500, maxRetransmits=0)
         self.assertEqual(
             str(cm.exception),
@@ -3964,16 +3957,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"],
             ["new", "connecting", "connected", "connecting", "connected", "closed"],
         )
         self.assertEqual(
@@ -4157,16 +4150,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4263,16 +4256,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4369,16 +4362,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4505,16 +4498,16 @@
 
         # close data channel
         await self.closeDataChannel(dc)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
@@ -4934,16 +4927,16 @@
 
         # allow media to flow long enough to collect stats
         await asyncio.sleep(2)
 
         # close
         await pc1.close()
         await pc2.close()
-        self.assertEqual(pc1.iceConnectionState, "closed")
-        self.assertEqual(pc2.iceConnectionState, "closed")
+        self.assertClosed(pc1)
+        self.assertClosed(pc2)
 
         # check state changes
         self.assertEqual(
             pc1_states["connectionState"], ["new", "connecting", "connected", "closed"]
         )
         self.assertEqual(
             pc1_states["iceConnectionState"], ["new", "checking", "completed", "closed"]
```

### Comparing `aiortc-1.7.0/tests/test_rtcrtpreceiver.py` & `aiortc-1.8.0/tests/test_rtcrtpreceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,14 +446,36 @@
             await receiver.receive(RTCRtpReceiveParameters(codecs=[VP8_CODEC]))
 
             # receive RTP with unknown payload type
             packet = RtpPacket(payload_type=123)
             await receiver._handle_rtp_packet(packet, arrival_time_ms=0)
 
     @asynctest
+    async def test_rtp_disabled(self):
+        async with create_receiver("audio") as receiver:
+            self.assertEqual(receiver._enabled, True)
+            receiver._track = RemoteStreamTrack(kind="audio")
+
+            await receiver.receive(RTCRtpReceiveParameters(codecs=[PCMU_CODEC]))
+            receiver._enabled = False
+            self.assertEqual(receiver._enabled, False)
+
+            # receive RTP while disabled.
+            packet = RtpPacket(payload_type=0)
+            await receiver._handle_rtp_packet(packet, arrival_time_ms=0)
+
+            # check stats
+            report = await receiver.getStats()
+            self.assertIsInstance(report, RTCStatsReport)
+            self.assertEqual(
+                sorted([s.type for s in report.values()]),
+                ["transport"],
+            )
+
+    @asynctest
     async def test_rtp_rtx(self):
         async with create_receiver("video") as receiver:
             receiver._track = RemoteStreamTrack(kind="video")
 
             await receiver.receive(
                 RTCRtpReceiveParameters(
                     codecs=[
```

### Comparing `aiortc-1.7.0/tests/test_rtcrtpsender.py` & `aiortc-1.8.0/tests/test_rtcrtpsender.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,14 +386,39 @@
                     break
             self.assertIsNotNone(found_rtx)
             self.assertEqual(found_rtx.payload_type, 101)
             self.assertEqual(found_rtx.ssrc, 2345)
             self.assertEqual(found_rtx.payload[0:2], pack("!H", packet.sequence_number))
 
     @asynctest
+    async def test_disabled(self):
+        async with dummy_dtls_transport_pair() as (local_transport, _):
+            sender = RTCRtpSender(AudioStreamTrack(), local_transport)
+            self.assertEqual(sender.kind, "audio")
+            self.assertEqual(sender._enabled, True)
+
+            await sender.send(RTCRtpParameters(codecs=[PCMU_CODEC]))
+            sender._enabled = False
+            self.assertEqual(sender._enabled, False)
+
+            # check stats
+            report = await sender.getStats()
+            self.assertIsInstance(report, RTCStatsReport)
+            self.assertEqual(
+                sorted([s.type for s in report.values()]),
+                ["outbound-rtp", "transport"],
+            )
+
+            outbound_rtp = report["outbound-rtp_" + str(id(sender))]
+            self.assertEqual(outbound_rtp.packetsSent, 0)
+
+            # clean shutdown
+            await sender.stop()
+
+    @asynctest
     async def test_stop(self):
         async with dummy_dtls_transport_pair() as (local_transport, _):
             sender = RTCRtpSender(AudioStreamTrack(), local_transport)
             self.assertEqual(sender.kind, "audio")
 
             await sender.send(RTCRtpParameters(codecs=[PCMU_CODEC]))
```

### Comparing `aiortc-1.7.0/tests/test_rtcrtptransceiver.py` & `aiortc-1.8.0/tests/test_rtcrtptransceiver.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rtcsctptransport.py` & `aiortc-1.8.0/tests/test_rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rtcsessiondescription.py` & `aiortc-1.8.0/tests/test_rtcsessiondescription.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_rtp.py` & `aiortc-1.8.0/tests/test_rtp.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_sdp.py` & `aiortc-1.8.0/tests/test_sdp.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_utils.py` & `aiortc-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/test_vpx.py` & `aiortc-1.8.0/tests/test_vpx.py`

 * *Files identical despite different names*

### Comparing `aiortc-1.7.0/tests/utils.py` & `aiortc-1.8.0/tests/utils.py`

 * *Files identical despite different names*

