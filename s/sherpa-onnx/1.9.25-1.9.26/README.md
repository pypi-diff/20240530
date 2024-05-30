# Comparing `tmp/sherpa-onnx-1.9.25.tar.gz` & `tmp/sherpa-onnx-1.9.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.9.25.tar", last modified: Fri May 17 04:16:44 2024, max compression
+gzip compressed data, was "sherpa-onnx-1.9.26.tar", last modified: Thu May 30 10:43:17 2024, max compression
```

## Comparing `sherpa-onnx-1.9.25.tar` & `sherpa-onnx-1.9.26.tar`

### file list

```diff
@@ -1,541 +1,655 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.683219 sherpa-onnx-1.9.25/c-api-examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/add-punctuation-c-api.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.687219 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/c-api-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/audio-tagging-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/decode-file-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/offline-tts-c-api.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/speaker-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/spoken-language-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/c-api-examples/streaming-hlg-decode-file-c-api.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.691219 sherpa-onnx-1.9.25/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/asio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/cargs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/cppjieba.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/espeak-ng-for-piper.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/kaldi-decoder.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/kaldi-native-fbank.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/kaldifst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-aarch64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-arm-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-riscv64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-riscv64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-arm64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-arm64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-universal-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-universal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-osx-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-wasm-simd.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/onnxruntime.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/openfst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/piper-phonemize.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/portaudio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/sherpa-onnx-no-tts.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/sherpa-onnx.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/cmake/websocketpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.691219 sherpa-onnx-1.9.25/sherpa-onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.691219 sherpa-onnx-1.9.25/sherpa-onnx/c-api/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/c-api/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42968 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/c-api/c-api.cc
--rw-r--r--   0 runner    (1001) docker     (127)    46140 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/c-api/c-api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.735219 sherpa-onnx-1.9.25/sherpa-onnx/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa-play.h
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-ced-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-label-file.cc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-label-file.h
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/base64-decode.cc
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/base64-decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat.cc
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat.h
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/cppjieba-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/file-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/file-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/hypothesis.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/hypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/jieba-lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/jieba-lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/log.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/math.h
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/microphone.h
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ced-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ced-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-nemo-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-nemo-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-character-frontend.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-character-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-conformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-conformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lstm-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lstm-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-client.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/onnx-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/onnx-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/parse-options.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/parse-options.h
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/provider.cc
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/provider.h
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/resample.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/resample.h
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/session.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/session.h
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice.h
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack.cc
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack.h
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/symbol-table.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/symbol-table.h
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/tee-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/text-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/text-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/transducer-keyword-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/transducer-keyword-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose.cc
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind.cc
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/utfcpp-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-reader.cc
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-reader.h
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.735219 sherpa-onnx-1.9.25/sherpa-onnx/jni/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/jni.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14927 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/jni/wave-reader.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.739219 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/AudioTagging.kt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/FeatureConfig.kt
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/KeywordSpotter.kt
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflinePunctuation.kt
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflineRecognizer.kt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflineStream.kt
--rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OnlineRecognizer.kt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OnlineStream.kt
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/Speaker.kt
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/Vad.kt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/WaveReader.kt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.739219 sherpa-onnx-1.9.25/sherpa-onnx/python/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/display.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/faked-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/sherpa-onnx.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_feature_extractor_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_keyword_spotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_offline_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_online_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_online_transducer_model_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7132 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_speaker_recognition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-05-17 04:06:28.000000 sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_text2token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:44.751219 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 04:16:44.000000 sherpa-onnx-1.9.25/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.262479 sherpa-onnx-1.9.26/
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 10:43:17.262479 sherpa-onnx-1.9.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.178478 sherpa-onnx-1.9.26/c-api-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/add-punctuation-c-api.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.178478 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/c-api-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/audio-tagging-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/decode-file-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/offline-tts-c-api.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/speaker-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/spoken-language-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/c-api-examples/streaming-hlg-decode-file-c-api.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.186478 sherpa-onnx-1.9.26/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/asio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/cargs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/cppjieba.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/espeak-ng-for-piper.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/kaldi-decoder.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/kaldi-native-fbank.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/kaldifst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-aarch64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-arm-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-riscv64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-riscv64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-arm64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-arm64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-universal-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-universal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-osx-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-wasm-simd.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-arm64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/onnxruntime.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/openfst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/piper-phonemize.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/portaudio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/sherpa-onnx-no-tts.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/sherpa-onnx.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/simple-sentencepiece.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/cmake/websocketpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:43:17.262479 sherpa-onnx-1.9.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.186478 sherpa-onnx-1.9.26/sherpa-onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.186478 sherpa-onnx-1.9.26/sherpa-onnx/c-api/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/c-api/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44282 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/c-api/c-api.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    47132 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/c-api/c-api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.230478 sherpa-onnx-1.9.26/sherpa-onnx/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa-play.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-ced-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-label-file.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-label-file.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/base64-decode.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/base64-decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/cppjieba-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/file-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/file-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/hypothesis.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/hypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/jieba-lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/jieba-lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/log.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/math.h
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/microphone.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ced-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ced-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-character-frontend.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-character-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-conformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-conformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lstm-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lstm-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15241 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-transducer-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-nemo-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-nemo-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-client.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/onnx-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/onnx-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/parse-options.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/parse-options.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/provider.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/provider.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/resample.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/resample.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/session.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/session.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/symbol-table.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/symbol-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/tee-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/text-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/text-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/text2token-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/transducer-keyword-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/transducer-keyword-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind.h
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/utfcpp-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/analysis_options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/assets/streaming-asr.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/assets/vad.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/info.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/main.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/speaker_identification_test.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/streaming_asr.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/streaming_transducer_asr_test.dart
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/utils.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/vad.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/lib/vad_test.dart
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/flutter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/flutter/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/my_application.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/linux/my_application.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Flutter/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Flutter/Flutter-Debug.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Flutter/Flutter-Release.xcconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.234478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/AppDelegate.swift
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.174478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)   102994 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_1024.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36406 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Assets.xcassets/AppIcon.appiconset/app_icon_64.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Base.lproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    23729 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Base.lproj/MainMenu.xib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Configs/AppInfo.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Configs/Debug.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Configs/Release.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Configs/Warnings.xcconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/DebugProfile.entitlements
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Info.plist
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/MainFlutterWindow.swift
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner/Release.entitlements
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    32905 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.174478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/project.xcworkspace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.174478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/xcshareddata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcodeproj/xcshareddata/xcschemes/Runner.xcscheme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/Runner.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/RunnerTests/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/macos/RunnerTests/RunnerTests.swift
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/pubspec.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.238478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/flutter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/flutter/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/Runner.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/flutter_window.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/flutter_window.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/resource.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/resources/app_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/runner.exe.manifest
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/win32_window.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/example/windows/runner/win32_window.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/sherpa_onnx.dart
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/online_recognizer.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/online_stream.dart
+-rw-r--r--   0 runner    (1001) docker     (127)    30774 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/sherpa_onnx_bindings.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/speaker_identification.dart
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/vad.dart
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/wave_reader.dart
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/lib/src/wave_writer.dart
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/linux/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/macos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/macos/sherpa_onnx.podspec
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/pubspec.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.242478 sherpa-onnx-1.9.26/sherpa-onnx/flutter/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/flutter/windows/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.246478 sherpa-onnx-1.9.26/sherpa-onnx/jni/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/jni.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15425 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/jni/wave-writer.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.246478 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/AudioTagging.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/FeatureConfig.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/KeywordSpotter.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflinePunctuation.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflineRecognizer.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflineStream.kt
+-rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OnlineRecognizer.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OnlineStream.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/Speaker.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/Vad.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/WaveReader.kt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.246478 sherpa-onnx-1.9.26/sherpa-onnx/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.258478 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/display.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/faked-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/sherpa-onnx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.258478 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25330 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.262479 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_feature_extractor_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_keyword_spotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_offline_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_online_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_online_transducer_model_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_speaker_recognition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-05-30 10:33:12.000000 sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_text2token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:43:17.262479 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27041 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 10:43:17.000000 sherpa-onnx-1.9.26/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.9.25/CMakeLists.txt` & `sherpa-onnx-1.9.26/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 cmake_minimum_required(VERSION 3.13 FATAL_ERROR)
+
+set(CMAKE_OSX_DEPLOYMENT_TARGET "10.14" CACHE STRING "Minimum OS X deployment version. Used only for macOS")
+
 project(sherpa-onnx)
 
-set(SHERPA_ONNX_VERSION "1.9.25")
+set(SHERPA_ONNX_VERSION "1.9.26")
 
 # Disable warning about
 #
 # "The DOWNLOAD_EXTRACT_TIMESTAMP option was not given and policy CMP0135 is
 #  not set.
 if (CMAKE_VERSION VERSION_GREATER_EQUAL "3.24.0")
   cmake_policy(SET CMP0135 NEW)
@@ -230,14 +233,15 @@
     message(STATUS "Link libstdc++ dynamically")
   endif()
 endif()
 
 include(kaldi-native-fbank)
 include(kaldi-decoder)
 include(onnxruntime)
+include(simple-sentencepiece)
 set(ONNXRUNTIME_DIR ${onnxruntime_SOURCE_DIR})
 message(STATUS "ONNXRUNTIME_DIR: ${ONNXRUNTIME_DIR}")
 
 if(SHERPA_ONNX_ENABLE_PORTAUDIO)
   include(portaudio)
 endif()
```

### Comparing `sherpa-onnx-1.9.25/LICENSE` & `sherpa-onnx-1.9.26/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/PKG-INFO` & `sherpa-onnx-1.9.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.9.25
+Version: 1.9.26
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.9.25/README.md` & `sherpa-onnx-1.9.26/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/CMakeLists.txt` & `sherpa-onnx-1.9.26/c-api-examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/README.md` & `sherpa-onnx-1.9.26/c-api-examples/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/add-punctuation-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/add-punctuation-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/alsa.cc` & `sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/alsa.h` & `sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/asr-microphone-example/c-api-alsa.cc` & `sherpa-onnx-1.9.26/c-api-examples/asr-microphone-example/c-api-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/audio-tagging-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/audio-tagging-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/decode-file-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/offline-tts-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/offline-tts-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/run.sh` & `sherpa-onnx-1.9.26/c-api-examples/run.sh`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/speaker-identification-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/speaker-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/spoken-language-identification-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/spoken-language-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/c-api-examples/streaming-hlg-decode-file-c-api.c` & `sherpa-onnx-1.9.26/c-api-examples/streaming-hlg-decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/asio.cmake` & `sherpa-onnx-1.9.26/cmake/asio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/cargs.cmake` & `sherpa-onnx-1.9.26/cmake/cargs.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/cmake_extension.py` & `sherpa-onnx-1.9.26/cmake/cmake_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
     if is_windows():
         binaries += [
             "espeak-ng.dll",
             "kaldi-decoder-core.dll",
             "kaldi-native-fbank-core.dll",
             "onnxruntime.dll",
+            "ssentencepiece_core.dll",
             "piper_phonemize.dll",
             "sherpa-onnx-c-api.dll",
             "sherpa-onnx-core.dll",
             "sherpa-onnx-fstfar.lib",
             "sherpa-onnx-fst.lib",
             "sherpa-onnx-kaldifst-core.lib",
             "sherpa-onnx-portaudio.dll",
```

