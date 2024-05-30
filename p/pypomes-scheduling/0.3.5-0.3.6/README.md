# Comparing `tmp/pypomes_scheduling-0.3.5.tar.gz` & `tmp/pypomes_scheduling-0.3.6.tar.gz`

## Comparing `pypomes_scheduling-0.3.5.tar` & `pypomes_scheduling-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/README.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pypomes_scheduling-0.3.6/PKG-INFO
```

### Comparing `pypomes_scheduling-0.3.5/src/pypomes_scheduling/__init__.py` & `pypomes_scheduling-0.3.6/src/pypomes_scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.3.5/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.3.6/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,33 +3,37 @@
 import sys
 from datetime import datetime
 from logging import Logger
 from pypomes_core import APP_PREFIX, TIMEZONE_LOCAL, env_get_int, exc_format
 from typing import Final
 from .threaded_scheduler import _ThreadedScheduler
 
-SCHEDULER_RETRY_INTERVAL: Final[int] = env_get_int(f"{APP_PREFIX}_SCHEDULER_RETRY_INTERVAL", 10)
+SCHEDULER_RETRY_INTERVAL: Final[int] = env_get_int(key=f"{APP_PREFIX}_SCHEDULER_RETRY_INTERVAL",
+                                                   def_value=10)
 
 __DEFAULT_BADGE: Final[str] = "__default__"
 
+# ruff: noqa: W605
 __REGEX_VERIFY_CRON: Final[str] = (
     "/(@(annually|yearly|monthly|weekly|daily|hourly|reboot))|"
     "(@every (\d+(ns|us|µs|ms|s|m|h))+)|((((\d+,)+\d+|(\d+(\/|-)\d+)|\d+|\*) ?){5,7})"
 )
 
 # dict holding the schedulers created:
 #   <{ <badge-1>: <scheduler-instance-1>,
 #     ...
 #     <badge-n>: <scheduler-instance-n>
 #   }>
 __schedulers: dict = {}
 
 
