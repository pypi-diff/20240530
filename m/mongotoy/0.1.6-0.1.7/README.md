# Comparing `tmp/mongotoy-0.1.6.tar.gz` & `tmp/mongotoy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotoy-0.1.6.tar", max compression
+gzip compressed data, was "mongotoy-0.1.7.tar", max compression
```

## Comparing `mongotoy-0.1.6.tar` & `mongotoy-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.6/LICENSE
--rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.6/mongotoy/__init__.py
--rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.6/mongotoy/cache.py
--rw-r--r--   0        0        0    49525 2024-05-20 17:47:01.468567 mongotoy-0.1.6/mongotoy/db.py
--rw-r--r--   0        0        0    16382 2024-04-04 16:29:46.366685 mongotoy-0.1.6/mongotoy/documents.py
--rw-r--r--   0        0        0     6693 2024-04-03 17:32:35.942331 mongotoy-0.1.6/mongotoy/errors.py
--rw-r--r--   0        0        0     7731 2024-04-15 16:35:24.067748 mongotoy-0.1.6/mongotoy/expressions.py
--rw-r--r--   0        0        0    13701 2024-05-20 17:54:14.699669 mongotoy-0.1.6/mongotoy/fields.py
--rw-r--r--   0        0        0     2231 2024-03-18 19:06:51.253634 mongotoy-0.1.6/mongotoy/geodata.py
--rw-r--r--   0        0        0    41509 2024-05-20 18:39:19.540368 mongotoy-0.1.6/mongotoy/mappers.py
--rw-r--r--   0        0        0     5415 2024-04-04 16:29:08.681600 mongotoy-0.1.6/mongotoy/references.py
--rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.6/mongotoy/sync.py
--rw-r--r--   0        0        0    11992 2024-04-17 17:44:47.007889 mongotoy-0.1.6/mongotoy/types.py
--rw-r--r--   0        0        0      715 2024-05-20 18:40:07.576988 mongotoy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6484 2024-04-14 05:31:35.928668 mongotoy-0.1.6/README.md
--rw-r--r--   0        0        0     7128 1970-01-01 00:00:00.000000 mongotoy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-02-23 16:52:07.516625 mongotoy-0.1.7/LICENSE
+-rw-r--r--   0        0        0      151 2024-04-06 23:50:55.339800 mongotoy-0.1.7/mongotoy/__init__.py
+-rw-r--r--   0        0        0     2342 2024-03-18 19:02:50.653179 mongotoy-0.1.7/mongotoy/cache.py
+-rw-r--r--   0        0        0    51073 2024-05-25 17:45:12.573856 mongotoy-0.1.7/mongotoy/db.py
+-rw-r--r--   0        0        0    17816 2024-05-24 18:57:39.792740 mongotoy-0.1.7/mongotoy/documents.py
+-rw-r--r--   0        0        0     6484 2024-05-23 17:21:28.373060 mongotoy-0.1.7/mongotoy/errors.py
+-rw-r--r--   0        0        0    10476 2024-05-25 21:20:20.166550 mongotoy-0.1.7/mongotoy/expressions.py
+-rw-r--r--   0        0        0    13355 2024-05-23 18:18:50.441822 mongotoy-0.1.7/mongotoy/fields.py
+-rw-r--r--   0        0        0     5499 2024-05-25 18:07:39.801209 mongotoy-0.1.7/mongotoy/geodata.py
+-rw-r--r--   0        0        0    41732 2024-05-23 17:44:07.699063 mongotoy-0.1.7/mongotoy/mappers.py
+-rw-r--r--   0        0        0     5415 2024-05-24 17:43:55.411153 mongotoy-0.1.7/mongotoy/references.py
+-rw-r--r--   0        0        0     1813 2024-04-07 17:20:09.221000 mongotoy-0.1.7/mongotoy/sync.py
+-rw-r--r--   0        0        0    10959 2024-05-23 17:44:07.707067 mongotoy-0.1.7/mongotoy/types.py
+-rw-r--r--   0        0        0      715 2024-05-30 14:48:08.013144 mongotoy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6484 2024-04-14 05:31:35.928668 mongotoy-0.1.7/README.md
+-rw-r--r--   0        0        0     7128 1970-01-01 00:00:00.000000 mongotoy-0.1.7/PKG-INFO
```

### Comparing `mongotoy-0.1.6/LICENSE` & `mongotoy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.6/mongotoy/cache.py` & `mongotoy-0.1.7/mongotoy/cache.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.6/mongotoy/db.py` & `mongotoy-0.1.7/mongotoy/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 import bson
 import gridfs
 import pymongo
 from motor.core import AgnosticClient, AgnosticDatabase, AgnosticCollection, AgnosticClientSession
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorGridFSBucket, AsyncIOMotorGridOut
 from motor.motor_gridfs import AgnosticGridFSBucket
+from pymongo.collation import Collation
 from pymongo.read_concern import ReadConcern
 
 from mongotoy import documents, expressions, references, fields, types, sync
-from mongotoy.errors import EngineError, NoResultsError, ManyResultsError, SessionError
+from mongotoy.errors import EngineError, NoResultError, SessionError
 
 __all__ = (
     'Engine',
     'Session',
 )
 
 from mongotoy.expressions import Query
@@ -112,22 +113,22 @@
             read_concern=self._read_concern,
             write_concern=self._write_concern
         )
 
     def _get_document_indexes(
         self,
         document_cls: typing.Type[documents.BaseDocument],
-        parent: str = None
+        parent_field: str = None
     ) -> list[pymongo.IndexModel]:
         """
         Retrieves document indexes.
 
         Args:
             document_cls (typing.Type[documents.BaseDocument]): The document class.
-            parent (str, optional): The parent document.
+            parent_field (str, optional): The parent field.
 
         Returns:
             list[pymongo.IndexModel]: List of pymongo IndexModels.
         """
         from mongotoy import mappers
 
         indexes = []
@@ -136,41 +137,41 @@
             index = field.get_index()
             if index:
                 i_doc = index.document
                 i_keys = i_doc.pop('key')
                 i_new_keys = []
                 for i_key, i_type in i_keys.items():
                     i_new_keys.append(
-                        (f'{parent}.{i_key}' if parent else i_key, i_type)
+                        (f'{parent_field}.{i_key}' if parent_field else i_key, i_type)
                     )
                 indexes.append(pymongo.IndexModel(i_new_keys, **i_doc))
 
             # Unwrap ManyMapper
             mapper = field.mapper
             if isinstance(mapper, mappers.SequenceMapper):
                 mapper = mapper.unwrap()
 
             # Add Geo Index
             if isinstance(
                 mapper,
                 (
                     mappers.MultiPointMapper,
                     mappers.MultiLineStringMapper,
-                    mappers.PolygonMapper,
+                    mappers.MultiPolygonMapper,
                 )
             ):
                 indexes.append(
                     pymongo.IndexModel(
-                        [(f'{parent}.{field.alias}' if parent else field.alias, pymongo.GEOSPHERE)]
+                        [(f'{parent_field}.{field.alias}' if parent_field else field.alias, pymongo.GEOSPHERE)]
                     )
                 )
 
             # Add EmbeddedDocument indexes
             if isinstance(mapper, mappers.EmbeddedDocumentMapper):
-                indexes.extend(self._get_document_indexes(mapper.document_cls, parent=field.alias))
+                indexes.extend(self._get_document_indexes(mapper.document_cls, parent_field=field.alias))
 
         return indexes
 
     def _get_document_collection(self, document_cls: typing.Type[T]) -> AgnosticCollection:
         """
         Retrieves the document collection.
 
@@ -199,16 +200,22 @@
 
         Args:
             document_cls (typing.Type[T]): The document class.
             driver_session (AgnosticClientSession, optional): The database session.
         """
         indexes = self._get_document_indexes(document_cls)
         collection = self._get_document_collection(document_cls)
+
         if indexes:
-            await collection.create_indexes(indexes, session=driver_session)
+            options = {}
+            # Add collation to the index
+            if document_cls.document_config.collation:
+                options['collation'] = document_cls.document_config.collation
+
+            await collection.create_indexes(indexes, session=driver_session, **options)
 
     async def _create_document_collection(
         self,
         document_cls: typing.Type[T],
         driver_session: AgnosticClientSession = None
     ):
         """
@@ -217,95 +224,109 @@
         Args:
             document_cls (typing.Type[T]): The document class.
             driver_session (AgnosticClientSession, optional): The database session.
         """
         config = document_cls.document_config
         options = {'check_exists': False}
 
-        # Configure options for capped collections
-        if config.capped:
+        # Configure options for capped collection
+        if config.capped_collection:
             options['capped'] = True
-            options['size'] = config.capped_size
-            if config.capped_max:
-                options['max'] = config.capped_max
+            options['size'] = config.capped_collection_size
+            if config.capped_collection_max:
+                options['max'] = config.capped_collection_max
 
-        # Configure options for timeseries collections
+        # Configure options for timeseries collection
         if config.timeseries_field:
             timeseries = {
-                'timeField': config.timeseries_field,
-                'granularity': config.timeseries_granularity
+                'timeField': documents.get_document_field(
+                    document_cls,
+                    field_name=config.timeseries_field
+                ).alias,
+                'granularity': config.timeseries_granularity or 'seconds'
             }
             if config.timeseries_meta_field:
-                timeseries['metaField'] = config.timeseries_meta_field
+                timeseries['metaField'] = documents.get_document_field(
+                    document_cls,
+                    field_name=config.timeseries_meta_field
+                ).alias
 
             options['timeseries'] = timeseries
             if config.timeseries_expire_after_seconds:
                 options['expireAfterSeconds'] = config.timeseries_expire_after_seconds
 