### Comparing `sherpa-onnx-1.9.25/cmake/cppjieba.cmake` & `sherpa-onnx-1.9.26/cmake/cppjieba.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/eigen.cmake` & `sherpa-onnx-1.9.26/cmake/eigen.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/espeak-ng-for-piper.cmake` & `sherpa-onnx-1.9.26/cmake/espeak-ng-for-piper.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/googletest.cmake` & `sherpa-onnx-1.9.26/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/kaldi-decoder.cmake` & `sherpa-onnx-1.9.26/cmake/kaldi-decoder.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/kaldi-native-fbank.cmake` & `sherpa-onnx-1.9.26/cmake/kaldi-native-fbank.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/kaldifst.cmake` & `sherpa-onnx-1.9.26/cmake/kaldifst.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-aarch64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-aarch64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-aarch64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-arm-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-arm-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-arm.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-arm.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-riscv64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-riscv64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-riscv64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-riscv64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64-gpu.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-linux-x86_64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-linux-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-arm64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-arm64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-arm64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-arm64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-universal-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-universal-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-universal.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-universal.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-x86_64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-osx-x86_64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-osx-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-wasm-simd.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-wasm-simd.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-gpu.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-static-debug.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x64.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86-static-debug.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86-static.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime-win-x86.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime-win-x86.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/onnxruntime.cmake` & `sherpa-onnx-1.9.26/cmake/onnxruntime.cmake`

 * *Files 5% similar despite different names*

```diff
@@ -83,17 +83,22 @@
           message(FATAL_ERROR "Support only CMAKE_BUILD_TYPE being Release, Debug, RelWithDebInfo, or MinSizeRel. Given: ${CMAKE_BUILD_TYPE}")
         endif()
       endif()
 
       if(SHERPA_ONNX_ENABLE_GPU)
         message(FATAL_ERROR "GPU support for Win32 is not supported!")
       endif()
+    elseif(CMAKE_VS_PLATFORM_NAME STREQUAL ARM64 OR CMAKE_VS_PLATFORM_NAME STREQUAL arm64)
+      # for 64-bit windows (arm64)
+      if(NOT BUILD_SHARED_LIBS)
+        message(FATAL_ERROR "Please pass -DBUILD_SHARED_LIBS=ON to cmake")
+      endif()
+      include(onnxruntime-win-arm64)
     else()
-      # for 64-bit windows
-
+      # for 64-bit windows (x64)
       if(BUILD_SHARED_LIBS)
         message(STATUS "Use dynamic onnxruntime libraries")
         if(SHERPA_ONNX_ENABLE_GPU)
           include(onnxruntime-win-x64-gpu)
         else()
           include(onnxruntime-win-x64)
         endif()
```

### Comparing `sherpa-onnx-1.9.25/cmake/openfst.cmake` & `sherpa-onnx-1.9.26/cmake/openfst.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright (c)  2020  Xiaomi Corporation (author: Fangjun Kuang)
 
 function(download_openfst)
   include(FetchContent)
 
-  set(openfst_URL  "https://github.com/csukuangfj/openfst/archive/refs/tags/sherpa-onnx-2024-04-09.tar.gz")
-  set(openfst_URL2 "https://hub.nuaa.cf/csukuangfj/openfst/archive/refs/tags/sherpa-onnx-2024-04-09.tar.gz")
-  set(openfst_HASH "SHA256=d6bdb1700fa38938807184c69a5abe133e730af80822bb85c8f228768a969b92")
+  set(openfst_URL  "https://github.com/csukuangfj/openfst/archive/refs/tags/sherpa-onnx-2024-05-22-2.tar.gz")
+  set(openfst_URL2 "https://hub.nuaa.cf/csukuangfj/openfst/archive/refs/tags/sherpa-onnx-2024-05-22-2.tar.gz")
+  set(openfst_HASH "SHA256=ec52d32ab46ac884d77c87918155ca9d0cae424095ce3bd7e3cc7eaab8235a39")
 
   # If you don't have access to the Internet,
   # please pre-download it
   set(possible_file_locations
-    $ENV{HOME}/Downloads/openfst-sherpa-onnx-2024-04-09.tar.gz
-    ${CMAKE_SOURCE_DIR}/openfst-sherpa-onnx-2024-04-09.tar.gz
-    ${CMAKE_BINARY_DIR}/openfst-sherpa-onnx-2024-04-09.tar.gz
-    /tmp/openfst-sherpa-onnx-2024-04-09.tar.gz
-    /star-fj/fangjun/download/github/openfst-sherpa-onnx-2024-04-09.tar.gz
+    $ENV{HOME}/Downloads/openfst-sherpa-onnx-2024-05-22-2.tar.gz
+    ${CMAKE_SOURCE_DIR}/openfst-sherpa-onnx-2024-05-22-2.tar.gz
+    ${CMAKE_BINARY_DIR}/openfst-sherpa-onnx-2024-05-22-2.tar.gz
+    /tmp/openfst-sherpa-onnx-2024-05-22-2.tar.gz
+    /star-fj/fangjun/download/github/openfst-sherpa-onnx-2024-05-22-2.tar.gz
   )
 
   foreach(f IN LISTS possible_file_locations)
     if(EXISTS ${f})
       set(openfst_URL  "${f}")
       file(TO_CMAKE_PATH "${openfst_URL}" openfst_URL)
       set(openfst_URL2)
```

### Comparing `sherpa-onnx-1.9.25/cmake/piper-phonemize.cmake` & `sherpa-onnx-1.9.26/cmake/piper-phonemize.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/portaudio.cmake` & `sherpa-onnx-1.9.26/cmake/portaudio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/pybind11.cmake` & `sherpa-onnx-1.9.26/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/cmake/sherpa-onnx-no-tts.pc.in` & `sherpa-onnx-1.9.26/cmake/sherpa-onnx-no-tts.pc.in`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 Version: @SHERPA_ONNX_VERSION@
 Cflags: -I"${includedir}"
 
 # Note: -lcargs is required only for the following file
 # https://github.com/k2-fsa/sherpa-onnx/blob/master/c-api-examples/decode-file-c-api.c
 # We add it here so that users don't need to specify -lcargs when compiling decode-file-c-api.c
-Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fst -lkaldi-native-fbank-core -lonnxruntime -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_WITH_CARGS@ @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
+Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fst -lkaldi-native-fbank-core -lonnxruntime -lssentencepiece_core -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_WITH_CARGS@ @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
```

### Comparing `sherpa-onnx-1.9.25/cmake/sherpa-onnx.pc.in` & `sherpa-onnx-1.9.26/cmake/sherpa-onnx.pc.in`

 * *Files 6% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 Version: @SHERPA_ONNX_VERSION@
 Cflags: -I"${includedir}"
 
 # Note: -lcargs is required only for the following file
 # https://github.com/k2-fsa/sherpa-onnx/blob/master/c-api-examples/decode-file-c-api.c
 # We add it here so that users don't need to specify -lcargs when compiling decode-file-c-api.c
-Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fstfar -lsherpa-onnx-fst -lkaldi-native-fbank-core -lpiper_phonemize -lespeak-ng -lucd -lonnxruntime -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_WITH_CARGS@ @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
+Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fstfar -lsherpa-onnx-fst -lkaldi-native-fbank-core -lpiper_phonemize -lespeak-ng -lucd -lonnxruntime -lssentencepiece_core -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_WITH_CARGS@ @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
```

### Comparing `sherpa-onnx-1.9.25/cmake/websocketpp.cmake` & `sherpa-onnx-1.9.26/cmake/websocketpp.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/setup.py` & `sherpa-onnx-1.9.26/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/c-api/c-api.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/c-api/c-api.cc`

 * *Files 2% similar despite different names*

```diff
@@ -440,32 +440,70 @@
   memset(r, 0, sizeof(SherpaOnnxOfflineRecognizerResult));
 
   char *pText = new char[text.size() + 1];
   std::copy(text.begin(), text.end(), pText);
   pText[text.size()] = 0;
   r->text = pText;
 
