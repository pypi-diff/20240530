# Comparing `tmp/async-lambda-unstable-0.4.1.tar.gz` & `tmp/async-lambda-unstable-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lambda-unstable-0.4.1.tar", last modified: Fri May 24 15:56:34 2024, max compression
+gzip compressed data, was "async-lambda-unstable-0.4.3.tar", last modified: Thu May 30 12:49:13 2024, max compression
```

## Comparing `async-lambda-unstable-0.4.1.tar` & `async-lambda-unstable-0.4.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.250310 async-lambda-unstable-0.4.1/
--rw-r--r--   0 henryjones   (501) staff       (20)    17863 2024-05-24 15:56:34.250106 async-lambda-unstable-0.4.1/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)    17603 2024-05-24 15:54:30.000000 async-lambda-unstable-0.4.1/README.md
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.247336 async-lambda-unstable-0.4.1/async_lambda/
--rw-r--r--   0 henryjones   (501) staff       (20)      945 2024-05-24 15:44:18.000000 async-lambda-unstable-0.4.1/async_lambda/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     3545 2024-05-24 13:59:50.000000 async-lambda-unstable-0.4.1/async_lambda/build_config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/async_lambda/cli.py
--rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.4.1/async_lambda/client.py
--rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    21760 2024-05-24 15:55:09.000000 async-lambda-unstable-0.4.1/async_lambda/controller.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1206 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/async_lambda/defer.py
--rw-r--r--   0 henryjones   (501) staff       (20)      809 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/async_lambda/env.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.247720 async-lambda-unstable-0.4.1/async_lambda/models/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/models/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     2662 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.1/async_lambda/models/case_insensitive_dict.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.248623 async-lambda-unstable-0.4.1/async_lambda/models/events/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1246 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/api_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/base_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)      519 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/dynamodb_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/managed_sqs_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)       77 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/scheduled_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/models/events/unmanaged_sqs_event.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.248894 async-lambda-unstable-0.4.1/async_lambda/models/mock/
--rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/models/mock/mock_context.py
--rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.4.1/async_lambda/models/mock/mock_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)    19669 2024-05-24 15:12:01.000000 async-lambda-unstable-0.4.1/async_lambda/models/task.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.1/async_lambda/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/async_lambda/util.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-24 15:56:34.249842 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)    17863 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)     1022 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       73 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-05-24 15:56:34.000000 async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/top_level.txt
--rw-r--r--   0 henryjones   (501) staff       (20)      849 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.1/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-05-24 15:56:34.250353 async-lambda-unstable-0.4.1/setup.cfg
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.416205 async-lambda-unstable-0.4.3/
+-rw-r--r--   0 henryjones   (501) staff       (20)    19060 2024-05-30 12:49:13.416017 async-lambda-unstable-0.4.3/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)    18800 2024-05-30 12:42:38.000000 async-lambda-unstable-0.4.3/README.md
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.413627 async-lambda-unstable-0.4.3/async_lambda/
+-rw-r--r--   0 henryjones   (501) staff       (20)      945 2024-05-30 12:43:38.000000 async-lambda-unstable-0.4.3/async_lambda/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     3545 2024-05-24 13:59:50.000000 async-lambda-unstable-0.4.3/async_lambda/build_config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/async_lambda/cli.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.4.3/async_lambda/client.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    21721 2024-05-30 12:42:51.000000 async-lambda-unstable-0.4.3/async_lambda/controller.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1206 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/async_lambda/defer.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      809 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/async_lambda/env.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      936 2024-05-30 11:36:23.000000 async-lambda-unstable-0.4.3/async_lambda/middleware.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.413993 async-lambda-unstable-0.4.3/async_lambda/models/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/models/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     2662 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.3/async_lambda/models/case_insensitive_dict.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.414862 async-lambda-unstable-0.4.3/async_lambda/models/events/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1246 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/api_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/base_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      519 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/dynamodb_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/managed_sqs_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)       77 2024-05-17 12:22:31.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/scheduled_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/models/events/unmanaged_sqs_event.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.415124 async-lambda-unstable-0.4.3/async_lambda/models/mock/
+-rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/models/mock/mock_context.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.4.3/async_lambda/models/mock/mock_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    19905 2024-05-30 12:42:51.000000 async-lambda-unstable-0.4.3/async_lambda/models/task.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.4.3/async_lambda/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/async_lambda/util.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-05-30 12:49:13.415852 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)    19060 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)     1049 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       73 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-05-30 12:49:13.000000 async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/top_level.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)      849 2024-05-15 10:00:59.000000 async-lambda-unstable-0.4.3/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-05-30 12:49:13.416246 async-lambda-unstable-0.4.3/setup.cfg
```

### Comparing `async-lambda-unstable-0.4.1/PKG-INFO` & `async-lambda-unstable-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: async-lambda-unstable
-Version: 0.4.1
-Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
-Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
-Description-Content-Type: text/markdown
-Provides-Extra: local
-
 # async-lambda
 
 `async-lambda` is a framework for creating `AWS Lambda` applications with built
 in support for asynchronous invocation via a SQS Queue. This is useful if you
 have workloads you need to split up into separate execution contexts.
 
 `async-lambda` converts your application into a `Serverless Application Model (SAM)`