+        # Add collation to options
+        if config.collation:
+            options['collation'] = config.collation
+
+        # Add extra options to a collection
+        if config.extra_collection_options:
+            options.update(config.extra_collection_options)
+
         # Create the collection with configured options
         await self.database.create_collection(
             name=document_cls.__collection_name__,
             codec_options=config.codec_options or self._codec_options,
             read_preference=config.read_preference or self._read_preference,
             read_concern=config.read_concern or self._read_concern,
             write_concern=config.write_concern or self._write_concern,
             session=driver_session,
             **options
         )
 
     async def _exec_migration(
         self,
         document_cls: typing.Type[T],
-        skip_exist: bool = True,
-        driver_session: AgnosticClientSession = None
+        driver_session: AgnosticClientSession = None,
+        check_exist: bool = True,
     ):
         """
         Executes document migration.
 
         Args:
             document_cls (typing.Type[T]): The document class.
-            skip_exist (bool, optional): Whether to skip if a collection exists.
             driver_session (AgnosticClientSession, optional): The database session.
+            check_exist (bool, optional): Whether to check if a collection exists.
         """
-        do_apply = True
+        do_migration = True
 
         # Skip if a collection already exists
-        if skip_exist:
+        if check_exist:
             collections = await self.database.list_collection_names(session=driver_session)
             if document_cls.__collection_name__ in collections:
-                do_apply = False
+                do_migration = False
 
         # Create collection and indexes
-        if do_apply:
+        if do_migration:
             await self._create_document_collection(document_cls, driver_session=driver_session)
             await self._create_document_indexes(document_cls, driver_session=driver_session)
 
     # noinspection PyMethodMayBeStatic,PyUnresolvedReferences
     async def _exec_seeding(
         self,
         func: typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]],
         session: 'Session',
-        skip_exist: bool = True
+        check_exist: bool = True
     ):
         """
         Executes seeding.
 
         Args:
             func (typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]]): The seeding function.
             session (Session): The session object.
-            skip_exist (bool, optional): Whether to skip if seeding already exists.
+            check_exist (bool, optional): Whether to check if seeding already exists.
         """
         if not inspect.iscoroutinefunction(func):
             raise TypeError('Seeding function must be async')
 
         func_path = f'{func.__module__}.{func.__name__}'
         do_seeding = True
 
         # Skip if seeding already applied
-        if skip_exist:
+        if check_exist:
             # noinspection PyProtectedMember
             if await session.objects(Seeding).filter(
                 Seeding.function == func_path
             )._count():
                 do_seeding = False
 
         if do_seeding:
@@ -353,15 +374,15 @@
             session (Session, optional): The session object.
         """
         driver_session = session.driver_session if session else None
         collections = await self.database.list_collection_names(session=driver_session)
         await asyncio.gather(*[
             self._exec_migration(
                 doc_cls,
-                skip_exist=False,
+                check_exist=False,
                 driver_session=driver_session
             ) for doc_cls in documents_cls if doc_cls.__collection_name__ not in collections
         ])
 
     async def _seeding(
         self,
         func: typing.Callable[['Session'], typing.Coroutine[typing.Any, typing.Any, None]],
@@ -385,22 +406,22 @@
         Executes seeding for multiple functions.
 
         Args:
             funcs (list[Callable[['Session'], Coroutine[Any, Any, None]]]): List of seeding functions.
             session (Session, optional): The session object.
         """
         # noinspection PyProtectedMember
-        seeds = await session.objects(Seeding)._fetch()
+        seeds = await session.objects(Seeding)._all()
         seeds = [s.function for s in seeds]
         # noinspection PyUnresolvedReferences
         await asyncio.gather(*[
             self._exec_seeding(
                 func,
                 session=session,
-                skip_exist=False
+                check_exist=False
             ) for func in funcs if f'{func.__module__}.{func.__name__}' not in seeds
         ])
 
     def session(self) -> 'Session':
         """
         Creates a new MongoDB session.
 
@@ -545,17 +566,23 @@
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         """
         Enables the use of the 'async with' statement. Ends the session upon exiting the context.
         """
         await self._end()
 
     def __enter__(self) -> 'Session':
+        """
+        Enables the use of the 'with' statement.
+        """
         return sync.run_sync(self.__aenter__)()
 
     def __exit__(self, exc_type, exc_value, traceback):
+        """
+        Enables the use of the 'with' statement. Ends the session upon exiting the context.
+        """
         sync.run_sync(self.__aexit__)(exc_type, exc_value, traceback)
 
     async def _start(self):
         """
         Starts the MongoDB session.
 
         Raises:
@@ -646,31 +673,34 @@
                 Query()
             )
             # Get referenced docs
             async for ref_doc in ref_doc_objects.filter(query):
                 do_delete = False
                 # Scan all references
                 for field_name, reference in refs.items():
+                    # Mark to delete
                     if not reference.is_many:
                         do_delete = True
                         break
 
                     # Get reference value
                     value = getattr(ref_doc, field_name)
                     if value:
                         # Wipe doc from value
                         value = [
                             i for i in value
                             if getattr(i, reference.ref_field.name) != getattr(doc, reference.ref_field.name)
                         ]
+                        # Mark to delete
                         if not value:
                             do_delete = True
                             break
-                        setattr(ref_doc, field_name, value)
+
                         # Apply update
+                        setattr(ref_doc, field_name, value)
                         operations.append(self._save(ref_doc))
 
                 # Apply delete
                 if do_delete:
                     operations.append(self._delete(ref_doc, delete_cascade=True))
 
         await asyncio.gather(*operations)
@@ -708,26 +738,37 @@
         Creates a new MongoDB transaction.
 
         Returns:
             Transaction: A new MongoDB transaction associated with the engine
         """
         return Transaction(session=self)
 
-    def objects(self, document_cls: typing.Type[T], dereference_deep: int = 0) -> 'Objects[T]':
+    def objects(
+        self,
+        document_cls: typing.Type[T],
+        dereference_deep: int = 0,
+        collation: typing.Optional[Collation] = None
+    ) -> 'Objects[T]':
         """
         Returns an object manager for the specified document class.
 
         Args:
             document_cls (typing.Type[T]): The document class.
             dereference_deep (int): Depth of dereferencing.
+            collation (Collation, optional): The collation to use when query documents.
 
         Returns:
             Objects[T]: An object manager.
         """
-        return Objects(document_cls, session=self, dereference_deep=dereference_deep)
+        return Objects(
+            document_cls,
+            session=self,
+            dereference_deep=dereference_deep,
+            collation=collation
+        )
 
     def fs(self, chunk_size_bytes: int = gridfs.DEFAULT_CHUNK_SIZE) -> 'FsBucket':
         """
         Returns a GridFS bucket manager.
 
         Args:
             chunk_size_bytes (int): The chunk size in bytes.
@@ -827,17 +868,31 @@
         """
         if exc_value:
             await self._abort()
         else:
             await self._commit()
 
     def __enter__(self) -> 'Transaction':
+        """
+        Enables the use of the 'with' statement.
+
+        Returns:
+            Transaction: The transaction instance.
+        """
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
+        """
+        Enables the use of the 'with' statement. Ends the transaction upon exiting the context.
+
+        Args:
+            exc_type: The type of the exception.
+            exc_value: The exception value.
+            traceback: The exception traceback.
+        """
         sync.run_sync(self.__aexit__)(exc_type, exc_value, traceback)
 
     async def _commit(self):
         """
         Commits changes and closes the MongoDB transaction.
 
         Raises:
@@ -869,20 +924,29 @@
         Represents a query set for retrieving documents from the database.
         This class provides methods for filtering, sorting, limiting, and executing queries asynchronously.
 
         Args:
             document_cls (typing.Type[T]): The document class associated with the query set.
             session (Session): The session object used for database operations.
             dereference_deep (int, optional): The depth of dereferencing for referenced documents.
+            collation (Collation, optional): The collation to use when query documents.
+
         """
 
-    def __init__(self, document_cls: typing.Type[T], session: Session, dereference_deep: int = 0):
+    def __init__(
+        self,
+        document_cls: typing.Type[T],
+        session: Session,
+        dereference_deep: int = 0,
+        collation: typing.Optional[Collation] = None
+    ):
         self._document_cls = document_cls
         self._session = session
         self._dereference_deep = dereference_deep
+        self._collation = collation
         self._collection = session.engine.collection(document_cls)
         self._filter = expressions.Query()
         self._sort = expressions.Sort()
         self._skip = 0
         self._limit = 0
 
     def __copy__(self, **options) -> 'Objects[T]':
@@ -894,115 +958,105 @@
 
         Returns:
             Objects[T]: A shallow copy of the query set with specified options.
         """
         objs = Objects(
             document_cls=self._document_cls,
             session=self._session,
-            dereference_deep=self._dereference_deep
+            dereference_deep=self._dereference_deep,
+            collation=self._collation
         )
-        setattr(objs, '_collection', self._collection)
         setattr(objs, '_filter', options.get('_filter', self._filter))
         setattr(objs, '_sort', options.get('_sort', self._sort))
         setattr(objs, '_skip', options.get('_skip', self._skip))
         setattr(objs, '_limit', options.get('_limit', self._limit))
 
         return objs
 
     async def __aiter__(self) -> typing.AsyncGenerator[T, None]:
         """
         Asynchronously iterates over the result set, executing the query.
 
         Yields:
             T: The parsed document instances.
-
-        Raises:
-            NoResultsError: If no results are found.
-            ManyResultsError: If more than one result is found.
         """
+        # Create pipeline
         # noinspection PyTypeChecker
         pipeline = references.build_dereference_pipeline(
             references=self._document_cls.__references__.values(),
             deep=self._dereference_deep
         )
 
+        # Apply filters, sorting and limits
         if self._filter:
             pipeline.append({'$match': self._filter})
         if self._sort:
             pipeline.append({'$sort': self._sort})
         if self._skip > 0:
             pipeline.append({'$skip': self._skip})
         if self._limit > 0:
             pipeline.append({'$limit': self._limit})
 
-        cursor = self._collection.aggregate(pipeline, session=self._session.driver_session)
+        # Aggregation query options
+        options = {}
+
+        # Add collation to aggregation query
+        collation = self._collation or self._document_cls.document_config.collation
+        if collation:
+            options['collation'] = collation
+
+        cursor = self._collection.aggregate(pipeline, session=self._session.driver_session, **options)
         async for data in cursor:
             yield self._document_cls(**data)
 
     def __iter__(self) -> typing.Generator[T, None, None]:
-        for doc in sync.as_sync_gen(self.__aiter__()):
-            yield doc
-
-    async def _create(self, **data) -> T:
         """
-        Creates a new document in the database.
+        Synchronously iterates over the result set, executing the query.
 
-        Args:
-            **data: Keyword arguments representing the document data.
-
-        Returns:
-            T: The newly created document instance.
+        Yields:
+            T: The parsed document instances.
         """
-        doc = self._document_cls(**data)
-        # noinspection PyProtectedMember
-        await self._session._save(doc, save_references=True)
-        return doc
+        for doc in sync.as_sync_gen(self.__aiter__()):
+            yield doc
 
-    async def _fetch(self) -> list[T]:
+    async def _all(self) -> list[T]:
         """
         Retrieves all documents in the result set.
 
         Returns:
-            list[T]: The list of parsed document instances.
+            list[T]: The list of document instances.
         """
         return [doc async for doc in self]
 
-    async def _fetch_one(self) -> T:
+    async def _one(self) -> T:
         """
-        Retrieves a specific document in the result set.
+        Retrieves one document in the result set.
 
         Returns:
-            T: The parsed document instance.
+            T: The document instance.
 
         Raises:
             NoResultsError: If no results are found.
-            ManyResultsError: If more than one result is found.
         """
-        docs = await self.limit(2)._fetch()
+        docs = await self.limit(1)._all()
         if not docs:
-            raise NoResultsError()
-        if len(docs) > 1:
-            raise ManyResultsError()
+            raise NoResultError()
         return docs[0]
 
-    # noinspection PyShadowingBuiltins
-    async def _fetch_by_id(self, value: typing.Any) -> T:
+    async def _one_or_none(self) -> typing.Optional[T]:
         """
-        Retrieves a document by its identifier.
-
-        Args:
-            value (typing.Any): The identifier value.
+        Retrieves one document in the result set, or None if not exist.
 
         Returns:
-            T: The parsed document instance.
+            Optional[T]: The document instance or None.
         """
-        # noinspection PyProtectedMember
-        return await self.filter(
-            self._document_cls.id == self._document_cls.id._field.mapper.__validate_value__(value)
-        )._fetch_one()
+        try:
+            return await self._one()
+        except NoResultError:
+            pass
 
     async def _count(self) -> int:
         """
         Counts the number of documents in the result set.
 
         Returns:
             int: The count of documents.
@@ -1066,28 +1120,24 @@
 
         Returns:
             Objects[T]: The updated query set with the limit value set.
         """
         return self.__copy__(_limit=limit)
 
     @sync.proxy
-    def create(self, **data) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
-        return self._create(**data)
+    def all(self) -> typing.Coroutine[typing.Any, typing.Any, list[T]] | list[T]:
+        return self._all()
 
     @sync.proxy
-    def fetch(self) -> typing.Coroutine[typing.Any, typing.Any, list[T]] | list[T]:
-        return self._fetch()
+    def one(self) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
+        return self._one()
 
     @sync.proxy
-    def fetch_one(self) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
-        return self._fetch_one()
-
-    @sync.proxy
-    def fetch_by_id(self, value: typing.Any) -> typing.Coroutine[typing.Any, typing.Any, T] | T:
-        return self._fetch_by_id(value)
+    def one_or_none(self) -> typing.Coroutine[typing.Any, typing.Any, typing.Optional[T]] | typing.Optional[T]:
+        return self._one_or_none()
 
     @sync.proxy
     def count(self) -> typing.Coroutine[typing.Any, typing.Any, int] | int:
         return self._count()
 
 
 # noinspection PyProtectedMember
@@ -1152,15 +1202,15 @@
             filename=filename,
             source=src,
             metadata=metadata,
             chunk_size_bytes=chunk_size_bytes or self._chunk_size_bytes,
             session=self._session.driver_session
         )
         # Update obj info
-        obj = await self._fetch_by_id(obj.id)
+        obj = await self.filter(FsObject.id == obj.id)._one()
 
         return obj
 
     async def _exist(self, filename: str) -> bool:
         """
         Checks if a file exists in the file system bucket.
 
@@ -1179,15 +1229,15 @@
 
         Args:
             filename (str): The name of the file.
 
         Returns:
             list[FsObject]: A list of file objects representing revisions.
         """