-  if (!result.timestamps.empty()) {
-    r->timestamps = new float[result.timestamps.size()];
-    std::copy(result.timestamps.begin(), result.timestamps.end(),
-              r->timestamps);
-    r->count = result.timestamps.size();
+  // copy json
+  const auto &json = result.AsJsonString();
+  char *pJson = new char[json.size() + 1];
+  std::copy(json.begin(), json.end(), pJson);
+  pJson[json.size()] = 0;
+  r->json = pJson;
+
+  // copy tokens
+  auto count = result.tokens.size();
+  if (count > 0) {
+    size_t total_length = 0;
+    for (const auto &token : result.tokens) {
+      // +1 for the null character at the end of each token
+      total_length += token.size() + 1;
+    }
+
+    r->count = count;
+    // Each word ends with nullptr
+    char *tokens = new char[total_length]{};
+    char **tokens_temp = new char *[r->count];
+    int32_t pos = 0;
+    for (int32_t i = 0; i < r->count; ++i) {
+      tokens_temp[i] = tokens + pos;
+      memcpy(tokens + pos, result.tokens[i].c_str(), result.tokens[i].size());
+      // +1 to move past the null character
+      pos += result.tokens[i].size() + 1;
+    }
+    r->tokens_arr = tokens_temp;
+
+    if (!result.timestamps.empty()) {
+      r->timestamps = new float[r->count];
+      std::copy(result.timestamps.begin(), result.timestamps.end(),
+                r->timestamps);
+    } else {
+      r->timestamps = nullptr;
+    }
+
+    r->tokens = tokens;
   } else {
-    r->timestamps = nullptr;
     r->count = 0;
+    r->timestamps = nullptr;
+    r->tokens = nullptr;
+    r->tokens_arr = nullptr;
   }
 
   return r;
 }
 
 void DestroyOfflineRecognizerResult(
     const SherpaOnnxOfflineRecognizerResult *r) {
   if (r) {
     delete[] r->text;
     delete[] r->timestamps;
+    delete[] r->tokens;
+    delete[] r->tokens_arr;
+    delete[] r->json;
     delete r;
   }
 }
 
 const char *GetOfflineStreamResultAsJson(
     const SherpaOnnxOfflineStream *stream) {
   const sherpa_onnx::OfflineRecognitionResult &result =
@@ -557,14 +595,21 @@
 SherpaOnnxOnlineStream *CreateKeywordStream(
     const SherpaOnnxKeywordSpotter *spotter) {
   SherpaOnnxOnlineStream *stream =
       new SherpaOnnxOnlineStream(spotter->impl->CreateStream());
   return stream;
 }
 
+SherpaOnnxOnlineStream *CreateKeywordStreamWithKeywords(
+    const SherpaOnnxKeywordSpotter *spotter, const char *keywords) {
+  SherpaOnnxOnlineStream *stream =
+      new SherpaOnnxOnlineStream(spotter->impl->CreateStream(keywords));
+  return stream;
+}
+
 int32_t IsKeywordStreamReady(SherpaOnnxKeywordSpotter *spotter,
                              SherpaOnnxOnlineStream *stream) {
   return spotter->impl->IsReady(stream->impl.get());
 }
 
 void DecodeKeywordStream(SherpaOnnxKeywordSpotter *spotter,
                          SherpaOnnxOnlineStream *stream) {
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/c-api/c-api.h` & `sherpa-onnx-1.9.26/sherpa-onnx/c-api/c-api.h`

 * *Files 2% similar despite different names*

```diff
@@ -477,15 +477,35 @@
   // Pointer to continuous memory which holds timestamps
   //
   // It is NULL if the model does not support timestamps
   float *timestamps;
 
   // number of entries in timestamps
   int32_t count;
-  // TODO(fangjun): Add more fields
+
+  // Pointer to continuous memory which holds string based tokens
+  // which are separated by \0
+  const char *tokens;
+
+  // a pointer array containing the address of the first item in tokens
+  const char *const *tokens_arr;
+
+  /** Return a json string.
+   *
+   * The returned string contains:
+   *   {
+   *     "text": "The recognition result",
+   *     "tokens": [x, x, x],
+   *     "timestamps": [x, x, x],
+   *     "segment": x,
+   *     "start_time": x,
+   *     "is_final": true|false
+   *   }
+   */
+  const char *json;
 } SherpaOnnxOfflineRecognizerResult;
 
 /// Get the result of the offline stream.
 ///
 /// We assume you have called DecodeOfflineStream() or
 /// DecodeMultipleOfflineStreams() with the given stream before calling
 /// this function.
@@ -579,14 +599,24 @@
 ///
 /// @param spotter A pointer returned by CreateKeywordSpotter()
 /// @return Return a pointer to an OnlineStream. The user has to invoke
 ///         DestroyOnlineStream() to free it to avoid memory leak.
 SHERPA_ONNX_API SherpaOnnxOnlineStream *CreateKeywordStream(
     const SherpaOnnxKeywordSpotter *spotter);
 
+/// Create an online stream for accepting wave samples with the specified hot
+/// words.
+///
+/// @param spotter A pointer returned by CreateKeywordSpotter()
+/// @param keywords A pointer points to the keywords that you set
+/// @return Return a pointer to an OnlineStream. The user has to invoke
+///         DestroyOnlineStream() to free it to avoid memory leak.
+SHERPA_ONNX_API SherpaOnnxOnlineStream *CreateKeywordStreamWithKeywords(
+    const SherpaOnnxKeywordSpotter *spotter, const char *keywords);
+
 /// Return 1 if there are enough number of feature frames for decoding.
 /// Return 0 otherwise.
 ///
 /// @param spotter A pointer returned by CreateKeywordSpotter
 /// @param stream  A pointer returned by CreateKeywordStream
 SHERPA_ONNX_API int32_t IsKeywordStreamReady(SherpaOnnxKeywordSpotter *spotter,
                                              SherpaOnnxOnlineStream *stream);
@@ -609,15 +639,15 @@
 /// @param n  Number of elements in the given streams array.
 SHERPA_ONNX_API void DecodeMultipleKeywordStreams(
     SherpaOnnxKeywordSpotter *spotter, SherpaOnnxOnlineStream **streams,
     int32_t n);
 
 /// Get the decoding results so far for an OnlineStream.
 ///
-/// @param recognizer A pointer returned by CreateKeywordSpotter().
+/// @param spotter A pointer returned by CreateKeywordSpotter().
 /// @param stream A pointer returned by CreateKeywordStream().
 /// @return A pointer containing the result. The user has to invoke
 ///         DestroyKeywordResult() to free the returned pointer to
 ///         avoid memory leak.
 SHERPA_ONNX_API const SherpaOnnxKeywordResult *GetKeywordResult(
     SherpaOnnxKeywordSpotter *spotter, SherpaOnnxOnlineStream *stream);
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
   online-rnn-lm.cc
   online-stream.cc
   online-transducer-decoder.cc
   online-transducer-greedy-search-decoder.cc
   online-transducer-model-config.cc
   online-transducer-model.cc
   online-transducer-modified-beam-search-decoder.cc
+  online-transducer-nemo-model.cc
+  online-transducer-greedy-search-nemo-decoder.cc
   online-wenet-ctc-model-config.cc
   online-wenet-ctc-model.cc
   online-zipformer-transducer-model.cc
   online-zipformer2-ctc-model-config.cc
   online-zipformer2-ctc-model.cc
   online-zipformer2-transducer-model.cc
   onnx-utils.cc
@@ -161,14 +163,15 @@
 if(ANDROID_NDK)
   target_link_libraries(sherpa-onnx-core android log)
 endif()
 
 target_link_libraries(sherpa-onnx-core
   kaldi-native-fbank-core
   kaldi-decoder-core
+  ssentencepiece_core
 )
 
 if(SHERPA_ONNX_ENABLE_GPU)
   target_link_libraries(sherpa-onnx-core
     onnxruntime_providers_cuda
     onnxruntime_providers_shared
   )
@@ -487,14 +490,15 @@
     cat-test.cc
     circular-buffer-test.cc
     context-graph-test.cc
     packed-sequence-test.cc
     pad-sequence-test.cc
     slice-test.cc
     stack-test.cc
+    text2token-test.cc
     transpose-test.cc
     unbind-test.cc
     utfcpp-test.cc
   )
   if(SHERPA_ONNX_ENABLE_TTS)
     list(APPEND sherpa_onnx_test_srcs
       cppjieba-test.cc
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/README.md` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa-play.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa-play.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa-play.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/alsa.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-ced-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-ced-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-label-file.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-label-file.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-label-file.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-label-file.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/audio-tagging.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/audio-tagging.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/base64-decode.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/base64-decode.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/cat.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/cat.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/circular-buffer.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/circular-buffer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/context-graph.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/context-graph.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/cppjieba-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/cppjieba-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/display.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/display.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/endpoint.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/endpoint.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/endpoint.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/features.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/features.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/features.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/file-utils.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/file-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/file-utils.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/file-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/hypothesis.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/hypothesis.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/hypothesis.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/hypothesis.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/jieba-lexicon.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/jieba-lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/jieba-lexicon.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/jieba-lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/keyword-spotter.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/keyword-spotter.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/lexicon.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/lexicon.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/log.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/log.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/log.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/log.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/macros.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/macros.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/math.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/math.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/microphone.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ced-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ced-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ced-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ced-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ct-transformer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ct-transformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-fst-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,16 @@
               static_cast<const float *>(p_log_probs),
               static_cast<const float *>(p_log_probs) + vocab_size)));
       p_log_probs += vocab_size;
 
       if (y != blank_id_ && y != prev_id) {
         r.tokens.push_back(y);
         r.timestamps.push_back(t);
-        prev_id = y;
       }
+      prev_id = y;
     }  // for (int32_t t = 0; ...)
 
     ans.push_back(std::move(r));
   }
   return ans;
 }
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-lm.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-model-config.cc`

 * *Files 18% similar despite different names*

```diff
@@ -31,27 +31,46 @@
                "Specify a provider to use: cpu, cuda, coreml");
 
   po->Register("model-type", &model_type,
                "Specify it to reduce model initialization time. "
                "Valid values are: transducer, paraformer, nemo_ctc, whisper, "
                "tdnn, zipformer2_ctc"
                "All other values lead to loading the model twice.");
+  po->Register("modeling-unit", &modeling_unit,
+               "The modeling unit of the model, commonly used units are bpe, "
+               "cjkchar, cjkchar+bpe, etc. Currently, it is needed only when "
+               "hotwords are provided, we need it to encode the hotwords into "
+               "token sequence.");
+  po->Register("bpe-vocab", &bpe_vocab,
+               "The vocabulary generated by google's sentencepiece program. "
+               "It is a file has two columns, one is the token, the other is "
+               "the log probability, you can get it from the directory where "
+               "your bpe model is generated. Only used when hotwords provided "
+               "and the modeling unit is bpe or cjkchar+bpe");
 }
 
 bool OfflineModelConfig::Validate() const {
   if (num_threads < 1) {
     SHERPA_ONNX_LOGE("num_threads should be > 0. Given %d", num_threads);
     return false;
   }
 
   if (!FileExists(tokens)) {
     SHERPA_ONNX_LOGE("tokens: %s does not exist", tokens.c_str());
     return false;
   }
 
+  if (!modeling_unit.empty() &&
+      (modeling_unit == "bpe" || modeling_unit == "cjkchar+bpe")) {
+    if (!FileExists(bpe_vocab)) {
+      SHERPA_ONNX_LOGE("bpe_vocab: %s does not exist", bpe_vocab.c_str());
+      return false;
+    }
+  }
+
   if (!paraformer.model.empty()) {
     return paraformer.Validate();
   }
 
   if (!nemo_ctc.model.empty()) {
     return nemo_ctc.Validate();
   }
@@ -86,13 +105,15 @@
   os << "tdnn=" << tdnn.ToString() << ", ";
   os << "zipformer_ctc=" << zipformer_ctc.ToString() << ", ";
   os << "wenet_ctc=" << wenet_ctc.ToString() << ", ";
   os << "tokens=\"" << tokens << "\", ";
   os << "num_threads=" << num_threads << ", ";
   os << "debug=" << (debug ? "True" : "False") << ", ";
   os << "provider=\"" << provider << "\", ";
-  os << "model_type=\"" << model_type << "\")";
+  os << "model_type=\"" << model_type << "\", ";
+  os << "modeling_unit=\"" << modeling_unit << "\", ";
+  os << "bpe_vocab=\"" << bpe_vocab << "\")";
 
   return os.str();
 }
 
 }  // namespace sherpa_onnx
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-model-config.h`

 * *Files 19% similar despite different names*

```diff
@@ -37,36 +37,43 @@
   //  - transducer. The given model is from icefall
   //  - paraformer. It is a paraformer model
   //  - nemo_ctc. It is a NeMo CTC model.
   //
   // All other values are invalid and lead to loading the model twice.
   std::string model_type;
 
+  std::string modeling_unit = "cjkchar";
+  std::string bpe_vocab;
+
   OfflineModelConfig() = default;
   OfflineModelConfig(const OfflineTransducerModelConfig &transducer,
                      const OfflineParaformerModelConfig &paraformer,
                      const OfflineNemoEncDecCtcModelConfig &nemo_ctc,
                      const OfflineWhisperModelConfig &whisper,
                      const OfflineTdnnModelConfig &tdnn,
                      const OfflineZipformerCtcModelConfig &zipformer_ctc,
                      const OfflineWenetCtcModelConfig &wenet_ctc,
                      const std::string &tokens, int32_t num_threads, bool debug,
-                     const std::string &provider, const std::string &model_type)
+                     const std::string &provider, const std::string &model_type,
+                     const std::string &modeling_unit,
+                     const std::string &bpe_vocab)
       : transducer(transducer),
         paraformer(paraformer),
         nemo_ctc(nemo_ctc),
         whisper(whisper),
         tdnn(tdnn),
         zipformer_ctc(zipformer_ctc),
         wenet_ctc(wenet_ctc),
         tokens(tokens),
         num_threads(num_threads),
         debug(debug),
         provider(provider),
-        model_type(model_type) {}
+        model_type(model_type),
+        modeling_unit(modeling_unit),
+        bpe_vocab(bpe_vocab) {}
 
   void Register(ParseOptions *po);
   bool Validate() const;
 
   std::string ToString() const;
 };
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-paraformer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-punctuation.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-punctuation.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
           text.append(sym);
         }
       } else {
         // not an ascii
         mergeable = false;
 
         if (i > 0) {
-          const uint8_t *p = reinterpret_cast<const uint8_t *>(
-              sym_table[src.tokens[i - 1]].c_str());
-          if (p[0] < 0x80) {
+          const uint8_t p = reinterpret_cast<const uint8_t *>(
+              sym_table[src.tokens[i - 1]].c_str())[0];
+          if (p < 0x80) {
             // put a space between ascii and non-ascii
             text.append(" ");
           }
         }
         text.append(sym);
       }
     } else {
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #include "sherpa-onnx/csrc/offline-transducer-decoder.h"
 #include "sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h"
 #include "sherpa-onnx/csrc/offline-transducer-model.h"
 #include "sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h"
 #include "sherpa-onnx/csrc/pad-sequence.h"
 #include "sherpa-onnx/csrc/symbol-table.h"
 #include "sherpa-onnx/csrc/utils.h"
+#include "ssentencepiece/csrc/ssentencepiece.h"
 
 namespace sherpa_onnx {
 
 static OfflineRecognitionResult Convert(
     const OfflineTransducerDecoderResult &src, const SymbolTable &sym_table,
     int32_t frame_shift_ms, int32_t subsampling_factor) {
   OfflineRecognitionResult r;
@@ -72,25 +73,31 @@
 class OfflineRecognizerTransducerImpl : public OfflineRecognizerImpl {
  public:
   explicit OfflineRecognizerTransducerImpl(
       const OfflineRecognizerConfig &config)
       : config_(config),
         symbol_table_(config_.model_config.tokens),
         model_(std::make_unique<OfflineTransducerModel>(config_.model_config)) {
-    if (!config_.hotwords_file.empty()) {
-      InitHotwords();
-    }
     if (config_.decoding_method == "greedy_search") {
       decoder_ = std::make_unique<OfflineTransducerGreedySearchDecoder>(
           model_.get(), config_.blank_penalty);
     } else if (config_.decoding_method == "modified_beam_search") {
       if (!config_.lm_config.model.empty()) {
         lm_ = OfflineLM::Create(config.lm_config);
       }
 
+      if (!config_.model_config.bpe_vocab.empty()) {
+        bpe_encoder_ = std::make_unique<ssentencepiece::Ssentencepiece>(
+            config_.model_config.bpe_vocab);
+      }
+
+      if (!config_.hotwords_file.empty()) {
+        InitHotwords();
+      }
+
       decoder_ = std::make_unique<OfflineTransducerModifiedBeamSearchDecoder>(
           model_.get(), lm_.get(), config_.max_active_paths,
           config_.lm_config.scale, config_.blank_penalty);
     } else {
       SHERPA_ONNX_LOGE("Unsupported decoding method: %s",
                        config_.decoding_method.c_str());
       exit(-1);
@@ -108,14 +115,24 @@
       decoder_ = std::make_unique<OfflineTransducerGreedySearchDecoder>(
           model_.get(), config_.blank_penalty);
     } else if (config_.decoding_method == "modified_beam_search") {
       if (!config_.lm_config.model.empty()) {
         lm_ = OfflineLM::Create(mgr, config.lm_config);
       }
 
+      if (!config_.model_config.bpe_vocab.empty()) {
+        auto buf = ReadFile(mgr, config_.model_config.bpe_vocab);
+        std::istringstream iss(std::string(buf.begin(), buf.end()));
+        bpe_encoder_ = std::make_unique<ssentencepiece::Ssentencepiece>(iss);
+      }
+
+      if (!config_.hotwords_file.empty()) {
+        InitHotwords(mgr);
+      }
+
       decoder_ = std::make_unique<OfflineTransducerModifiedBeamSearchDecoder>(
           model_.get(), lm_.get(), config_.max_active_paths,
           config_.lm_config.scale, config_.blank_penalty);
     } else {
       SHERPA_ONNX_LOGE("Unsupported decoding method: %s",
                        config_.decoding_method.c_str());
       exit(-1);
@@ -124,15 +141,16 @@
 #endif
 
   std::unique_ptr<OfflineStream> CreateStream(
       const std::string &hotwords) const override {
     auto hws = std::regex_replace(hotwords, std::regex("/"), "\n");
     std::istringstream is(hws);
     std::vector<std::vector<int32_t>> current;
-    if (!EncodeHotwords(is, symbol_table_, &current)) {
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, symbol_table_,
+                        bpe_encoder_.get(), &current)) {
       SHERPA_ONNX_LOGE("Encode hotwords failed, skipping, hotwords are : %s",
                        hotwords.c_str());
     }
     current.insert(current.end(), hotwords_.begin(), hotwords_.end());
 
     auto context_graph =
         std::make_shared<ContextGraph>(current, config_.hotwords_score);
@@ -203,27 +221,55 @@
     std::ifstream is(config_.hotwords_file);
     if (!is) {
       SHERPA_ONNX_LOGE("Open hotwords file failed: %s",
                        config_.hotwords_file.c_str());
       exit(-1);
     }
 
-    if (!EncodeHotwords(is, symbol_table_, &hotwords_)) {
-      SHERPA_ONNX_LOGE("Encode hotwords failed.");
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, symbol_table_,
+                        bpe_encoder_.get(), &hotwords_)) {
+      SHERPA_ONNX_LOGE(
+          "Failed to encode some hotwords, skip them already, see logs above "
+          "for details.");
+    }
+    hotwords_graph_ =
+        std::make_shared<ContextGraph>(hotwords_, config_.hotwords_score);
+  }
+
+#if __ANDROID_API__ >= 9
+  void InitHotwords(AAssetManager *mgr) {
+    // each line in hotwords_file contains space-separated words
+
+    auto buf = ReadFile(mgr, config_.hotwords_file);
+
+    std::istringstream is(std::string(buf.begin(), buf.end()));
+
+    if (!is) {
+      SHERPA_ONNX_LOGE("Open hotwords file failed: %s",
+                       config_.hotwords_file.c_str());
       exit(-1);
     }
+
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, symbol_table_,
+                        bpe_encoder_.get(), &hotwords_)) {
+      SHERPA_ONNX_LOGE(
+          "Failed to encode some hotwords, skip them already, see logs above "
+          "for details.");
+    }
     hotwords_graph_ =
         std::make_shared<ContextGraph>(hotwords_, config_.hotwords_score);
   }
+#endif
 
  private:
   OfflineRecognizerConfig config_;
   SymbolTable symbol_table_;
   std::vector<std::vector<int32_t>> hotwords_;
   ContextGraphPtr hotwords_graph_;
+  std::unique_ptr<ssentencepiece::Ssentencepiece> bpe_encoder_;
   std::unique_ptr<OfflineTransducerModel> model_;
   std::unique_ptr<OfflineTransducerDecoder> decoder_;
   std::unique_ptr<OfflineLM> lm_;
 };
 
 }  // namespace sherpa_onnx
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer.cc`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,17 @@
                "Note: It is a positive value. "
                "Increasing value will lead to lower deletion at the cost"
                "of higher insertions. "
                "Currently only applicable for transducer models.");
 
   po->Register(
       "hotwords-file", &hotwords_file,
-      "The file containing hotwords, one words/phrases per line, and for each"
-      "phrase the bpe/cjkchar are separated by a space. For example: "
-      "▁HE LL O ▁WORLD"
-      "你 好 世 界");
+      "The file containing hotwords, one words/phrases per line, For example: "
+      "HELLO WORLD"
+      "你好世界");
 
   po->Register("hotwords-score", &hotwords_score,
                "The bonus score for each token in context word/phrase. "
                "Used only when decoding_method is modified_beam_search");
 }
 
 bool OfflineRecognizerConfig::Validate() const {
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-recognizer.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-recognizer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-rnn-lm.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-rnn-lm.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-stream.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tdnn-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tdnn-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-nemo-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-nemo-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-transducer-nemo-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-transducer-nemo-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-character-frontend.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-character-frontend.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-character-frontend.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-character-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-frontend.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts-vits-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts-vits-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-tts.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-tts.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-websocket-server.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-wenet-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-whisper-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-whisper-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/offline-zipformer-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/offline-zipformer-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-conformer-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-conformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-conformer-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-conformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-fst-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lm.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lstm-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lstm-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-lstm-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-lstm-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-model-config.cc`

 * *Files 24% similar despite different names*

```diff
@@ -28,14 +28,27 @@
 
   po->Register("debug", &debug,
                "true to print model information while loading it.");
 
   po->Register("provider", &provider,
                "Specify a provider to use: cpu, cuda, coreml");
 
+  po->Register("modeling-unit", &modeling_unit,
+               "The modeling unit of the model, commonly used units are bpe, "
+               "cjkchar, cjkchar+bpe, etc. Currently, it is needed only when "
+               "hotwords are provided, we need it to encode the hotwords into "
+               "token sequence.");
+
+  po->Register("bpe-vocab", &bpe_vocab,
+               "The vocabulary generated by google's sentencepiece program. "
+               "It is a file has two columns, one is the token, the other is "
+               "the log probability, you can get it from the directory where "
+               "your bpe model is generated. Only used when hotwords provided "
+               "and the modeling unit is bpe or cjkchar+bpe");
+
   po->Register("model-type", &model_type,
                "Specify it to reduce model initialization time. "
                "Valid values are: conformer, lstm, zipformer, zipformer2, "
                "wenet_ctc, nemo_ctc. "
                "All other values lead to loading the model twice.");
 }
 
