# Comparing `tmp/nestipy_schedule-0.1.0.tar.gz` & `tmp/nestipy_schedule-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_schedule-0.1.0.tar", max compression
+gzip compressed data, was "nestipy_schedule-0.1.1.tar", max compression
```

## Comparing `nestipy_schedule-0.1.0.tar` & `nestipy_schedule-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_schedule-0.1.0/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_schedule-0.1.0/README.md
--rw-r--r--   0        0        0      416 2024-05-28 07:53:33.403457 nestipy_schedule-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      392 2024-05-28 09:49:32.425980 nestipy_schedule-0.1.0/src/nestipy_schedule/__init__.py
--rw-r--r--   0        0        0      265 2024-05-28 08:00:02.314057 nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_builder.py
--rw-r--r--   0        0        0      771 2024-05-28 10:09:20.949926 nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_decorator.py
--rw-r--r--   0        0        0      392 2024-05-28 09:42:38.903215 nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_metadata.py
--rw-r--r--   0        0        0     2873 2024-05-28 10:08:48.337707 nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_module.py
--rw-r--r--   0        0        0     1708 2024-05-28 10:04:17.691898 nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_registry.py
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 nestipy_schedule-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_schedule-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_schedule-0.1.1/README.md
+-rw-r--r--   0        0        0      416 2024-05-30 08:04:14.187544 nestipy_schedule-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      392 2024-05-28 09:49:32.425980 nestipy_schedule-0.1.1/src/nestipy_schedule/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-28 08:00:02.314057 nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_builder.py
+-rw-r--r--   0        0        0      755 2024-05-30 08:03:47.043848 nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_decorator.py
+-rw-r--r--   0        0        0      392 2024-05-28 09:42:38.903215 nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_metadata.py
+-rw-r--r--   0        0        0     2804 2024-05-30 08:03:27.496089 nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_module.py
+-rw-r--r--   0        0        0      564 2024-05-30 08:02:53.904549 nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_registry.py
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 nestipy_schedule-0.1.1/PKG-INFO
```

### Comparing `nestipy_schedule-0.1.0/LICENSE` & `nestipy_schedule-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_schedule-0.1.0/README.md` & `nestipy_schedule-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_decorator.py` & `nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Union, Any, Type
 
 from nestipy.metadata import SetMetadata
 
-from nestipy_schedule.schedule_metadata import ScheduleMetadata, ScheduleData
+from .schedule_metadata import ScheduleMetadata, ScheduleData
 
 
 def Cron(cron: str, timezone: str = None, name: str = None) -> Callable[[Union[Type, Callable[..., Any]]], Any]:
     return SetMetadata(ScheduleMetadata.Schedule, ScheduleData(ScheduleMetadata.Cron, cron, timezone, name))
 
 
 def Interval(seconds: int, timezone: str = None, name: str = None):
```

### Comparing `nestipy_schedule-0.1.0/src/nestipy_schedule/schedule_module.py` & `nestipy_schedule-0.1.1/src/nestipy_schedule/schedule_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 import inspect
 from datetime import datetime, timedelta
 from typing import Annotated
 
 from apscheduler.triggers.cron import CronTrigger
-from apscheduler.triggers.interval import IntervalTrigger
 from apscheduler.triggers.date import DateTrigger
-
+from apscheduler.triggers.interval import IntervalTrigger
 from nestipy.common import Module
 from nestipy.core import DiscoverService
 from nestipy.dynamic_module import NestipyModule
 from nestipy.ioc import Inject
 from nestipy.metadata import Reflect
 
-from .schedule_metadata import ScheduleMetadata, ScheduleData
 from .schedule_builder import ConfigurableModuleClass, ScheduleOption, SCHEDULE_OPTION
+from .schedule_metadata import ScheduleMetadata, ScheduleData
 from .schedule_registry import SchedulerRegistry
 
 
 @Module(
     providers=[SchedulerRegistry],
     exports=[SchedulerRegistry]
 )
 class ScheduleModule(ConfigurableModuleClass, NestipyModule):
     _config: Annotated[ScheduleOption, Inject(SCHEDULE_OPTION)]
     _discovery: Annotated[DiscoverService, Inject()]
     _registry: Annotated[SchedulerRegistry, Inject()]
 
     async def on_startup(self):
         self.setup_all_jobs()
-        self._registry.get_scheduler().start()
+        self._registry.start()
 
     async def on_shutdown(self):
-        self._registry.get_scheduler().shutdown(wait=False)
+        self._registry.shutdown(wait=False)
 
     @classmethod
     def _is_schedule(cls, method: callable):
         return Reflect.get_metadata(method, ScheduleMetadata.Schedule, None) is not None
 
     def add_job(self, method: callable):
         schedule: ScheduleData = Reflect.get_metadata(
             method, ScheduleMetadata.Schedule,
             ScheduleData(ScheduleMetadata.Timeout, 5000)
         )
-        scheduler = self._registry.get_scheduler()
         match schedule.schedule:
             case ScheduleMetadata.Cron:
                 trigger = CronTrigger.from_crontab(schedule.value, timezone=schedule.timezone)
-                return scheduler.add_job(method, trigger=trigger, id=schedule.name)
+                return self._registry.add_job(method, trigger=trigger, id=schedule.name)
             case ScheduleMetadata.Interval:
                 trigger = IntervalTrigger(seconds=schedule.value, timezone=schedule.timezone)
-                return scheduler.add_job(method, trigger=trigger, id=schedule.name)
+                return self._registry.add_job(method, trigger=trigger, id=schedule.name)
             case ScheduleMetadata.Timeout:
                 run_date = datetime.now(tz=schedule.timezone) + timedelta(milliseconds=schedule.value)
                 trigger = DateTrigger(run_date=run_date, timezone=schedule.timezone)
-                return scheduler.add_job(method, trigger=trigger, id=schedule.name)
+                return self._registry.add_job(method, trigger=trigger, id=schedule.name)
 
     def setup_all_jobs(self):
         instances = self._discovery.get_all_controller() + self._discovery.get_all_provider()
         for p in instances:
             elements = inspect.getmembers(p, lambda a: inspect.isfunction(a) or inspect.iscoroutinefunction(a))
             methods = [
                 method for (method, _) in elements
```

### Comparing `nestipy_schedule-0.1.0/PKG-INFO` & `nestipy_schedule-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy-schedule
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy-schedule Version: 0.1.0 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-schedule Version: 0.1.1 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0) Description-Content-Type: text/
 markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
```

