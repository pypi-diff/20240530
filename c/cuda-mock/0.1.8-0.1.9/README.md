# Comparing `tmp/cuda-mock-0.1.8.tar.gz` & `tmp/cuda-mock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cuda-mock-0.1.8.tar", last modified: Mon Apr 29 12:50:34 2024, max compression
+gzip compressed data, was "dist/cuda-mock-0.1.9.tar", last modified: Thu May  9 15:28:21 2024, max compression
```

## Comparing `cuda-mock-0.1.8.tar` & `cuda-mock-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1495 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3919 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/GlobalVarMgr.h
--rw-r--r--   0 root         (0) root         (0)     3118 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/backtrace.h
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/cuda_mock.h
--rw-r--r--   0 root         (0) root         (0)     3205 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/env_util.h
--rw-r--r--   0 root         (0) root         (0)    13039 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/hook.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/logger/
--rw-r--r--   0 root         (0) root         (0)     1899 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/StringRef.h
--rw-r--r--   0 root         (0) root         (0)    16271 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/logger.h
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/logger/logger_stl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/include/profile/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/profile/Timer.h
--rw-r--r--   0 root         (0) root         (0)    24151 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/support.h
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/include/xpu_mock.h
--rw-r--r--   0 root         (0) root         (0)      350 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/ctypes_helper.py
--rw-r--r--   0 root         (0) root         (0)     8620 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/cuda_mock_impl.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/dynamic_obj.py
--rw-r--r--   0 root         (0) root         (0)    19425 2024-04-29 12:42:02.000000 cuda-mock-0.1.8/src/cuda_mock/gpu_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:42:35.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-29 12:50:34.000000 cuda-mock-0.1.8/src/cuda_mock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4082 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3774 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/include/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/GlobalVarMgr.h
+-rw-r--r--   0 root         (0) root         (0)     3144 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/backtrace.h
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/cuda_mock.h
+-rw-r--r--   0 root         (0) root         (0)      266 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/env_mgr.h
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/env_util.h
+-rw-r--r--   0 root         (0) root         (0)    13039 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/hook.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/include/logger/
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/logger/StringRef.h
+-rw-r--r--   0 root         (0) root         (0)    15942 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/logger/logger.h
+-rw-r--r--   0 root         (0) root         (0)      658 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/logger/logger_stl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/include/profile/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/profile/Timer.h
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/support.h
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/include/xpu_mock.h
+-rw-r--r--   0 root         (0) root         (0)      350 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/src/cuda_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/src/cuda_mock/ctypes_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/src/cuda_mock/cuda_mock_impl.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/src/cuda_mock/dynamic_obj.py
+-rw-r--r--   0 root         (0) root         (0)    19425 2024-05-09 15:18:52.000000 cuda-mock-0.1.9/src/cuda_mock/gpu_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4082 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 15:19:30.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-09 15:28:21.000000 cuda-mock-0.1.9/src/cuda_mock.egg-info/top_level.txt
```

### Comparing `cuda-mock-0.1.8/LICENSE` & `cuda-mock-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/PKG-INFO` & `cuda-mock-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.8
+Version: 0.1.9
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -54,18 +54,14 @@
 - 注意要在`import torch`/`import paddle`之后`import cuda_mock; cuda_mock.xpu_initialize()`
 - 使用方法:
 
     ```python
     import paddle
     import cuda_mock; cuda_mock.xpu_initialize() # 加入这一行
     ```