@@ -46,14 +59,22 @@
   }
 
   if (!FileExists(tokens)) {
     SHERPA_ONNX_LOGE("tokens: '%s' does not exist", tokens.c_str());
     return false;
   }
 
+  if (!modeling_unit.empty() &&
+      (modeling_unit == "bpe" || modeling_unit == "cjkchar+bpe")) {
+    if (!FileExists(bpe_vocab)) {
+      SHERPA_ONNX_LOGE("bpe_vocab: %s does not exist", bpe_vocab.c_str());
+      return false;
+    }
+  }
+
   if (!paraformer.encoder.empty()) {
     return paraformer.Validate();
   }
 
   if (!wenet_ctc.model.empty()) {
     return wenet_ctc.Validate();
   }
@@ -79,13 +100,15 @@
   os << "zipformer2_ctc=" << zipformer2_ctc.ToString() << ", ";
   os << "nemo_ctc=" << nemo_ctc.ToString() << ", ";
   os << "tokens=\"" << tokens << "\", ";
   os << "num_threads=" << num_threads << ", ";
   os << "warm_up=" << warm_up << ", ";
   os << "debug=" << (debug ? "True" : "False") << ", ";
   os << "provider=\"" << provider << "\", ";
-  os << "model_type=\"" << model_type << "\")";
+  os << "model_type=\"" << model_type << "\", ";
+  os << "modeling_unit=\"" << modeling_unit << "\", ";
+  os << "bpe_vocab=\"" << bpe_vocab << "\")";
 
   return os.str();
 }
 
 }  // namespace sherpa_onnx
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-model-config.h`

 * *Files 6% similar despite different names*

```diff
@@ -33,34 +33,45 @@
   //  - zipformer2, zipformer2 transducer or CTC from icefall
   //  - wenet_ctc, wenet CTC model
   //  - nemo_ctc, NeMo CTC model
   //
   // All other values are invalid and lead to loading the model twice.
   std::string model_type;
 
