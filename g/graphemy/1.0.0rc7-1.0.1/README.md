# Comparing `tmp/graphemy-1.0.0rc7.tar.gz` & `tmp/graphemy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0rc7.tar", max compression
+gzip compressed data, was "graphemy-1.0.1.tar", max compression
```

## Comparing `graphemy-1.0.0rc7.tar` & `graphemy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc7/graphemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc7/graphemy/database/__init__.py
--rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc7/graphemy/database/operations.py
--rw-r--r--   0        0        0     1771 2024-05-16 15:41:00.229255 graphemy-1.0.0rc7/graphemy/database/utils.py
--rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc7/graphemy/dl.py
--rw-r--r--   0        0        0     4005 2024-05-16 15:41:37.220215 graphemy-1.0.0rc7/graphemy/models.py
--rw-r--r--   0        0        0     8273 2024-05-16 15:41:00.259464 graphemy-1.0.0rc7/graphemy/router.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc7/graphemy/schemas/__init__.py
--rw-r--r--   0        0        0     8460 2024-05-16 15:42:16.520947 graphemy-1.0.0rc7/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc7/graphemy/schemas/models.py
--rw-r--r--   0        0        0     4822 2024-05-16 15:10:05.941065 graphemy-1.0.0rc7/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc7/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-16 15:44:16.068116 graphemy-1.0.0rc7/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc7/README.md
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc7/PKG-INFO
+-rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.1/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.1/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.1/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1771 2024-05-16 15:41:00.229255 graphemy-1.0.1/graphemy/database/utils.py
+-rw-r--r--   0        0        0     4244 2024-05-30 01:06:15.458296 graphemy-1.0.1/graphemy/dl.py
+-rw-r--r--   0        0        0     4133 2024-05-30 01:06:15.458296 graphemy-1.0.1/graphemy/models.py
+-rw-r--r--   0        0        0     8713 2024-05-30 01:06:15.459302 graphemy-1.0.1/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.1/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     8313 2024-05-30 03:17:17.813989 graphemy-1.0.1/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.1/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     5896 2024-05-30 01:06:15.461302 graphemy-1.0.1/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2464 2024-05-30 03:19:18.463511 graphemy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4013 2024-05-30 01:06:15.444872 graphemy-1.0.1/README.md
+-rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 graphemy-1.0.1/PKG-INFO
```

### Comparing `graphemy-1.0.0rc7/graphemy/__init__.py` & `graphemy-1.0.1/graphemy/__init__.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc7/graphemy/database/operations.py` & `graphemy-1.0.1/graphemy/database/operations.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc7/graphemy/database/utils.py` & `graphemy-1.0.1/graphemy/database/utils.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc7/graphemy/dl.py` & `graphemy-1.0.1/graphemy/dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,40 +50,38 @@
     A customized DataLoader that handles additional filtering mechanisms during data
     retrieval processes. It is capable of using predefined filter methods to process data
     based on request-specific parameters.
 
     Attributes:
         filter_method (callable): A method that applies additional filtering to the data
             based on the request context and specified filters.
-        request: The context of the request, used to pass additional parameters to the
+        context: The context of the request, used to pass additional parameters to the
             filter_method.
 
     Methods:
         load: Overridden to apply filters before returning the data, enhancing the
             DataLoader's functionality to cater to complex querying needs.
     """
 
-    def __init__(self, filter_method=None, request=None, **kwargs):
+    def __init__(self, filter_method=None, context: dict = None, **kwargs):
         self.filter_method = filter_method
-        self.request = request
+        self.context = context
         super().__init__(**kwargs)
 
-    async def load(self, keys, filters: dict | None = False):
-        if filters == False:
-            return await super().load(keys)
+    async def load(self, keys, filters: dict | None):
         filters['keys'] = (
             tuple(keys)
             if isinstance(keys, list)
             else keys.strip()
             if isinstance(keys, str)
             else keys
         )
         data = await super().load(dict_to_tuple(filters))
         if self.filter_method:
-            data = self.filter_method(data, self.request)
+            data = self.filter_method(data, self.context)
         return data
 
 
 def dict_to_tuple(data: dict) -> tuple:
     """
     Converts a dictionary into a tuple, recursively processing nested dictionaries
     and lists to ensure they are in a hashable and comparable format. This is essential
```

### Comparing `graphemy-1.0.0rc7/graphemy/models.py` & `graphemy-1.0.1/graphemy/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import abc
+import re
+
 from sqlmodel import SQLModel
 from strawberry.type import StrawberryType
 from strawberry.types import Info
 
 from .dl import Dl
 from .schemas.generators import get_dl_function
 from .setup import Setup
@@ -55,14 +58,17 @@
     __queryname__: str = ''
     __enginename__: str = 'default'
 
     class Strawberry:
         pass
 
     def __init_subclass__(cls):
+        cls.__tablename__ = re.sub(
+            r'(?<!^)(?=[A-Z])', '_', cls.__name__
+        ).lower()
         cls.__queryname__ = (
             cls.__queryname__ if cls.__queryname__ else cls.__tablename__ + 's'
         )
         Setup.classes[cls.__name__] = cls
         to_remove = []
         for attr_name, attr_type in cls.__annotations__.items():
             if hasattr(cls, attr_name):
@@ -72,9 +78,9 @@
                     dl_field = get_dl_function(
                         attr_name, attr_type, attr_value
                     )
                     setattr(cls, attr_name, dl_field)
         for attr in to_remove:
             del cls.__annotations__[attr]
 
-    async def permission_getter(info: Info, request_type: str) -> bool:
-        return True
+    async def permission_getter(context: dict, request_type: str) -> bool:
+        pass
```

### Comparing `graphemy-1.0.0rc7/graphemy/router.py` & `graphemy-1.0.1/graphemy/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import inspect
 import sys
 from types import GenericAlias
 from typing import Callable, Dict
 
 import strawberry
+import strawberry.tools
+import strawberry.utils
+import strawberry.utils.typing
 from fastapi import Request, Response
 from graphql.error import GraphQLError
 from graphql.error.graphql_error import format_error as format_graphql_error
 from sqlalchemy.engine.base import Engine
 from strawberry.fastapi import GraphQLRouter
 from strawberry.http import GraphQLHTTPResponse
 from strawberry.types import ExecutionResult
@@ -40,30 +43,37 @@
         keys (iterable): A collection of keys for which data needs to be fetched.
     Returns:
         An iterable of empty lists corresponding to each key.
     """
     return {k: [] for k in keys}.values()
 
 
-class Query:
-    """
-    A class used as a container for defining GraphQL queries. All the resolvers associated
-    with fetching data are attached to instances of this class or its subclasses.
-    """
+def genre_empty_query():
+    class Query:
+        """
+        A class used as a container for defining GraphQL queries. All the resolvers associated
+        with fetching data are attached to instances of this class or its subclasses.
+        """
 
-    pass
+        pass
 
+    return Query
 
-class Mutation:
-    """
-    A class used as a container for defining GraphQL mutations. It contains methods that
-    alter data state in the database, typically involving create, update, and delete operations.
-    """
 
-    pass
+def genre_empty_mutation():
+    class Mutation:
+        __auto_generated__ = True
+        """
+        A class used as a container for defining GraphQL mutations. It contains methods that
+        alter data state in the database, typically involving create, update, and delete operations.
+        """
+
+        pass
+
+    return Mutation
 
 
 async def hello_world(self, info) -> str:
     """
     A simple resolver function returning a greeting message.
     Returns:
         A string greeting 'Hello World'.
@@ -92,32 +102,36 @@
         **kwargs: Additional keyword arguments passed to the base GraphQLRouter.
     """
 
     functions = []
 
     def __init__(
         self,
-        query: object = Query,
-        mutation: object = Mutation,
+        query: object | None = None,
+        mutation: object | None = None,
         context_getter: Callable | None = None,
         permission_getter: Callable | None = None,
         dl_filter: Callable | None = None,
         query_filter: Callable | None = None,
         engine: Engine | Dict[str, Engine] = None,
         extensions: list = [],
         enable_queries: bool = True,
         enable_put_mutations: bool = False,
         enable_delete_mutations: bool = False,
         auto_foreign_keys: bool = False,
         **kwargs,
     ):
+        if not query:
+            query = genre_empty_query()
+        if not mutation:
+            mutation = genre_empty_mutation()
         functions: Dict[str, tuple] = {}
         Setup.setup(
             engine=engine,
-            get_perm=permission_getter,
+            permission_getter=permission_getter,
             query_filter=query_filter,
         )
         need_query = True
         need_mutation = True
         for cls in Setup.classes.values():
             set_schema(cls, functions, auto_foreign_keys)
             if cls.__enable_query__ == None:
@@ -170,30 +184,30 @@
                 await context_getter(request, response)
                 if context_getter
                 else {}
             )
             for k, (func, return_class) in functions.items():
                 context[k] = GraphemyDataLoader(
                     load_fn=func
-                    if await Setup.get_permission(
+                    if await Setup.permission_getter(
                         return_class, context, 'query'
                     )
                     else fake_dl_list
                     if type(inspect.signature(func).return_annotation)
                     == GenericAlias
                     else fake_dl_one,
                     filter_method=dl_filter,
-                    request=request,
+                    context=context,
                 )
             return context
 
         schema = strawberry.Schema(
             query=strawberry.type(query),
             mutation=None
-            if need_mutation and mutation == Mutation
+            if need_mutation and hasattr(mutation, '__auto_generated__')
             else strawberry.type(mutation),
             extensions=extensions,
         )
         super().__init__(schema=schema, context_getter=get_context, **kwargs)
 
     async def process_result(
         self, request: Request, result: ExecutionResult
```

### Comparing `graphemy-1.0.0rc7/graphemy/schemas/generators.py` & `graphemy-1.0.1/graphemy/schemas/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 def set_schema(
     cls: 'Graphemy',
     functions: Dict[str, Tuple[Callable, 'Graphemy']],
     auto_foreign_keys,
 ) -> None:
     """Set the Strawberry schema for a Graphemy class."""
-
     # Define a class to hold Strawberry schema fields
     class Schema:
         pass
 
     foreign_keys_info = []
     for attr in [
         attr for attr in cls.__dict__.values() if hasattr(attr, 'dl')
@@ -65,49 +64,45 @@
             source = (
                 attr.source if isinstance(attr.source, list) else [attr.source]
             )
             target = (
                 attr.target if isinstance(attr.target, list) else [attr.target]
             )
             target = [returned_class.__tablename__ + '.' + t for t in target]
-            filtered_pairs = [
-                (s, t)
-                for s, t in zip(source, target)
-                if not (
-                    isinstance(s, int)
-                    or s.startswith('_')
-                    or isinstance(t, int)
-                    or t.startswith('_')
-                )
-            ]
-            source, target = (
-                zip(*filtered_pairs) if filtered_pairs else ([], [])
-            )
 
-            if len(source) > 0 and len(target) > 0:
+            if (
+                len(source) > 0
+                and len(target) > 0
+                and not any(
+                    isinstance(item, int)
+                    or (isinstance(item, str) and item.startswith('_'))
+                    for item in source + target
+                )
+            ):
                 cls.__table__.append_constraint(
                     ForeignKeyConstraint(source, target)
                 )
                 foreign_keys_info.append((source, target))
         if not attr.dl_name in functions:
             functions[attr.dl_name] = (
                 get_dl_field(attr, returned_class),
                 returned_class,
             )
-    extra_schema = strawberry.type(
-        cls.Strawberry, name=f'{cls.__name__}Schema2'
-    )
-    strawberry_schema = strawberry.experimental.pydantic.type(
-        cls, all_fields=True, name=f'{cls.__name__}Schema'
-    )(Schema)
-    if extra_schema.__annotations__:
-        strawberry_schema = merge_types(
-            f'{cls.__name__}Schema', (strawberry_schema, extra_schema)
-        )
-    cls.__strawberry_schema__ = strawberry_schema
+    if not cls.__strawberry_schema__:
+        extra_schema = strawberry.type(
+            cls.Strawberry, name=f'{cls.__name__}Schema2'
+        )
+        strawberry_schema = strawberry.experimental.pydantic.type(
+            cls, all_fields=True, name=f'{cls.__name__}Schema'
+        )(Schema)
+        if extra_schema.__annotations__:
+            strawberry_schema = merge_types(
+                f'{cls.__name__}Schema', (strawberry_schema, extra_schema)
+            )
+        cls.__strawberry_schema__ = strawberry_schema
 
 
 def get_dl_field(attr, returned_class: 'Graphemy') -> callable:
     returned_schema = returned_class.__strawberry_schema__
     if attr.many:
         returned_schema = list[returned_schema]
     else:
@@ -206,31 +201,30 @@
             strawberry.field(default=None, graphql_type=Optional[field]),
         )
     filter = strawberry.input(name=f'{cls.__name__}Filter')(Filter)
 
     async def query(
         self, info: Info, filters: filter | None = None
     ) -> list[cls.__strawberry_schema__]:
-        if not await cls.permission_getter(
-            info, 'query'
-        ) or not await Setup.get_permission(cls, info.context, 'query'):
+        if not await Setup.has_permission(cls, info.context, 'query'):
             return []
-        data = await get_all(cls, filters, Setup.query_filter(cls, info))
+        data = await get_all(
+            cls, filters, Setup.query_filter(cls, info.context)
+        )
         return data
 
     return (
         strawberry.field(
             query, permission_classes=[Setup.get_auth(cls, 'query')]
         ),
         filter,
     )
 
 
 def get_put_mutation(cls: 'Graphemy') -> StrawberryField:
-
     pk = [pk.name for pk in inspect(cls).primary_key]
 
     class Filter:
         pass
 
     for field_name, field in cls.__annotations__.items():
         setattr(
```

### Comparing `graphemy-1.0.0rc7/graphemy/setup.py` & `graphemy-1.0.1/graphemy/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import TYPE_CHECKING, Dict
+from typing import TYPE_CHECKING, Callable, Dict
 
+import strawberry
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import sessionmaker
-from sqlmodel import Session
+from sqlmodel import Session, SQLModel
 from strawberry.permission import BasePermission
 
 if TYPE_CHECKING:
     from .models import Graphemy
 
 
 class Setup:
@@ -22,30 +23,30 @@
         async_engine (bool): A flag indicating if the engine configuration supports asynchronous
             operations.
         classes (Dict[str, 'Graphemy']): A registry of model classes that might be involved in GraphQL
             queries or mutations.
     """
 
     engine: Dict[str, Engine] = None
-    get_permission: callable = None
+    permission_getter: Callable
     async_engine = False
     classes: Dict[str, 'Graphemy'] = {}
 
     @classmethod
-    async def execute_query(cls, query, engine):
+    async def execute_query(cls, query, engine) -> list:
         """
         Executes a given SQL query using the specified database engine, either asynchronously or synchronously
         based on the engine configuration.
 
         Args:
             query: The SQL query to be executed.
             engine (str): The key of the engine in the 'engine' attribute to be used for the query.
 
         Returns:
-            The result of the query execution, typically a list of database records.
+            list: The result of the query execution, typically a list of database records.
         """
         if cls.async_engine:
             async_session = sessionmaker(
                 cls.engine[engine], class_=AsyncSession, expire_on_commit=False
             )
             async with async_session() as session:
                 r = await session.execute(query)