-def scheduler_create(errors: list[str] | None, badge: str = __DEFAULT_BADGE,
-                     is_daemon: bool = True, timezone: pytz.BaseTzInfo = TIMEZONE_LOCAL,
+def scheduler_create(errors: list[str] | None,
+                     badge: str = __DEFAULT_BADGE,
+                     is_daemon: bool = True,
+                     timezone: pytz.BaseTzInfo = TIMEZONE_LOCAL,
                      retry_interval: int = SCHEDULER_RETRY_INTERVAL,
                      logger: Logger = None) -> bool:
     """
     Create the threaded job scheduler.
 
     This is a wrapper around the package *APScheduler*.
 
@@ -39,31 +43,37 @@
     :param timezone: the timezone to be used (defaults to the configured local timezone)
     :param retry_interval: interval between retry attempts, in minutes (defaults to the configured value)
     :param logger: optional logger for logging the scheduler's operations
     :return: True if the scheduler was created, or False otherwise
     """
     # inicialize the return variable
     result: bool = False
-    
+
     # has the scheduler been created ?
-    if __get_scheduler(errors, badge, False) is None:
+    if __get_scheduler(errors=errors,
+                       badge=badge,
+                       must_exist=False,
+                       logger=logger) is None:
         # no, create it
         try:
-            __schedulers[badge] = _ThreadedScheduler(timezone, retry_interval, logger)
+            __schedulers[badge] = _ThreadedScheduler(timezone=timezone,
+                                                     retry_interval=retry_interval,
+                                                     logger=logger)
             if is_daemon:
                 __schedulers[badge].daemon = True
             result = True
         except Exception as e:
+            exc_err: str = exc_format(exc=e,
+                                      exc_info=sys.exc_info())
             err_msg: str = (
-                f"Error creating the job scheduler '{badge}': "
-                f"{exc_format(e, sys.exc_info())}"
+                f"Error creating the job scheduler '{badge}': {exc_err}"
             )
             if logger:
-                logger.error(err_msg)
-            if errors is not None:
+                logger.error(msg=err_msg)
+            if isinstance(errors, list):
                 errors.append(err_msg)
 
     return result
 
 
 def scheduler_destroy(badge: str = __DEFAULT_BADGE) -> None:
     """
@@ -77,47 +87,51 @@
     # does the scheduler exist ?
     if scheduler:
         # yes, stop and discard it
         scheduler.stop()
         __schedulers.pop(badge)
 
 
-def scheduler_start(errors: list[str] | None, badge: str = __DEFAULT_BADGE) -> bool:
+def scheduler_start(errors: list[str] | None,
+                    badge: str = __DEFAULT_BADGE) -> bool:
     """
     Start the scheduler.
 
     :param errors: incidental errors
     :param badge: badge identifying the scheduler (defaults to __DEFAULT_BADGE)
     :return: True if the scheduler has been started, or False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # retrieve the scheduler
-    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
+    scheduler: _ThreadedScheduler = __get_scheduler(errors=errors,
+                                                    badge=badge)
 
     # proceed, if the scheduler was retrieved
     if scheduler:
         try:
             scheduler.start()
             result = True
         except Exception as e:
+            exc_err: str = exc_format(exc=e,
+                                      exc_info=sys.exc_info())
             err_msg: str = (
-                f"Error starting the scheduler '{badge}': "
-                f"{exc_format(e, sys.exc_info())}"
+                f"Error starting the scheduler '{badge}': {exc_err}"
             )
             if scheduler.logger:
-                scheduler.logger.error(err_msg)
-            if errors is not None:
+                scheduler.logger.error(msg=err_msg)
+            if isinstance(errors, list):
                 errors.append(err_msg)
 
     return result
 
 
-def scheduler_stop(errors: list[str], badge: str = __DEFAULT_BADGE) -> bool:
+def scheduler_stop(errors: list[str],
+                   badge: str = __DEFAULT_BADGE) -> bool:
     """
     Stop the scheduler.
 
     :param errors: incidental errors
     :param badge: badge identifying the scheduler (defaults to __DEFAULT_BADGE)
     :return: True if the scheduler has been stopped, or False otherwise
     """
@@ -131,18 +145,24 @@
     if scheduler:
         scheduler.stop()
         result = True
 
     return result
 
 
-def scheduler_add_job(errors: list[str] | None, job: callable, job_id: str, job_name: str,
-                      job_cron: str = None, job_start: datetime = None,
-                      job_args: tuple = None, job_kwargs: dict = None,
-                      badge: str = __DEFAULT_BADGE, logger: Logger = None) -> bool:
+def scheduler_add_job(errors: list[str] | None,
+                      job: callable,
+                      job_id: str,
+                      job_name: str,
+                      job_cron: str = None,
+                      job_start: datetime = None,
+                      job_args: tuple = None,
+                      job_kwargs: dict = None,
+                      badge: str = __DEFAULT_BADGE,
+                      logger: Logger = None) -> bool:
     """
     Schedule the job identified as *job_id* and named as *job_name*.
 
     The scheduling is performed with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
     Positional arguments for the scheduled job may be provided in *job_args*.
     Named arguments for the scheduled job may be provided in *job_kwargs*.
     Return *True* if the scheduling was successful.
@@ -157,30 +177,39 @@
     :param job_kwargs: the named arguments for the scheduled job
     :param badge: badge identifying the scheduler (defaults to __DEFAULT_BADGE)
     :param logger: optional logger
     :return: True if the job was successfully scheduled, or False otherwise
     """
     # initialize the return variable
     result: bool = False
-    
+
     # retrieve the scheduler
-    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
-    
+    scheduler: _ThreadedScheduler = __get_scheduler(errors=errors,
+                                                    badge=badge)
+
     # was the scheduler retrieved ?
     if scheduler:
         # yes, proceed
-        result = __scheduler_add_job(errors, scheduler, job, job_id, job_name,
-                                     job_cron, job_start, job_args, job_kwargs, logger)
-
+        result = __scheduler_add_job(errors=errors,
+                                     scheduler=scheduler,
+                                     job=job,
+                                     job_id=job_id,
+                                     job_name=job_name,
+                                     job_cron=job_cron,
+                                     job_start=job_start,
+                                     job_args=job_args,
+                                     job_kwargs=job_kwargs,
+                                     logger=logger)
     return result
 
 
 def scheduler_add_jobs(errors: list[str] | None,
                        jobs: list[tuple[callable, str, str, str, datetime, tuple, dict]],
-                       badge: str = __DEFAULT_BADGE, logger: Logger = None) -> int:
+                       badge: str = __DEFAULT_BADGE,
+                       logger: Logger = None) -> int:
     r"""
     Schedule the jobs described in *jobs*, starting at the given timestamp.
 
     Each element in the job list is a *tuple* with the following job data items:
         - callable function: the function to be invoked by the scheduler (*callable*)
         - job id: the id of the job to be started (*str*)
         - job name: the name of the job to be started (*str*)
@@ -195,16 +224,17 @@
     :param logger: optional logger
     :return: the number of jobs effectively scheduled
     """
     # initialize the return variable
     result: int = 0
 
     # retrieve the scheduler