+  // Valid values:
+  //  - cjkchar
+  //  - bpe
+  //  - cjkchar+bpe
+  std::string modeling_unit = "cjkchar";
+  std::string bpe_vocab;
+
   OnlineModelConfig() = default;
   OnlineModelConfig(const OnlineTransducerModelConfig &transducer,
                     const OnlineParaformerModelConfig &paraformer,
                     const OnlineWenetCtcModelConfig &wenet_ctc,
                     const OnlineZipformer2CtcModelConfig &zipformer2_ctc,
                     const OnlineNeMoCtcModelConfig &nemo_ctc,
                     const std::string &tokens, int32_t num_threads,
                     int32_t warm_up, bool debug, const std::string &provider,
-                    const std::string &model_type)
+                    const std::string &model_type,
+                    const std::string &modeling_unit,
+                    const std::string &bpe_vocab)
       : transducer(transducer),
         paraformer(paraformer),
         wenet_ctc(wenet_ctc),
         zipformer2_ctc(zipformer2_ctc),
         nemo_ctc(nemo_ctc),
         tokens(tokens),
         num_threads(num_threads),
         warm_up(warm_up),
         debug(debug),
         provider(provider),
-        model_type(model_type) {}
+        model_type(model_type),
+        modeling_unit(modeling_unit),
+        bpe_vocab(bpe_vocab) {}
 
   void Register(ParseOptions *po);
   bool Validate() const;
 
   std::string ToString() const;
 };
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-nemo-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-nemo-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-paraformer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-ctc-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,17 @@
           text.append(sym);
         }
       } else {
         // not an ascii
         mergeable = false;
 
         if (i > 0) {
-          const uint8_t *p = reinterpret_cast<const uint8_t *>(
-              sym_table[src.tokens[i - 1]].c_str());
-          if (p[0] < 0x80) {
+          const uint8_t p = reinterpret_cast<const uint8_t *>(
+              sym_table[src.tokens[i - 1]].c_str())[0];
+          if (p < 0x80) {
             // put a space between ascii and non-ascii
             text.append(" ");
           }
         }
         text.append(sym);
       }
     } else {
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer-transducer-impl.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #include <regex>  // NOLINT
 #include <sstream>
 #include <string>
 #include <utility>
 #include <vector>
 
 #if __ANDROID_API__ >= 9
-#include <strstream>
-
 #include "android/asset_manager.h"
 #include "android/asset_manager_jni.h"
 #endif
 
 #include "sherpa-onnx/csrc/file-utils.h"
 #include "sherpa-onnx/csrc/macros.h"
 #include "sherpa-onnx/csrc/online-lm.h"
@@ -29,23 +27,22 @@
 #include "sherpa-onnx/csrc/online-transducer-decoder.h"
 #include "sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h"
 #include "sherpa-onnx/csrc/online-transducer-model.h"
 #include "sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h"
 #include "sherpa-onnx/csrc/onnx-utils.h"
 #include "sherpa-onnx/csrc/symbol-table.h"
 #include "sherpa-onnx/csrc/utils.h"
+#include "ssentencepiece/csrc/ssentencepiece.h"
 
 namespace sherpa_onnx {
 
-static OnlineRecognizerResult Convert(const OnlineTransducerDecoderResult &src,
-                                      const SymbolTable &sym_table,
-                                      float frame_shift_ms,
-                                      int32_t subsampling_factor,
-                                      int32_t segment,
-                                      int32_t frames_since_start) {
+OnlineRecognizerResult Convert(const OnlineTransducerDecoderResult &src,
+                               const SymbolTable &sym_table,
+                               float frame_shift_ms, int32_t subsampling_factor,
+                               int32_t segment, int32_t frames_since_start) {
   OnlineRecognizerResult r;
   r.tokens.reserve(src.tokens.size());
   r.timestamps.reserve(src.tokens.size());
 
   for (auto i : src.tokens) {
     auto sym = sym_table[i];
 
@@ -90,14 +87,19 @@
     if (sym_.Contains("<unk>")) {
       unk_id_ = sym_["<unk>"];
     }
 
     model_->SetFeatureDim(config.feat_config.feature_dim);
 
     if (config.decoding_method == "modified_beam_search") {
+      if (!config_.model_config.bpe_vocab.empty()) {
+        bpe_encoder_ = std::make_unique<ssentencepiece::Ssentencepiece>(
+            config_.model_config.bpe_vocab);
+      }
+
       if (!config_.hotwords_file.empty()) {
         InitHotwords();
       }
 
       if (!config_.lm_config.model.empty()) {
         lm_ = OnlineLM::Create(config.lm_config);
       }
@@ -136,14 +138,20 @@
 #if 0
       // TODO(fangjun): Implement it
       if (!config_.lm_config.model.empty()) {
         lm_ = OnlineLM::Create(mgr, config.lm_config);
       }
 #endif
 
+      if (!config_.model_config.bpe_vocab.empty()) {
+        auto buf = ReadFile(mgr, config_.model_config.bpe_vocab);
+        std::istringstream iss(std::string(buf.begin(), buf.end()));
+        bpe_encoder_ = std::make_unique<ssentencepiece::Ssentencepiece>(iss);
+      }
+
       if (!config_.hotwords_file.empty()) {
         InitHotwords(mgr);
       }
 
       decoder_ = std::make_unique<OnlineTransducerModifiedBeamSearchDecoder>(
           model_.get(), lm_.get(), config_.max_active_paths,
           config_.lm_config.scale, unk_id_, config_.blank_penalty,
@@ -170,15 +178,16 @@
   }
 
   std::unique_ptr<OnlineStream> CreateStream(
       const std::string &hotwords) const override {
     auto hws = std::regex_replace(hotwords, std::regex("/"), "\n");
     std::istringstream is(hws);
     std::vector<std::vector<int32_t>> current;
-    if (!EncodeHotwords(is, sym_, &current)) {
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, sym_,
+                        bpe_encoder_.get(), &current)) {
       SHERPA_ONNX_LOGE("Encode hotwords failed, skipping, hotwords are : %s",
                        hotwords.c_str());
     }
     current.insert(current.end(), hotwords_.begin(), hotwords_.end());
     auto context_graph =
         std::make_shared<ContextGraph>(current, config_.hotwords_score);
     auto stream =
@@ -329,14 +338,17 @@
       // result is not empty
       const auto &r = s->GetResult();
       if (!r.tokens.empty() && r.tokens.back() != 0) {
         s->GetCurrentSegment() += 1;
       }
     }
 
+    // reset encoder states
+    s->SetStates(model_->GetEncoderInitStates());
+
     // we keep the decoder_out
     decoder_->UpdateDecoderOut(&s->GetResult());
     Ort::Value decoder_out = std::move(s->GetResult().decoder_out);
 
     auto r = decoder_->GetEmptyResult();
     if (config_.decoding_method == "modified_beam_search" &&
         nullptr != s->GetContextGraph()) {
@@ -359,39 +371,43 @@
     std::ifstream is(config_.hotwords_file);
     if (!is) {
       SHERPA_ONNX_LOGE("Open hotwords file failed: %s",
                        config_.hotwords_file.c_str());
       exit(-1);
     }
 
-    if (!EncodeHotwords(is, sym_, &hotwords_)) {
-      SHERPA_ONNX_LOGE("Encode hotwords failed.");
-      exit(-1);
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, sym_,
+                        bpe_encoder_.get(), &hotwords_)) {
+      SHERPA_ONNX_LOGE(
+          "Failed to encode some hotwords, skip them already, see logs above "
+          "for details.");
     }
     hotwords_graph_ =
         std::make_shared<ContextGraph>(hotwords_, config_.hotwords_score);
   }
 
 #if __ANDROID_API__ >= 9
   void InitHotwords(AAssetManager *mgr) {
     // each line in hotwords_file contains space-separated words
 
     auto buf = ReadFile(mgr, config_.hotwords_file);
 
-    std::istrstream is(buf.data(), buf.size());
+    std::istringstream is(std::string(buf.begin(), buf.end()));
 
     if (!is) {
       SHERPA_ONNX_LOGE("Open hotwords file failed: %s",
                        config_.hotwords_file.c_str());
       exit(-1);
     }
 
-    if (!EncodeHotwords(is, sym_, &hotwords_)) {
-      SHERPA_ONNX_LOGE("Encode hotwords failed.");
-      exit(-1);
+    if (!EncodeHotwords(is, config_.model_config.modeling_unit, sym_,
+                        bpe_encoder_.get(), &hotwords_)) {
+      SHERPA_ONNX_LOGE(
+          "Failed to encode some hotwords, skip them already, see logs above "
+          "for details.");
     }
     hotwords_graph_ =
         std::make_shared<ContextGraph>(hotwords_, config_.hotwords_score);
   }
 #endif
 
   void InitOnlineStream(OnlineStream *stream) const {
@@ -409,14 +425,15 @@
     stream->SetStates(model_->GetEncoderInitStates());
   }
 
  private:
   OnlineRecognizerConfig config_;
   std::vector<std::vector<int32_t>> hotwords_;
   ContextGraphPtr hotwords_graph_;
+  std::unique_ptr<ssentencepiece::Ssentencepiece> bpe_encoder_;
   std::unique_ptr<OnlineTransducerModel> model_;
   std::unique_ptr<OnlineLM> lm_;
   std::unique_ptr<OnlineTransducerDecoder> decoder_;
   SymbolTable sym_;
   Endpoint endpoint_;
   int32_t unk_id_ = -1;
 };
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer.cc`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,15 @@
   oss << " ]";
   return oss.str();
 }
 
 std::string OnlineRecognizerResult::AsJsonString() const {
   std::ostringstream os;
   os << "{ ";
-  os << "\"text\": "
-     << "\"" << text << "\""
-     << ", ";
+  os << "\"text\": " << "\"" << text << "\"" << ", ";
   os << "\"tokens\": " << VecToString(tokens) << ", ";
   os << "\"timestamps\": " << VecToString(timestamps, 2) << ", ";
   os << "\"ys_probs\": " << VecToString(ys_probs, 6) << ", ";
   os << "\"lm_probs\": " << VecToString(lm_probs, 6) << ", ";
   os << "\"context_scores\": " << VecToString(context_scores, 6) << ", ";
   os << "\"segment\": " << segment << ", ";
   os << "\"start_time\": " << std::fixed << std::setprecision(2) << start_time
@@ -85,18 +83,17 @@
                "of higher insertions. "
                "Currently only applicable for transducer models.");
   po->Register("hotwords-score", &hotwords_score,
                "The bonus score for each token in context word/phrase. "
                "Used only when decoding_method is modified_beam_search");
   po->Register(
       "hotwords-file", &hotwords_file,
-      "The file containing hotwords, one words/phrases per line, and for each"
-      "phrase the bpe/cjkchar are separated by a space. For example: "
-      "▁HE LL O ▁WORLD"
-      "你 好 世 界");
+      "The file containing hotwords, one words/phrases per line, For example: "
+      "HELLO WORLD"
+      "你好世界");
   po->Register("decoding-method", &decoding_method,
                "decoding method,"
                "now support greedy_search and modified_beam_search.");
   po->Register("temperature-scale", &temperature_scale,
                "Temperature scale for confidence computation in decoding.");
 }
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-recognizer.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-recognizer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-rnn-lm.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-rnn-lm.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-stream.cc`

 * *Files 9% similar despite different names*

```diff
@@ -86,14 +86,20 @@
 
   void SetStates(std::vector<Ort::Value> states) {
     states_ = std::move(states);
   }
 
   std::vector<Ort::Value> &GetStates() { return states_; }
 
+  void SetNeMoDecoderStates(std::vector<Ort::Value> decoder_states) {
+    decoder_states_ = std::move(decoder_states);
+  }
+
+  std::vector<Ort::Value> &GetNeMoDecoderStates() { return decoder_states_; }
+
   const ContextGraphPtr &GetContextGraph() const { return context_graph_; }
 
   std::vector<float> &GetParaformerFeatCache() {
     return paraformer_feat_cache_;
   }
 
   std::vector<float> &GetParaformerEncoderOutCache() {
@@ -125,14 +131,15 @@
   int32_t segment_ = 0;
   OnlineTransducerDecoderResult result_;
   TransducerKeywordResult prev_keyword_result_;
   TransducerKeywordResult keyword_result_;
   TransducerKeywordResult empty_keyword_result_;
   OnlineCtcDecoderResult ctc_result_;
   std::vector<Ort::Value> states_;  // states for transducer or ctc models
+  std::vector<Ort::Value> decoder_states_;  // states for nemo transducer models
   std::vector<float> paraformer_feat_cache_;
   std::vector<float> paraformer_encoder_out_cache_;
   std::vector<float> paraformer_alpha_cache_;
   OnlineParaformerDecoderResult paraformer_result_;
   std::unique_ptr<kaldi_decoder::FasterDecoder> faster_decoder_;
   int32_t faster_decoder_processed_frames_ = 0;
 };
@@ -214,14 +221,23 @@
   impl_->SetStates(std::move(states));
 }
 
 std::vector<Ort::Value> &OnlineStream::GetStates() {
   return impl_->GetStates();
 }
 
+void OnlineStream::SetNeMoDecoderStates(
+    std::vector<Ort::Value> decoder_states) {
+  return impl_->SetNeMoDecoderStates(std::move(decoder_states));
+}
+
+std::vector<Ort::Value> &OnlineStream::GetNeMoDecoderStates() {
+  return impl_->GetNeMoDecoderStates();
+}
+
 const ContextGraphPtr &OnlineStream::GetContextGraph() const {
   return impl_->GetContextGraph();
 }
 
 void OnlineStream::SetFasterDecoder(
     std::unique_ptr<kaldi_decoder::FasterDecoder> decoder) {
   impl_->SetFasterDecoder(std::move(decoder));
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-stream.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-stream.h`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 
   void SetParaformerResult(const OnlineParaformerDecoderResult &r);
   OnlineParaformerDecoderResult &GetParaformerResult();
 
   void SetStates(std::vector<Ort::Value> states);
   std::vector<Ort::Value> &GetStates();
 
+  void SetNeMoDecoderStates(std::vector<Ort::Value> decoder_states);
+  std::vector<Ort::Value> &GetNeMoDecoderStates();
+
   /**
    * Get the context graph corresponding to this stream.
    *
    * @return Return the context graph for this stream.
    */
   const ContextGraphPtr &GetContextGraph() const;
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-client.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-client.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-websocket-server.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-wenet-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-ctc-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/online-zipformer2-transducer-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/online-zipformer2-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/onnx-utils.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/onnx-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/onnx-utils.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/onnx-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/packed-sequence.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/packed-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/pad-sequence.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/pad-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/parse-options.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/parse-options.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/parse-options.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/parse-options.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-lexicon.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-lexicon.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/piper-phonemize-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/piper-phonemize-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/provider.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/provider.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/provider.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/provider.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/resample.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/resample.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/resample.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/resample.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/session.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/session.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/session.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/session.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-microphone.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-offline.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/silero-vad-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/silero-vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/slice.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/slice.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-extractor.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-extractor.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/speaker-embedding-manager.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/speaker-embedding-manager.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-impl.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/spoken-language-identification.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/spoken-language-identification.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/stack.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/stack.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/symbol-table.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/symbol-table.cc`

 * *Files 12% similar despite different names*

```diff
@@ -34,43 +34,14 @@
 }
 #endif
 
 void SymbolTable::Init(std::istream &is) {
   std::string sym;
   int32_t id;
   while (is >> sym >> id) {
-    if (sym.size() >= 3) {
-      // For BPE-based models, we replace ▁ with a space
-      // Unicode 9601, hex 0x2581, utf8 0xe29681
-      const uint8_t *p = reinterpret_cast<const uint8_t *>(sym.c_str());
-      if (p[0] == 0xe2 && p[1] == 0x96 && p[2] == 0x81) {
-        sym = sym.replace(0, 3, " ");
-      }
-    }
-
-    // for byte-level BPE
-    // id 0 is blank, id 1 is sos/eos, id 2 is unk
-    if (id >= 3 && id <= 258 && sym.size() == 6 && sym[0] == '<' &&
-        sym[1] == '0' && sym[2] == 'x' && sym[5] == '>') {
-      std::ostringstream os;
-      os << std::hex << std::uppercase << (id - 3);
-
-      if (std::string(sym.data() + 3, sym.data() + 5) == os.str()) {
-        uint8_t i = id - 3;
-        sym = std::string(&i, &i + 1);
-      }
-    }
-
-    assert(!sym.empty());
-
-    // for byte bpe, after replacing ▁ with a space, whose ascii is also 0x20,
-    // there is a conflict between the real byte 0x20 and ▁, so we disable
-    // the following check.
-    //
-    // Note: Only id2sym_ matters as we use it to convert ID to symbols.
 #if 0
     // we disable the test here since for some multi-lingual BPE models
     // from NeMo, the same symbol can appear multiple times with different IDs.
     if (sym != " ") {
       assert(sym2id_.count(sym) == 0);
     }
 #endif
@@ -88,16 +59,38 @@
   char sep = ' ';
   for (const auto &p : sym2id_) {
     os << p.first << sep << p.second << "\n";
   }
   return os.str();
 }
 
-const std::string &SymbolTable::operator[](int32_t id) const {
-  return id2sym_.at(id);
+const std::string SymbolTable::operator[](int32_t id) const {
+  std::string sym = id2sym_.at(id);
+  if (sym.size() >= 3) {
+    // For BPE-based models, we replace ▁ with a space
+    // Unicode 9601, hex 0x2581, utf8 0xe29681
+    const uint8_t *p = reinterpret_cast<const uint8_t *>(sym.c_str());
+    if (p[0] == 0xe2 && p[1] == 0x96 && p[2] == 0x81) {
+      sym = sym.replace(0, 3, " ");
+    }
+  }
+
+  // for byte-level BPE
+  // id 0 is blank, id 1 is sos/eos, id 2 is unk
+  if (id >= 3 && id <= 258 && sym.size() == 6 && sym[0] == '<' &&
+      sym[1] == '0' && sym[2] == 'x' && sym[5] == '>') {
+    std::ostringstream os;
+    os << std::hex << std::uppercase << (id - 3);
+
+    if (std::string(sym.data() + 3, sym.data() + 5) == os.str()) {
+      uint8_t i = id - 3;
+      sym = std::string(&i, &i + 1);
+    }
+  }
+  return sym;
 }
 
 int32_t SymbolTable::operator[](const std::string &sym) const {
   return sym2id_.at(sym);
 }
 
 bool SymbolTable::Contains(int32_t id) const { return id2sym_.count(id) != 0; }
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/symbol-table.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/symbol-table.h`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   SymbolTable(AAssetManager *mgr, const std::string &filename);
 #endif
 
   /// Return a string representation of this symbol table
   std::string ToString() const;
 
   /// Return the symbol corresponding to the given ID.
-  const std::string &operator[](int32_t id) const;
+  const std::string operator[](int32_t id) const;
   /// Return the ID corresponding to the given symbol.
   int32_t operator[](const std::string &sym) const;
 
   /// Return true if there is a symbol with the given ID.
   bool Contains(int32_t id) const;
 
   /// Return true if there is a given symbol in the symbol table.
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/tee-stream.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/tee-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/text-utils.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/text-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/text-utils.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/text-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/transducer-keyword-decoder.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/transducer-keyword-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/transducer-keyword-decoder.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/transducer-keyword-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/transpose.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/transpose.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind-test.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/unbind.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/unbind.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/utils.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/utils.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 // sherpa-onnx/csrc/utils.cc
 //
 // Copyright      2023  Xiaomi Corporation
 
 #include "sherpa-onnx/csrc/utils.h"
 
+#include <cassert>
 #include <iostream>
 #include <sstream>
 #include <string>
 #include <utility>
 #include <vector>
 
 #include "sherpa-onnx/csrc/log.h"
 #include "sherpa-onnx/csrc/macros.h"
+#include "sherpa-onnx/csrc/text-utils.h"
 
 namespace sherpa_onnx {
 
-static bool EncodeBase(std::istream &is, const SymbolTable &symbol_table,
+static bool EncodeBase(const std::vector<std::string> &lines,
+                       const SymbolTable &symbol_table,
                        std::vector<std::vector<int32_t>> *ids,
                        std::vector<std::string> *phrases,
                        std::vector<float> *scores,
                        std::vector<float> *thresholds) {
-  SHERPA_ONNX_CHECK(ids != nullptr);
   ids->clear();
 
   std::vector<int32_t> tmp_ids;
   std::vector<float> tmp_scores;
   std::vector<float> tmp_thresholds;
   std::vector<std::string> tmp_phrases;
 
   std::string line;
   std::string word;
   bool has_scores = false;
   bool has_thresholds = false;
   bool has_phrases = false;
+  bool has_oov = false;
 
-  while (std::getline(is, line)) {
+  for (const auto &line : lines) {
     float score = 0;
     float threshold = 0;
     std::string phrase = "";
 
     std::istringstream iss(line);
     while (iss >> word) {
-      if (word.size() >= 3) {
-        // For BPE-based models, we replace ▁ with a space
-        // Unicode 9601, hex 0x2581, utf8 0xe29681
-        const uint8_t *p = reinterpret_cast<const uint8_t *>(word.c_str());
-        if (p[0] == 0xe2 && p[1] == 0x96 && p[2] == 0x81) {
-          word = word.replace(0, 3, " ");
-        }
-      }
       if (symbol_table.Contains(word)) {
         int32_t id = symbol_table[word];
         tmp_ids.push_back(id);
       } else {
         switch (word[0]) {
           case ':':  // boosting score for current keyword
             score = std::stof(word.substr(1));
@@ -67,15 +62,16 @@
             has_phrases = true;
             break;
           default:
             SHERPA_ONNX_LOGE(
                 "Cannot find ID for token %s at line: %s. (Hint: words on "
                 "the same line are separated by spaces)",
                 word.c_str(), line.c_str());
-            return false;
+            has_oov = true;
+            break;
         }
       }
     }
     ids->push_back(std::move(tmp_ids));
     tmp_scores.push_back(score);
     tmp_phrases.push_back(phrase);
     tmp_thresholds.push_back(threshold);
@@ -97,25 +93,105 @@
   if (thresholds != nullptr) {
     if (has_thresholds) {
       thresholds->swap(tmp_thresholds);
     } else {
       thresholds->clear();
     }
   }
-  return true;
+  return !has_oov;
 }
 
-bool EncodeHotwords(std::istream &is, const SymbolTable &symbol_table,
+bool EncodeHotwords(std::istream &is, const std::string &modeling_unit,
+                    const SymbolTable &symbol_table,
+                    const ssentencepiece::Ssentencepiece *bpe_encoder,
                     std::vector<std::vector<int32_t>> *hotwords) {
-  return EncodeBase(is, symbol_table, hotwords, nullptr, nullptr, nullptr);
+  std::vector<std::string> lines;
+  std::string line;
+  std::string word;
+
+  while (std::getline(is, line)) {
+    std::string score;
+    std::string phrase;
+
+    std::ostringstream oss;
+    std::istringstream iss(line);
+    while (iss >> word) {
+      switch (word[0]) {
+        case ':':  // boosting score for current keyword
+          score = word;
+          break;
+        default:
+          if (!score.empty()) {
+            SHERPA_ONNX_LOGE(
+                "Boosting score should be put after the words/phrase, given "
+                "%s.",
+                line.c_str());
+            return false;
+          }
+          oss << " " << word;
+          break;
+      }
+    }
+    phrase = oss.str().substr(1);
+    std::istringstream piss(phrase);
+    oss.clear();
+    oss.str("");
+    while (piss >> word) {
+      if (modeling_unit == "cjkchar") {
+        for (const auto &w : SplitUtf8(word)) {
+          oss << " " << w;
+        }
+      } else if (modeling_unit == "bpe") {
+        std::vector<std::string> bpes;
+        bpe_encoder->Encode(word, &bpes);
+        for (const auto &bpe : bpes) {
+          oss << " " << bpe;
+        }
+      } else {
+        if (modeling_unit != "cjkchar+bpe") {
+          SHERPA_ONNX_LOGE(
+              "modeling_unit should be one of bpe, cjkchar or cjkchar+bpe, "
+              "given "
+              "%s",
+              modeling_unit.c_str());
+          exit(-1);
+        }
+        for (const auto &w : SplitUtf8(word)) {
+          if (isalpha(w[0])) {
+            std::vector<std::string> bpes;
+            bpe_encoder->Encode(w, &bpes);
+            for (const auto &bpe : bpes) {
+              oss << " " << bpe;
+            }
+          } else {
+            oss << " " << w;
+          }
+        }
+      }
+    }
+    std::string encoded_phrase = oss.str().substr(1);
+    oss.clear();
+    oss.str("");
+    oss << encoded_phrase;
+    if (!score.empty()) {
+      oss << " " << score;
+    }
+    lines.push_back(oss.str());
+  }
+  return EncodeBase(lines, symbol_table, hotwords, nullptr, nullptr, nullptr);
 }
 
 bool EncodeKeywords(std::istream &is, const SymbolTable &symbol_table,
                     std::vector<std::vector<int32_t>> *keywords_id,
                     std::vector<std::string> *keywords,
                     std::vector<float> *boost_scores,
                     std::vector<float> *threshold) {
-  return EncodeBase(is, symbol_table, keywords_id, keywords, boost_scores,
+  std::vector<std::string> lines;
+  std::string line;
+  while (std::getline(is, line)) {
+    lines.push_back(line);
+  }
+  return EncodeBase(lines, symbol_table, keywords_id, keywords, boost_scores,
                     threshold);
 }
 
 }  // namespace sherpa_onnx
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/utils.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/utils.h`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #ifndef SHERPA_ONNX_CSRC_UTILS_H_
 #define SHERPA_ONNX_CSRC_UTILS_H_
 
 #include <string>
 #include <vector>
 
 #include "sherpa-onnx/csrc/symbol-table.h"
+#include "ssentencepiece/csrc/ssentencepiece.h"
 
 namespace sherpa_onnx {
 
 /* Encode the hotwords in an input stream to be tokens ids.
  *
  * @param is The input stream, it contains several lines, one hotword for each
  *           line. For each hotword, the tokens (cjkchar or bpe) are separated
@@ -21,15 +22,17 @@
  *                      function returns fasle.
  *
  * @@param hotwords  The encoded ids to be written to.
  *
  * @return  If all the symbols from ``is`` are in the symbol_table, returns true
  *          otherwise returns false.
  */
-bool EncodeHotwords(std::istream &is, const SymbolTable &symbol_table,
+bool EncodeHotwords(std::istream &is, const std::string &modeling_unit,
+                    const SymbolTable &symbol_table,
+                    const ssentencepiece::Ssentencepiece *bpe_encoder_,
                     std::vector<std::vector<int32_t>> *hotwords_id);
 
 /* Encode the keywords in an input stream to be tokens ids.
  *
  * @param is The input stream, it contains several lines, one hotword for each
  *           line. For each hotword, the tokens (cjkchar or bpe) are separated
  *           by spaces, it might contain boosting score (starting with :),
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model-config.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/vad-model.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/voice-activity-detector.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/voice-activity-detector.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-reader.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-reader.cc`

 * *Files 24% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
     if (subchunk1_id != 0x20746d66) {
       SHERPA_ONNX_LOGE("Expected subchunk1_id 0x20746d66. Given: 0x%08x\n",
                        subchunk1_id);
       return false;
     }
 
-    if (subchunk1_size != 16) {  // 16 for PCM
+    // NAudio uses 18
+    // See https://github.com/naudio/NAudio/issues/1132
+    if (subchunk1_size != 16 && subchunk1_size != 18) {  // 16 for PCM
       SHERPA_ONNX_LOGE("Expected subchunk1_size 16. Given: %d\n",
                        subchunk1_size);
       return false;
     }
 
     if (audio_format != 1) {  // 1 for PCM
       SHERPA_ONNX_LOGE("Expected audio_format 1. Given: %d\n", audio_format);
@@ -112,14 +114,38 @@
   }
 
   if (!header.Validate()) {
     *is_ok = false;
     return {};
   }
 
+  if (header.subchunk1_size == 18) {
+    // this is for NAudio. It puts extra bytes after bits_per_sample
+    // See
+    // https://github.com/naudio/NAudio/blob/master/NAudio.Core/Wave/WaveFormats/WaveFormat.cs#L223
+
+    is.seekg(36, std::istream::beg);
+
+    int16_t extra_size = -1;
+    is.read(reinterpret_cast<char *>(&extra_size), sizeof(int16_t));
+    if (extra_size != 0) {
+      SHERPA_ONNX_LOGE(
+          "Extra size should be 0 for wave from NAudio. Current extra size "
+          "%d\n",
+          extra_size);
+      *is_ok = false;
+      return {};
+    }
+
+    is.read(reinterpret_cast<char *>(&header.subchunk2_id),
+            sizeof(header.subchunk2_id));
+    is.read(reinterpret_cast<char *>(&header.subchunk2_size),
+            sizeof(header.subchunk2_size));
+  }
+
   header.SeekToDataChunk(is);
   if (!is) {
     *is_ok = false;
     return {};
   }
 
   *sampling_rate = header.sample_rate;
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-reader.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-reader.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-writer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/csrc/wave-writer.h` & `sherpa-onnx-1.9.26/sherpa-onnx/csrc/wave-writer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/CMakeLists.txt` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   online-recognizer.cc
   online-stream.cc
   speaker-embedding-extractor.cc
   speaker-embedding-manager.cc
   spoken-language-identification.cc
   voice-activity-detector.cc
   wave-reader.cc
+  wave-writer.cc
 )
 
 if(SHERPA_ONNX_ENABLE_TTS)
   list(APPEND sources
     offline-tts.cc
   )
 endif()
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/common.h` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/common.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/jni.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/jni.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/keyword-spotter.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-punctuation.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-recognizer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,26 @@
 
   fid = env->GetFieldID(model_config_cls, "modelType", "Ljava/lang/String;");
   s = (jstring)env->GetObjectField(model_config, fid);
   p = env->GetStringUTFChars(s, nullptr);
   ans.model_config.model_type = p;
   env->ReleaseStringUTFChars(s, p);
 
+  fid = env->GetFieldID(model_config_cls, "modelingUnit", "Ljava/lang/String;");
+  s = (jstring)env->GetObjectField(model_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.model_config.modeling_unit = p;
+  env->ReleaseStringUTFChars(s, p);
+
+  fid = env->GetFieldID(model_config_cls, "bpeVocab", "Ljava/lang/String;");
+  s = (jstring)env->GetObjectField(model_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.model_config.bpe_vocab = p;
+  env->ReleaseStringUTFChars(s, p);
+
   // transducer
   fid = env->GetFieldID(model_config_cls, "transducer",
                         "Lcom/k2fsa/sherpa/onnx/OfflineTransducerModelConfig;");
   jobject transducer_config = env->GetObjectField(model_config, fid);
   jclass transducer_config_cls = env->GetObjectClass(transducer_config);
 
   fid = env->GetFieldID(transducer_config_cls, "encoder", "Ljava/lang/String;");
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/offline-tts.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/online-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/online-recognizer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -191,14 +191,26 @@
 
   fid = env->GetFieldID(model_config_cls, "modelType", "Ljava/lang/String;");
   s = (jstring)env->GetObjectField(model_config, fid);
   p = env->GetStringUTFChars(s, nullptr);
   ans.model_config.model_type = p;
   env->ReleaseStringUTFChars(s, p);
 
+  fid = env->GetFieldID(model_config_cls, "modelingUnit", "Ljava/lang/String;");
+  s = (jstring)env->GetObjectField(model_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.model_config.modeling_unit = p;
+  env->ReleaseStringUTFChars(s, p);
+
+  fid = env->GetFieldID(model_config_cls, "bpeVocab", "Ljava/lang/String;");
+  s = (jstring)env->GetObjectField(model_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.model_config.bpe_vocab = p;
+  env->ReleaseStringUTFChars(s, p);
+
   //---------- rnn lm model config ----------
   fid = env->GetFieldID(cls, "lmConfig",
                         "Lcom/k2fsa/sherpa/onnx/OnlineLMConfig;");
   jobject lm_model_config = env->GetObjectField(config, fid);
   jclass lm_model_config_cls = env->GetObjectClass(lm_model_config);
 
   fid = env->GetFieldID(lm_model_config_cls, "model", "Ljava/lang/String;");
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/online-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/spoken-language-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/voice-activity-detector.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/jni/wave-reader.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/jni/wave-reader.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/AudioTagging.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/AudioTagging.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/KeywordSpotter.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/KeywordSpotter.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflinePunctuation.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflinePunctuation.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflineRecognizer.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflineRecognizer.kt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     var whisper: OfflineWhisperModelConfig = OfflineWhisperModelConfig(),
     var nemo: OfflineNemoEncDecCtcModelConfig = OfflineNemoEncDecCtcModelConfig(),
     var numThreads: Int = 1,
     var debug: Boolean = false,
     var provider: String = "cpu",
     var modelType: String = "",
     var tokens: String,
+    var modelingUnit: String = "",
+    var bpeVocab: String = "",
 )
 
 data class OfflineRecognizerConfig(
     var featConfig: FeatureConfig = FeatureConfig(),
     var modelConfig: OfflineModelConfig,
     // var lmConfig: OfflineLMConfig(), // TODO(fangjun): enable it
     var decodingMethod: String = "greedy_search",
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OfflineStream.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OfflineStream.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OnlineRecognizer.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OnlineRecognizer.kt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     var zipformer2Ctc: OnlineZipformer2CtcModelConfig = OnlineZipformer2CtcModelConfig(),
     var neMoCtc: OnlineNeMoCtcModelConfig = OnlineNeMoCtcModelConfig(),
     var tokens: String,
     var numThreads: Int = 1,
     var debug: Boolean = false,
     var provider: String = "cpu",
     var modelType: String = "",
+    var modelingUnit: String = "",
+    var bpeVocab: String = "",
 )
 
 data class OnlineLMConfig(
     var model: String = "",
     var scale: Float = 0.5f,
 )
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/OnlineStream.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/OnlineStream.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/Speaker.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/Speaker.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/Vad.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/Vad.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/kotlin-api/WaveReader.kt` & `sherpa-onnx-1.9.26/sherpa-onnx/kotlin-api/WaveReader.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/endpoint.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/faked-alsa.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/faked-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/features.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-model-config.cc`

 * *Files 10% similar despite different names*

```diff
@@ -32,34 +32,38 @@
       .def(py::init<const OfflineTransducerModelConfig &,
                     const OfflineParaformerModelConfig &,
                     const OfflineNemoEncDecCtcModelConfig &,
                     const OfflineWhisperModelConfig &,
                     const OfflineTdnnModelConfig &,
                     const OfflineZipformerCtcModelConfig &,
                     const OfflineWenetCtcModelConfig &, const std::string &,
-                    int32_t, bool, const std::string &, const std::string &>(),
+                    int32_t, bool, const std::string &, const std::string &,
+                    const std::string &, const std::string &>(),
            py::arg("transducer") = OfflineTransducerModelConfig(),
            py::arg("paraformer") = OfflineParaformerModelConfig(),
            py::arg("nemo_ctc") = OfflineNemoEncDecCtcModelConfig(),
            py::arg("whisper") = OfflineWhisperModelConfig(),
            py::arg("tdnn") = OfflineTdnnModelConfig(),
            py::arg("zipformer_ctc") = OfflineZipformerCtcModelConfig(),
            py::arg("wenet_ctc") = OfflineWenetCtcModelConfig(),
            py::arg("tokens"), py::arg("num_threads"), py::arg("debug") = false,
-           py::arg("provider") = "cpu", py::arg("model_type") = "")
+           py::arg("provider") = "cpu", py::arg("model_type") = "",
+           py::arg("modeling_unit") = "cjkchar", py::arg("bpe_vocab") = "")
       .def_readwrite("transducer", &PyClass::transducer)
       .def_readwrite("paraformer", &PyClass::paraformer)
       .def_readwrite("nemo_ctc", &PyClass::nemo_ctc)
       .def_readwrite("whisper", &PyClass::whisper)
       .def_readwrite("tdnn", &PyClass::tdnn)
       .def_readwrite("zipformer_ctc", &PyClass::zipformer_ctc)
       .def_readwrite("wenet_ctc", &PyClass::wenet_ctc)
       .def_readwrite("tokens", &PyClass::tokens)
       .def_readwrite("num_threads", &PyClass::num_threads)
       .def_readwrite("debug", &PyClass::debug)
       .def_readwrite("provider", &PyClass::provider)
       .def_readwrite("model_type", &PyClass::model_type)
+      .def_readwrite("modeling_unit", &PyClass::modeling_unit)
+      .def_readwrite("bpe_vocab", &PyClass::bpe_vocab)
       .def("validate", &PyClass::Validate)
       .def("__str__", &PyClass::ToString);
 }
 
 }  // namespace sherpa_onnx
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-tts.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-model-config.cc`

 * *Files 10% similar despite different names*

```diff
@@ -28,31 +28,35 @@
   py::class_<PyClass>(*m, "OnlineModelConfig")
       .def(py::init<const OnlineTransducerModelConfig &,
                     const OnlineParaformerModelConfig &,
                     const OnlineWenetCtcModelConfig &,
                     const OnlineZipformer2CtcModelConfig &,
                     const OnlineNeMoCtcModelConfig &, const std::string &,
                     int32_t, int32_t, bool, const std::string &,
+                    const std::string &, const std::string &,
                     const std::string &>(),
            py::arg("transducer") = OnlineTransducerModelConfig(),
            py::arg("paraformer") = OnlineParaformerModelConfig(),
            py::arg("wenet_ctc") = OnlineWenetCtcModelConfig(),
            py::arg("zipformer2_ctc") = OnlineZipformer2CtcModelConfig(),
            py::arg("nemo_ctc") = OnlineNeMoCtcModelConfig(), py::arg("tokens"),
            py::arg("num_threads"), py::arg("warm_up") = 0,
            py::arg("debug") = false, py::arg("provider") = "cpu",
-           py::arg("model_type") = "")
+           py::arg("model_type") = "", py::arg("modeling_unit") = "",
+           py::arg("bpe_vocab") = "")
       .def_readwrite("transducer", &PyClass::transducer)
       .def_readwrite("paraformer", &PyClass::paraformer)
       .def_readwrite("wenet_ctc", &PyClass::wenet_ctc)
       .def_readwrite("zipformer2_ctc", &PyClass::zipformer2_ctc)
       .def_readwrite("nemo_ctc", &PyClass::nemo_ctc)
       .def_readwrite("tokens", &PyClass::tokens)
       .def_readwrite("num_threads", &PyClass::num_threads)
       .def_readwrite("debug", &PyClass::debug)
       .def_readwrite("provider", &PyClass::provider)
       .def_readwrite("model_type", &PyClass::model_type)
+      .def_readwrite("modeling_unit", &PyClass::modeling_unit)
+      .def_readwrite("bpe_vocab", &PyClass::bpe_vocab)
       .def("validate", &PyClass::Validate)
       .def("__str__", &PyClass::ToString);
 }
 
 }  // namespace sherpa_onnx
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-stream.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/vad-model.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/csrc/wave-writer.cc` & `sherpa-onnx-1.9.26/sherpa-onnx/python/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/__init__.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     write_wave,
 )
 
 from .keyword_spotter import KeywordSpotter
 from .offline_recognizer import OfflineRecognizer
 from .online_recognizer import OnlineRecognizer
 from .utils import text2token
-__version__ = '1.9.25'
+__version__ = '1.9.26'
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/cli.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/cli.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         sample_rate: int = 16000,
         feature_dim: int = 80,
         decoding_method: str = "greedy_search",
         max_active_paths: int = 4,
         hotwords_file: str = "",
         hotwords_score: float = 1.5,
         blank_penalty: float = 0.0,
+        modeling_unit: str = "cjkchar",
+        bpe_vocab: str = "",
         debug: bool = False,
         provider: str = "cpu",
         model_type: str = "transducer",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/offline-transducer/index.html>`_
@@ -87,14 +89,24 @@
             The file containing hotwords, one words/phrases per line, and for each
             phrase the bpe/cjkchar are separated by a space.
           hotwords_score:
             The hotword score of each token for biasing word/phrase. Used only if
             hotwords_file is given with modified_beam_search as decoding method.
           blank_penalty:
             The penalty applied on blank symbol during decoding.
+          modeling_unit:
+            The modeling unit of the model, commonly used units are bpe, cjkchar,
+            cjkchar+bpe, etc. Currently, it is needed only when hotwords are
+            provided, we need it to encode the hotwords into token sequence.
+            and the modeling unit is bpe or cjkchar+bpe.
+          bpe_vocab:
+            The vocabulary generated by google's sentencepiece program.
+            It is a file has two columns, one is the token, the other is
+            the log probability, you can get it from the directory where
+            your bpe model is generated. Only used when hotwords provided
           debug:
             True to show debug messages.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
@@ -103,14 +115,16 @@
                 decoder_filename=decoder,
                 joiner_filename=joiner,
             ),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
+            modeling_unit=modeling_unit,
+            bpe_vocab=bpe_vocab,
             model_type=model_type,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         decoding_method: str = "greedy_search",
         max_active_paths: int = 4,
         hotwords_score: float = 1.5,
         blank_penalty: float = 0.0,
         hotwords_file: str = "",
         provider: str = "cpu",
         model_type: str = "",
+        modeling_unit: str = "cjkchar",
+        bpe_vocab: str = "",
         lm: str = "",
         lm_scale: float = 0.1,
         temperature_scale: float = 2.0,
         debug: bool = False,
     ):
         """
         Please refer to
@@ -132,14 +134,24 @@
             It affects only confidence values, the decoding uses the original
             logits without temperature.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
           model_type:
             Online transducer model type. Valid values are: conformer, lstm,
             zipformer, zipformer2. All other values lead to loading the model twice.
+          modeling_unit:
+            The modeling unit of the model, commonly used units are bpe, cjkchar,
+            cjkchar+bpe, etc. Currently, it is needed only when hotwords are
+            provided, we need it to encode the hotwords into token sequence.
+          bpe_vocab:
+            The vocabulary generated by google's sentencepiece program.
+            It is a file has two columns, one is the token, the other is
+            the log probability, you can get it from the directory where
+            your bpe model is generated. Only used when hotwords provided
+            and the modeling unit is bpe or cjkchar+bpe.
         """
         self = cls.__new__(cls)
         _assert_file_exists(tokens)
         _assert_file_exists(encoder)
         _assert_file_exists(decoder)
         _assert_file_exists(joiner)
 
@@ -153,14 +165,16 @@
 
         model_config = OnlineModelConfig(
             transducer=transducer_config,
             tokens=tokens,
             num_threads=num_threads,
             provider=provider,
             model_type=model_type,
+            modeling_unit=modeling_unit,
+            bpe_vocab=bpe_vocab,
             debug=debug,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
             low_freq=low_freq,
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/CMakeLists.txt` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_feature_extractor_config.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_feature_extractor_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_keyword_spotter.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_offline_recognizer.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_online_recognizer.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_online_transducer_model_config.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_online_transducer_model_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_speaker_recognition.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_speaker_recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             print(f"{model_dir} does not exist - skip it")
             return
         for filename in model_dir.glob("*.onnx"):
             print(filename)
             test_zh_models(filename)
             test_en_and_zh_models(filename)
 
-    def test_3dpeaker_models(self):
+    def _test_3dpeaker_models(self):
         model_dir = Path(d) / "3dspeaker"
         if not model_dir.is_dir():
             print(f"{model_dir} does not exist - skip it")
             return
         for filename in model_dir.glob("*.onnx"):
             print(filename)
             test_en_and_zh_models(filename)
```

### Comparing `sherpa-onnx-1.9.25/sherpa-onnx/python/tests/test_text2token.py` & `sherpa-onnx-1.9.26/sherpa-onnx/python/tests/test_text2token.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.25/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.9.26/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.9.25
+Version: 1.9.26
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