@@ -187,32 +179,65 @@
     event.querystring_params # request querystring params
     event.body # request body
     event.headers # This is a case insensitive dict
 ```
 
 # Middleware
 
-Middleware functions can be registered with controllers which will execute before the task code is run.
-These functions can be configured to trigger on specific types of tasks and can modify the `event`.
+Middleware functions can be registered with controllers which will wrap the execution of tasks.
+These functions can be configured to trigger on specific types of tasks and can trigger
+side effects and modify the `event` or `response` objects.
+
+Middleware functions must have the signature `Callable[[BaseEvent, Callable[[BaseEvent], T]], T]`.
+The first argument is the `event`, and the second argument (`call_next`) is a function which will propagate the
+calls down the middleware/task stack. The `call_next` function must be called, and its result in most cases be returned.
+If this is not done then tasks will not run as expected.
+
+**Extreme care should be taken with middleware as a simple mistake can have catastrophic effects.**
+
+- Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
 
-Middleware functions must have the signature `Callable[[BaseEvent], BaseEvent]`.
-Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
-Middleware functions which are registered more than once will only be run once.
+- Middleware functions which are registered more than once will only be run once.
 
 Registration can be done when the `AsyncLambdaController` is initialized with the parameter `middleware` or by using the `add_middleware` method.
 
+Middleware functions have three sections:
+
+1. Pre task
+2. Task execution
+3. Post task
+
+```python
+def async_lambda_middleware(event: BaseEvent, call_next):
+    # pre task
+    result = call_next(event) # task execution
+    # post task
+    return result
+```
+
+If there are multiple middleware functions then `call_next` will actually be calling the next middleware function in the stack.
+
+For example if there is middleware functions `A` and `B` registered in that order.
+Then the execution order would go:
+
+`A(Pre)` -> `B(Pre)` -> `Task` -> `B(Post)` -> `A(Post)`
+
 EX:
 
 ```python
-def async_task_only_middleware(event: ManagedSQSEvent):
+def async_task_only_middleware(event: ManagedSQSEvent, call_next):
     print(f"Invocation Payload: {event}")
-    return event
-
-def all_task_types_middleware(event: BaseEvent):
-    print(f"This task is of the type {type(event)}")
+    result = call_next(event)
+    print(f"Invocation Result: {result}")
+    return result
+
+def all_task_types_middleware(event: BaseEvent, call_next):
+    print(f"This event is of the type {type(event)}")
+    result = call_next(event)
+    print(f"The result is of the type {type(result)}")
     return event
 
 controller = AsyncLambdaController(middleware=[([BaseEvent], all_task_types_middleware)])
 
 controller.add_middleware([ManagedSQSEvent], async_task_only_middleware)
 
 @controller.async_task("ATask")