-- 关闭打印backtrace（获取backtrace性能下降比较严重）
-    ```
-    export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'
-    ```
 
 ### 实现自定义hook函数  
 - 实现自定义hook installer例子:
     ```python
     class PythonHookInstaller(cuda_mock.HookInstaller):
         def is_target_lib(self, name):
             return name.find("libcuda_mock_impl.so") != -1
@@ -91,9 +87,9 @@
 - ```export LOG_LEVEL=WARN,TRACE=INFO```
 
 ### 环境变量
 
 | 环境变量 | 用法示例 | 可选值 | 默认值 | 说明 |
 | ------ | ------- | ----- | ----- | ---- |
 | LOG_LEVEL | `export LOG_LEVEL=WARN,TRACE=INFO` | 日志级别有:INFO,WARN,ERROR,FATAL, 日志模块有: PROFILE,TRACE,HOOK,PYTHON,LAST | 全局日志级别默认为WARN,各个日志模块的默认日志级别为INFO | 日志级别, 日志模块级别 |
-| HOOK_DISABLE_TRACE | `export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为1,即所有接口默认关闭backtrace | 是否关闭backtrace |
-| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='cuda_mock.log'` |  文件路径 | - | 是否将日志重定向到文件 |
+| HOOK_ENABLE_TRACE | `export HOOK_ENABLE_TRACE='xpuMemcpy=1,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为0,即所有接口默认关闭backtrace | 是否开启backtrace |
+| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='/tmp/'` |  日志输出文件夹 | - | 是否将日志重定向到文件 |
```

### Comparing `cuda-mock-0.1.8/README.md` & `cuda-mock-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,14 @@
 - 注意要在`import torch`/`import paddle`之后`import cuda_mock; cuda_mock.xpu_initialize()`
 - 使用方法:
 
     ```python
     import paddle
     import cuda_mock; cuda_mock.xpu_initialize() # 加入这一行
     ```
-- 关闭打印backtrace（获取backtrace性能下降比较严重）
-    ```
-    export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'
-    ```
 
 ### 实现自定义hook函数  
 - 实现自定义hook installer例子:
     ```python
     class PythonHookInstaller(cuda_mock.HookInstaller):
         def is_target_lib(self, name):
             return name.find("libcuda_mock_impl.so") != -1
@@ -79,9 +75,9 @@
 - ```export LOG_LEVEL=WARN,TRACE=INFO```
 
 ### 环境变量
 
 | 环境变量 | 用法示例 | 可选值 | 默认值 | 说明 |
 | ------ | ------- | ----- | ----- | ---- |
 | LOG_LEVEL | `export LOG_LEVEL=WARN,TRACE=INFO` | 日志级别有:INFO,WARN,ERROR,FATAL, 日志模块有: PROFILE,TRACE,HOOK,PYTHON,LAST | 全局日志级别默认为WARN,各个日志模块的默认日志级别为INFO | 日志级别, 日志模块级别 |
-| HOOK_DISABLE_TRACE | `export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为1,即所有接口默认关闭backtrace | 是否关闭backtrace |
-| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='cuda_mock.log'` |  文件路径 | - | 是否将日志重定向到文件 |
+| HOOK_ENABLE_TRACE | `export HOOK_ENABLE_TRACE='xpuMemcpy=1,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为0,即所有接口默认关闭backtrace | 是否开启backtrace |
+| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='/tmp/'` |  日志输出文件夹 | - | 是否将日志重定向到文件 |
```

### Comparing `cuda-mock-0.1.8/include/GlobalVarMgr.h` & `cuda-mock-0.1.9/include/GlobalVarMgr.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/backtrace.h` & `cuda-mock-0.1.9/include/backtrace.h`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 #include <functional>
 #include <iosfwd>
 #include <string>
 #include <unordered_map>
 #include <vector>
 
 #include "env_util.h"
+#include "env_mgr.h"
 