@@ -55,47 +56,73 @@
                 r = session.exec(query).all()
                 return r
 
     @classmethod
     def setup(
         cls,
         engine: Dict[str, Engine] | Engine,
-        get_perm=None,
+        permission_getter=None,
         query_filter=None,
     ):
         """
         Configures the database engines and sets default functions for permission checks and query filtering.
 
         Args:
             engine (Dict[str, Engine] | Engine): A dictionary of engines or a single engine to be used.
-            get_perm (callable): A function to determine if a request is permitted.
+            permission_getter (callable): A function to determine if a request is permitted.
             query_filter (callable): A function to filter queries based on specific conditions.
         """
-        if engine and 'async' in engine.__module__:
-            cls.async_engine = True
+
         if isinstance(engine, Dict):
             cls.engine = engine
         else:
             cls.engine = {'default': engine}
+        if engine and 'async' in cls.engine['default'].__module__:
+            cls.async_engine = True
         if query_filter:
             cls.query_filter = query_filter
         else:
 
             def query_filter_default(cls, info):
                 return True
 
             cls.query_filter = query_filter_default
-        if get_perm:
-            cls.get_permission = get_perm
+        if permission_getter:
+            cls.permission_getter = permission_getter
         else:
 
-            async def get_permission(module_class, context, type):
+            async def permission_getter(module_class, info, type):
                 return True
 
-            cls.get_permission = get_permission
+            cls.permission_getter = permission_getter
+
+    @classmethod
+    async def has_permission(
+        cls, module: 'Graphemy', context: dict, request_type: str
+    ) -> bool:
+        """
+        Determines if a user has permission to execute a GraphQL query or mutation based on the
+        provided context and request type.
+
+        Args:
+            module ('Graphemy'): The model class for which permissions are being checked.
+            context (dict): The context of the GraphQL request.
+            request_type (str): The type of request (e.g., 'query' or 'mutation') to determine the appropriate permissions.
+
+        Returns:
+            A boolean indicating if the user has permission to execute the request.
+        """
+        permission = await module.permission_getter(context, request_type)
+        if isinstance(permission, bool):
+            return permission
+        else:
+            permission = await cls.permission_getter(
+                module, context, request_type
+            )
+        return permission
 
     @classmethod
     def get_auth(cls, module: 'Graphemy', request_type: str) -> BasePermission:
         """
         Creates a custom Strawberry GraphQL permission class that performs authentication and authorization checks.
 
         Args:
@@ -103,18 +130,18 @@
             request_type (str): The type of request (e.g., 'query' or 'mutation') to determine the appropriate permissions.
 
         Returns:
             An instance of a Strawberry permission class that can be used to control access to GraphQL operations.
         """
 
         class IsAuthenticated(BasePermission):
-            async def has_permission(self, source, info, **kwargs) -> bool:
-                if not await module.permission_getter(
-                    info, request_type
-                ) or not await cls.get_permission(
+            async def has_permission(
+                self, source, info: strawberry.Info, **kwargs
+            ) -> bool:
+                if not await cls.has_permission(
                     module, info.context, request_type
                 ):
                     info.context['response'].status_code = 403
                     if not 'errors' in info.context['request'].scope:
                         info.context['request'].scope['errors'] = [module]
                     elif not module in info.context['request'].scope['errors']:
                         info.context['request'].scope['errors'].append(module)
```

### Comparing `graphemy-1.0.0rc7/LICENSE` & `graphemy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc7/pyproject.toml` & `graphemy-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-rc.7"
+version = "1.0.1"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
 license = "MIT"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Topic :: Database",
     "Topic :: Database :: Database Engines/Servers",
     "Intended Audience :: Developers",
     "Framework :: FastAPI",
     "Programming Language :: Python :: 3.12",
     "Natural Language :: English",
 ]
 [tool.poetry.urls]
 "Documentation" = "https://graphemy.readthedocs.io/en/latest/"
 "Repository" = "https://github.com/MDoreto/graphemy"
 "Bug Tracker" = "https://github.com/MDoreto/graphemy/issues"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-sqlmodel = "0.0.14"
-strawberry-graphql = {extras = ["debug-server"], version = "^0.211.1"}
-fastapi = "^0.104.1"
-python-dotenv = "^1.0.0"
+sqlmodel = "0.0.18"
+strawberry-graphql = {extras = ["debug-server"], version = "^0.229.1"}
+fastapi = "^0.111.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 blue = "^0.9.1"
 isort = "^5.12.0"
 taskipy = "^1.12.0"
 pytest-asyncio = "^0.21.1"
 httpx = "^0.25.0"
 pytest-env = "^1.1.1"
 aiosqlite = "^0.20.0"
+gevent = "^24.2.1"
 
 
 [tool.poetry.group.doc.dependencies]
 mkdocs-material = "^9.4.7"
 mkdocstrings = "^0.23.0"
 mkdocstrings-python = "^1.7.3"
 mkdocs-macros-plugin = "^1.0.5"
@@ -53,22 +53,31 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = "."
-addopts = "--doctest-modules"
 
+[tool.coverage.run]
+concurrency = ["thread","gevent"]
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.taskipy.tasks]
-example = "uvicorn examples.tutorial.main:app --reload --port 8001"
+ex_basic = "uvicorn examples.tutorial.basic.main:app --reload --port 8001"
+ex_dl = "uvicorn examples.tutorial.relationship.main:app --reload --port 8001"
 lint = "blue . && isort ."
 docs = "mkdocs serve"
+pre_publish = "poetry export --output requirements-docs.txt --with doc --without-hashes   "
 pre_test = "task lint"
 test = "pytest -s -x --cov=graphemy -vv -W ignore::DeprecationWarning"
 post_test = "coverage html"
 publish = "poetry publish --build"