-    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
-    
+    scheduler: _ThreadedScheduler = __get_scheduler(errors=errors,
+                                                    badge=badge)
+
     # proceed, if the scheduler was retrieved
     if scheduler:
         # traverse the job list and attempt the scheduling
         for job in jobs:
             # process the required parameters
             job_function: callable = job[0]
             job_id: str = job[1]
@@ -212,47 +242,63 @@
 
             # process the optional arguments
             job_cron: str = job[3] if len(job) > 3 else None
             job_start: datetime = job[4] if len(job) > 4 else None
             job_args: tuple = job[5] if len(job) > 5 else None
             job_kwargs: dict = job[6] if len(job) > 6 else None
             # add to the return valiable, if scheduling was successful
-            if __scheduler_add_job(errors, scheduler, job_function, job_id, job_name,
-                                   job_cron, job_start, job_args, job_kwargs, logger):
+            if __scheduler_add_job(errors=errors,
+                                   scheduler=scheduler,
+                                   job=job_function,
+                                   job_id=job_id,
+                                   job_name=job_name,
+                                   job_cron=job_cron,
+                                   job_start=job_start,
+                                   job_args=job_args,
+                                   job_kwargs=job_kwargs,
+                                   logger=logger):
                 result += 1
 
     return result
 
 
-def __get_scheduler(errors: list[str] | None, badge: str,
-                    must_exist: bool = True, logger: Logger = None) -> _ThreadedScheduler:
+def __get_scheduler(errors: list[str] | None,
+                    badge: str,
+                    must_exist: bool = True,
+                    logger: Logger = None) -> _ThreadedScheduler:
     """
     Retrieve the scheduler identified by *badge*.
 
     :param errors: incidental errors
     :param badge: badge identifying the scheduler
     :param must_exist: True if scheduler must exist
     :param logger: optional logger
     :return: the scheduler retrieved, or None otherwise
     """
     result: _ThreadedScheduler = __schedulers.get(badge)
     if must_exist and result is None:
         err_msg: str = f"Job scheduler '{badge}' has not been created"
         if logger:
-            logger.error(err_msg)
-        if errors is not None:
+            logger.error(msg=err_msg)
+        if isinstance(errors, list):
             errors.append(err_msg)
-        
+
     return result
 
 