```

### Comparing `async-lambda-unstable-0.4.1/README.md` & `async-lambda-unstable-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: async-lambda-unstable
+Version: 0.4.3
+Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
+Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
+Description-Content-Type: text/markdown
+Provides-Extra: local
+
 # async-lambda
 
 `async-lambda` is a framework for creating `AWS Lambda` applications with built
 in support for asynchronous invocation via a SQS Queue. This is useful if you
 have workloads you need to split up into separate execution contexts.
 
 `async-lambda` converts your application into a `Serverless Application Model (SAM)`
@@ -179,32 +187,65 @@
     event.querystring_params # request querystring params
     event.body # request body
     event.headers # This is a case insensitive dict
 ```
 
 # Middleware
 
-Middleware functions can be registered with controllers which will execute before the task code is run.
-These functions can be configured to trigger on specific types of tasks and can modify the `event`.
+Middleware functions can be registered with controllers which will wrap the execution of tasks.
+These functions can be configured to trigger on specific types of tasks and can trigger
+side effects and modify the `event` or `response` objects.
+
+Middleware functions must have the signature `Callable[[BaseEvent, Callable[[BaseEvent], T]], T]`.
+The first argument is the `event`, and the second argument (`call_next`) is a function which will propagate the
+calls down the middleware/task stack. The `call_next` function must be called, and its result in most cases be returned.
+If this is not done then tasks will not run as expected.
+
+**Extreme care should be taken with middleware as a simple mistake can have catastrophic effects.**
+
+- Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
 
-Middleware functions must have the signature `Callable[[BaseEvent], BaseEvent]`.
-Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
-Middleware functions which are registered more than once will only be run once.
+- Middleware functions which are registered more than once will only be run once.
 
 Registration can be done when the `AsyncLambdaController` is initialized with the parameter `middleware` or by using the `add_middleware` method.
 
+Middleware functions have three sections:
+
+1. Pre task
+2. Task execution
+3. Post task
+
+```python
+def async_lambda_middleware(event: BaseEvent, call_next):
+    # pre task
+    result = call_next(event) # task execution
+    # post task
+    return result
+```
+
+If there are multiple middleware functions then `call_next` will actually be calling the next middleware function in the stack.
+
+For example if there is middleware functions `A` and `B` registered in that order.
+Then the execution order would go:
+
+`A(Pre)` -> `B(Pre)` -> `Task` -> `B(Post)` -> `A(Post)`
+
 EX:
 
 ```python
-def async_task_only_middleware(event: ManagedSQSEvent):
+def async_task_only_middleware(event: ManagedSQSEvent, call_next):
     print(f"Invocation Payload: {event}")
-    return event
-
-def all_task_types_middleware(event: BaseEvent):
-    print(f"This task is of the type {type(event)}")
+    result = call_next(event)
+    print(f"Invocation Result: {result}")
+    return result
+
+def all_task_types_middleware(event: BaseEvent, call_next):
+    print(f"This event is of the type {type(event)}")
+    result = call_next(event)
+    print(f"The result is of the type {type(result)}")
     return event
 
 controller = AsyncLambdaController(middleware=[([BaseEvent], all_task_types_middleware)])
 
 controller.add_middleware([ManagedSQSEvent], async_task_only_middleware)
 
 @controller.async_task("ATask")
```

### Comparing `async-lambda-unstable-0.4.1/async_lambda/__init__.py` & `async-lambda-unstable-0.4.3/async_lambda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .models.events.api_event import APIEvent as APIEvent
 from .models.events.base_event import BaseEvent as BaseEvent
 from .models.events.dynamodb_event import DynamoDBEvent as DynamoDBEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent as ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent as ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent as UnmanagedSQSEvent
 