+
+
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:",
+    ]
```

### Comparing `graphemy-1.0.0rc7/README.md` & `graphemy-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,226 +1,251 @@
-00000000: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000010: 2f2f 6772 6170 6865 6d79 2e72 6561 6474  //graphemy.readt
-00000020: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000030: 6573 742f 6173 7365 7473 2f6c 6f67 6f2e  est/assets/logo.
-00000040: 706e 6722 2077 6964 7468 3d22 3230 3022  png" width="200"
-00000050: 3e0d 0a0d 0a23 2047 5241 5048 454d 590d  >....# GRAPHEMY.
-00000060: 0a5b 215b 446f 6375 6d65 6e74 6174 696f  .[![Documentatio
-00000070: 6e20 5374 6174 7573 5d28 6874 7470 733a  n Status](https:
-00000080: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
-00000090: 672f 7072 6f6a 6563 7473 2f67 7261 7068  g/projects/graph
-000000a0: 656d 792f 6261 6467 652f 3f76 6572 7369  emy/badge/?versi
-000000b0: 6f6e 3d6c 6174 6573 7429 5d28 6874 7470  on=latest)](http
-000000c0: 733a 2f2f 6772 6170 6865 6d79 2e72 6561  s://graphemy.rea
-000000d0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-000000e0: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
-000000f0: 6573 7429 0d0a 5b21 5b63 6f64 6563 6f76  est)..[![codecov
-00000100: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-00000110: 762e 696f 2f67 682f 4d44 6f72 6574 6f2f  v.io/gh/MDoreto/
-00000120: 6772 6170 6865 6d79 2f67 7261 7068 2f62  graphemy/graph/b
-00000130: 6164 6765 2e73 7667 3f74 6f6b 656e 3d47  adge.svg?token=G
-00000140: 4a44 4d56 4241 3432 3529 5d28 6874 7470  JDMVBA425)](http
-00000150: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00000160: 682f 4d44 6f72 6574 6f2f 6772 6170 6865  h/MDoreto/graphe
-00000170: 6d79 290d 0a21 5b43 495d 2868 7474 7073  my)..![CI](https
-00000180: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d44  ://github.com/MD
-00000190: 6f72 6574 6f2f 6772 6170 6865 6d79 2f61  oreto/graphemy/a
-000001a0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-000001b0: 2f70 6970 656c 696e 652e 796d 6c2f 6261  /pipeline.yml/ba
-000001c0: 6467 652e 7376 6729 0d0a 0d0a 4120 5079  dge.svg)....A Py
-000001d0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
-000001e0: 2069 6e74 6567 7261 7469 6e67 2053 514c   integrating SQL
-000001f0: 4d6f 6465 6c20 616e 6420 5374 7261 7762  Model and Strawb
-00000200: 6572 7279 2c20 7072 6f76 6964 696e 6720  erry, providing 
-00000210: 6120 7365 616d 6c65 7373 2047 7261 7068  a seamless Graph
-00000220: 514c 2069 6e74 6567 7261 7469 6f6e 2077  QL integration w
-00000230: 6974 6820 4661 7374 4150 4920 616e 6420  ith FastAPI and 
-00000240: 6164 7661 6e63 6564 2066 6561 7475 7265  advanced feature
-00000250: 7320 666f 7220 6461 7461 6261 7365 2069  s for database i
-00000260: 6e74 6572 6163 7469 6f6e 732e 0d0a 0d0a  nteractions.....
-00000270: 0d0a 2323 204f 7665 7276 6965 770d 0a0d  ..## Overview...
-00000280: 0a54 6865 2047 7261 7068 656d 7920 6973  .The Graphemy is
-00000290: 2064 6573 6967 6e65 6420 746f 2073 696d   designed to sim
-000002a0: 706c 6966 7920 616e 6420 7374 7265 616d  plify and stream
-000002b0: 6c69 6e65 2074 6865 2069 6e74 6567 7261  line the integra
-000002c0: 7469 6f6e 206f 6620 5351 4c4d 6f64 656c  tion of SQLModel
-000002d0: 2061 6e64 2053 7472 6177 6265 7272 7920   and Strawberry 
-000002e0: 696e 2050 7974 686f 6e20 7072 6f6a 6563  in Python projec
-000002f0: 7473 2e20 5468 6973 206c 6962 7261 7279  ts. This library
-00000300: 2061 6c6c 6f77 7320 796f 7520 746f 2063   allows you to c
-00000310: 7265 6174 6520 6120 7369 6e67 6c65 2063  reate a single c
-00000320: 6c61 7373 206d 6f64 656c 2c20 7768 6963  lass model, whic
-00000330: 682c 206f 6e63 6520 6465 636c 6172 6564  h, once declared
-00000340: 2c20 6175 746f 6d61 7469 6361 6c6c 7920  , automatically 
-00000350: 7072 6f76 6964 6573 2047 7261 7068 514c  provides GraphQL
-00000360: 2071 7565 7269 6573 2076 6961 2053 7472   queries via Str
-00000370: 6177 6265 7272 792e 2054 6865 7365 2071  awberry. These q
-00000380: 7565 7269 6573 2063 616e 2062 6520 6561  ueries can be ea
-00000390: 7369 6c79 2069 6e74 6567 7261 7465 6420  sily integrated 
-000003a0: 696e 746f 2061 2046 6173 7441 5049 2062  into a FastAPI b
-000003b0: 6163 6b65 6e64 2e20 416c 6c20 6765 6e65  ackend. All gene
-000003c0: 7261 7465 6420 726f 7574 6573 2069 6e63  rated routes inc
-000003d0: 6c75 6465 2066 696c 7465 7273 206f 6e20  lude filters on 
-000003e0: 616c 6c20 6669 656c 6473 2c20 696e 636c  all fields, incl
-000003f0: 7564 696e 6720 6120 6375 7374 6f6d 2064  uding a custom d
-00000400: 6174 6520 6669 6c74 6572 2e20 4164 6469  ate filter. Addi
-00000410: 7469 6f6e 616c 6c79 2c20 6974 2066 6163  tionally, it fac
-00000420: 696c 6974 6174 6573 2074 6865 2063 7265  ilitates the cre
-00000430: 6174 696f 6e20 6f66 206d 7574 6174 696f  ation of mutatio
-00000440: 6e73 2066 6f72 2064 6174 6120 6d6f 6469  ns for data modi
-00000450: 6669 6361 7469 6f6e 2061 6e64 2064 656c  fication and del
-00000460: 6574 696f 6e20 6279 2073 696d 706c 7920  etion by simply 
-00000470: 7365 7474 696e 6720 6120 7661 7269 6162  setting a variab
-00000480: 6c65 2069 6e20 7468 6520 6d6f 6465 6c2e  le in the model.
-00000490: 2054 6865 206c 6962 7261 7279 2061 6c73   The library als
-000004a0: 6f20 6861 6e64 6c65 7320 7461 626c 6520  o handles table 
-000004b0: 7265 6c61 7469 6f6e 7368 6970 7320 6566  relationships ef
-000004c0: 6669 6369 656e 746c 7920 7573 696e 6720  ficiently using 
-000004d0: 5374 7261 7762 6572 7279 2773 2064 6174  Strawberry's dat
-000004e0: 616c 6f61 6465 7273 2c20 7072 6f76 6964  aloaders, provid
-000004f0: 696e 6720 6120 7369 676e 6966 6963 616e  ing a significan
-00000500: 7420 7065 7266 6f72 6d61 6e63 6520 626f  t performance bo
-00000510: 6f73 742e 204d 6f72 656f 7665 722c 2069  ost. Moreover, i
-00000520: 7420 6f66 6665 7273 2061 2070 7265 2d63  t offers a pre-c
-00000530: 6f6e 6669 6775 7265 6420 6175 7468 656e  onfigured authen
-00000540: 7469 6361 7469 6f6e 2073 6574 7570 2c20  tication setup, 
-00000550: 7768 6963 6820 6361 6e20 6265 2063 6f6e  which can be con
-00000560: 6669 6775 7265 6420 7769 7468 206a 7573  figured with jus
-00000570: 7420 7477 6f20 6675 6e63 7469 6f6e 732e  t two functions.
-00000580: 0d0a 0d0a 2323 2046 6561 7475 7265 730d  ....## Features.
-00000590: 0a0d 0a2d 2049 6e74 6567 7261 7469 6f6e  ...- Integration
-000005a0: 206f 6620 5351 4c4d 6f64 656c 2061 6e64   of SQLModel and
-000005b0: 2053 7472 6177 6265 7272 7920 666f 7220   Strawberry for 
-000005c0: 4772 6170 6851 4c20 7375 7070 6f72 742e  GraphQL support.
-000005d0: 0d0a 2d20 4175 746f 6d61 7469 6320 6765  ..- Automatic ge
-000005e0: 6e65 7261 7469 6f6e 206f 6620 4772 6170  neration of Grap
-000005f0: 6851 4c20 7175 6572 6965 7320 666f 7220  hQL queries for 
-00000600: 4661 7374 4150 492e 0d0a 2d20 506f 7765  FastAPI...- Powe
-00000610: 7266 756c 2066 696c 7465 7269 6e67 2063  rful filtering c
-00000620: 6170 6162 696c 6974 6965 732c 2069 6e63  apabilities, inc
-00000630: 6c75 6469 6e67 2063 7573 746f 6d20 6461  luding custom da
-00000640: 7465 2066 696c 7465 7273 2e0d 0a2d 2045  te filters...- E
-00000650: 6666 6f72 746c 6573 7320 6372 6561 7469  ffortless creati
-00000660: 6f6e 206f 6620 6d75 7461 7469 6f6e 7320  on of mutations 
-00000670: 666f 7220 6461 7461 206d 616e 6970 756c  for data manipul
-00000680: 6174 696f 6e2e 0d0a 2d20 4566 6669 6369  ation...- Effici
-00000690: 656e 7420 6861 6e64 6c69 6e67 206f 6620  ent handling of 
-000006a0: 7461 626c 6520 7265 6c61 7469 6f6e 7368  table relationsh
-000006b0: 6970 7320 7573 696e 6720 5374 7261 7762  ips using Strawb
-000006c0: 6572 7279 2773 2064 6174 616c 6f61 6465  erry's dataloade
-000006d0: 7273 2e0d 0a2d 2050 7265 2d63 6f6e 6669  rs...- Pre-confi
-000006e0: 6775 7265 6420 6175 7468 656e 7469 6361  gured authentica
-000006f0: 7469 6f6e 2073 6574 7570 2066 6f72 2065  tion setup for e
-00000700: 6173 7920 636f 6e66 6967 7572 6174 696f  asy configuratio
-00000710: 6e2e 0d0a 0d0a 2323 2050 7265 7265 7175  n.....## Prerequ
-00000720: 6973 6974 6573 0d0a 0d0a 4265 666f 7265  isites....Before
-00000730: 2079 6f75 2062 6567 696e 2075 7369 6e67   you begin using
-00000740: 2047 7261 7068 656d 792c 2069 7420 6973   Graphemy, it is
-00000750: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
-00000760: 6465 6420 7468 6174 2079 6f75 2068 6176  ded that you hav
-00000770: 6520 736f 6d65 2070 7269 6f72 206b 6e6f  e some prior kno
-00000780: 776c 6564 6765 206f 6620 7468 6520 6573  wledge of the es
-00000790: 7365 6e74 6961 6c20 6c69 6272 6172 6965  sential librarie
-000007a0: 7320 7570 6f6e 2077 6869 6368 2074 6869  s upon which thi
-000007b0: 7320 7072 6f6a 6563 7420 6973 2062 7569  s project is bui
-000007c0: 6c74 2e20 5468 6973 2077 696c 6c20 6865  lt. This will he
-000007d0: 6c70 2079 6f75 206d 616b 6520 7468 6520  lp you make the 
-000007e0: 6d6f 7374 206f 6620 7468 6520 6665 6174  most of the feat
-000007f0: 7572 6573 2061 6e64 2063 6172 7279 206f  ures and carry o
-00000800: 7574 2069 6e74 6567 7261 7469 6f6e 7320  ut integrations 
-00000810: 6d6f 7265 2065 6666 6563 7469 7665 6c79  more effectively
-00000820: 2e20 506c 6561 7365 206d 616b 6520 7375  . Please make su
-00000830: 7265 2079 6f75 2061 7265 2066 616d 696c  re you are famil
-00000840: 6961 7220 7769 7468 2074 6865 2066 6f6c  iar with the fol
-00000850: 6c6f 7769 6e67 206c 6962 7261 7269 6573  lowing libraries
-00000860: 3a0d 0a0d 0a2a 2a46 6173 7441 5049 2a2a  :....**FastAPI**
-00000870: 3a20 4120 6d6f 6465 726e 2066 7261 6d65  : A modern frame
-00000880: 776f 726b 2066 6f72 2062 7569 6c64 696e  work for buildin
-00000890: 6720 6661 7374 2077 6562 2041 5049 7320  g fast web APIs 
-000008a0: 7769 7468 2050 7974 686f 6e2e 2049 6620  with Python. If 
-000008b0: 796f 7520 6172 6520 6e6f 7420 616c 7265  you are not alre
-000008c0: 6164 7920 6661 6d69 6c69 6172 2077 6974  ady familiar wit
-000008d0: 6820 4661 7374 4150 492c 2079 6f75 2063  h FastAPI, you c
-000008e0: 616e 2072 6566 6572 2074 6f20 7468 6520  an refer to the 
-000008f0: 5b46 6173 7441 5049 2064 6f63 756d 656e  [FastAPI documen
-00000900: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-00000910: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-00000920: 2e63 6f6d 2f29 2e0d 0a0d 0a2a 2a53 514c  .com/).....**SQL
-00000930: 4d6f 6465 6c2a 2a3a 2041 6e20 6f62 6a65  Model**: An obje
-00000940: 6374 2d72 656c 6174 696f 6e61 6c20 6d61  ct-relational ma
-00000950: 7070 696e 6720 284f 524d 2920 6c69 6272  pping (ORM) libr
-00000960: 6172 7920 666f 7220 5079 7468 6f6e 2074  ary for Python t
-00000970: 6861 7420 7369 6d70 6c69 6669 6573 2061  hat simplifies a
-00000980: 6e64 2073 7472 6561 6d6c 696e 6573 2064  nd streamlines d
-00000990: 6174 6162 6173 6520 696e 7465 7261 6374  atabase interact
-000009a0: 696f 6e73 2e20 546f 206c 6561 726e 206d  ions. To learn m
-000009b0: 6f72 6520 6162 6f75 7420 5351 4c4d 6f64  ore about SQLMod
-000009c0: 656c 2c20 7669 7369 7420 7468 6520 5b53  el, visit the [S
-000009d0: 514c 4d6f 6465 6c20 646f 6375 6d65 6e74  QLModel document
-000009e0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f73  ation](https://s
-000009f0: 716c 6d6f 6465 6c2e 7469 616e 676f 6c6f  qlmodel.tiangolo
-00000a00: 2e63 6f6d 2f29 2e0d 0a0d 0a2a 2a53 7472  .com/).....**Str
-00000a10: 6177 6265 7272 792a 2a3a 2041 2050 7974  awberry**: A Pyt
-00000a20: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
-00000a30: 6465 636c 6172 6174 6976 656c 7920 6372  declaratively cr
-00000a40: 6561 7469 6e67 2047 7261 7068 514c 2073  eating GraphQL s
-00000a50: 6368 656d 6173 2e20 466f 7220 696e 2d64  chemas. For in-d
-00000a60: 6570 7468 2069 6e66 6f72 6d61 7469 6f6e  epth information
-00000a70: 206f 6e20 7573 696e 6720 5374 7261 7762   on using Strawb
-00000a80: 6572 7279 2c20 6163 6365 7373 2074 6865  erry, access the
-00000a90: 205b 5374 7261 7762 6572 7279 2064 6f63   [Strawberry doc
-00000aa0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00000ab0: 733a 2f2f 7374 7261 7762 6572 7279 2e72  s://strawberry.r
-00000ac0: 6f63 6b73 2f29 2e0d 0a0d 0a48 6176 696e  ocks/).....Havin
-00000ad0: 6720 6120 736f 6c69 6420 756e 6465 7273  g a solid unders
-00000ae0: 7461 6e64 696e 6720 6f66 2074 6865 7365  tanding of these
-00000af0: 206c 6962 7261 7269 6573 2069 7320 6372   libraries is cr
-00000b00: 7563 6961 6c20 746f 206d 616b 696e 6720  ucial to making 
-00000b10: 7468 6520 6d6f 7374 206f 6620 5072 6f6a  the most of Proj
-00000b20: 6563 7420 4e61 6d65 2061 6e64 2065 6666  ect Name and eff
-00000b30: 6f72 746c 6573 736c 7920 6372 6561 7469  ortlessly creati
-00000b40: 6e67 2047 7261 7068 514c 2041 5049 732e  ng GraphQL APIs.
-00000b50: 0d0a 0d0a 2323 2043 7265 6174 6520 6120  ....## Create a 
-00000b60: 5072 6f6a 6563 740d 0a0d 0a49 2072 6563  Project....I rec
-00000b70: 6f6d 656e 6420 796f 7520 7573 6520 506f  omend you use Po
-00000b80: 6574 7279 2c20 6275 7420 796f 7520 6361  etry, but you ca
-00000b90: 6e20 7573 6520 7468 6520 656e 7669 726f  n use the enviro
-00000ba0: 6d65 6e74 206d 616e 6167 6572 2074 6861  ment manager tha
-00000bb0: 7420 796f 7520 7761 6e74 2e20 536f 2069  t you want. So i
-00000bc0: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-00000bd0: 706f 6574 7279 2c20 7374 6172 7420 7468  poetry, start th
-00000be0: 6520 7072 6f6a 6563 743a 0d0a 0d0a 6060  e project:....``
-00000bf0: 6062 6173 680d 0a23 2043 7265 6174 6520  `bash..# Create 
-00000c00: 706f 6574 7279 2070 726f 6a65 6374 0d0a  poetry project..
-00000c10: 706f 6574 7279 206e 6577 2067 7261 7068  poetry new graph
-00000c20: 656d 7920 7475 746f 7269 616c 0d0a 0d0a  emy tutorial....
-00000c30: 2320 5374 6172 7420 456e 7669 726f 6e6d  # Start Environm
-00000c40: 656e 7420 0d0a 706f 6574 7279 2073 6865  ent ..poetry she
-00000c50: 6c6c 0d0a 6060 600d 0a0d 0a59 6f75 2063  ll..```....You c
-00000c60: 616e 2061 6c73 6f20 7573 6520 7468 6520  an also use the 
-00000c70: 656e 7669 726f 6e6d 656e 7420 6d61 6e61  environment mana
-00000c80: 6765 7220 7761 6e74 6564 2c20 7375 6368  ger wanted, such
-00000c90: 2061 7320 7669 7274 7561 6c65 6e76 0d0a   as virtualenv..
-00000ca0: 0d0a 6060 6062 6173 680d 0a23 2043 7265  ..```bash..# Cre
-00000cb0: 6174 6520 6120 6469 7265 6374 6f72 7920  ate a directory 
-00000cc0: 666f 7220 7475 746f 7269 616c 0d0a 6d6b  for tutorial..mk
-00000cd0: 6469 7220 6772 6170 6865 6d79 2d74 7574  dir graphemy-tut
-00000ce0: 6f72 6961 6c0d 0a0d 0a23 2045 6e74 6572  orial....# Enter
-00000cf0: 2069 6e74 6f20 7468 6174 2064 6972 6563   into that direc
-00000d00: 746f 7279 0d0a 6364 2067 7261 7068 656d  tory..cd graphem
-00000d10: 790d 0a0d 0a23 2043 7265 6174 6520 7669  y....# Create vi
-00000d20: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-00000d30: 740d 0a70 7974 686f 6e20 2d6d 2076 656e  t..python -m ven
-00000d40: 7620 7665 6e76 0d0a 0d0a 2353 7461 7274  v venv....#Start
-00000d50: 2045 6e76 6972 6f6e 6d65 6e74 0d0a 7665   Environment..ve
-00000d60: 6e76 2f53 6372 6970 7473 2f41 6374 6976  nv/Scripts/Activ
-00000d70: 6174 650d 0a60 6060 0d0a 0d0a 2323 2052  ate..```....## R
-00000d80: 6571 7569 7265 6d65 6e74 730d 0a0d 0a4e  equirements....N
-00000d90: 6f77 2069 6e73 7461 6c6c 2047 7261 7068  ow install Graph
-00000da0: 656d 7920 3a29 200d 0a60 6060 6261 7368  emy :) ..```bash
-00000db0: 0d0a 706f 6574 7279 2061 6464 2067 7261  ..poetry add gra
-00000dc0: 7068 656d 790d 0a60 6060 0d0a 4f72 2075  phemy..```..Or u
-00000dd0: 7369 6e67 2064 6566 6175 6c74 2070 7974  sing default pyt
-00000de0: 686f 6e20 656e 7620 7769 7468 2070 6970  hon env with pip
-00000df0: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7069  :....```bash..pi
-00000e00: 7020 696e 7374 616c 6c20 6772 6170 6865  p install graphe
-00000e10: 6d79 0d0a 6060 60                        my..```
+00000000: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000010: 6572 223e 0d0a 2020 3c69 6d67 2073 7263  er">..  <img src
+00000020: 3d22 2e2f 646f 6373 2f61 7373 6574 732f  ="./docs/assets/
+00000030: 6c6f 676f 2e70 6e67 2220 2f3e 0d0a 3c2f  logo.png" />..</
+00000040: 703e 0d0a 0d0a 2320 4752 4150 4845 4d59  p>....# GRAPHEMY
+00000050: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000060: 6572 223e 0d0a 2020 2020 3c65 6d3e 496e  er">..    <em>In
+00000070: 7465 6772 6174 696e 6720 5351 4c4d 6f64  tegrating SQLMod
+00000080: 656c 2061 6e64 2053 7472 6177 6265 7272  el and Strawberr
+00000090: 792c 2070 726f 7669 6469 6e67 2061 2073  y, providing a s
+000000a0: 6561 6d6c 6573 7320 4772 6170 6851 4c20  eamless GraphQL 
+000000b0: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
+000000c0: 2044 6174 6162 6173 6573 2065 6173 7920   Databases easy 
+000000d0: 616e 6420 6661 7374 2e3c 2f65 6d3e 0d0a  and fast.</em>..
+000000e0: 3c2f 703e 0d0a 0d0a 5b21 5b44 6f63 756d  </p>....[![Docum
+000000f0: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
+00000100: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
+00000110: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+00000120: 732f 6772 6170 6865 6d79 2f62 6164 6765  s/graphemy/badge
+00000130: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
+00000140: 295d 2868 7474 7073 3a2f 2f67 7261 7068  )](https://graph
+00000150: 656d 792e 7265 6164 7468 6564 6f63 732e  emy.readthedocs.
+00000160: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
+00000170: 6467 653d 6c61 7465 7374 290d 0a5b 215b  dge=latest)..[![
+00000180: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
+00000190: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f4d  /codecov.io/gh/M
+000001a0: 446f 7265 746f 2f67 7261 7068 656d 792f  Doreto/graphemy/
+000001b0: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+000001c0: 746f 6b65 6e3d 474a 444d 5642 4134 3235  token=GJDMVBA425
+000001d0: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+000001e0: 6f76 2e69 6f2f 6768 2f4d 446f 7265 746f  ov.io/gh/MDoreto
+000001f0: 2f67 7261 7068 656d 7929 0d0a 215b 4349  /graphemy)..![CI
+00000200: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000210: 2e63 6f6d 2f4d 446f 7265 746f 2f67 7261  .com/MDoreto/gra
+00000220: 7068 656d 792f 6163 7469 6f6e 732f 776f  phemy/actions/wo
+00000230: 726b 666c 6f77 732f 7069 7065 6c69 6e65  rkflows/pipeline
+00000240: 2e79 6d6c 2f62 6164 6765 2e73 7667 290d  .yml/badge.svg).
+00000250: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000260: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000270: 6374 2f67 7261 7068 656d 7922 2074 6172  ct/graphemy" tar
+00000280: 6765 743d 225f 626c 616e 6b22 3e0d 0a20  get="_blank">.. 
+00000290: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000002a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000002b0: 2e69 6f2f 7079 7069 2f76 2f67 7261 7068  .io/pypi/v/graph
+000002c0: 656d 793f 636f 6c6f 723d 2532 3333 3444  emy?color=%2334D
+000002d0: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
+000002e0: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
+000002f0: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
+00000300: 0d0a 3c2f 613e 0d0a 0d0a 0d0a 2d2d 2d0d  ..</a>......---.
+00000310: 0a0d 0a2a 2a44 6f63 756d 656e 7461 7469  ...**Documentati
+00000320: 6f6e 2a2a 3a20 3c61 2068 7265 663d 2268  on**: <a href="h
+00000330: 7474 7073 3a2f 2f67 7261 7068 656d 792e  ttps://graphemy.
+00000340: 7265 6164 7468 6564 6f63 732e 696f 2220  readthedocs.io" 
+00000350: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000360: 6874 7470 733a 2f2f 6772 6170 6865 6d79  https://graphemy
+00000370: 2e72 6561 6474 6865 646f 6373 2e69 6f3c  .readthedocs.io<
+00000380: 2f61 3e0d 0a0d 0a2a 2a53 6f75 7263 6520  /a>....**Source 
+00000390: 436f 6465 2a2a 3a20 3c61 2068 7265 663d  Code**: <a href=
+000003a0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000003b0: 636f 6d2f 4d44 6f72 6574 6f2f 6772 6170  com/MDoreto/grap
+000003c0: 6865 6d79 2220 7461 7267 6574 3d22 5f62  hemy" target="_b
+000003d0: 6c61 6e6b 223e 6874 7470 733a 2f2f 6769  lank">https://gi
+000003e0: 7468 7562 2e63 6f6d 2f4d 446f 7265 746f  thub.com/MDoreto
+000003f0: 2f67 7261 7068 656d 793c 2f61 3e0d 0a0d  /graphemy</a>...
+00000400: 0a2d 2d2d 0d0a 0d0a 0d0a 2323 204f 7665  .---......## Ove
+00000410: 7276 6965 770d 0a0d 0a54 6865 2047 7261  rview....The Gra
+00000420: 7068 656d 7920 6973 2064 6573 6967 6e65  phemy is designe
+00000430: 6420 746f 2073 696d 706c 6966 7920 616e  d to simplify an
+00000440: 6420 7374 7265 616d 6c69 6e65 2074 6865  d streamline the
+00000450: 2069 6e74 6567 7261 7469 6f6e 206f 6620   integration of 
+00000460: 5351 4c4d 6f64 656c 2061 6e64 2053 7472  SQLModel and Str
+00000470: 6177 6265 7272 7920 696e 2050 7974 686f  awberry in Pytho
+00000480: 6e20 7072 6f6a 6563 7473 2e20 5468 6973  n projects. This
+00000490: 206c 6962 7261 7279 2061 6c6c 6f77 7320   library allows 
+000004a0: 796f 7520 746f 2063 7265 6174 6520 6120  you to create a 
+000004b0: 7369 6e67 6c65 2063 6c61 7373 206d 6f64  single class mod
+000004c0: 656c 2c20 7768 6963 682c 206f 6e63 6520  el, which, once 
+000004d0: 6465 636c 6172 6564 2c20 6175 746f 6d61  declared, automa
+000004e0: 7469 6361 6c6c 7920 7072 6f76 6964 6573  tically provides
+000004f0: 2047 7261 7068 514c 2071 7565 7269 6573   GraphQL queries
+00000500: 2076 6961 2053 7472 6177 6265 7272 792e   via Strawberry.
+00000510: 2054 6865 7365 2071 7565 7269 6573 2063   These queries c
+00000520: 616e 2062 6520 6561 7369 6c79 2069 6e74  an be easily int
+00000530: 6567 7261 7465 6420 696e 746f 2061 2046  egrated into a F
+00000540: 6173 7441 5049 2062 6163 6b65 6e64 2e20  astAPI backend. 
+00000550: 416c 6c20 6765 6e65 7261 7465 6420 726f  All generated ro
+00000560: 7574 6573 2069 6e63 6c75 6465 2066 696c  utes include fil
+00000570: 7465 7273 206f 6e20 616c 6c20 6669 656c  ters on all fiel
+00000580: 6473 2c20 696e 636c 7564 696e 6720 6120  ds, including a 
+00000590: 6375 7374 6f6d 2064 6174 6520 6669 6c74  custom date filt
+000005a0: 6572 2e20 4164 6469 7469 6f6e 616c 6c79  er. Additionally
+000005b0: 2c20 6974 2066 6163 696c 6974 6174 6573  , it facilitates
+000005c0: 2074 6865 2063 7265 6174 696f 6e20 6f66   the creation of
+000005d0: 206d 7574 6174 696f 6e73 2066 6f72 2064   mutations for d
+000005e0: 6174 6120 6d6f 6469 6669 6361 7469 6f6e  ata modification
+000005f0: 2061 6e64 2064 656c 6574 696f 6e20 6279   and deletion by
+00000600: 2073 696d 706c 7920 7365 7474 696e 6720   simply setting 
+00000610: 6120 7661 7269 6162 6c65 2069 6e20 7468  a variable in th
+00000620: 6520 6d6f 6465 6c2e 2054 6865 206c 6962  e model. The lib
+00000630: 7261 7279 2061 6c73 6f20 6861 6e64 6c65  rary also handle
+00000640: 7320 7461 626c 6520 7265 6c61 7469 6f6e  s table relation
+00000650: 7368 6970 7320 6566 6669 6369 656e 746c  ships efficientl
+00000660: 7920 7573 696e 6720 5374 7261 7762 6572  y using Strawber
+00000670: 7279 2773 2064 6174 616c 6f61 6465 7273  ry's dataloaders
+00000680: 2c20 7072 6f76 6964 696e 6720 6120 7369  , providing a si
+00000690: 676e 6966 6963 616e 7420 7065 7266 6f72  gnificant perfor
+000006a0: 6d61 6e63 6520 626f 6f73 742e 204d 6f72  mance boost. Mor
+000006b0: 656f 7665 722c 2069 7420 6f66 6665 7273  eover, it offers
+000006c0: 2061 2070 7265 2d63 6f6e 6669 6775 7265   a pre-configure
+000006d0: 6420 6175 7468 656e 7469 6361 7469 6f6e  d authentication
+000006e0: 2073 6574 7570 2c20 7768 6963 6820 6361   setup, which ca
+000006f0: 6e20 6265 2063 6f6e 6669 6775 7265 6420  n be configured 
+00000700: 7769 7468 206a 7573 7420 7477 6f20 6675  with just two fu
+00000710: 6e63 7469 6f6e 732e 0d0a 0d0a 2323 2046  nctions.....## F
+00000720: 6561 7475 7265 730d 0a0d 0a2d 2049 6e74  eatures....- Int
+00000730: 6567 7261 7469 6f6e 206f 6620 5351 4c4d  egration of SQLM
+00000740: 6f64 656c 2061 6e64 2053 7472 6177 6265  odel and Strawbe
+00000750: 7272 7920 666f 7220 4772 6170 6851 4c20  rry for GraphQL 
+00000760: 7375 7070 6f72 742e 0d0a 2d20 4175 746f  support...- Auto
+00000770: 6d61 7469 6320 6765 6e65 7261 7469 6f6e  matic generation
+00000780: 206f 6620 4772 6170 6851 4c20 7175 6572   of GraphQL quer
+00000790: 6965 7320 666f 7220 4661 7374 4150 492e  ies for FastAPI.
+000007a0: 0d0a 2d20 506f 7765 7266 756c 2066 696c  ..- Powerful fil
+000007b0: 7465 7269 6e67 2063 6170 6162 696c 6974  tering capabilit
+000007c0: 6965 732c 2069 6e63 6c75 6469 6e67 2063  ies, including c
+000007d0: 7573 746f 6d20 6461 7465 2066 696c 7465  ustom date filte
+000007e0: 7273 2e0d 0a2d 2045 6666 6f72 746c 6573  rs...- Effortles
+000007f0: 7320 6372 6561 7469 6f6e 206f 6620 6d75  s creation of mu
+00000800: 7461 7469 6f6e 7320 666f 7220 6461 7461  tations for data
+00000810: 206d 616e 6970 756c 6174 696f 6e2e 0d0a   manipulation...
+00000820: 2d20 4566 6669 6369 656e 7420 6861 6e64  - Efficient hand
+00000830: 6c69 6e67 206f 6620 7461 626c 6520 7265  ling of table re
+00000840: 6c61 7469 6f6e 7368 6970 7320 7573 696e  lationships usin
+00000850: 6720 5374 7261 7762 6572 7279 2773 2064  g Strawberry's d
+00000860: 6174 616c 6f61 6465 7273 2e0d 0a2d 2050  ataloaders...- P
+00000870: 7265 2d63 6f6e 6669 6775 7265 6420 6175  re-configured au
+00000880: 7468 656e 7469 6361 7469 6f6e 2073 6574  thentication set
+00000890: 7570 2066 6f72 2065 6173 7920 636f 6e66  up for easy conf
+000008a0: 6967 7572 6174 696f 6e2e 0d0a 0d0a 2323  iguration.....##
+000008b0: 2050 7265 7265 7175 6973 6974 6573 0d0a   Prerequisites..
+000008c0: 0d0a 4265 666f 7265 2079 6f75 2062 6567  ..Before you beg
+000008d0: 696e 2075 7369 6e67 2047 7261 7068 656d  in using Graphem
+000008e0: 792c 2069 7420 6973 2068 6967 686c 7920  y, it is highly 
+000008f0: 7265 636f 6d6d 656e 6465 6420 7468 6174  recommended that
+00000900: 2079 6f75 2068 6176 6520 736f 6d65 2070   you have some p
+00000910: 7269 6f72 206b 6e6f 776c 6564 6765 206f  rior knowledge o
+00000920: 6620 7468 6520 6573 7365 6e74 6961 6c20  f the essential 
+00000930: 6c69 6272 6172 6965 7320 7570 6f6e 2077  libraries upon w
+00000940: 6869 6368 2074 6869 7320 7072 6f6a 6563  hich this projec
+00000950: 7420 6973 2062 7569 6c74 2e20 5468 6973  t is built. This
+00000960: 2077 696c 6c20 6865 6c70 2079 6f75 206d   will help you m
+00000970: 616b 6520 7468 6520 6d6f 7374 206f 6620  ake the most of 
+00000980: 7468 6520 6665 6174 7572 6573 2061 6e64  the features and
+00000990: 2063 6172 7279 206f 7574 2069 6e74 6567   carry out integ
+000009a0: 7261 7469 6f6e 7320 6d6f 7265 2065 6666  rations more eff
+000009b0: 6563 7469 7665 6c79 2e20 506c 6561 7365  ectively. Please
+000009c0: 206d 616b 6520 7375 7265 2079 6f75 2061   make sure you a
+000009d0: 7265 2066 616d 696c 6961 7220 7769 7468  re familiar with
+000009e0: 2074 6865 2066 6f6c 6c6f 7769 6e67 206c   the following l
+000009f0: 6962 7261 7269 6573 3a0d 0a0d 0a2a 2a46  ibraries:....**F
+00000a00: 6173 7441 5049 2a2a 3a20 4120 6d6f 6465  astAPI**: A mode
+00000a10: 726e 2066 7261 6d65 776f 726b 2066 6f72  rn framework for
+00000a20: 2062 7569 6c64 696e 6720 6661 7374 2077   building fast w
+00000a30: 6562 2041 5049 7320 7769 7468 2050 7974  eb APIs with Pyt
+00000a40: 686f 6e2e 2049 6620 796f 7520 6172 6520  hon. If you are 
+00000a50: 6e6f 7420 616c 7265 6164 7920 6661 6d69  not already fami
+00000a60: 6c69 6172 2077 6974 6820 4661 7374 4150  liar with FastAP
+00000a70: 492c 2079 6f75 2063 616e 2072 6566 6572  I, you can refer
+00000a80: 2074 6f20 7468 6520 5b46 6173 7441 5049   to the [FastAPI
+00000a90: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00000aa0: 6874 7470 733a 2f2f 6661 7374 6170 692e  https://fastapi.
+00000ab0: 7469 616e 676f 6c6f 2e63 6f6d 2f29 2e0d  tiangolo.com/)..
+00000ac0: 0a0d 0a2a 2a53 514c 4d6f 6465 6c2a 2a3a  ...**SQLModel**:
+00000ad0: 2041 6e20 6f62 6a65 6374 2d72 656c 6174   An object-relat
+00000ae0: 696f 6e61 6c20 6d61 7070 696e 6720 284f  ional mapping (O
+00000af0: 524d 2920 6c69 6272 6172 7920 666f 7220  RM) library for 
+00000b00: 5079 7468 6f6e 2074 6861 7420 7369 6d70  Python that simp
+00000b10: 6c69 6669 6573 2061 6e64 2073 7472 6561  lifies and strea
+00000b20: 6d6c 696e 6573 2064 6174 6162 6173 6520  mlines database 
+00000b30: 696e 7465 7261 6374 696f 6e73 2e20 546f  interactions. To
+00000b40: 206c 6561 726e 206d 6f72 6520 6162 6f75   learn more abou
+00000b50: 7420 5351 4c4d 6f64 656c 2c20 7669 7369  t SQLModel, visi
+00000b60: 7420 7468 6520 5b53 514c 4d6f 6465 6c20  t the [SQLModel 
+00000b70: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
+00000b80: 7474 7073 3a2f 2f73 716c 6d6f 6465 6c2e  ttps://sqlmodel.
+00000b90: 7469 616e 676f 6c6f 2e63 6f6d 2f29 2e0d  tiangolo.com/)..
+00000ba0: 0a0d 0a2a 2a53 7472 6177 6265 7272 792a  ...**Strawberry*
+00000bb0: 2a3a 2041 2050 7974 686f 6e20 6c69 6272  *: A Python libr
+00000bc0: 6172 7920 666f 7220 6465 636c 6172 6174  ary for declarat
+00000bd0: 6976 656c 7920 6372 6561 7469 6e67 2047  ively creating G
+00000be0: 7261 7068 514c 2073 6368 656d 6173 2e20  raphQL schemas. 
+00000bf0: 466f 7220 696e 2d64 6570 7468 2069 6e66  For in-depth inf
+00000c00: 6f72 6d61 7469 6f6e 206f 6e20 7573 696e  ormation on usin
+00000c10: 6720 5374 7261 7762 6572 7279 2c20 6163  g Strawberry, ac
+00000c20: 6365 7373 2074 6865 205b 5374 7261 7762  cess the [Strawb
+00000c30: 6572 7279 2064 6f63 756d 656e 7461 7469  erry documentati
+00000c40: 6f6e 5d28 6874 7470 733a 2f2f 7374 7261  on](https://stra
+00000c50: 7762 6572 7279 2e72 6f63 6b73 2f29 2e0d  wberry.rocks/)..
+00000c60: 0a0d 0a48 6176 696e 6720 6120 736f 6c69  ...Having a soli
+00000c70: 6420 756e 6465 7273 7461 6e64 696e 6720  d understanding 
+00000c80: 6f66 2074 6865 7365 206c 6962 7261 7269  of these librari
+00000c90: 6573 2069 7320 6372 7563 6961 6c20 746f  es is crucial to
+00000ca0: 206d 616b 696e 6720 7468 6520 6d6f 7374   making the most
+00000cb0: 206f 6620 4772 6170 6865 6d79 2061 6e64   of Graphemy and
+00000cc0: 2065 6666 6f72 746c 6573 736c 7920 6372   effortlessly cr
+00000cd0: 6561 7469 6e67 2047 7261 7068 514c 2041  eating GraphQL A
+00000ce0: 5049 732e 0d0a 0d0a 2323 2043 7265 6174  PIs.....## Creat
+00000cf0: 6520 6120 5072 6f6a 6563 740d 0a0d 0a49  e a Project....I
+00000d00: 2072 6563 6f6d 656e 6420 796f 7520 7573   recomend you us
+00000d10: 6520 506f 6574 7279 2c20 6275 7420 796f  e Poetry, but yo
+00000d20: 7520 6361 6e20 7573 6520 7468 6520 656e  u can use the en
+00000d30: 7669 726f 6d65 6e74 206d 616e 6167 6572  viroment manager
+00000d40: 2074 6861 7420 796f 7520 7761 6e74 2e20   that you want. 
+00000d50: 536f 2069 6620 796f 7520 6172 6520 7573  So if you are us
+00000d60: 696e 6720 706f 6574 7279 2c20 7374 6172  ing poetry, star
+00000d70: 7420 7468 6520 7072 6f6a 6563 743a 0d0a  t the project:..
+00000d80: 0d0a 6060 6062 6173 680d 0a23 2043 7265  ..```bash..# Cre
+00000d90: 6174 6520 706f 6574 7279 2070 726f 6a65  ate poetry proje
+00000da0: 6374 0d0a 706f 6574 7279 206e 6577 2067  ct..poetry new g
+00000db0: 7261 7068 656d 7920 7475 746f 7269 616c  raphemy tutorial
+00000dc0: 0d0a 0d0a 2320 5374 6172 7420 456e 7669  ....# Start Envi
+00000dd0: 726f 6e6d 656e 7420 0d0a 706f 6574 7279  ronment ..poetry
+00000de0: 2073 6865 6c6c 0d0a 6060 600d 0a0d 0a59   shell..```....Y
+00000df0: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00000e00: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+00000e10: 6d61 6e61 6765 7220 7761 6e74 6564 2c20  manager wanted, 
+00000e20: 7375 6368 2061 7320 7669 7274 7561 6c65  such as virtuale
+00000e30: 6e76 0d0a 0d0a 6060 6062 6173 680d 0a23  nv....```bash..#
+00000e40: 2043 7265 6174 6520 6120 6469 7265 6374   Create a direct
+00000e50: 6f72 7920 666f 7220 7475 746f 7269 616c  ory for tutorial
+00000e60: 0d0a 6d6b 6469 7220 6772 6170 6865 6d79  ..mkdir graphemy
+00000e70: 2d74 7574 6f72 6961 6c0d 0a0d 0a23 2045  -tutorial....# E
+00000e80: 6e74 6572 2069 6e74 6f20 7468 6174 2064  nter into that d
+00000e90: 6972 6563 746f 7279 0d0a 6364 2067 7261  irectory..cd gra
+00000ea0: 7068 656d 790d 0a0d 0a23 2043 7265 6174  phemy....# Creat
+00000eb0: 6520 7669 7274 7561 6c20 656e 7669 726f  e virtual enviro
+00000ec0: 6e6d 656e 740d 0a70 7974 686f 6e20 2d6d  nment..python -m
+00000ed0: 2076 656e 7620 7665 6e76 0d0a 0d0a 2353   venv venv....#S
+00000ee0: 7461 7274 2045 6e76 6972 6f6e 6d65 6e74  tart Environment
+00000ef0: 0d0a 7665 6e76 2f53 6372 6970 7473 2f41  ..venv/Scripts/A
+00000f00: 6374 6976 6174 650d 0a60 6060 0d0a 0d0a  ctivate..```....
+00000f10: 2323 2052 6571 7569 7265 6d65 6e74 730d  ## Requirements.
+00000f20: 0a0d 0a4e 6f77 2069 6e73 7461 6c6c 2047  ...Now install G
+00000f30: 7261 7068 656d 7920 3a29 200d 0a60 6060  raphemy :) ..```
+00000f40: 6261 7368 0d0a 706f 6574 7279 2061 6464  bash..poetry add
+00000f50: 2067 7261 7068 656d 790d 0a60 6060 0d0a   graphemy..```..
+00000f60: 4f72 2075 7369 6e67 2064 6566 6175 6c74  Or using default
+00000f70: 2070 7974 686f 6e20 656e 7620 7769 7468   python env with
+00000f80: 2070 6970 3a0d 0a0d 0a60 6060 6261 7368   pip:....```bash
+00000f90: 0d0a 7069 7020 696e 7374 616c 6c20 6772  ..pip install gr
+00000fa0: 6170 6865 6d79 0d0a 6060 600d 0a         aphemy..```..
```

### Comparing `graphemy-1.0.0rc7/PKG-INFO` & `graphemy-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,297 +1,319 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6772 6170  : 2.1.Name: grap
 00000020: 6865 6d79 0a56 6572 7369 6f6e 3a20 312e  hemy.Version: 1.