-        return await self.filter(Query.Eq('filename', filename))._fetch()
+        return await self.filter(Query.Eq('filename', filename))._all()
 
     @sync.proxy
     def create(
         self,
         filename: str,
         src: typing.IO | bytes,
         metadata: dict = None,
@@ -1314,14 +1364,15 @@
         """
         grid_out = await fs._bucket.open_download_stream_by_name(
             filename=self.filename,
             revision=revision,
             session=fs._session.driver_session
         )
 
+        # noinspection PyTypeChecker
         return FsObjectStream(grid_out)
 
     async def _delete(self, fs: FsBucket):
         await fs._bucket.delete(
             file_id=self.id,
             session=fs._session.driver_session
         )
@@ -1370,15 +1421,15 @@
         self._driver_grid_out = grid_out
 
     async def _read(self, size: int = -1) -> bytes:
         """
         Reads data from the file asynchronously.
 
         Args:
-            size (int, optional): The number of bytes to read. If not specified or negative, reads until EOF.
+            size (int, optional): The number of bytes to read. If not specified or negative, read until EOF.
 
         Returns:
             bytes: The data read from the file.
         """
         return await self._driver_grid_out.read(size)
 
     # noinspection SpellCheckingInspection
@@ -1392,15 +1443,15 @@
         return await self._driver_grid_out.readchunk()
 
     async def _readline(self, size: int = -1) -> bytes:
         """
         Reads a line from the file asynchronously.
 
         Args:
-            size (int, optional): The maximum number of bytes to read. If not specified or negative, reads until EOF.
+            size (int, optional): The maximum number of bytes to read. If not specified or negative, read until EOF.
 
         Returns:
             bytes: The line read from the file.
         """
         return await self._driver_grid_out.readline(size)
 
     def seek(self, pos: int, whence: int = os.SEEK_SET) -> int:
@@ -1466,10 +1517,10 @@
     Attributes:
         function (str): The name or identifier of the seeding function.
         applied_at (datetime.datetime): The timestamp when the seeding was applied.
 
     """
 
     function: str = fields.field(id_field=True)
-    applied_at: datetime.datetime = fields.field(default_factory=datetime.datetime.utcnow)
+    applied_at: datetime.datetime = fields.field(default_factory=datetime.datetime.now)
 
     __collection_name__ = 'mongotoy.seeding'
```

### Comparing `mongotoy-0.1.6/mongotoy/documents.py` & `mongotoy-0.1.7/mongotoy/documents.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import typing
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Any, Literal
 
 import bson
 import pymongo
+from pymongo.collation import Collation
 from pymongo.read_concern import ReadConcern
 
 from mongotoy import cache, expressions, references, fields, mappers
 from mongotoy.errors import DocumentError, ValidationError, DocumentValidationError
 
 __all__ = (
     'EmbeddedDocument',
@@ -42,47 +43,47 @@
         """
         # Add base classes fields
         _fields = OrderedDict()
         for base in bases:
             _fields.update(getattr(base, '__fields__', {}))
 
         # Add class namespace declared fields
-        for field_name, anno_type in namespace.get('__annotations__', {}).items():
-            options = namespace.get(field_name, fields.FieldOptions())
+        for field_name, annotated_type in namespace.get('__annotations__', {}).items():
+            options = namespace.get(field_name, expressions.EmptyValue)
             if not isinstance(options, fields.FieldOptions):
-                # noinspection PyTypeChecker,SpellCheckingInspection
-                raise DocumentError(
-                    loc=(name, field_name),
-                    msg=f'Invalid field descriptor {type(options)}. '
-                        f'Use mongotoy.field() or mongotoy.reference() descriptors'
-                )
+                options = fields.FieldOptions(default=options)
+
             try:
                 _fields[field_name] = fields.Field(
-                    mapper=mappers.build_mapper(anno_type, options=options),
+                    mapper=mappers.build_mapper(annotated_type, options=options),
                     options=options
                 )
             except TypeError as e:
                 # noinspection PyTypeChecker
                 raise DocumentError(
                     loc=(name, field_name),
-                    msg=f'Invalid field annotation {anno_type}. {str(e)}'
+                    msg=f'Invalid field annotation {annotated_type}. {str(e)}'
                 ) from None
+
             except Exception as e:
                 # noinspection PyTypeChecker
                 raise DocumentError(
                     loc=(name, field_name),
                     msg=str(e)
                 )
 
         # Update namespace with fields
         namespace.update(_fields)
+
         # Build class
         _cls = super().__new__(mcls, name, bases, namespace)
+
         # Set cls fields
         _cls.__fields__ = _fields
+
         # Register class
         cache.documents.add_type(name, _cls)
 
         return _cls
 
 
 # noinspection PyUnresolvedReferences
@@ -101,23 +102,25 @@
 
     if TYPE_CHECKING:
         __fields__: dict[str, fields.Field]
         __data__: dict[str, Any]
 
     def __init__(self, **data):
         self.__data__ = {}
-        errors = []
+        val_errors = []
+
         for field in self.__fields__.values():
             value = data.get(field.alias, data.get(field.name, expressions.EmptyValue))
             try:
                 field.__set__(self, value=value)
             except ValidationError as e:
-                errors.extend(e.errors)
-        if errors:
-            raise DocumentValidationError(self.__class__, errors=errors)
+                val_errors.extend(e.errors)
+
+        if val_errors:
+            raise DocumentValidationError(self.__class__, errors=val_errors)
 
     def _dump(
         self,
         mode: Literal['dict', 'json', 'bson'] | None,
         by_alias: bool = False,
         exclude_empty: bool = False,
         exclude_null: bool = False
@@ -236,55 +239,82 @@
 
 class EmbeddedDocument(BaseDocument):
     """
     Class representing an embedded document.
 
     This class serves as a base for defining embedded documents within other documents. It inherits functionality
     from the BaseDocument class.
+
     """
 
 
 @dataclasses.dataclass
 class DocumentConfig:
     """
     Represents configuration options for a document in MongoDB.
 
     This data class defines various settings such as indexes, capped collection options, timeseries collection options,
     codec options, read preference, read concern, write concern, and extra options for a MongoDB document.
 
     Attributes:
         indexes (list[pymongo.IndexModel]): List of index models for the document.
-        capped (bool): Indicates if the collection is capped (default is False).
-        capped_size (int): The maximum size of the capped collection in bytes (default is 16 MB).
-        capped_max (int): The maximum number of documents allowed in a capped collection (default is None).
         timeseries_field (str): The field name to use as the time field for timeseries collections (default is None).
         timeseries_meta_field (str): The field name for metadata in timeseries collections (default is None).
         timeseries_granularity (Literal['seconds', 'minutes', 'hours']): The granularity of time intervals.
-        timeseries_expire_after_seconds (int): The expiration time for documents in a timeseries collection, in seconds.
+        timeseries_expire_after_seconds (int): The expiration time for documents in a timeseries collection, in seconds
+        capped_collection (bool): Indicates if the collection is capped (default is False).
+        capped_collection_size (int): The maximum size of the capped collection in bytes (default is 16 MB).
+        capped_collection_max (int): The maximum number of documents allowed in a capped collection (default is None).
+        collation (Collation): The collation to use in a document collection (default is None).
+        extra_collection_options (dict): Extra options for the document collection (default is an empty dictionary).
         codec_options (bson.CodecOptions): The BSON codec options (default is None).
         read_preference (pymongo.ReadPreference): The read preference for the document (default is None).
         read_concern (ReadConcern): The read concern for the document (default is None).
         write_concern (pymongo.WriteConcern): The written concern for the document (default is None).
-        extra_options (dict): Extra options for the document configuration (default is an empty dictionary).
 
     """
 
-    indexes: list[pymongo.IndexModel] = dataclasses.field(default_factory=lambda: list())
-    capped: bool = dataclasses.field(default=False)
-    capped_size: int = dataclasses.field(default=16 * (2 ** 20))  # 16 Mb
-    capped_max: int = dataclasses.field(default=None)
+    indexes: list[pymongo.IndexModel] = dataclasses.field(default_factory=list)
     timeseries_field: str = dataclasses.field(default=None)
     timeseries_meta_field: str = dataclasses.field(default=None)
-    timeseries_granularity: Literal['seconds', 'minutes', 'hours'] = dataclasses.field(default='seconds')
+    timeseries_granularity: Literal['seconds', 'minutes', 'hours'] = dataclasses.field(default=None)
     timeseries_expire_after_seconds: int = dataclasses.field(default=None)
+    capped_collection: bool = dataclasses.field(default=False)
+    capped_collection_size: int = dataclasses.field(default=16 * (2 ** 20))  # 16 Mb
+    capped_collection_max: int = dataclasses.field(default=None)
+    collation: Collation = dataclasses.field(default=None)
+    extra_collection_options: dict = dataclasses.field(default_factory=dict)
     codec_options: bson.CodecOptions = dataclasses.field(default=None)
     read_preference: pymongo.ReadPreference = dataclasses.field(default=None)
     read_concern: ReadConcern = dataclasses.field(default=None)
     write_concern: pymongo.WriteConcern = dataclasses.field(default=None)
-    extra_options: dict = dataclasses.field(default_factory=lambda: dict())
+
+    def merge(self, new_config: 'DocumentConfig'):
+        """
+        Merge the current document configuration with a new configuration.
+
+        This function updates the current configuration with values from the new configuration,
+        prioritizing the values from the current configuration if they are defined.
+
+        Args:
+            new_config (DocumentConfig): The new configuration to merge.
+
+        """
+        # Merge indexes
+        self.indexes.extend(new_config.indexes)
+
+        # Merge timeseries fields
+        self.timeseries_field = self.timeseries_field or new_config.timeseries_field
+        self.timeseries_meta_field = self.timeseries_meta_field or new_config.timeseries_meta_field
+
+        # Merge timeseries settings
+        self.timeseries_granularity = self.timeseries_granularity or new_config.timeseries_granularity
+        self.timeseries_expire_after_seconds = (
+            self.timeseries_expire_after_seconds or new_config.timeseries_expire_after_seconds
+        )
 
 
 class DocumentMeta(BaseDocumentMeta):
     """
     Metaclass for document class.
     """
 
@@ -304,57 +334,68 @@
 
         Raises:
             DocumentError: If an error occurs during class creation.
 
         """
         _cls = super().__new__(mcls, name, bases, namespace)
 
+        # Process document fields
         _id_field = None
         _references = OrderedDict()
         for field in _cls.__fields__.values():
             # Check id field
-            # noinspection PyProtectedMember
-            if field._options.id_field:
+            if field.options.id_field:
                 _id_field = field
 
             # Unwrap SequenceMapper
             _mapper = field.mapper
             _is_many = False
             if isinstance(_mapper, mappers.SequenceMapper):
                 _mapper = _mapper.unwrap()
                 _is_many = True
 
             # Add references
             if isinstance(_mapper, mappers.ReferencedDocumentMapper):
-                # noinspection PyProtectedMember,PyUnresolvedReferences
                 _references[field.name] = references.Reference(
-                    document_cls=_mapper._document_cls,
-                    ref_field=_mapper._options.ref_field,
-                    key_name=_mapper._options.key_name or f'{field.alias}_{_mapper._options.ref_field}',
+                    document_cls=getattr(_mapper, '_document_cls'),
+                    ref_field=_mapper.options.ref_field,
+                    key_name=_mapper.options.key_name or f'{field.alias}_{_mapper.options.ref_field}',
                     is_many=_is_many,
                     name=field.alias
                 )
 
+        # Create id field if not exist
         if not _id_field:
             _options = fields.FieldOptions(
                 id_field=True,
                 default_factory=bson.ObjectId
             )
             _id_field = fields.Field(
                 mapper=mappers.ObjectIdMapper(options=_options),
                 options=_options
             )
             _id_field.__set_name__(_cls, 'id')
 
-        # Set class props
+        # Merge base configs
+        _base_config = DocumentConfig()
+        for base in bases:
+            _config = getattr(base, 'document_config', None)
+            if _config:
+                _base_config.merge(_config)
+
+        # Get Document config from namespace and merge with base config
+        _doc_config = namespace.get('document_config', DocumentConfig())
+        _doc_config.merge(_base_config)
+
+        # Set Document class properties
+        _cls.id = _id_field
+        _cls.document_config = _doc_config
+        _cls.__collection_name__ = namespace.get('__collection_name__', f'{name.lower()}s')
         _cls.__fields__['id'] = _id_field
         _cls.__references__ = _references
-        _cls.__collection_name__ = namespace.get('__collection_name__', f'{name.lower()}s')
-        _cls.id = _id_field
-        _cls.document_config = namespace.get('document_config', DocumentConfig())
 
         return _cls
 
 
 class Document(BaseDocument, metaclass=DocumentMeta):
     """
     Represents a document in MongoDB.
```

### Comparing `mongotoy-0.1.6/mongotoy/errors.py` & `mongotoy-0.1.7/mongotoy/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 class ErrorWrapper:
     # noinspection SpellCheckingInspection
     """
         Wrapper class for handling errors in the mongotoy library.
 
         Args:
-            loc (str): The location where the error occurred.
             error (Exception): The wrapped error instance.
+            loc (str): The location where the error occurred.
 
         Raises:
             TypeError: If `loc` is not a tuple of strings.
         """
 
-    def __init__(self, loc: tuple[str], error: Union[Exception, 'ErrorWrapper']):
+    def __init__(self, error: Union[Exception, 'ErrorWrapper'], loc: tuple[str] = tuple()):
         self._loc, self._error = self._unwrap_error(loc, error)
 
     def _unwrap_error(self, loc: tuple[str], error: Exception) -> tuple[tuple[str], Exception]:
         """
         Recursively unwrap nested ErrorWrapper instances to get the original error and its location.
 
         Parameters:
@@ -59,41 +59,41 @@
         Get the formatted error message.
 
         Returns:
             str: The formatted error message.
         """
         return f'{".".join(self.loc)} -> {str(self.error)}'
 
-    def dump_dict(self) -> dict:
+    def dump_json(self) -> dict:
         """
-        Convert the error information to a dictionary.
+        Convert the error information to a valid json.
 
         Returns:
-            dict: A dictionary containing the location and string representation of the error.
+            dict: A json valid containing the location and string representation of the error.
         """
         return {
             'type': self.error.__class__.__name__,
             'loc': list(self.loc),
             'error': str(self.error)
         }
 
 
 class ValidationError(Exception):
     # noinspection SpellCheckingInspection
     """
         Exception class to represent data validation errors in the mongotoy library.
 
         Args:
-            errors (list[ErrorWrapper]): List of ErrorWrapper instances containing details of validation errors.
+            *errors (ErrorWrapper): List of ErrorWrapper instances containing details of validation errors.
 
         Raises:
             TypeError: If `errors` is not a list of ErrorWrapper instances.
         """
 
-    def __init__(self, errors: list[ErrorWrapper]):
+    def __init__(self, *errors: ErrorWrapper):
         if not all(isinstance(e, ErrorWrapper) for e in errors):
             raise TypeError("Errors must be a list of ErrorWrapper instances.")
 
         self._errors = errors
         super().__init__(self._get_message())
 
     def _get_message(self) -> str:
@@ -112,26 +112,26 @@
     def errors(self) -> list[ErrorWrapper]:
         """
         Get the list of validation errors.
 
         Returns:
             list[ErrorWrapper]: List of ErrorWrapper instances representing validation errors.
         """
-        return self._errors
+        return list(self._errors)
 
-    def dump_dict(self) -> dict:
+    def dump_json(self) -> dict:
         """
-        Convert the validation error information to a dictionary.
+        Convert the validation error information to a valid json.
 
         Returns:
-            dict: A dictionary containing the details of validation errors.
+            dict: A json valid containing the details of validation errors.
         """
         return {
             'type': 'ValidationError',
-            'errors': [e.dump_dict() for e in self.errors]
+            'errors': [e.dump_json() for e in self.errors]
         }
 
 
 class DocumentValidationError(ValidationError):
     # noinspection SpellCheckingInspection
     """
         Exception class to represent data validation errors at documents in the mongotoy library.
@@ -139,39 +139,39 @@
         Args:
             document_cls (typing.Type): The type of document where the validation error occurred.
             errors (list[ErrorWrapper]): List of ErrorWrapper instances containing details of validation errors.
         """
 
     def __init__(self, document_cls: typing.Type, errors: list[ErrorWrapper]):
         self._document_cls = document_cls
-        super().__init__(errors)
+        super().__init__(*errors)
 
     def _get_message(self) -> str:
         """
         Get the error message for the document validation exception.
 
         Returns:
             str: The error message indicating the invalid fields.
         """
         msg = f'Invalid data at:'
         for err in self.errors:
-            msg += f'\n  * {ErrorWrapper(loc=(self._document_cls.__name__,), error=err).get_message()}'
+            msg += f'\n  * {ErrorWrapper(error=err, loc=(self._document_cls.__name__,)).get_message()}'
         return msg
 
-    def dump_dict(self) -> dict:
+    def dump_json(self) -> dict:
         """
-        Convert the document validation error information to a dictionary.
+        Convert the document validation error information to a valid json.
 
         Returns:
-            dict: A dictionary containing the details of document validation errors.
+            dict: A json valid containing the details of document validation errors.
         """
         return {
             'type': 'DocumentValidationError',
             'document': self._document_cls.__name__,
-            'errors': super().dump_dict()['errors']
+            'errors': super().dump_json()['errors']
         }
 
 
 class DocumentError(Exception):
     # noinspection SpellCheckingInspection
     """
         Exception class to represent errors related to document definitions in the mongotoy library.
@@ -199,23 +199,14 @@
     Error raised for session-related issues.
 
     This exception is raised when there are errors related to session operations
 
     """
 
 
-class NoResultsError(Exception):
+class NoResultError(Exception):
     """
     Error raised when no results are found.
 
-    This exception is raised when an operation expects results but none are found.
-
-    """
-
-
-class ManyResultsError(Exception):
-    """
-    Error raised when multiple results are found.
-
-    This exception is raised when an operation expects a single result but multiple results are found.
+    This exception is raised when an operation expects a result, but none are found.
 
     """
```

### Comparing `mongotoy-0.1.6/mongotoy/expressions.py` & `mongotoy-0.1.7/mongotoy/expressions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import re
+import typing
 from typing import Literal
 
 import pymongo
 
+from mongotoy import geodata
+
 EmptyValue = type('EmptyValue', (), {})()
 IndexType = Literal[-1, 1, '2d', '2dsphere', 'hashed', 'text']
 
 
 # noinspection PyPep8Naming
 class Sort(dict[str, Literal[-1, 1] | dict]):
     """
@@ -254,14 +257,98 @@
             value (re.Pattern): The regular expression pattern.
 
         Returns:
             Query: The regex query expression.
         """
         return cls({str(field): {'$regex': value}})
 
+    @classmethod
+    def Intersects(cls, field, value: geodata.Geometry) -> 'Query':
+        """
+        Creates a geo intersects query expression.
+
+        Selects documents whose geospatial data intersects with a specified GeoJSON object;
+        i.e. where the intersection of the data and the specified object is non-empty.
+
+        Args:
+            field: The field name.
+            value (geodata.Geometry): The geometry.
+
+        Returns:
+            Query: The geo intersects query expression.
+        """
+        return cls({
+            str(field): {
+                '$geoIntersects': {
+                    '$geometry': value.dump_json()
+                }
+            }
+        })
+
+    @classmethod
+    def Within(cls, field, value: geodata.Polygon | geodata.MultiPolygon) -> 'Query':
+        """
+        Creates a geo within query expression.
+
+        Selects documents with geospatial data that exists entirely within a specified shape.
+
+        Args:
+            field: The field name.
+            value (geodata.Polygon | geodata.MultiPolygon): The polygon or multipolygon geometry.
+
+        Returns:
+            Query: The geo within query expression.
+        """
+        return cls({
+            str(field): {
+                '$geoWithin': {
+                    '$geometry': value.dump_json()
+                }
+            }
+        })
+
+    @classmethod
+    def Near(
+        cls,
+        field,
+        value: geodata.Point,
+        max_distance: typing.Optional[int] = None,
+        min_distance: typing.Optional[int] = None,
+        as_near_sphere: bool = False
+    ) -> 'Query':
+        """
+        Creates a geo near query expression.
+
+        Specifies a point for which a geospatial query returns the documents from nearest to farthest
+
+        Args:
+            field: The field name.
+            value (geodata.Point): The center point geometry.
+            max_distance (int, Optional): Max distance (in meters) from the center point.
+            min_distance (int, Optional): Min distance (in meters) from the center point.
+            as_near_sphere (bool): Calculates distances using spherical geometry.
+
+        Returns:
+            Query: The geo near query expression.
+        """
+        near_op = '$nearSphere' if as_near_sphere else '$near'
+        near_exp = {
+            '$geometry': value.dump_json()
+        }
+        if max_distance:
+            near_exp['$maxDistance'] = max_distance
+        if min_distance:
+            near_exp['$minDistance'] = min_distance
+
+        return cls({
+            str(field): {
+                near_op: near_exp
+            }
+        })
+
 
 # noinspection PyPep8Naming
 def Q(**kwargs) -> Query:
     """
     Constructor function to create Query expression.
 
     Args:
```

### Comparing `mongotoy-0.1.6/mongotoy/fields.py` & `mongotoy-0.1.7/mongotoy/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import re
 import typing
 
 import pymongo
 
 from mongotoy import expressions, mappers
 from mongotoy.errors import ValidationError, ErrorWrapper
 
@@ -43,74 +44,66 @@
         unique: bool = False,
         lt: typing.Any = None,
         lte: typing.Any = None,
         gt: typing.Any = None,
         gte: typing.Any = None,
         min_items: typing.Optional[int] = None,
         max_items: typing.Optional[int] = None,
-        min_len: typing.Optional[int] = None,
-        max_len: typing.Optional[int] = None,
+        min_length: typing.Optional[int] = None,
+        max_length: typing.Optional[int] = None,
         choices: typing.Optional[list[str]] = None,
+        regex: re.Pattern = None,
         **extra
 ) -> FieldOptions:
     """
     Create a field descriptor for a document.
 
     Args:
         alias (str, optional): Alias for the field. Defaults to None.
         id_field (bool, optional): Indicates if the field is an ID field. Defaults to False.
         default (Any, optional): Default value for the field. Defaults to EmptyValue.
         default_factory (Callable[[], Any], optional): Factory function for generating default values. Defaults to None.
         index (IndexType, optional): Type of index for the field. Defaults to None.
         sparse (bool, optional): Whether the index should be sparse. Defaults to False.
         unique (bool, optional): Whether the index should be unique. Defaults to False.
-        lt (Any): Upper bound for the field value
-        lte (Any): Upper bound (inclusive) for the field value
-        gt (Any): Lower bound for the field value
-        gte (Any): Lower bound (inclusive) for the field value
-        min_items (int, optional): Minimum number of items for sequence fields
-        max_items (int, optional): Maximum  number of items for sequence fields
-        min_len (int, optional): Minimum length for string fields
-        max_len (int, optional): Maximum length for string fields
-        choices (list[str], optional): List of allowed choices for string fields
-        extra: Extra configurations
+        lt (Any): Upper bound for the field value.
+        lte (Any): Upper bound (inclusive) for the field value.
+        gt (Any): Lower bound for the field value.
+        gte (Any): Lower bound (inclusive) for the field value.
+        min_items (int, optional): Minimum number of items for sequence fields.
+        max_items (int, optional): Maximum number of items for sequence fields.
+        min_length (int, optional): Minimum length for string fields.
+        max_length (int, optional): Maximum length for string fields.
+        choices (list[str], optional): List of allowed choices for string fields.
+        regex (re.Pattern): Regular expression for string fields.
+        extra: Extra options for customization. Defaults to empty dict.
 
     Returns:
         FieldOptions: Field descriptor.
 
     """
-    extra_configs = {**extra}
-    if lt is not None:
-        extra_configs['lt'] = lt
-    if lte is not None:
-        extra_configs['lte'] = lte
-    if gt is not None:
-        extra_configs['gt'] = gt
-    if gte is not None:
-        extra_configs['gte'] = gte
-    if min_items is not None:
-        extra_configs['min_items'] = min_items
-    if max_items is not None:
-        extra_configs['max_items'] = max_items
-    if min_len is not None:
-        extra_configs['min_len'] = min_len
-    if max_len is not None:
-        extra_configs['max_len'] = max_len
-    if choices:
-        extra_configs['choices'] = choices
-
     return FieldOptions(
         alias=alias,
         id_field=id_field,
         default=default,
         default_factory=default_factory,
         index=index,
         sparse=sparse,
         unique=unique,
-        extra=extra_configs
+        lt=lt,
+        lte=lte,
+        gt=gt,
+        gte=gte,
+        min_items=min_items,
+        max_items=max_items,
+        min_length=min_length,
+        max_length=max_length,
+        choices=choices,
+        regex=regex,
+        extra=extra
     )
 
 
 def reference(ref_field: str = 'id', key_name: str = None) -> FieldOptions:
     """
     Create a reference field descriptor for a document.
 
@@ -160,14 +153,18 @@
         Returns:
             Mapper: The mapper object.
 
         """
         return self._mapper
 
     @property
+    def options(self) -> FieldOptions:
+        return self._options
+
+    @property
     def name(self) -> str:
         """
         Get the name of the field.
 
         Returns:
             str: The name of the field.
 
@@ -207,18 +204,15 @@
 
         Returns:
             Any: The value of the field.
 
         """
         if not instance:
             return FieldProxy(self)
-        value = instance.__data__.get(self.name, expressions.EmptyValue)
-        if value in (expressions.EmptyValue, None):
-            return value
-        return self.mapper.dump_value(value)
+        return instance.__data__.get(self.name, expressions.EmptyValue)
 
     def __set__(self, instance, value):
         """
         Set the value of the field.
 
         Args:
             instance: The instance of the owner class.
@@ -260,25 +254,24 @@
             Any: The validated value.
 
         Raises:
             ValidationError: If validation fails.
 
         """
         try:
-            # Validate value
+            # Map value
             value = self.mapper(value)
 
             # Check id value
             if self.alias == '_id' and value is expressions.EmptyValue:
-                raise ValidationError([
-                    ErrorWrapper(loc=tuple(), error=ValueError('Id field value required'))
-                ])
+                raise ValidationError(ErrorWrapper(ValueError('Id field value required')))
+
         except ValidationError as e:
             raise ValidationError(
-                errors=[ErrorWrapper(loc=(self.name,), error=i) for i in e.errors]
+                *[ErrorWrapper(err, loc=(self.name,)) for err in e.errors]
             ) from None
 
         return value
 
 
 class FieldProxy:
     """
```

### Comparing `mongotoy-0.1.6/mongotoy/mappers.py` & `mongotoy-0.1.7/mongotoy/mappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import dataclasses
 import datetime
 import decimal
 import json
+import re
 import typing
 import uuid
 from types import UnionType, NoneType
 
 import bson
 
 from mongotoy import cache, expressions, types, geodata
@@ -26,26 +27,50 @@
 @dataclasses.dataclass
 class MapperOptions:
     """
     Represents the options for configuring a Mapper instance.
     Attributes:
         nullable (bool): Flag indicating whether the field is nullable. Defaults to False.
         default (Any): Default value for the field. Defaults to expressions.EmptyValue.
-        default_factory (Callable[[], Any] | None): Factory function to generate default values. Defaults to None.
+        default_factory (Callable[[], Any]): Factory function to generate default values. Defaults to None.
         ref_field (str): Field name to use as a reference. Defaults to None.
         key_name (str): Name of the key when using a reference. Defaults to None.
+        lt (Any): Upper bound for the field value.
+        lte (Any): Upper bound (inclusive) for the field value.
+        gt (Any): Lower bound for the field value.
+        gte (Any): Lower bound (inclusive) for the field value.
+        min_items (int): Minimum number of items for sequence fields.
+        max_items (int): Maximum number of items for sequence fields.
+        min_length (int): Minimum length for string fields.
+        max_length (int): Maximum length for string fields.
+        choices (list[str]): List of allowed choices for string fields.
+        regex (re.Pattern): Regular expression for string fields.
         extra (dict): Extra options for customization. Defaults to empty dict.
     """
     nullable: bool = dataclasses.field(default=False)
     default: typing.Any = dataclasses.field(default=expressions.EmptyValue)
-    default_factory: typing.Callable[[], typing.Any] | None = dataclasses.field(default=None)
+    default_factory: typing.Callable[[], typing.Any] = dataclasses.field(default=None)
     ref_field: str = dataclasses.field(default=None)
     key_name: str = dataclasses.field(default=None)
+    lt: typing.Any = dataclasses.field(default=None)
+    lte: typing.Any = dataclasses.field(default=None)
+    gt: typing.Any = dataclasses.field(default=None)
+    gte: typing.Any = dataclasses.field(default=None)
+    min_items: int = dataclasses.field(default=None)
+    max_items: int = dataclasses.field(default=None)
+    min_length: int = dataclasses.field(default=None)
+    max_length: int = dataclasses.field(default=None)
+    choices: list[str] = dataclasses.field(default=None)
+    regex: re.Pattern = dataclasses.field(default=None)
     extra: dict = dataclasses.field(default_factory=dict)
 
+    def get_default_value(self) -> typing.Any:
+        """Return the default value."""
+        return self.default_factory() if self.default_factory else self.default
+
 
 def build_mapper(mapper_bind: typing.Type, options: MapperOptions) -> 'Mapper':
     """
     Build a data mapper based on annotations.
 
     Args:
         mapper_bind (Type): Type annotation for the mapper.
@@ -164,87 +189,81 @@
     """
 
     if typing.TYPE_CHECKING:
         __bind__: typing.Type
 
     def __init__(self, options: MapperOptions):
         self._options = options
-        self._default_factory = options.default_factory if options.default_factory else lambda: options.default
+
+    @property
+    def options(self) -> MapperOptions:
+        return self._options
 
     def __call__(self, value) -> typing.Any:
         """
-        Validate the value.
+        Maps and validate the value.
 
         Args:
             value (Any): The value to be validated.
 
         Raises:
             ValueError: If the value is invalid.
 
         Returns:
             Any: The validated value.
 
         """
+        # Get default value
         if value is expressions.EmptyValue:
-            value = self._default_factory()
+            value = self.options.get_default_value()
             if value is expressions.EmptyValue:
                 return value
 
         try:
+            # Check nullability
             if value is None:
-                if not self._options.nullable:
+                if not self.options.nullable:
                     raise ValueError('Null value not allowed')
                 return value
 
-            value = self.__validate_value__(value)
+            # Validate value
+            value = self.validate_value(value)
+
         except (TypeError, ValueError) as e:
-            raise ValidationError(errors=[ErrorWrapper(loc=tuple(), error=e)]) from None
+            raise ValidationError(ErrorWrapper(e)) from None
 
         return value
 
     @abc.abstractmethod
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
-        Abstract validator to be implemented in child mappers.
+        Abstract value validator to be implemented in child mappers.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         """
         raise NotImplementedError
 
-    def dump_value(self, value) -> typing.Any:
-        """
-        Dump the value to be access direct from object instance.
-
-        Args:
-            value: The value to be dumped.
-
-        Returns:
-            Any: The dumped value.
-
-        """
-        return value
-
     def dump_dict(self, value, **options) -> typing.Any:
         """
         Dump the value to be in a dictionary.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped value.
 
         """
-        return self.dump_value(value)
+        return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the value to valid JSON.
 
         Args:
             value: The value to be dumped.
@@ -276,70 +295,69 @@
     Base mapper for data types supporting the following comparators:
     - lt (less than)
     - lte (less than or equal to)
     - gt (greater than)
     - gte (greater than or equal to)
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the input value against the specified comparators.
         Args:
             value: The value to be validated.
         Returns:
             The validated value.
         Raises:
             TypeError: If the input value is not of the expected data type.
             ValueError: If the value does not meet the specified comparator conditions.
         """
         if not isinstance(value, self.__bind__):
             raise TypeError(f'Invalid data type {type(value)}, expected {self.__bind__}')
 
-        # Validate extra options
-        if self._options.extra:
-            if 'lt' in self._options.extra:
-                if value >= self._options.extra['lt']:
-                    raise ValueError(
-                        f'Invalid value {value}, required lt={self._options.extra["lt"]}'
-                    )
-            if 'lte' in self._options.extra:
-                if value > self._options.extra['lte']:
-                    raise ValueError(
-                        f'Invalid value {value}, required lte={self._options.extra["lte"]}'
-                    )
-            if 'gt' in self._options.extra:
-                if value <= self._options.extra['gt']:
-                    raise ValueError(
-                        f'Invalid value {value}, required gt={self._options.extra["gt"]}'
-                    )
-            if 'gte' in self._options.extra:
-                if value < self._options.extra['gte']:
-                    raise ValueError(
-                        f'Invalid value {value}, required gte={self._options.extra["gte"]}'
-                    )
+        # Validate comparators
+        if self.options.lt is not None:
+            if value >= self.options.lt:
+                raise ValueError(
+                    f'Invalid value {value}, required lt={self.options.lt}'
+                )
+        if self.options.lte is not None:
+            if value > self.options.lte:
+                raise ValueError(
+                    f'Invalid value {value}, required lte={self.options.lte}'
+                )
+        if self.options.gt is not None:
+            if value <= self.options.gt:
+                raise ValueError(
+                    f'Invalid value {value}, required gt={self.options.gt}'
+                )
+        if self.options.gte is not None:
+            if value < self.options.gte:
+                raise ValueError(
+                    f'Invalid value {value}, required gte={self.options.gte}'
+                )
 
         return value
 
 
 class SequenceMapper(Mapper):
     """
     Base mapper for handling sequence of elements.
     """
 
     def __init__(self, mapper: Mapper, options: MapperOptions):
         """
-        Initialize the ManyMapper.
+        Initialize the SequenceMapper.
 
         Args:
             mapper (Mapper): The mapper for the list items.
             options (MapperOptions): Mapper configuration params.
 
         """
         self._mapper = mapper
-        # SequenceMapper must be a least an empty sequence not an EmptyValue for ReferencedDocumentMapper
+        # SequenceMapper must be at least an empty sequence, not an EmptyValue for ReferencedDocumentMapper
         if options.default is expressions.EmptyValue and isinstance(self.unwrap(), ReferencedDocumentMapper):
             options.default = self.__bind__()
         super().__init__(options)
 
     @property
     def mapper(self) -> Mapper:
         """
@@ -355,15 +373,15 @@
         """Get the innermost mapper that isn't a SequenceMapper"""
         mapper_ = self.mapper
         while isinstance(mapper_, SequenceMapper):
             mapper_ = mapper_.mapper
         return mapper_
 
     # noinspection PyTypeChecker
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the list value.
 
         Args:
             value: The list value to be validated.
 
         Returns:
@@ -372,36 +390,37 @@
         Raises:
             ValidationError: If validation fails.
 
         """
         if not isinstance(value, self.__bind__):
             raise TypeError(f'Invalid data type {type(value)}, required is {self.__bind__}')
 
-        # Validate extra options
-        if self._options.extra:
-            if 'min_items' in self._options.extra:
-                if len(value) < self._options.extra['min_items']:
-                    raise ValueError(
-                        f'Invalid value len {len(value)}, required min_items={self._options.extra["min_items"]}'
-                    )
-            if 'max_items' in self._options.extra:
-                if len(value) > self._options.extra['max_items']:
-                    raise ValueError(
-                        f'Invalid value len {len(value)}, required max_items={self._options.extra["max_items"]}'
-                    )
+        # Validate length
+        if self.options.min_items is not None:
+            if len(value) < self.options.min_items:
+                raise ValueError(
+                    f'Invalid length {len(value)}, required min_items={self.options.min_items}'
+                )
+        if self.options.max_items is not None:
+            if len(value) > self.options.max_items:
+                raise ValueError(
+                    f'Invalid length {len(value)}, required max_items={self.options.max_items}'
+                )
 
         new_value = []
-        errors = []
+        val_errors = []
+
         for i, val in enumerate(value):
             try:
                 new_value.append(self.mapper(val))
             except ValidationError as e:
-                errors.extend([ErrorWrapper(loc=(str(i),), error=j) for j in e.errors])
-        if errors:
-            raise ValidationError(errors=errors)
+                val_errors.extend([ErrorWrapper(err, loc=(str(i),)) for err in e.errors])
+
+        if val_errors:
+            raise ValidationError(*val_errors)
 
         return self.__bind__(new_value)
 
     def dump_dict(self, value, **options) -> typing.Any:
         """
         Dump the list value to be in a dictionary.
 
@@ -409,15 +428,15 @@
             value: The list value to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped list value.
 
         """
-        return self.__bind__([self.mapper.dump_dict(i, **options) for i in value])
+        return self.__bind__((self.mapper.dump_dict(i, **options) for i in value))
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the list value to JSON.
 
         Args:
             value: The list value to be dumped.
@@ -471,15 +490,15 @@
         Returns:
             Type['documents.BaseDocument']: The class of the embedded document.
 
         """
         from mongotoy import documents
         return documents.get_embedded_document_cls(self._document_cls)
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the embedded document value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -553,34 +572,14 @@
         document_cls: typing.Type['documents.BaseDocument'] | str,
         options: MapperOptions
     ):
         if not options.ref_field:
             options.ref_field = 'id'
         super().__init__(document_cls, options)
 