-static bool disable_log_backtrace(const char* func) {
+static bool enable_log_backtrace(const char* func) {
     auto ctrl = hook::get_env_value<std::vector<std::pair<std::string, int>>>(
-        "HOOK_DISABLE_TRACE");
+        env_mgr::HOOK_ENABLE_TRACE);
     auto iter = std::find_if(ctrl.begin(), ctrl.end(),
                              [&](auto& pair) { return pair.first == func; });
     if (iter != ctrl.end()) {
         return iter->second;
     }
     return false;
 }
 
 #define IF_ENABLE_LOG_TRACE(func)                                            \
     do {                                                                     \
-        if (!disable_log_backtrace(func)) {                                  \
+        if (enable_log_backtrace(func)) {                                    \
             trace::CallFrames callFrames;                                    \
             callFrames.CollectNative();                                      \
             callFrames.CollectPython();                                      \
             MLOG(TRACE, INFO) << __func__ << " with frame:\n" << callFrames; \
         }                                                                    \
     } while (0)
```

### Comparing `cuda-mock-0.1.8/include/cuda_mock.h` & `cuda-mock-0.1.9/include/cuda_mock.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/env_util.h` & `cuda-mock-0.1.9/include/env_util.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/hook.h` & `cuda-mock-0.1.9/include/hook.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/logger/StringRef.h` & `cuda-mock-0.1.9/include/logger/StringRef.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/logger/logger.h` & `cuda-mock-0.1.9/include/logger/logger.h`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,18 @@
     LogStream(std::shared_ptr<LogConsumer>& logConsumer,
               const std::shared_ptr<LogConfig>& cfg);
     ~LogStream();
 
     void flush();
 
     LogLevel getLevel() const { return level_; }
+    void setLevel(LogLevel level) { level_ = level; }
+    void setModuleLevel(LogModule m, LogLevel level) {
+        module_set_[static_cast<int>(m)] = level;
+    }
 
     bool IsModuleEnable(size_t m, size_t l) {
         return l >= static_cast<size_t>(module_set_[m]);
     }
 
     const char* getStrLevel(LogLevel level) {
         constexpr const char* console_str[] = {
@@ -291,17 +295,15 @@
         LogStream::instance()
             << LogStream::instance().getStrLevel(level) << str
             << LogStream::instance().logHeader()
             << "[TS:" << logger::LogStream::instance().time_duration() << "]";
     }
 
     ~LogWrapper() {
-        if (LOG_CONDITATION(level_)) {
-            LogStream::instance().flush();
-        }
+        LogStream::instance().flush();
         totalDur += std::chrono::high_resolution_clock::now() - st_;
         // crash here
         if (LOGGER_UNLIKELY(level_ == LogLevel::fatal)) {
             LogStream::instance().log_fatal();
         }
     }
     LogLevel level_;
@@ -309,41 +311,27 @@
     static thread_local std::chrono::high_resolution_clock::duration totalDur;
 };
 
 struct MLogWrapper : public LogWrapper {
     explicit MLogWrapper(const char* module, LogLevel level, const char* str)
         : LogWrapper(level, str), module_(module) {}
 
-    ~MLogWrapper() {
-        if (MLOG_CONDITATION(module_, level_)) {
-            LogStream::instance().flush();
-        }
-        totalDur += std::chrono::high_resolution_clock::now() - st_;
-        // crash here
-        if (LOGGER_UNLIKELY(level_ == LogLevel::fatal)) {
-            LogStream::instance().log_fatal();
-        }
-    }
 
     const char* module_;
 };
 
 template <typename T>
 static const LogWrapper& operator<<(const LogWrapper& s, T&& t) {
-    if (LOG_CONDITATION(s.level_)) {
-        LogStream::instance() << std::forward<T>(t);
-    }
+    LogStream::instance() << std::forward<T>(t);
     return s;
 }
 
 template <typename T>
 static const MLogWrapper& operator<<(const MLogWrapper& s, T&& t) {
-    if (MLOG_CONDITATION(s.module_, s.level_)) {
-        LogStream::instance() << std::forward<T>(t);
-    }
+    LogStream::instance() << std::forward<T>(t);
     return s;
 }
 
 class StreamPlaceHolder {};
 
 static void operator<(const StreamPlaceHolder&, const LogWrapper&) {}
 static void operator<(const StreamPlaceHolder&, const MLogWrapper&) {}
```

### Comparing `cuda-mock-0.1.8/include/logger/logger_stl.h` & `cuda-mock-0.1.9/include/logger/logger_stl.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/profile/Timer.h` & `cuda-mock-0.1.9/include/profile/Timer.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/include/support.h` & `cuda-mock-0.1.9/include/support.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/setup.py` & `cuda-mock-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         subprocess.check_call(['cmake', f'{script_dir}'] + cmake_args + ninja_args, cwd=build_dir)
         subprocess.check_call(['cmake', '--build', '.'], cwd=build_dir)
         subprocess.check_call([f'{install_cmd}', 'install'], cwd=build_dir)
 
 setup(
     name="cuda-mock",
-    version="0.1.8",
+    version="0.1.9",
     author="lipracer",
     author_email="lipracer@gmail.com",
     description="a tools hook some api call at runtime",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
     url="https://github.com/lipracer/torch-cuda-mock",
```

### Comparing `cuda-mock-0.1.8/src/cuda_mock/cuda_mock_impl.py` & `cuda-mock-0.1.9/src/cuda_mock/cuda_mock_impl.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/src/cuda_mock/dynamic_obj.py` & `cuda-mock-0.1.9/src/cuda_mock/dynamic_obj.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/src/cuda_mock/gpu_validation.py` & `cuda-mock-0.1.9/src/cuda_mock/gpu_validation.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.8/src/cuda_mock.egg-info/PKG-INFO` & `cuda-mock-0.1.9/src/cuda_mock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuda-mock
-Version: 0.1.8
+Version: 0.1.9
 Summary: mock cuda runtime api
 Home-page: https://github.com/lipracer/torch-cuda-mock
 Author: lipracer
 Author-email: lipracer <lipracer@gmail.com>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -54,18 +54,14 @@
 - 注意要在`import torch`/`import paddle`之后`import cuda_mock; cuda_mock.xpu_initialize()`
 - 使用方法:
 
     ```python
     import paddle
     import cuda_mock; cuda_mock.xpu_initialize() # 加入这一行
     ```
-- 关闭打印backtrace（获取backtrace性能下降比较严重）
-    ```
-    export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'
-    ```
 
 ### 实现自定义hook函数  
 - 实现自定义hook installer例子:
     ```python
     class PythonHookInstaller(cuda_mock.HookInstaller):
         def is_target_lib(self, name):
             return name.find("libcuda_mock_impl.so") != -1
@@ -91,9 +87,9 @@
 - ```export LOG_LEVEL=WARN,TRACE=INFO```
 
 ### 环境变量
 
 | 环境变量 | 用法示例 | 可选值 | 默认值 | 说明 |
 | ------ | ------- | ----- | ----- | ---- |
 | LOG_LEVEL | `export LOG_LEVEL=WARN,TRACE=INFO` | 日志级别有:INFO,WARN,ERROR,FATAL, 日志模块有: PROFILE,TRACE,HOOK,PYTHON,LAST | 全局日志级别默认为WARN,各个日志模块的默认日志级别为INFO | 日志级别, 日志模块级别 |
-| HOOK_DISABLE_TRACE | `export HOOK_DISABLE_TRACE='xpuMemcpy=0,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为1,即所有接口默认关闭backtrace | 是否关闭backtrace |
-| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='cuda_mock.log'` |  文件路径 | - | 是否将日志重定向到文件 |
+| HOOK_ENABLE_TRACE | `export HOOK_ENABLE_TRACE='xpuMemcpy=1,xpuSetDevice=0'`  | xpuMalloc,xpuFree,xpuWait,xpuMemcpy,xpuSetDevice,xpuCurrentDeviceId | 默认所有接口的的值均为0,即所有接口默认关闭backtrace | 是否开启backtrace |
+| LOG_OUTPUT_PATH |  `export LOG_OUTPUT_PATH='/tmp/'` |  日志输出文件夹 | - | 是否将日志重定向到文件 |
```

### Comparing `cuda-mock-0.1.8/src/cuda_mock.egg-info/SOURCES.txt` & `cuda-mock-0.1.9/src/cuda_mock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 include/GlobalVarMgr.h
 include/backtrace.h
 include/cuda_mock.h
+include/env_mgr.h
 include/env_util.h
 include/hook.h
 include/support.h
 include/xpu_mock.h
 include/logger/StringRef.h
 include/logger/logger.h
 include/logger/logger_stl.h
```