-__version__ = "0.4.1"
+__version__ = "0.4.3"
```

### Comparing `async-lambda-unstable-0.4.1/async_lambda/build_config.py` & `async-lambda-unstable-0.4.3/async_lambda/build_config.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/cli.py` & `async-lambda-unstable-0.4.3/async_lambda/cli.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/client.py` & `async-lambda-unstable-0.4.3/async_lambda/client.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/controller.py` & `async-lambda-unstable-0.4.3/async_lambda/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,80 @@
 import functools
 import json
 import logging
 import re
 import time
 from datetime import datetime, timezone
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 from uuid import uuid4
 
 from . import env
 from .build_config import get_build_config_for_stage
 from .client import get_s3_client, get_sqs_client
+from .middleware import MET, RT, MiddlewareFunction, MiddlewareRegistration
 from .models.events.api_event import APIEvent
 from .models.events.base_event import BaseEvent
 from .models.events.dynamodb_event import DynamoDBEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent
 from .models.mock.mock_context import MockLambdaContext
 from .models.mock.mock_event import MockSQSLambdaEvent
 from .models.task import AsyncLambdaTask, TaskTriggerType
 from .util import make_cf_tags
 
 logger = logging.getLogger(__name__)
 
-MET = TypeVar("MET", bound=BaseEvent)
-
-MiddlewareFunction = Callable[[MET], MET]
-MiddlewareRegistration = Tuple[List[Type[MET]], MiddlewareFunction[MET]]
-
 
 class AsyncLambdaController:
     is_sub: bool
     lane_count: Optional[int] = None
     propagate_lane_assignment: Optional[bool] = None
     tasks: Dict[str, AsyncLambdaTask]
     current_task_id: Optional[str] = None
     current_lane: Optional[int] = None
     current_invocation_id: Optional[str] = None
     parent_controller: Optional["AsyncLambdaController"] = None
     middleware: List[MiddlewareRegistration]
+
     dlq_task_id: Optional[str] = None
 
     def __init__(
         self,
         is_sub: bool = False,
         lane_count: Optional[int] = None,
         propagate_lane_assignment: Optional[bool] = None,
         middleware: Optional[List[MiddlewareRegistration]] = None,
+        exception_handler: Optional[Callable[[Exception], None]] = None,
     ):
         self.tasks = dict()
         self.is_sub = is_sub
         self.lane_count = lane_count
         self.propagate_lane_assignment = propagate_lane_assignment
         self.middleware = middleware or list()
+        self.exception_handler = exception_handler
 
     def add_middleware(
-        self, event_types: List[Type[BaseEvent]], func: MiddlewareFunction[MET]
+        self, event_types: List[Type[BaseEvent]], func: MiddlewareFunction[MET, RT]
     ):
         self.middleware.append((event_types, func))
 
-    def execute_middleware(
-        self, event: MET, _ran_fns: Optional[List[Callable]] = None
-    ) -> Tuple[MET, List[Callable]]:
-        if _ran_fns is None:
-            _ran_fns = list()
+    def get_middleware_for_event(self, event: MET) -> List[MiddlewareFunction[MET, RT]]:
         if self.parent_controller is not None:
-            event, _ran_fns = self.parent_controller.execute_middleware(event, _ran_fns)
+            _middleware_functions = self.parent_controller.get_middleware_for_event(
+                event
+            )
+        else:
+            _middleware_functions = list()
+
         for event_types, func in self.middleware:
-            if func in _ran_fns:
-                continue
             if any(isinstance(event, event_type) for event_type in event_types):