-    def __validate_value__(self, value) -> typing.Any:
-        """
-        Validate the referenced document value.
-
-        Args:
-            value: The value to be validated.
-
-        Returns:
-            Any: The validated value.
-
-        Raises:
-            ValueError: If validation fails due to missing referenced field value.
-        """
-        value = super().__validate_value__(value)
-        if getattr(value, self.ref_field.name) is expressions.EmptyValue:
-            raise ValueError(
-                f'Referenced field {self.document_cls.__name__}.{self.ref_field.name} value required'
-            )
-        return value
-
     @property
     def document_cls(self) -> typing.Type['documents.Document']:
         """
         Get the class of the referenced document.
 
         Returns:
             Type['documents.BaseDocument']: The class of the referenced document.
@@ -595,15 +594,35 @@
         Get the reference field.
 
         Returns:
             Field: The reference field.
 
         """
         from mongotoy import documents
-        return documents.get_document_field(self.document_cls, field_name=self._options.ref_field)
+        return documents.get_document_field(self.document_cls, field_name=self.options.ref_field)
+
+    def validate_value(self, value) -> typing.Any:
+        """
+        Validate the referenced document value.
+
+        Args:
+            value: The value to be validated.
+
+        Returns:
+            Any: The validated value.
+
+        Raises:
+            ValueError: If validation fails due to missing referenced field value.
+        """
+        value = super().validate_value(value)
+        if getattr(value, self.ref_field.name) is expressions.EmptyValue:
+            raise ValueError(
+                f'Referenced field {self.document_cls.__name__}.{self.ref_field.name} value required'
+            )
+        return value
 
     def dump_bson(self, value, **options) -> typing.Any:
         """
         Dump the value to BSON.
 
         Args:
             value: The value to be dumped.
@@ -617,15 +636,15 @@
 
 
 class StrMapper(Mapper, bind=str):
     """
     Mapper for handling string values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the string value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -634,31 +653,33 @@
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if not isinstance(value, str):
             raise TypeError(f'Invalid data type {type(value)}, required is {str}')
 