-00000030: 302e 3072 6337 0a53 756d 6d61 7279 3a20  0.0rc7.Summary: 
-00000040: 4120 5079 7468 6f6e 206c 6962 7261 7279  A Python library
-00000050: 2066 6f72 2069 6e74 6567 7261 7469 6e67   for integrating
-00000060: 2053 514c 4d6f 6465 6c20 616e 6420 5374   SQLModel and St
-00000070: 7261 7762 6572 7279 2c20 7072 6f76 6964  rawberry, provid
-00000080: 696e 6720 6120 7365 616d 6c65 7373 2047  ing a seamless G
-00000090: 7261 7068 514c 2069 6e74 6567 7261 7469  raphQL integrati
-000000a0: 6f6e 2077 6974 6820 4661 7374 4150 4920  on with FastAPI 
-000000b0: 616e 6420 6164 7661 6e63 6564 2066 6561  and advanced fea
-000000c0: 7475 7265 7320 666f 7220 6461 7461 6261  tures for databa
-000000d0: 7365 2069 6e74 6572 6163 7469 6f6e 732e  se interactions.
-000000e0: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000100: 446f 7265 746f 2f67 7261 7068 656d 790a  Doreto/graphemy.
-00000110: 4c69 6365 6e73 653a 204d 4954 0a41 7574  License: MIT.Aut
-00000120: 686f 723a 204d 6174 6865 7573 2044 6f72  hor: Matheus Dor
-00000130: 6574 6f0a 4175 7468 6f72 2d65 6d61 696c  eto.Author-email
-00000140: 3a20 6d61 7468 6575 7364 6f72 6574 6f2e  : matheusdoreto.
-00000150: 6d64 4067 6d61 696c 2e63 6f6d 0a52 6571  md@gmail.com.Req
-00000160: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-00000170: 332e 3132 2c3c 342e 300a 436c 6173 7369  3.12,<4.0.Classi
-00000180: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
-00000190: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
-000001a0: 4265 7461 0a43 6c61 7373 6966 6965 723a  Beta.Classifier:
-000001b0: 2046 7261 6d65 776f 726b 203a 3a20 4661   Framework :: Fa
-000001c0: 7374 4150 490a 436c 6173 7369 6669 6572  stAPI.Classifier
-000001d0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-000001e0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-000001f0: 730a 436c 6173 7369 6669 6572 3a20 4c69  s.Classifier: Li
-00000200: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000210: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000220: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000230: 204e 6174 7572 616c 204c 616e 6775 6167   Natural Languag
-00000240: 6520 3a3a 2045 6e67 6c69 7368 0a43 6c61  e :: English.Cla
-00000250: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000260: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000270: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
-00000280: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000290: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002a0: 2050 7974 686f 6e20 3a3a 2033 2e31 320a   Python :: 3.12.
-000002b0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000002c0: 6320 3a3a 2044 6174 6162 6173 650a 436c  c :: Database.Cl
-000002d0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000002e0: 3a3a 2044 6174 6162 6173 6520 3a3a 2044  :: Database :: D
-000002f0: 6174 6162 6173 6520 456e 6769 6e65 732f  atabase Engines/
-00000300: 5365 7276 6572 730a 5265 7175 6972 6573  Servers.Requires
-00000310: 2d44 6973 743a 2066 6173 7461 7069 2028  -Dist: fastapi (
-00000320: 3e3d 302e 3130 342e 312c 3c30 2e31 3035  >=0.104.1,<0.105
-00000330: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000340: 743a 2070 7974 686f 6e2d 646f 7465 6e76  t: python-dotenv
-00000350: 2028 3e3d 312e 302e 302c 3c32 2e30 2e30   (>=1.0.0,<2.0.0
-00000360: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000370: 2073 716c 6d6f 6465 6c20 283d 3d30 2e30   sqlmodel (==0.0
-00000380: 2e31 3429 0a52 6571 7569 7265 732d 4469  .14).Requires-Di
-00000390: 7374 3a20 7374 7261 7762 6572 7279 2d67  st: strawberry-g
-000003a0: 7261 7068 716c 5b64 6562 7567 2d73 6572  raphql[debug-ser
-000003b0: 7665 725d 2028 3e3d 302e 3231 312e 312c  ver] (>=0.211.1,
-000003c0: 3c30 2e32 3132 2e30 290a 5072 6f6a 6563  <0.212.0).Projec
-000003d0: 742d 5552 4c3a 2042 7567 2054 7261 636b  t-URL: Bug Track
-000003e0: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
-000003f0: 7562 2e63 6f6d 2f4d 446f 7265 746f 2f67  ub.com/MDoreto/g
-00000400: 7261 7068 656d 792f 6973 7375 6573 0a50  raphemy/issues.P
-00000410: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000420: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000430: 3a2f 2f67 7261 7068 656d 792e 7265 6164  ://graphemy.read
-00000440: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000450: 7465 7374 2f0a 5072 6f6a 6563 742d 5552  test/.Project-UR
-00000460: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
-00000470: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000480: 6d2f 4d44 6f72 6574 6f2f 6772 6170 6865  m/MDoreto/graphe
-00000490: 6d79 0a44 6573 6372 6970 7469 6f6e 2d43  my.Description-C
-000004a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000004b0: 742f 6d61 726b 646f 776e 0a0a 3c69 6d67  t/markdown..<img
-000004c0: 2073 7263 3d22 6874 7470 733a 2f2f 6772   src="https://gr
-000004d0: 6170 6865 6d79 2e72 6561 6474 6865 646f  aphemy.readthedo
-000004e0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-000004f0: 6173 7365 7473 2f6c 6f67 6f2e 706e 6722  assets/logo.png"
-00000500: 2077 6964 7468 3d22 3230 3022 3e0a 0a23   width="200">..#
-00000510: 2047 5241 5048 454d 590a 5b21 5b44 6f63   GRAPHEMY.[![Doc
-00000520: 756d 656e 7461 7469 6f6e 2053 7461 7475  umentation Statu
-00000530: 735d 2868 7474 7073 3a2f 2f72 6561 6474  s](https://readt
-00000540: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-00000550: 6374 732f 6772 6170 6865 6d79 2f62 6164  cts/graphemy/bad
-00000560: 6765 2f3f 7665 7273 696f 6e3d 6c61 7465  ge/?version=late
-00000570: 7374 295d 2868 7474 7073 3a2f 2f67 7261  st)](https://gra
-00000580: 7068 656d 792e 7265 6164 7468 6564 6f63  phemy.readthedoc
-00000590: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
-000005a0: 6261 6467 653d 6c61 7465 7374 290a 5b21  badge=latest).[!
-000005b0: 5b63 6f64 6563 6f76 5d28 6874 7470 733a  [codecov](https:
-000005c0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000005d0: 4d44 6f72 6574 6f2f 6772 6170 6865 6d79  MDoreto/graphemy
-000005e0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-000005f0: 3f74 6f6b 656e 3d47 4a44 4d56 4241 3432  ?token=GJDMVBA42
-00000600: 3529 5d28 6874 7470 733a 2f2f 636f 6465  5)](https://code
-00000610: 636f 762e 696f 2f67 682f 4d44 6f72 6574  cov.io/gh/MDoret
-00000620: 6f2f 6772 6170 6865 6d79 290a 215b 4349  o/graphemy).![CI
-00000630: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000640: 2e63 6f6d 2f4d 446f 7265 746f 2f67 7261  .com/MDoreto/gra
-00000650: 7068 656d 792f 6163 7469 6f6e 732f 776f  phemy/actions/wo
-00000660: 726b 666c 6f77 732f 7069 7065 6c69 6e65  rkflows/pipeline
-00000670: 2e79 6d6c 2f62 6164 6765 2e73 7667 290a  .yml/badge.svg).
-00000680: 0a41 2050 7974 686f 6e20 6c69 6272 6172  .A Python librar
-00000690: 7920 666f 7220 696e 7465 6772 6174 696e  y for integratin
-000006a0: 6720 5351 4c4d 6f64 656c 2061 6e64 2053  g SQLModel and S
-000006b0: 7472 6177 6265 7272 792c 2070 726f 7669  trawberry, provi
-000006c0: 6469 6e67 2061 2073 6561 6d6c 6573 7320  ding a seamless 
-000006d0: 4772 6170 6851 4c20 696e 7465 6772 6174  GraphQL integrat
-000006e0: 696f 6e20 7769 7468 2046 6173 7441 5049  ion with FastAPI
-000006f0: 2061 6e64 2061 6476 616e 6365 6420 6665   and advanced fe
-00000700: 6174 7572 6573 2066 6f72 2064 6174 6162  atures for datab
-00000710: 6173 6520 696e 7465 7261 6374 696f 6e73  ase interactions
-00000720: 2e0a 0a0a 2323 204f 7665 7276 6965 770a  ....## Overview.
-00000730: 0a54 6865 2047 7261 7068 656d 7920 6973  .The Graphemy is
-00000740: 2064 6573 6967 6e65 6420 746f 2073 696d   designed to sim
-00000750: 706c 6966 7920 616e 6420 7374 7265 616d  plify and stream
-00000760: 6c69 6e65 2074 6865 2069 6e74 6567 7261  line the integra
-00000770: 7469 6f6e 206f 6620 5351 4c4d 6f64 656c  tion of SQLModel
-00000780: 2061 6e64 2053 7472 6177 6265 7272 7920   and Strawberry 
-00000790: 696e 2050 7974 686f 6e20 7072 6f6a 6563  in Python projec
-000007a0: 7473 2e20 5468 6973 206c 6962 7261 7279  ts. This library
-000007b0: 2061 6c6c 6f77 7320 796f 7520 746f 2063   allows you to c
-000007c0: 7265 6174 6520 6120 7369 6e67 6c65 2063  reate a single c
-000007d0: 6c61 7373 206d 6f64 656c 2c20 7768 6963  lass model, whic
-000007e0: 682c 206f 6e63 6520 6465 636c 6172 6564  h, once declared
-000007f0: 2c20 6175 746f 6d61 7469 6361 6c6c 7920  , automatically 
-00000800: 7072 6f76 6964 6573 2047 7261 7068 514c  provides GraphQL
-00000810: 2071 7565 7269 6573 2076 6961 2053 7472   queries via Str
-00000820: 6177 6265 7272 792e 2054 6865 7365 2071  awberry. These q
-00000830: 7565 7269 6573 2063 616e 2062 6520 6561  ueries can be ea
-00000840: 7369 6c79 2069 6e74 6567 7261 7465 6420  sily integrated 
-00000850: 696e 746f 2061 2046 6173 7441 5049 2062  into a FastAPI b
-00000860: 6163 6b65 6e64 2e20 416c 6c20 6765 6e65  ackend. All gene
-00000870: 7261 7465 6420 726f 7574 6573 2069 6e63  rated routes inc
-00000880: 6c75 6465 2066 696c 7465 7273 206f 6e20  lude filters on 
-00000890: 616c 6c20 6669 656c 6473 2c20 696e 636c  all fields, incl
-000008a0: 7564 696e 6720 6120 6375 7374 6f6d 2064  uding a custom d
-000008b0: 6174 6520 6669 6c74 6572 2e20 4164 6469  ate filter. Addi
-000008c0: 7469 6f6e 616c 6c79 2c20 6974 2066 6163  tionally, it fac
-000008d0: 696c 6974 6174 6573 2074 6865 2063 7265  ilitates the cre
-000008e0: 6174 696f 6e20 6f66 206d 7574 6174 696f  ation of mutatio
-000008f0: 6e73 2066 6f72 2064 6174 6120 6d6f 6469  ns for data modi
-00000900: 6669 6361 7469 6f6e 2061 6e64 2064 656c  fication and del
-00000910: 6574 696f 6e20 6279 2073 696d 706c 7920  etion by simply 
-00000920: 7365 7474 696e 6720 6120 7661 7269 6162  setting a variab
-00000930: 6c65 2069 6e20 7468 6520 6d6f 6465 6c2e  le in the model.
-00000940: 2054 6865 206c 6962 7261 7279 2061 6c73   The library als
-00000950: 6f20 6861 6e64 6c65 7320 7461 626c 6520  o handles table 
-00000960: 7265 6c61 7469 6f6e 7368 6970 7320 6566  relationships ef
-00000970: 6669 6369 656e 746c 7920 7573 696e 6720  ficiently using 
-00000980: 5374 7261 7762 6572 7279 2773 2064 6174  Strawberry's dat
-00000990: 616c 6f61 6465 7273 2c20 7072 6f76 6964  aloaders, provid
-000009a0: 696e 6720 6120 7369 676e 6966 6963 616e  ing a significan
-000009b0: 7420 7065 7266 6f72 6d61 6e63 6520 626f  t performance bo
-000009c0: 6f73 742e 204d 6f72 656f 7665 722c 2069  ost. Moreover, i
-000009d0: 7420 6f66 6665 7273 2061 2070 7265 2d63  t offers a pre-c
-000009e0: 6f6e 6669 6775 7265 6420 6175 7468 656e  onfigured authen
-000009f0: 7469 6361 7469 6f6e 2073 6574 7570 2c20  tication setup, 
-00000a00: 7768 6963 6820 6361 6e20 6265 2063 6f6e  which can be con
-00000a10: 6669 6775 7265 6420 7769 7468 206a 7573  figured with jus
-00000a20: 7420 7477 6f20 6675 6e63 7469 6f6e 732e  t two functions.
-00000a30: 0a0a 2323 2046 6561 7475 7265 730a 0a2d  ..## Features..-
-00000a40: 2049 6e74 6567 7261 7469 6f6e 206f 6620   Integration of 
-00000a50: 5351 4c4d 6f64 656c 2061 6e64 2053 7472  SQLModel and Str
-00000a60: 6177 6265 7272 7920 666f 7220 4772 6170  awberry for Grap
-00000a70: 6851 4c20 7375 7070 6f72 742e 0a2d 2041  hQL support..- A
-00000a80: 7574 6f6d 6174 6963 2067 656e 6572 6174  utomatic generat
-00000a90: 696f 6e20 6f66 2047 7261 7068 514c 2071  ion of GraphQL q
-00000aa0: 7565 7269 6573 2066 6f72 2046 6173 7441  ueries for FastA
-00000ab0: 5049 2e0a 2d20 506f 7765 7266 756c 2066  PI..- Powerful f
-00000ac0: 696c 7465 7269 6e67 2063 6170 6162 696c  iltering capabil
-00000ad0: 6974 6965 732c 2069 6e63 6c75 6469 6e67  ities, including
-00000ae0: 2063 7573 746f 6d20 6461 7465 2066 696c   custom date fil
-00000af0: 7465 7273 2e0a 2d20 4566 666f 7274 6c65  ters..- Effortle
-00000b00: 7373 2063 7265 6174 696f 6e20 6f66 206d  ss creation of m
-00000b10: 7574 6174 696f 6e73 2066 6f72 2064 6174  utations for dat
-00000b20: 6120 6d61 6e69 7075 6c61 7469 6f6e 2e0a  a manipulation..
-00000b30: 2d20 4566 6669 6369 656e 7420 6861 6e64  - Efficient hand
-00000b40: 6c69 6e67 206f 6620 7461 626c 6520 7265  ling of table re
-00000b50: 6c61 7469 6f6e 7368 6970 7320 7573 696e  lationships usin
-00000b60: 6720 5374 7261 7762 6572 7279 2773 2064  g Strawberry's d
-00000b70: 6174 616c 6f61 6465 7273 2e0a 2d20 5072  ataloaders..- Pr
-00000b80: 652d 636f 6e66 6967 7572 6564 2061 7574  e-configured aut
-00000b90: 6865 6e74 6963 6174 696f 6e20 7365 7475  hentication setu
-00000ba0: 7020 666f 7220 6561 7379 2063 6f6e 6669  p for easy confi
-00000bb0: 6775 7261 7469 6f6e 2e0a 0a23 2320 5072  guration...## Pr
-00000bc0: 6572 6571 7569 7369 7465 730a 0a42 6566  erequisites..Bef
-00000bd0: 6f72 6520 796f 7520 6265 6769 6e20 7573  ore you begin us
-00000be0: 696e 6720 4772 6170 6865 6d79 2c20 6974  ing Graphemy, it
-00000bf0: 2069 7320 6869 6768 6c79 2072 6563 6f6d   is highly recom
-00000c00: 6d65 6e64 6564 2074 6861 7420 796f 7520  mended that you 
-00000c10: 6861 7665 2073 6f6d 6520 7072 696f 7220  have some prior 
-00000c20: 6b6e 6f77 6c65 6467 6520 6f66 2074 6865  knowledge of the
-00000c30: 2065 7373 656e 7469 616c 206c 6962 7261   essential libra
-00000c40: 7269 6573 2075 706f 6e20 7768 6963 6820  ries upon which 
-00000c50: 7468 6973 2070 726f 6a65 6374 2069 7320  this project is 
-00000c60: 6275 696c 742e 2054 6869 7320 7769 6c6c  built. This will
-00000c70: 2068 656c 7020 796f 7520 6d61 6b65 2074   help you make t
-00000c80: 6865 206d 6f73 7420 6f66 2074 6865 2066  he most of the f
-00000c90: 6561 7475 7265 7320 616e 6420 6361 7272  eatures and carr
-00000ca0: 7920 6f75 7420 696e 7465 6772 6174 696f  y out integratio
-00000cb0: 6e73 206d 6f72 6520 6566 6665 6374 6976  ns more effectiv
-00000cc0: 656c 792e 2050 6c65 6173 6520 6d61 6b65  ely. Please make
-00000cd0: 2073 7572 6520 796f 7520 6172 6520 6661   sure you are fa
-00000ce0: 6d69 6c69 6172 2077 6974 6820 7468 6520  miliar with the 
-00000cf0: 666f 6c6c 6f77 696e 6720 6c69 6272 6172  following librar
-00000d00: 6965 733a 0a0a 2a2a 4661 7374 4150 492a  ies:..**FastAPI*
-00000d10: 2a3a 2041 206d 6f64 6572 6e20 6672 616d  *: A modern fram
-00000d20: 6577 6f72 6b20 666f 7220 6275 696c 6469  ework for buildi
-00000d30: 6e67 2066 6173 7420 7765 6220 4150 4973  ng fast web APIs
-00000d40: 2077 6974 6820 5079 7468 6f6e 2e20 4966   with Python. If
-00000d50: 2079 6f75 2061 7265 206e 6f74 2061 6c72   you are not alr
-00000d60: 6561 6479 2066 616d 696c 6961 7220 7769  eady familiar wi
-00000d70: 7468 2046 6173 7441 5049 2c20 796f 7520  th FastAPI, you 
-00000d80: 6361 6e20 7265 6665 7220 746f 2074 6865  can refer to the
-00000d90: 205b 4661 7374 4150 4920 646f 6375 6d65   [FastAPI docume
-00000da0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000db0: 2f66 6173 7461 7069 2e74 6961 6e67 6f6c  /fastapi.tiangol
-00000dc0: 6f2e 636f 6d2f 292e 0a0a 2a2a 5351 4c4d  o.com/)...**SQLM
-00000dd0: 6f64 656c 2a2a 3a20 416e 206f 626a 6563  odel**: An objec
-00000de0: 742d 7265 6c61 7469 6f6e 616c 206d 6170  t-relational map
-00000df0: 7069 6e67 2028 4f52 4d29 206c 6962 7261  ping (ORM) libra
-00000e00: 7279 2066 6f72 2050 7974 686f 6e20 7468  ry for Python th
-00000e10: 6174 2073 696d 706c 6966 6965 7320 616e  at simplifies an
-00000e20: 6420 7374 7265 616d 6c69 6e65 7320 6461  d streamlines da
-00000e30: 7461 6261 7365 2069 6e74 6572 6163 7469  tabase interacti
-00000e40: 6f6e 732e 2054 6f20 6c65 6172 6e20 6d6f  ons. To learn mo
-00000e50: 7265 2061 626f 7574 2053 514c 4d6f 6465  re about SQLMode
-00000e60: 6c2c 2076 6973 6974 2074 6865 205b 5351  l, visit the [SQ
-00000e70: 4c4d 6f64 656c 2064 6f63 756d 656e 7461  LModel documenta
-00000e80: 7469 6f6e 5d28 6874 7470 733a 2f2f 7371  tion](https://sq
-00000e90: 6c6d 6f64 656c 2e74 6961 6e67 6f6c 6f2e  lmodel.tiangolo.
-00000ea0: 636f 6d2f 292e 0a0a 2a2a 5374 7261 7762  com/)...**Strawb
-00000eb0: 6572 7279 2a2a 3a20 4120 5079 7468 6f6e  erry**: A Python
-00000ec0: 206c 6962 7261 7279 2066 6f72 2064 6563   library for dec
-00000ed0: 6c61 7261 7469 7665 6c79 2063 7265 6174  laratively creat
-00000ee0: 696e 6720 4772 6170 6851 4c20 7363 6865  ing GraphQL sche
-00000ef0: 6d61 732e 2046 6f72 2069 6e2d 6465 7074  mas. For in-dept
-00000f00: 6820 696e 666f 726d 6174 696f 6e20 6f6e  h information on
-00000f10: 2075 7369 6e67 2053 7472 6177 6265 7272   using Strawberr
-00000f20: 792c 2061 6363 6573 7320 7468 6520 5b53  y, access the [S
-00000f30: 7472 6177 6265 7272 7920 646f 6375 6d65  trawberry docume
-00000f40: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000f50: 2f73 7472 6177 6265 7272 792e 726f 636b  /strawberry.rock
-00000f60: 732f 292e 0a0a 4861 7669 6e67 2061 2073  s/)...Having a s
-00000f70: 6f6c 6964 2075 6e64 6572 7374 616e 6469  olid understandi
-00000f80: 6e67 206f 6620 7468 6573 6520 6c69 6272  ng of these libr
-00000f90: 6172 6965 7320 6973 2063 7275 6369 616c  aries is crucial
-00000fa0: 2074 6f20 6d61 6b69 6e67 2074 6865 206d   to making the m
-00000fb0: 6f73 7420 6f66 2050 726f 6a65 6374 204e  ost of Project N
-00000fc0: 616d 6520 616e 6420 6566 666f 7274 6c65  ame and effortle
-00000fd0: 7373 6c79 2063 7265 6174 696e 6720 4772  ssly creating Gr
-00000fe0: 6170 6851 4c20 4150 4973 2e0a 0a23 2320  aphQL APIs...## 
-00000ff0: 4372 6561 7465 2061 2050 726f 6a65 6374  Create a Project
-00001000: 0a0a 4920 7265 636f 6d65 6e64 2079 6f75  ..I recomend you
-00001010: 2075 7365 2050 6f65 7472 792c 2062 7574   use Poetry, but
-00001020: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00001030: 2065 6e76 6972 6f6d 656e 7420 6d61 6e61   enviroment mana
-00001040: 6765 7220 7468 6174 2079 6f75 2077 616e  ger that you wan
-00001050: 742e 2053 6f20 6966 2079 6f75 2061 7265  t. So if you are
-00001060: 2075 7369 6e67 2070 6f65 7472 792c 2073   using poetry, s
-00001070: 7461 7274 2074 6865 2070 726f 6a65 6374  tart the project
-00001080: 3a0a 0a60 6060 6261 7368 0a23 2043 7265  :..```bash.# Cre
-00001090: 6174 6520 706f 6574 7279 2070 726f 6a65  ate poetry proje
-000010a0: 6374 0a70 6f65 7472 7920 6e65 7720 6772  ct.poetry new gr
-000010b0: 6170 6865 6d79 2074 7574 6f72 6961 6c0a  aphemy tutorial.
-000010c0: 0a23 2053 7461 7274 2045 6e76 6972 6f6e  .# Start Environ
-000010d0: 6d65 6e74 200a 706f 6574 7279 2073 6865  ment .poetry she
-000010e0: 6c6c 0a60 6060 0a0a 596f 7520 6361 6e20  ll.```..You can 
-000010f0: 616c 736f 2075 7365 2074 6865 2065 6e76  also use the env
-00001100: 6972 6f6e 6d65 6e74 206d 616e 6167 6572  ironment manager
-00001110: 2077 616e 7465 642c 2073 7563 6820 6173   wanted, such as
-00001120: 2076 6972 7475 616c 656e 760a 0a60 6060   virtualenv..```
-00001130: 6261 7368 0a23 2043 7265 6174 6520 6120  bash.# Create a 
-00001140: 6469 7265 6374 6f72 7920 666f 7220 7475  directory for tu
-00001150: 746f 7269 616c 0a6d 6b64 6972 2067 7261  torial.mkdir gra
-00001160: 7068 656d 792d 7475 746f 7269 616c 0a0a  phemy-tutorial..
-00001170: 2320 456e 7465 7220 696e 746f 2074 6861  # Enter into tha
-00001180: 7420 6469 7265 6374 6f72 790a 6364 2067  t directory.cd g
-00001190: 7261 7068 656d 790a 0a23 2043 7265 6174  raphemy..# Creat
-000011a0: 6520 7669 7274 7561 6c20 656e 7669 726f  e virtual enviro
-000011b0: 6e6d 656e 740a 7079 7468 6f6e 202d 6d20  nment.python -m 
-000011c0: 7665 6e76 2076 656e 760a 0a23 5374 6172  venv venv..#Star
-000011d0: 7420 456e 7669 726f 6e6d 656e 740a 7665  t Environment.ve
-000011e0: 6e76 2f53 6372 6970 7473 2f41 6374 6976  nv/Scripts/Activ
-000011f0: 6174 650a 6060 600a 0a23 2320 5265 7175  ate.```..## Requ
-00001200: 6972 656d 656e 7473 0a0a 4e6f 7720 696e  irements..Now in
-00001210: 7374 616c 6c20 4772 6170 6865 6d79 203a  stall Graphemy :
-00001220: 2920 0a60 6060 6261 7368 0a70 6f65 7472  ) .```bash.poetr
-00001230: 7920 6164 6420 6772 6170 6865 6d79 0a60  y add graphemy.`
-00001240: 6060 0a4f 7220 7573 696e 6720 6465 6661  ``.Or using defa
-00001250: 756c 7420 7079 7468 6f6e 2065 6e76 2077  ult python env w
-00001260: 6974 6820 7069 703a 0a0a 6060 6062 6173  ith pip:..```bas
-00001270: 680a 7069 7020 696e 7374 616c 6c20 6772  h.pip install gr
-00001280: 6170 6865 6d79 0a60 6060 0a              aphemy.```.
+00000030: 302e 310a 5375 6d6d 6172 793a 2041 2050  0.1.Summary: A P
+00000040: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00000050: 7220 696e 7465 6772 6174 696e 6720 5351  r integrating SQ
+00000060: 4c4d 6f64 656c 2061 6e64 2053 7472 6177  LModel and Straw
+00000070: 6265 7272 792c 2070 726f 7669 6469 6e67  berry, providing
+00000080: 2061 2073 6561 6d6c 6573 7320 4772 6170   a seamless Grap
+00000090: 6851 4c20 696e 7465 6772 6174 696f 6e20  hQL integration 
+000000a0: 7769 7468 2046 6173 7441 5049 2061 6e64  with FastAPI and
+000000b0: 2061 6476 616e 6365 6420 6665 6174 7572   advanced featur
+000000c0: 6573 2066 6f72 2064 6174 6162 6173 6520  es for database 
+000000d0: 696e 7465 7261 6374 696f 6e73 2e0a 486f  interactions..Ho
+000000e0: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+000000f0: 2f67 6974 6875 622e 636f 6d2f 4d44 6f72  /github.com/MDor
+00000100: 6574 6f2f 6772 6170 6865 6d79 0a4c 6963  eto/graphemy.Lic
+00000110: 656e 7365 3a20 4d49 540a 4175 7468 6f72  ense: MIT.Author
+00000120: 3a20 4d61 7468 6575 7320 446f 7265 746f  : Matheus Doreto
+00000130: 0a41 7574 686f 722d 656d 6169 6c3a 206d  .Author-email: m
+00000140: 6174 6865 7573 646f 7265 746f 2e6d 6440  atheusdoreto.md@
+00000150: 676d 6169 6c2e 636f 6d0a 5265 7175 6972  gmail.com.Requir
+00000160: 6573 2d50 7974 686f 6e3a 203e 3d33 2e31  es-Python: >=3.1
+00000170: 322c 3c34 2e30 0a43 6c61 7373 6966 6965  2,<4.0.Classifie
+00000180: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000190: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+000001a0: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+000001b0: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
+000001c0: 776f 726b 203a 3a20 4661 7374 4150 490a  work :: FastAPI.
+000001d0: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+000001e0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000001f0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
+00000200: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00000210: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000220: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
+00000230: 6c61 7373 6966 6965 723a 204e 6174 7572  lassifier: Natur
+00000240: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
+00000250: 6e67 6c69 7368 0a43 6c61 7373 6966 6965  nglish.Classifie
+00000260: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000270: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000280: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+00000290: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000002a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002b0: 6e20 3a3a 2033 2e31 320a 436c 6173 7369  n :: 3.12.Classi
+000002c0: 6669 6572 3a20 546f 7069 6320 3a3a 2044  fier: Topic :: D
+000002d0: 6174 6162 6173 650a 436c 6173 7369 6669  atabase.Classifi
+000002e0: 6572 3a20 546f 7069 6320 3a3a 2044 6174  er: Topic :: Dat
+000002f0: 6162 6173 6520 3a3a 2044 6174 6162 6173  abase :: Databas
+00000300: 6520 456e 6769 6e65 732f 5365 7276 6572  e Engines/Server
+00000310: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
+00000320: 2066 6173 7461 7069 2028 3e3d 302e 3131   fastapi (>=0.11
+00000330: 312e 302c 3c30 2e31 3132 2e30 290a 5265  1.0,<0.112.0).Re
+00000340: 7175 6972 6573 2d44 6973 743a 2073 716c  quires-Dist: sql
+00000350: 6d6f 6465 6c20 283d 3d30 2e30 2e31 3829  model (==0.0.18)
+00000360: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000370: 7374 7261 7762 6572 7279 2d67 7261 7068  strawberry-graph
+00000380: 716c 5b64 6562 7567 2d73 6572 7665 725d  ql[debug-server]
+00000390: 2028 3e3d 302e 3232 392e 312c 3c30 2e32   (>=0.229.1,<0.2
+000003a0: 3330 2e30 290a 5072 6f6a 6563 742d 5552  30.0).Project-UR
+000003b0: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
+000003c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003d0: 6f6d 2f4d 446f 7265 746f 2f67 7261 7068  om/MDoreto/graph
+000003e0: 656d 792f 6973 7375 6573 0a50 726f 6a65  emy/issues.Proje
+000003f0: 6374 2d55 524c 3a20 446f 6375 6d65 6e74  ct-URL: Document
+00000400: 6174 696f 6e2c 2068 7474 7073 3a2f 2f67  ation, https://g
+00000410: 7261 7068 656d 792e 7265 6164 7468 6564  raphemy.readthed
+00000420: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000430: 2f0a 5072 6f6a 6563 742d 5552 4c3a 2052  /.Project-URL: R
+00000440: 6570 6f73 6974 6f72 792c 2068 7474 7073  epository, https
+00000450: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d44  ://github.com/MD
+00000460: 6f72 6574 6f2f 6772 6170 6865 6d79 0a44  oreto/graphemy.D
+00000470: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000480: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000490: 726b 646f 776e 0a0a 0a3c 7020 616c 6967  rkdown...<p alig
+000004a0: 6e3d 2263 656e 7465 7222 3e0a 2020 3c69  n="center">.  <i
+000004b0: 6d67 2073 7263 3d22 2e2f 646f 6373 2f61  mg src="./docs/a
+000004c0: 7373 6574 732f 6c6f 676f 2e70 6e67 2220  ssets/logo.png" 
+000004d0: 2f3e 0a3c 2f70 3e0a 0a23 2047 5241 5048  />.</p>..# GRAPH
+000004e0: 454d 590a 3c70 2061 6c69 676e 3d22 6365  EMY.<p align="ce
+000004f0: 6e74 6572 223e 0a20 2020 203c 656d 3e49  nter">.    <em>I
+00000500: 6e74 6567 7261 7469 6e67 2053 514c 4d6f  ntegrating SQLMo
+00000510: 6465 6c20 616e 6420 5374 7261 7762 6572  del and Strawber
+00000520: 7279 2c20 7072 6f76 6964 696e 6720 6120  ry, providing a 
+00000530: 7365 616d 6c65 7373 2047 7261 7068 514c  seamless GraphQL
+00000540: 2069 6e74 6567 7261 7469 6f6e 2077 6974   integration wit
+00000550: 6820 4461 7461 6261 7365 7320 6561 7379  h Databases easy
+00000560: 2061 6e64 2066 6173 742e 3c2f 656d 3e0a   and fast.</em>.
+00000570: 3c2f 703e 0a0a 5b21 5b44 6f63 756d 656e  </p>..[![Documen
+00000580: 7461 7469 6f6e 2053 7461 7475 735d 2868  tation Status](h
+00000590: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
+000005a0: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
+000005b0: 6772 6170 6865 6d79 2f62 6164 6765 2f3f  graphemy/badge/?
+000005c0: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
+000005d0: 2868 7474 7073 3a2f 2f67 7261 7068 656d  (https://graphem
+000005e0: 792e 7265 6164 7468 6564 6f63 732e 696f  y.readthedocs.io
+000005f0: 2f65 6e2f 6c61 7465 7374 2f3f 6261 6467  /en/latest/?badg
+00000600: 653d 6c61 7465 7374 290a 5b21 5b63 6f64  e=latest).[![cod
+00000610: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
+00000620: 6465 636f 762e 696f 2f67 682f 4d44 6f72  decov.io/gh/MDor
+00000630: 6574 6f2f 6772 6170 6865 6d79 2f67 7261  eto/graphemy/gra
+00000640: 7068 2f62 6164 6765 2e73 7667 3f74 6f6b  ph/badge.svg?tok
+00000650: 656e 3d47 4a44 4d56 4241 3432 3529 5d28  en=GJDMVBA425)](
+00000660: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000670: 696f 2f67 682f 4d44 6f72 6574 6f2f 6772  io/gh/MDoreto/gr
+00000680: 6170 6865 6d79 290a 215b 4349 5d28 6874  aphemy).![CI](ht
+00000690: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006a0: 2f4d 446f 7265 746f 2f67 7261 7068 656d  /MDoreto/graphem
+000006b0: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
+000006c0: 6f77 732f 7069 7065 6c69 6e65 2e79 6d6c  ows/pipeline.yml
+000006d0: 2f62 6164 6765 2e73 7667 290a 3c61 2068  /badge.svg).<a h
+000006e0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000006f0: 692e 6f72 672f 7072 6f6a 6563 742f 6772  i.org/project/gr
+00000700: 6170 6865 6d79 2220 7461 7267 6574 3d22  aphemy" target="
+00000710: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
+00000720: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000730: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000740: 7069 2f76 2f67 7261 7068 656d 793f 636f  pi/v/graphemy?co
+00000750: 6c6f 723d 2532 3333 3444 3035 3826 6c61  lor=%2334D058&la
+00000760: 6265 6c3d 7079 7069 2532 3070 6163 6b61  bel=pypi%20packa
+00000770: 6765 2220 616c 743d 2250 6163 6b61 6765  ge" alt="Package
+00000780: 2076 6572 7369 6f6e 223e 0a3c 2f61 3e0a   version">.</a>.
+00000790: 0a0a 2d2d 2d0a 0a2a 2a44 6f63 756d 656e  ..---..**Documen
+000007a0: 7461 7469 6f6e 2a2a 3a20 3c61 2068 7265  tation**: <a hre
+000007b0: 663d 2268 7474 7073 3a2f 2f67 7261 7068  f="https://graph
+000007c0: 656d 792e 7265 6164 7468 6564 6f63 732e  emy.readthedocs.
+000007d0: 696f 2220 7461 7267 6574 3d22 5f62 6c61  io" target="_bla
+000007e0: 6e6b 223e 6874 7470 733a 2f2f 6772 6170  nk">https://grap
+000007f0: 6865 6d79 2e72 6561 6474 6865 646f 6373  hemy.readthedocs
+00000800: 2e69 6f3c 2f61 3e0a 0a2a 2a53 6f75 7263  .io</a>..**Sourc
+00000810: 6520 436f 6465 2a2a 3a20 3c61 2068 7265  e Code**: <a hre
+00000820: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000830: 622e 636f 6d2f 4d44 6f72 6574 6f2f 6772  b.com/MDoreto/gr
+00000840: 6170 6865 6d79 2220 7461 7267 6574 3d22  aphemy" target="
+00000850: 5f62 6c61 6e6b 223e 6874 7470 733a 2f2f  _blank">https://
+00000860: 6769 7468 7562 2e63 6f6d 2f4d 446f 7265  github.com/MDore
+00000870: 746f 2f67 7261 7068 656d 793c 2f61 3e0a  to/graphemy</a>.
+00000880: 0a2d 2d2d 0a0a 0a23 2320 4f76 6572 7669  .---...## Overvi
+00000890: 6577 0a0a 5468 6520 4772 6170 6865 6d79  ew..The Graphemy
+000008a0: 2069 7320 6465 7369 676e 6564 2074 6f20   is designed to 
+000008b0: 7369 6d70 6c69 6679 2061 6e64 2073 7472  simplify and str
+000008c0: 6561 6d6c 696e 6520 7468 6520 696e 7465  eamline the inte
+000008d0: 6772 6174 696f 6e20 6f66 2053 514c 4d6f  gration of SQLMo
+000008e0: 6465 6c20 616e 6420 5374 7261 7762 6572  del and Strawber
+000008f0: 7279 2069 6e20 5079 7468 6f6e 2070 726f  ry in Python pro
+00000900: 6a65 6374 732e 2054 6869 7320 6c69 6272  jects. This libr
+00000910: 6172 7920 616c 6c6f 7773 2079 6f75 2074  ary allows you t
+00000920: 6f20 6372 6561 7465 2061 2073 696e 676c  o create a singl
+00000930: 6520 636c 6173 7320 6d6f 6465 6c2c 2077  e class model, w
+00000940: 6869 6368 2c20 6f6e 6365 2064 6563 6c61  hich, once decla
+00000950: 7265 642c 2061 7574 6f6d 6174 6963 616c  red, automatical
+00000960: 6c79 2070 726f 7669 6465 7320 4772 6170  ly provides Grap
+00000970: 6851 4c20 7175 6572 6965 7320 7669 6120  hQL queries via 
+00000980: 5374 7261 7762 6572 7279 2e20 5468 6573  Strawberry. Thes
+00000990: 6520 7175 6572 6965 7320 6361 6e20 6265  e queries can be
+000009a0: 2065 6173 696c 7920 696e 7465 6772 6174   easily integrat
+000009b0: 6564 2069 6e74 6f20 6120 4661 7374 4150  ed into a FastAP
+000009c0: 4920 6261 636b 656e 642e 2041 6c6c 2067  I backend. All g
+000009d0: 656e 6572 6174 6564 2072 6f75 7465 7320  enerated routes 
+000009e0: 696e 636c 7564 6520 6669 6c74 6572 7320  include filters 
+000009f0: 6f6e 2061 6c6c 2066 6965 6c64 732c 2069  on all fields, i
+00000a00: 6e63 6c75 6469 6e67 2061 2063 7573 746f  ncluding a custo
+00000a10: 6d20 6461 7465 2066 696c 7465 722e 2041  m date filter. A
+00000a20: 6464 6974 696f 6e61 6c6c 792c 2069 7420  dditionally, it 
+00000a30: 6661 6369 6c69 7461 7465 7320 7468 6520  facilitates the 
+00000a40: 6372 6561 7469 6f6e 206f 6620 6d75 7461  creation of muta
+00000a50: 7469 6f6e 7320 666f 7220 6461 7461 206d  tions for data m
+00000a60: 6f64 6966 6963 6174 696f 6e20 616e 6420  odification and 
+00000a70: 6465 6c65 7469 6f6e 2062 7920 7369 6d70  deletion by simp
+00000a80: 6c79 2073 6574 7469 6e67 2061 2076 6172  ly setting a var
+00000a90: 6961 626c 6520 696e 2074 6865 206d 6f64  iable in the mod
+00000aa0: 656c 2e20 5468 6520 6c69 6272 6172 7920  el. The library 
+00000ab0: 616c 736f 2068 616e 646c 6573 2074 6162  also handles tab
+00000ac0: 6c65 2072 656c 6174 696f 6e73 6869 7073  le relationships
+00000ad0: 2065 6666 6963 6965 6e74 6c79 2075 7369   efficiently usi
+00000ae0: 6e67 2053 7472 6177 6265 7272 7927 7320  ng Strawberry's 
+00000af0: 6461 7461 6c6f 6164 6572 732c 2070 726f  dataloaders, pro
+00000b00: 7669 6469 6e67 2061 2073 6967 6e69 6669  viding a signifi
+00000b10: 6361 6e74 2070 6572 666f 726d 616e 6365  cant performance
+00000b20: 2062 6f6f 7374 2e20 4d6f 7265 6f76 6572   boost. Moreover
+00000b30: 2c20 6974 206f 6666 6572 7320 6120 7072  , it offers a pr
+00000b40: 652d 636f 6e66 6967 7572 6564 2061 7574  e-configured aut
+00000b50: 6865 6e74 6963 6174 696f 6e20 7365 7475  hentication setu
+00000b60: 702c 2077 6869 6368 2063 616e 2062 6520  p, which can be 
+00000b70: 636f 6e66 6967 7572 6564 2077 6974 6820  configured with 
+00000b80: 6a75 7374 2074 776f 2066 756e 6374 696f  just two functio
+00000b90: 6e73 2e0a 0a23 2320 4665 6174 7572 6573  ns...## Features
+00000ba0: 0a0a 2d20 496e 7465 6772 6174 696f 6e20  ..- Integration 
+00000bb0: 6f66 2053 514c 4d6f 6465 6c20 616e 6420  of SQLModel and 
+00000bc0: 5374 7261 7762 6572 7279 2066 6f72 2047  Strawberry for G
+00000bd0: 7261 7068 514c 2073 7570 706f 7274 2e0a  raphQL support..
+00000be0: 2d20 4175 746f 6d61 7469 6320 6765 6e65  - Automatic gene
+00000bf0: 7261 7469 6f6e 206f 6620 4772 6170 6851  ration of GraphQ
+00000c00: 4c20 7175 6572 6965 7320 666f 7220 4661  L queries for Fa
+00000c10: 7374 4150 492e 0a2d 2050 6f77 6572 6675  stAPI..- Powerfu
+00000c20: 6c20 6669 6c74 6572 696e 6720 6361 7061  l filtering capa
+00000c30: 6269 6c69 7469 6573 2c20 696e 636c 7564  bilities, includ
+00000c40: 696e 6720 6375 7374 6f6d 2064 6174 6520  ing custom date 
+00000c50: 6669 6c74 6572 732e 0a2d 2045 6666 6f72  filters..- Effor
+00000c60: 746c 6573 7320 6372 6561 7469 6f6e 206f  tless creation o
+00000c70: 6620 6d75 7461 7469 6f6e 7320 666f 7220  f mutations for 
+00000c80: 6461 7461 206d 616e 6970 756c 6174 696f  data manipulatio
+00000c90: 6e2e 0a2d 2045 6666 6963 6965 6e74 2068  n..- Efficient h
+00000ca0: 616e 646c 696e 6720 6f66 2074 6162 6c65  andling of table
+00000cb0: 2072 656c 6174 696f 6e73 6869 7073 2075   relationships u
+00000cc0: 7369 6e67 2053 7472 6177 6265 7272 7927  sing Strawberry'
+00000cd0: 7320 6461 7461 6c6f 6164 6572 732e 0a2d  s dataloaders..-
+00000ce0: 2050 7265 2d63 6f6e 6669 6775 7265 6420   Pre-configured 
+00000cf0: 6175 7468 656e 7469 6361 7469 6f6e 2073  authentication s
+00000d00: 6574 7570 2066 6f72 2065 6173 7920 636f  etup for easy co
+00000d10: 6e66 6967 7572 6174 696f 6e2e 0a0a 2323  nfiguration...##
+00000d20: 2050 7265 7265 7175 6973 6974 6573 0a0a   Prerequisites..
+00000d30: 4265 666f 7265 2079 6f75 2062 6567 696e  Before you begin
+00000d40: 2075 7369 6e67 2047 7261 7068 656d 792c   using Graphemy,
+00000d50: 2069 7420 6973 2068 6967 686c 7920 7265   it is highly re
+00000d60: 636f 6d6d 656e 6465 6420 7468 6174 2079  commended that y
+00000d70: 6f75 2068 6176 6520 736f 6d65 2070 7269  ou have some pri
+00000d80: 6f72 206b 6e6f 776c 6564 6765 206f 6620  or knowledge of 
+00000d90: 7468 6520 6573 7365 6e74 6961 6c20 6c69  the essential li
+00000da0: 6272 6172 6965 7320 7570 6f6e 2077 6869  braries upon whi
+00000db0: 6368 2074 6869 7320 7072 6f6a 6563 7420  ch this project 
+00000dc0: 6973 2062 7569 6c74 2e20 5468 6973 2077  is built. This w
+00000dd0: 696c 6c20 6865 6c70 2079 6f75 206d 616b  ill help you mak
+00000de0: 6520 7468 6520 6d6f 7374 206f 6620 7468  e the most of th
+00000df0: 6520 6665 6174 7572 6573 2061 6e64 2063  e features and c
+00000e00: 6172 7279 206f 7574 2069 6e74 6567 7261  arry out integra
+00000e10: 7469 6f6e 7320 6d6f 7265 2065 6666 6563  tions more effec
+00000e20: 7469 7665 6c79 2e20 506c 6561 7365 206d  tively. Please m
+00000e30: 616b 6520 7375 7265 2079 6f75 2061 7265  ake sure you are
+00000e40: 2066 616d 696c 6961 7220 7769 7468 2074   familiar with t
+00000e50: 6865 2066 6f6c 6c6f 7769 6e67 206c 6962  he following lib
+00000e60: 7261 7269 6573 3a0a 0a2a 2a46 6173 7441  raries:..**FastA
+00000e70: 5049 2a2a 3a20 4120 6d6f 6465 726e 2066  PI**: A modern f
+00000e80: 7261 6d65 776f 726b 2066 6f72 2062 7569  ramework for bui
+00000e90: 6c64 696e 6720 6661 7374 2077 6562 2041  lding fast web A
+00000ea0: 5049 7320 7769 7468 2050 7974 686f 6e2e  PIs with Python.
+00000eb0: 2049 6620 796f 7520 6172 6520 6e6f 7420   If you are not 
+00000ec0: 616c 7265 6164 7920 6661 6d69 6c69 6172  already familiar
+00000ed0: 2077 6974 6820 4661 7374 4150 492c 2079   with FastAPI, y
+00000ee0: 6f75 2063 616e 2072 6566 6572 2074 6f20  ou can refer to 
+00000ef0: 7468 6520 5b46 6173 7441 5049 2064 6f63  the [FastAPI doc
+00000f00: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+00000f10: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
+00000f20: 676f 6c6f 2e63 6f6d 2f29 2e0a 0a2a 2a53  golo.com/)...**S
+00000f30: 514c 4d6f 6465 6c2a 2a3a 2041 6e20 6f62  QLModel**: An ob
+00000f40: 6a65 6374 2d72 656c 6174 696f 6e61 6c20  ject-relational 
+00000f50: 6d61 7070 696e 6720 284f 524d 2920 6c69  mapping (ORM) li
+00000f60: 6272 6172 7920 666f 7220 5079 7468 6f6e  brary for Python
+00000f70: 2074 6861 7420 7369 6d70 6c69 6669 6573   that simplifies
+00000f80: 2061 6e64 2073 7472 6561 6d6c 696e 6573   and streamlines
+00000f90: 2064 6174 6162 6173 6520 696e 7465 7261   database intera
+00000fa0: 6374 696f 6e73 2e20 546f 206c 6561 726e  ctions. To learn
+00000fb0: 206d 6f72 6520 6162 6f75 7420 5351 4c4d   more about SQLM
+00000fc0: 6f64 656c 2c20 7669 7369 7420 7468 6520  odel, visit the 
+00000fd0: 5b53 514c 4d6f 6465 6c20 646f 6375 6d65  [SQLModel docume
+00000fe0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000ff0: 2f73 716c 6d6f 6465 6c2e 7469 616e 676f  /sqlmodel.tiango
+00001000: 6c6f 2e63 6f6d 2f29 2e0a 0a2a 2a53 7472  lo.com/)...**Str
+00001010: 6177 6265 7272 792a 2a3a 2041 2050 7974  awberry**: A Pyt
+00001020: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
+00001030: 6465 636c 6172 6174 6976 656c 7920 6372  declaratively cr
+00001040: 6561 7469 6e67 2047 7261 7068 514c 2073  eating GraphQL s
+00001050: 6368 656d 6173 2e20 466f 7220 696e 2d64  chemas. For in-d
+00001060: 6570 7468 2069 6e66 6f72 6d61 7469 6f6e  epth information
+00001070: 206f 6e20 7573 696e 6720 5374 7261 7762   on using Strawb
+00001080: 6572 7279 2c20 6163 6365 7373 2074 6865  erry, access the
+00001090: 205b 5374 7261 7762 6572 7279 2064 6f63   [Strawberry doc
+000010a0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000010b0: 733a 2f2f 7374 7261 7762 6572 7279 2e72  s://strawberry.r
+000010c0: 6f63 6b73 2f29 2e0a 0a48 6176 696e 6720  ocks/)...Having 
+000010d0: 6120 736f 6c69 6420 756e 6465 7273 7461  a solid understa
+000010e0: 6e64 696e 6720 6f66 2074 6865 7365 206c  nding of these l
+000010f0: 6962 7261 7269 6573 2069 7320 6372 7563  ibraries is cruc
+00001100: 6961 6c20 746f 206d 616b 696e 6720 7468  ial to making th
+00001110: 6520 6d6f 7374 206f 6620 4772 6170 6865  e most of Graphe
+00001120: 6d79 2061 6e64 2065 6666 6f72 746c 6573  my and effortles
+00001130: 736c 7920 6372 6561 7469 6e67 2047 7261  sly creating Gra
+00001140: 7068 514c 2041 5049 732e 0a0a 2323 2043  phQL APIs...## C
+00001150: 7265 6174 6520 6120 5072 6f6a 6563 740a  reate a Project.
+00001160: 0a49 2072 6563 6f6d 656e 6420 796f 7520  .I recomend you 
+00001170: 7573 6520 506f 6574 7279 2c20 6275 7420  use Poetry, but 
+00001180: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
+00001190: 656e 7669 726f 6d65 6e74 206d 616e 6167  enviroment manag
+000011a0: 6572 2074 6861 7420 796f 7520 7761 6e74  er that you want
+000011b0: 2e20 536f 2069 6620 796f 7520 6172 6520  . So if you are 
+000011c0: 7573 696e 6720 706f 6574 7279 2c20 7374  using poetry, st
+000011d0: 6172 7420 7468 6520 7072 6f6a 6563 743a  art the project:
+000011e0: 0a0a 6060 6062 6173 680a 2320 4372 6561  ..```bash.# Crea
+000011f0: 7465 2070 6f65 7472 7920 7072 6f6a 6563  te poetry projec
+00001200: 740a 706f 6574 7279 206e 6577 2067 7261  t.poetry new gra
+00001210: 7068 656d 7920 7475 746f 7269 616c 0a0a  phemy tutorial..
+00001220: 2320 5374 6172 7420 456e 7669 726f 6e6d  # Start Environm
+00001230: 656e 7420 0a70 6f65 7472 7920 7368 656c  ent .poetry shel
+00001240: 6c0a 6060 600a 0a59 6f75 2063 616e 2061  l.```..You can a
+00001250: 6c73 6f20 7573 6520 7468 6520 656e 7669  lso use the envi
+00001260: 726f 6e6d 656e 7420 6d61 6e61 6765 7220  ronment manager 
+00001270: 7761 6e74 6564 2c20 7375 6368 2061 7320  wanted, such as 
+00001280: 7669 7274 7561 6c65 6e76 0a0a 6060 6062  virtualenv..```b
+00001290: 6173 680a 2320 4372 6561 7465 2061 2064  ash.# Create a d
+000012a0: 6972 6563 746f 7279 2066 6f72 2074 7574  irectory for tut
+000012b0: 6f72 6961 6c0a 6d6b 6469 7220 6772 6170  orial.mkdir grap
+000012c0: 6865 6d79 2d74 7574 6f72 6961 6c0a 0a23  hemy-tutorial..#
+000012d0: 2045 6e74 6572 2069 6e74 6f20 7468 6174   Enter into that
+000012e0: 2064 6972 6563 746f 7279 0a63 6420 6772   directory.cd gr
+000012f0: 6170 6865 6d79 0a0a 2320 4372 6561 7465  aphemy..# Create
+00001300: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+00001310: 6d65 6e74 0a70 7974 686f 6e20 2d6d 2076  ment.python -m v
+00001320: 656e 7620 7665 6e76 0a0a 2353 7461 7274  env venv..#Start
+00001330: 2045 6e76 6972 6f6e 6d65 6e74 0a76 656e   Environment.ven
+00001340: 762f 5363 7269 7074 732f 4163 7469 7661  v/Scripts/Activa
+00001350: 7465 0a60 6060 0a0a 2323 2052 6571 7569  te.```..## Requi
+00001360: 7265 6d65 6e74 730a 0a4e 6f77 2069 6e73  rements..Now ins
+00001370: 7461 6c6c 2047 7261 7068 656d 7920 3a29  tall Graphemy :)
+00001380: 200a 6060 6062 6173 680a 706f 6574 7279   .```bash.poetry
+00001390: 2061 6464 2067 7261 7068 656d 790a 6060   add graphemy.``
+000013a0: 600a 4f72 2075 7369 6e67 2064 6566 6175  `.Or using defau
+000013b0: 6c74 2070 7974 686f 6e20 656e 7620 7769  lt python env wi
+000013c0: 7468 2070 6970 3a0a 0a60 6060 6261 7368  th pip:..```bash
+000013d0: 0a70 6970 2069 6e73 7461 6c6c 2067 7261  .pip install gra
+000013e0: 7068 656d 790a 6060 600a 0a              phemy.```..
```