-                event = func(event)
-                _ran_fns.append(func)
-        return event, _ran_fns
+                _middleware_functions.append(func)
+
+        return _middleware_functions
 
     def add_task(self, task: AsyncLambdaTask):
         """
         Adds a task to the async lambda controller.
         """
         if task.task_id in self.tasks:
             raise Exception(
@@ -407,15 +405,15 @@
         delay: Optional[int] = 0,
         force_sync: bool = False,
         lane: Optional[int] = None,
     ):
         """
         Invoke an Async-Lambda task.
         """
-        self._async_invoke(
+        return self._async_invoke(
             destination_task_id=task_id,
             payload=payload,
             delay=delay,
             force_sync=force_sync,
             lane=lane,
         )
```

### Comparing `async-lambda-unstable-0.4.1/async_lambda/defer.py` & `async-lambda-unstable-0.4.3/async_lambda/defer.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/env.py` & `async-lambda-unstable-0.4.3/async_lambda/env.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/case_insensitive_dict.py` & `async-lambda-unstable-0.4.3/async_lambda/models/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/events/api_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/events/api_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/events/base_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/events/base_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/events/dynamodb_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/events/dynamodb_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/events/managed_sqs_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/events/managed_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/events/unmanaged_sqs_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/events/unmanaged_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/mock/mock_event.py` & `async-lambda-unstable-0.4.3/async_lambda/models/mock/mock_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda/models/task.py` & `async-lambda-unstable-0.4.3/async_lambda/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .. import env
 from ..build_config import get_build_config_for_task
 from ..config import config
 
 if TYPE_CHECKING:
     from ..controller import AsyncLambdaController  # pragma: not covered
 
+from ..middleware import RT, MiddlewareStackExecutor
 from .events.dynamodb_event import DynamoDBEvent
 from .events.managed_sqs_event import ManagedSQSEvent
 from .events.scheduled_event import ScheduledEvent
 from .events.unmanaged_sqs_event import UnmanagedSQSEvent
 
 
 class TaskTriggerType(Enum):
@@ -29,33 +30,33 @@
 
 EventType = TypeVar(
     "EventType",
     bound=Union[ManagedSQSEvent, ScheduledEvent, UnmanagedSQSEvent, DynamoDBEvent],
 )
 
 
-class AsyncLambdaTask(Generic[EventType]):
+class AsyncLambdaTask(Generic[EventType, RT]):
     controller: "AsyncLambdaController"
     task_id: str
     trigger_type: TaskTriggerType
     trigger_config: dict
 
     timeout: int
     memory: int
     ephemeral_storage: int
     maximum_concurrency: Optional[Union[int, List[int]]]
     init_tasks: List[Union[Callable[[str], Any], Callable[[], Any]]]
     _has_run_init_tasks: bool
 
-    executable: Callable[[EventType], Any]
+    executable: Callable[[EventType], RT]
 
     def __init__(
         self,
         controller: "AsyncLambdaController",
-        executable: Callable[[EventType], Any],
+        executable: Callable[[EventType], RT],
         task_id: str,
         trigger_type: TaskTriggerType,
         trigger_config: Optional[dict] = None,
         timeout: int = 60,
         memory: int = 128,
         ephemeral_storage: int = 512,
         maximum_concurrency: Optional[Union[int, List[int]]] = None,
@@ -477,14 +478,17 @@
             return None
         if self.trigger_config.get("is_dlq_task"):
             return None
         if self.trigger_config.get("dlq_task_id") is not None:
             return self.controller.get_task(self.trigger_config["dlq_task_id"])
         return self.controller.get_dlq_task()
 
-    def execute(self, event: EventType) -> Any:
+    def execute(self, event: EventType) -> RT:
         """
         Executes the tasks function
         """
         self._run_init_tasks()
-        self.controller.execute_middleware(event)
-        return self.executable(event)
+        middleware = self.controller.get_middleware_for_event(event)
+        middleware_stack_executor = MiddlewareStackExecutor[EventType, RT](
+            middleware=middleware, final=self.executable
+        )
+        return middleware_stack_executor.call_next(event)
```

### Comparing `async-lambda-unstable-0.4.1/async_lambda/util.py` & `async-lambda-unstable-0.4.3/async_lambda/util.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/PKG-INFO` & `async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.4.1
+Version: 0.4.3
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
 
@@ -187,32 +187,65 @@
     event.querystring_params # request querystring params
     event.body # request body
     event.headers # This is a case insensitive dict
 ```
 
 # Middleware
 
-Middleware functions can be registered with controllers which will execute before the task code is run.
-These functions can be configured to trigger on specific types of tasks and can modify the `event`.
+Middleware functions can be registered with controllers which will wrap the execution of tasks.
+These functions can be configured to trigger on specific types of tasks and can trigger
+side effects and modify the `event` or `response` objects.
 
-Middleware functions must have the signature `Callable[[BaseEvent], BaseEvent]`.
-Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
-Middleware functions which are registered more than once will only be run once.
+Middleware functions must have the signature `Callable[[BaseEvent, Callable[[BaseEvent], T]], T]`.
+The first argument is the `event`, and the second argument (`call_next`) is a function which will propagate the
+calls down the middleware/task stack. The `call_next` function must be called, and its result in most cases be returned.
+If this is not done then tasks will not run as expected.
+
+**Extreme care should be taken with middleware as a simple mistake can have catastrophic effects.**
+
+- Middleware functions are run in the order which they were registered and parent controller middleware will be run first.
+
+- Middleware functions which are registered more than once will only be run once.
 
 Registration can be done when the `AsyncLambdaController` is initialized with the parameter `middleware` or by using the `add_middleware` method.
 
+Middleware functions have three sections:
+
+1. Pre task
+2. Task execution
+3. Post task
+
+```python
+def async_lambda_middleware(event: BaseEvent, call_next):
+    # pre task
+    result = call_next(event) # task execution
+    # post task
+    return result
+```
+
+If there are multiple middleware functions then `call_next` will actually be calling the next middleware function in the stack.
+
+For example if there is middleware functions `A` and `B` registered in that order.
+Then the execution order would go:
+
+`A(Pre)` -> `B(Pre)` -> `Task` -> `B(Post)` -> `A(Post)`
+
 EX:
 
 ```python
-def async_task_only_middleware(event: ManagedSQSEvent):
+def async_task_only_middleware(event: ManagedSQSEvent, call_next):
     print(f"Invocation Payload: {event}")
-    return event
-
-def all_task_types_middleware(event: BaseEvent):
-    print(f"This task is of the type {type(event)}")
+    result = call_next(event)
+    print(f"Invocation Result: {result}")
+    return result
+
+def all_task_types_middleware(event: BaseEvent, call_next):
+    print(f"This event is of the type {type(event)}")
+    result = call_next(event)
+    print(f"The result is of the type {type(result)}")
     return event
 
 controller = AsyncLambdaController(middleware=[([BaseEvent], all_task_types_middleware)])
 
 controller.add_middleware([ManagedSQSEvent], async_task_only_middleware)
 
 @controller.async_task("ATask")
```

### Comparing `async-lambda-unstable-0.4.1/async_lambda_unstable.egg-info/SOURCES.txt` & `async-lambda-unstable-0.4.3/async_lambda_unstable.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 async_lambda/build_config.py
 async_lambda/cli.py
 async_lambda/client.py
 async_lambda/config.py
 async_lambda/controller.py
 async_lambda/defer.py
 async_lambda/env.py
+async_lambda/middleware.py
 async_lambda/py.typed
 async_lambda/util.py
 async_lambda/models/__init__.py
 async_lambda/models/case_insensitive_dict.py
 async_lambda/models/task.py
 async_lambda/models/events/__init__.py
 async_lambda/models/events/api_event.py
```

### Comparing `async-lambda-unstable-0.4.1/pyproject.toml` & `async-lambda-unstable-0.4.3/pyproject.toml`

 * *Files identical despite different names*