-def __scheduler_add_job(errors: list[str], scheduler: _ThreadedScheduler,
-                        job: callable, job_id: str, job_name: str,
-                        job_cron: str = None, job_start: datetime = None,
-                        job_args: tuple = None, job_kwargs: dict = None, logger: Logger = None) -> bool:
+def __scheduler_add_job(errors: list[str],
+                        scheduler: _ThreadedScheduler,
+                        job: callable,
+                        job_id: str,
+                        job_name: str,
+                        job_cron: str = None,
+                        job_start: datetime = None,
+                        job_args: tuple = None,
+                        job_kwargs: dict = None,
+                        logger: Logger = None) -> bool:
     r"""
     Use *scheduler* to schedule the job identified as *job_id* and named as *job_name*.
 
     The scheduling is performed with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
     Positional arguments for the scheduled job may be provided in *job_args*.
     Named arguments for the scheduled job may be provided in *job_kwargs*.
     Return *True* if the scheduling was successful.
@@ -270,27 +316,34 @@
     :return: True if the job was successfully scheduled, or False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     err_msg: str | None = None
     # has a valid CRON expression been provided ?
-    if job_cron and not re.search(__REGEX_VERIFY_CRON, job_cron):
+    if job_cron and not re.search(pattern=__REGEX_VERIFY_CRON,
+                                  string=job_cron):
         # no, report the error
         err_msg = f"Invalid CRON expression: '{job_cron}'"
     else:
         # yes, proceed with the scheduling
         try:
-            scheduler.schedule_job(job, job_id, job_name, job_cron, job_start, job_args, job_kwargs)
+            scheduler.schedule_job(job=job,
+                                   job_id=job_id,
+                                   job_name=job_name,
+                                   job_cron=job_cron,
+                                   job_start=job_start,
+                                   job_args=job_args,
+                                   job_kwargs=job_kwargs)
             result = True
         except Exception as e:
             err_msg = (
                 f"Error scheduling the job '{job_name}', id '{job_id}', "
                 f"with CRON '{job_cron}': {exc_format(e, sys.exc_info())}"
             )
     if err_msg:
         if logger:
-            logger.error(err_msg)
-        if errors is not None:
+            logger.error(msg=err_msg)
+        if isinstance(errors, list):
             errors.append(err_msg)
 
     return result
```

### Comparing `pypomes_scheduling-0.3.5/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.3.6/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 class _ThreadedScheduler(threading.Thread):
     """
     A scalable implementation of *APScheduler*'s *BlockingScheduler*.
 
     This implementation may run as single or multiple instances, each instance on its own thread.
     """
 
-    def __init__(self, timezone: pytz.timezone, retry_interval: int, logger: Logger = None) -> None:
+    def __init__(self,
+                 timezone: pytz.timezone,
+                 retry_interval: int,
+                 logger: Logger = None) -> None:
         """
         Initialize the scheduler.
 
         This is the simplest possible scheduler. It runs on the foreground of its own thread, so when
         *start()* is invoked, the call never returns.
 
         :param timezone: the reference timezone in job timestamps
@@ -29,16 +32,16 @@
         # instance attributes
         self.stopped: bool = False
         self.logger: Logger = logger
         self.scheduler: BlockingScheduler = BlockingScheduler(logging=logger,
                                                               timezone=timezone,
                                                               jobstore_retry_interval=retry_interval)
         if self.logger:
-            self.logger.info("Instanced, with timezone "
-                             f"'{timezone}' and retry interval '{retry_interval}'")
+            self.logger.info(msg=("Instanced, with timezone "
+                                  f"'{timezone}' and retry interval '{retry_interval}'"))
 
     def run(self) -> None:
         """
         Start the scheduler in its own thread.
         """
         # stay in loop until 'stop()' is invoked
         while not self.stopped:
@@ -56,16 +59,22 @@
         """
           Stop the scheduler.
         """
         if self.logger:
             self.logger.info("Stopping...")
         self.stopped = True
 
-    def schedule_job(self, job: callable, job_id: str, job_name: str, job_cron: str = None,
-                     job_start: datetime = None, job_args: tuple = None, job_kwargs: dict = None) -> None:
+    def schedule_job(self,
+                     job: callable,
+                     job_id: str,
+                     job_name: str,
+                     job_cron: str = None,
+                     job_start: datetime = None,
+                     job_args: tuple = None,
+                     job_kwargs: dict = None) -> None:
         """
         Schedule the given *job*, with the given parameters.
 
         The CRON expression syntax is: <min> <hour> <day> <month> <day-of-week>
 
         :param job: the callable object to be scheduled
         :param job_id: the id of the scheduled job
@@ -112,8 +121,8 @@
         self.scheduler.add_job(func=job,
                                trigger=aps_trigger,
                                args=job_args,
                                kwargs=job_kwargs,
                                id=job_id,
                                name=job_name)
         if self.logger:
-            self.logger.info(f"Job '{job_name}' scheduled, with CRON '{job_cron}'")
+            self.logger.info(msg=f"Job '{job_name}' scheduled, with CRON '{job_cron}'")
```

### Comparing `pypomes_scheduling-0.3.5/LICENSE` & `pypomes_scheduling-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.3.5/pyproject.toml` & `pypomes_scheduling-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
-    "pypomes_core>=0.6.8",
+    "pypomes_core>=1.1.1",
     "APScheduler>=3.10.1",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Scheduling"
```