-        # Validate extra options
-        if self._options.extra:
-            if 'min_len' in self._options.extra:
-                if len(value) < self._options.extra['min_len']:
-                    raise ValueError(
-                        f'Invalid value len {len(value)}, required min_len={self._options.extra["min_len"]}'
-                    )
-            if 'max_len' in self._options.extra:
-                if len(value) > self._options.extra['max_len']:
-                    raise ValueError(
-                        f'Invalid value len {len(value)}, required max_len={self._options.extra["max_len"]}'
-                    )
-            if 'choices' in self._options.extra:
-                if value not in self._options.extra['choices']:
-                    raise ValueError(
-                        f'Invalid value {value}, required choices={self._options.extra["choices"]}'
-                    )
+        # Validation options
+        if self.options.min_length is not None:
+            if len(value) < self.options.min_length:
+                raise ValueError(
+                    f'Invalid length {len(value)}, required min_length={self.options.min_length}'
+                )
+        if self.options.max_length is not None:
+            if len(value) > self.options.max_length:
+                raise ValueError(
+                    f'Invalid length {len(value)}, required max_length={self.options.max_length}'
+                )
+        if self.options.choices:
+            if value not in self.options.choices:
+                raise ValueError(
+                    f'Invalid value {value}, required choices={self.options.choices}'
+                )
+        if self.options.regex:
+            if not self.options.regex.fullmatch(value):
+                raise ValueError(f'Invalid value {value}, required regex={self.options.regex.pattern}')
 
         return value
 
 
 class IntMapper(ComparableMapper, bind=int):
     """
     Mapper for handling integer values.
@@ -672,15 +693,15 @@
 
 
 class DecimalMapper(ComparableMapper, bind=decimal.Decimal):
     """
     Mapper for handling decimal values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the decimal value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -688,15 +709,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, bson.Decimal128):
             value = value.to_decimal()
-        value = super().__validate_value__(value)
+        value = super().validate_value(value)
         # Ensure decimal limits for MongoDB
         # https://www.mongodb.com/docs/upcoming/release-notes/3.4/#decimal-type
         ctx = decimal.Context(prec=34)
         return ctx.create_decimal(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
@@ -728,15 +749,15 @@
 
 
 class BoolMapper(Mapper, bind=bool):
     """
     Mapper for handling boolean values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the boolean value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -752,15 +773,15 @@
 
 
 class BinaryMapper(Mapper, bind=bytes):
     """
     Mapper for handling binary values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the binary value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -791,15 +812,15 @@
 
 
 class UUIDMapper(Mapper, bind=uuid.UUID):
     """
     Mapper for handling UUID values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the UUID value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -809,19 +830,14 @@
             TypeError: If validation fails due to incorrect data type.
 
         """
         if not isinstance(value, uuid.UUID):
             raise TypeError(f'Invalid data type {type(value)}, required is {uuid.UUID}')
         return value
 
-    def dump_value(self, value) -> typing.Any:
-        if self._options.extra.get('dump_as_str', False):
-            return str(value)
-        return value
-
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the UUID value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
@@ -829,15 +845,15 @@
         Returns:
             Any: The dumped value.
 
         """
         return str(value)
 
     def dump_bson(self, value, **options) -> typing.Any:
-        if self._options.extra.get('dump_bson_as_str', False):
+        if self.options.extra.get('dump_bson_as_str', False):
             return str(value)
         return value
 
 
 class DateTimeMapper(ComparableMapper, bind=datetime.datetime):
     """
     Mapper for handling datetime values.
@@ -859,15 +875,15 @@
 
 
 class DateMapper(ComparableMapper, bind=datetime.date):
     """
     Mapper for handling date values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the date value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -875,15 +891,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, datetime.datetime):
             value = value.date()
-        return super().__validate_value__(value)
+        return super().validate_value(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the date value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
@@ -911,15 +927,15 @@
 
 
 class TimeMapper(ComparableMapper, bind=datetime.time):
     """
     Mapper for handling time values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the time value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -927,15 +943,15 @@
 
         Raises:
             TypeError: If validation fails due to incorrect data type.
 
         """
         if isinstance(value, datetime.datetime):
             value = value.time()
-        return super().__validate_value__(value)
+        return super().validate_value(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the time value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
@@ -974,46 +990,46 @@
 class TupleMapper(SequenceMapper, bind=tuple):
     """
     Mapper for handling tuples.
 
     Inherits from ManyMapper and specifies 'tuple' as the binding type.
 
     """
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         if isinstance(value, list):
             value = tuple(value)
-        return super().__validate_value__(value)
+        return super().validate_value(value)
 
 
 class SetMapper(SequenceMapper, bind=set):
     """
     Mapper for handling sets.
 
     Inherits from ManyMapper and specifies 'set' as the binding type.
 
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         if isinstance(value, list):
             value = set(value)
-        return super().__validate_value__(value)
+        return super().validate_value(value)
 
     def dump_json(self, value, **options) -> typing.Any:
         return list(value)
 
     def dump_bson(self, value, **options) -> typing.Any:
         return list(value)
 
 
 class ObjectIdMapper(Mapper, bind=bson.ObjectId):
     """
     Mapper for handling BSON ObjectId values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the ObjectId value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1023,19 +1039,14 @@
             TypeError: If validation fails due to incorrect data type.
 
         """
         if not bson.ObjectId.is_valid(value):
             raise TypeError(f'Invalid data type {type(value)}, required is {bson.ObjectId}')
         return bson.ObjectId(value)
 
-    def dump_value(self, value) -> typing.Any:
-        if self._options.extra.get('dump_as_str', False):
-            return str(value)
-        return value
-
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the ObjectId value to a JSON-serializable format.
 
         Args:
             value: The value to be dumped.
             **options: Additional options.
@@ -1048,15 +1059,15 @@
 
 
 class Int64Mapper(Mapper, bind=bson.Int64):
     """
     Mapper for handling BSON Int64 values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the Int64 value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1086,15 +1097,15 @@
 
 
 class Decimal128Mapper(Mapper, bind=bson.Decimal128):
     """
     Mapper for handling BSON Decimal128 values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the Decimal128 value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1124,15 +1135,15 @@
 
 
 class RegexMapper(Mapper, bind=bson.Regex):
     """
     Mapper for handling BSON Regex values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the Regex value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1162,15 +1173,15 @@
 
 
 class CodeMapper(Mapper, bind=bson.Code):
     """
     Mapper for handling BSON Code values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the Code value.
 
         Args:
             value: The value to be validated.
 
         Returns:
@@ -1200,31 +1211,26 @@
 
 
 class ConstrainedStrMapper(StrMapper):
     """
     Mapper for handling constrained string values.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the string value.
 
         Args:
             value: The value to be validated.
 
         Returns:
             Any: The validated value.
 
         """
-        return self.__bind__(super().__validate_value__(value))
-
-    def dump_value(self, value) -> typing.Any:
-        if self._options.extra.get('dump_as_str', False):
-            return str(value)
-        return value
+        return str(self.__bind__(super().validate_value(value)))
 
     def dump_json(self, value, **options) -> typing.Any:
         """
         Dump the string value to JSON.
 
         Args:
             value: The value to be dumped.
@@ -1247,21 +1253,21 @@
         Returns:
             Any: The dumped value.
 
         """
         return str(value)
 
 
-class IpV4Mapper(ConstrainedStrMapper, bind=types.IpV4):
+class IpV4Mapper(ConstrainedStrMapper, bind=types.IPv4):
     """
     Mapper for handling IPv4 addresses.
     """
 
 
-class IpV6Mapper(ConstrainedStrMapper, bind=types.IpV6):
+class IpV6Mapper(ConstrainedStrMapper, bind=types.IPv6):
     """
     Mapper for handling IPv6 addresses.
     """
 
 
 class PortMapper(ConstrainedStrMapper, bind=types.Port):
     """
@@ -1283,15 +1289,15 @@
 
 class EmailMapper(ConstrainedStrMapper, bind=types.Email):
     """
     Mapper for handling email addresses.
     """
 
 
-class CardMapper(ConstrainedStrMapper, bind=types.Card):
+class CardMapper(ConstrainedStrMapper, bind=types.CardNumber):
     """
     Mapper for handling card numbers.
     """
 
 
 class SsnMapper(ConstrainedStrMapper, bind=types.Ssn):
     """
@@ -1326,28 +1332,29 @@
 class GeometryMapper(Mapper):
     """
     Mapper for handling geometry data.
 
     This mapper validates and handles geometry data.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the geometry data.
 
         Args:
             value (Any): The value to be validated.
 
         Returns:
             Any: The validated value.
 
         Raises:
             TypeError: If the value is not of the expected type.
         """
         if isinstance(value, dict):
+            # noinspection PyTypeChecker
             value = geodata.parse_geojson(value, parser=self.__bind__)
         if not isinstance(value, self.__bind__):
             raise TypeError(f'Invalid data type {type(value)}, expected {self.__bind__}')
         return value
 
     def dump_json(self, value, **options) -> typing.Any:
         """
@@ -1356,18 +1363,15 @@
         Args:
             value: The geometry data to be dumped.
             **options: Additional options.
 
         Returns:
             Any: The dumped geometry data.
         """
-        return {
-            'type': self.__bind__.__name__,
-            'coordinates': list(value)
-        }
+        return value.dump_json()
 
     def dump_bson(self, value, **options) -> typing.Any:
         """
         Dump the geometry data to BSON.
 
         Args:
             value: The geometry data to be dumped.
@@ -1418,15 +1422,15 @@
 class JsonMapper(Mapper, bind=types.Json):
     """
     Mapper for handling JSON data.
 
     This mapper validates and handles JSON data.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the JSON data.
 
         Args:
             value (Any): The JSON data to be validated.
 
         Returns:
@@ -1451,15 +1455,15 @@
 class BsonMapper(Mapper, bind=types.Bson):
     """
     Mapper for handling BSON data.
 
     This mapper validates and handles BSON data.
     """
 
-    def __validate_value__(self, value) -> typing.Any:
+    def validate_value(self, value) -> typing.Any:
         """
         Validate the BSON data.
 
         Args:
             value (Any): The BSON data to be validated.
 
         Returns:
```

### Comparing `mongotoy-0.1.6/mongotoy/references.py` & `mongotoy-0.1.7/mongotoy/references.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.6/mongotoy/sync.py` & `mongotoy-0.1.7/mongotoy/sync.py`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.6/mongotoy/types.py` & `mongotoy-0.1.7/mongotoy/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 import datetime
 import os
 import re
 import typing
 
 import bson
 
-from mongotoy import geodata
-
 if typing.TYPE_CHECKING:
     from mongotoy import db
 
+from mongotoy.geodata import Point as _Point
+from mongotoy.geodata import MultiPoint as _MultiPoint
+from mongotoy.geodata import LineString as _LineString
+from mongotoy.geodata import MultiLineString as _MultiLineString
+from mongotoy.geodata import Polygon as _Polygon
+from mongotoy.geodata import MultiPolygon as _MultiPolygon
+
 
-class IpV4(collections.UserString):
+class IPv4(collections.UserString):
     """
     Represents an IPv4 address.
 
     Args:
         value (str): The IPv4 address value.
 
     Raises:
@@ -29,15 +34,15 @@
 
     def __init__(self, value):
         if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid IPv4 address')
         super().__init__(value)
 
 
-class IpV6(collections.UserString):
+class IPv6(collections.UserString):
     """
     Represents an IPv6 address.
 
     Args:
         value (str): The IPv6 address value.
 
     Raises:
@@ -146,15 +151,15 @@
 
     def __init__(self, value):
         if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid email address')
         super().__init__(value)
 
 
-class Card(collections.UserString):
+class CardNumber(collections.UserString):
     """
     Represents a credit card number.
 
     Args:
         value (str): The credit card number value.
 
     Raises:
@@ -280,85 +285,49 @@
 
     def __init__(self, value):
         if not self._regex.fullmatch(value):
             raise ValueError(f'Value {value} is not a valid Semantic Version Number')
         super().__init__(value)
 
 
-class Point(geodata.Position):
+class Point(_Point):
     """
-    For type "Point", the "coordinates" member is a single position.
-
-    https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.2
+        This is a forwarding for type mongotoy.geodata.Point
     """
 
-    def __init__(self, *coordinates: int | float):
-        if len(coordinates) != 2:
-            raise TypeError(f'The Point must represent single position, i.e. [lat, long]')
-        super().__init__(*coordinates)
-
 
-class MultiPoint(list[Point]):
+class MultiPoint(_MultiPoint):
     """
-    For type "MultiPoint", the "coordinates" member is an array of
-    positions.
-
-    https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.3
+        This is a forwarding for type mongotoy.geodata.MultiPoint
     """
 
-    def __init__(self, *points: Point):
-        super().__init__([Point(*i) for i in points])
-
 
-class LineString(list[Point]):
+class LineString(_LineString):
     """
-    For type "LineString", the "coordinates" member is an array of two or
-    more positions.
-
-    https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.4
+        This is a forwarding for type mongotoy.geodata.LineString
     """
 
-    def __init__(self, *points: Point):
-        if not len(points) >= 2:
-            raise TypeError('The LineString must be an array of two or more Points')
-        super().__init__([Point(*i) for i in points])
 
-
-class MultiLineString(list[LineString]):
+class MultiLineString(_MultiLineString):
     """
-    For type "MultiLineString", the "coordinates" member is an array of
-    LineString coordinate arrays.
-
-    https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.5
+        This is a forwarding for type mongotoy.geodata.MultiLineString
     """
 
-    def __init__(self, *lines: LineString):
-        super().__init__([LineString(*i) for i in lines])
-
 
-class Polygon(list[LineString]):
+class Polygon(_Polygon):
     """
-    https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.6
+        This is a forwarding for type mongotoy.geodata.Polygon
     """
 
-    def __init__(self, *rings: LineString):
-        super().__init__([geodata.LinearRing(*i) for i in rings])
 
-
-class MultiPolygon(list[Polygon]):
+class MultiPolygon(_MultiPolygon):
     """
-     For type "MultiPolygon", the "coordinates" member is an array of
-     Polygon coordinate arrays.
-
-     https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.7
+        This is a forwarding for type mongotoy.geodata.MultiPolygon
     """
 
-    def __init__(self, *polygons: Polygon):
-        super().__init__([Polygon(*i) for i in polygons])
-
 
 class Json(dict):
     """
     Represents a valid json data.
     """
```

### Comparing `mongotoy-0.1.6/pyproject.toml` & `mongotoy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongotoy"
-version = "0.1.6"
+version = "0.1.7"
 description = "Comprehensive ODM for MongoDB"
 license = "Apache-2.0"
 authors = ["gurcuff91 <gf.meneses91@gmail.com>"]
 readme = "README.md"
 homepage = "https://gurcuff91.github.io/mongotoy"
 repository = "https://github.com/gurcuff91/mongotoy"
 keywords = ["mapping", "asyncio", "odm", "mongodb"]
```

### Comparing `mongotoy-0.1.6/README.md` & `mongotoy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mongotoy-0.1.6/PKG-INFO` & `mongotoy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongotoy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Comprehensive ODM for MongoDB
 Home-page: https://gurcuff91.github.io/mongotoy
 License: Apache-2.0
 Keywords: mapping,asyncio,odm,mongodb
 Author: gurcuff91
 Author-email: gf.meneses91@gmail.com
 Requires-Python: >=3.12,<4.0
```

