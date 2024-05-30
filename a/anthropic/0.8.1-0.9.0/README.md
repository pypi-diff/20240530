# Comparing `tmp/anthropic-0.8.1.tar.gz` & `tmp/anthropic-0.9.0.tar.gz`

## Comparing `anthropic-0.8.1.tar` & `anthropic-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/__init__.py
--rw-r--r--   0        0        0    57627 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_base_client.py
--rw-r--r--   0        0        0    21119 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_client.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_compat.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_constants.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_files.py
--rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_resource.py
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_response.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_types.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/py.typed
--rw-r--r--   0        0        0  1774213 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_logs.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_streams.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_typing.py
--rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/lib/__init__.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/lib/streaming/__init__.py
--rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/lib/streaming/_messages.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    31442 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/resources/beta/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/resources/beta/beta.py
--rw-r--r--   0        0        0    57521 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/resources/beta/messages.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/completion.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/content_block.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/content_block_delta_event.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/content_block_start_event.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/content_block_stop_event.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_create_params.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_delta_event.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_param.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_start_event.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_stop_event.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/message_stream_event.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/text_block_param.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 anthropic-0.8.1/src/anthropic/types/beta/text_delta.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 anthropic-0.8.1/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 anthropic-0.8.1/LICENSE
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 anthropic-0.8.1/README.md
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 anthropic-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 anthropic-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    57711 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0    21102 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_client.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_compat.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_files.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_response.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0    10080 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_types.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/py.typed
+-rw-r--r--   0        0        0  1774213 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_logs.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_streams.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_typing.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/lib/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/lib/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/lib/streaming/__init__.py
+-rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/lib/streaming/_messages.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    31260 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/resources/beta/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/resources/beta/beta.py
+-rw-r--r--   0        0        0    57318 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/resources/beta/messages.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/__init__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/content_block.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/content_block_delta_event.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/content_block_start_event.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/content_block_stop_event.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_create_params.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_delta_event.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_param.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_start_event.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_stop_event.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/message_stream_event.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/text_block_param.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 anthropic-0.9.0/src/anthropic/types/beta/text_delta.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 anthropic-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 anthropic-0.9.0/LICENSE
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 anthropic-0.9.0/README.md
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 anthropic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13272 2020-02-02 00:00:00.000000 anthropic-0.9.0/PKG-INFO
```

### Comparing `anthropic-0.8.1/src/anthropic/__init__.py` & `anthropic-0.9.0/src/anthropic/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     Transport,
     AsyncClient,
     AsyncStream,
     AsyncAnthropic,
     RequestOptions,
 )
 from ._version import __title__, __version__
-from ._constants import AI_PROMPT as AI_PROMPT
-from ._constants import HUMAN_PROMPT as HUMAN_PROMPT
+from ._constants import AI_PROMPT as AI_PROMPT, HUMAN_PROMPT as HUMAN_PROMPT
 from ._exceptions import (
     APIError,
     ConflictError,
     NotFoundError,
     AnthropicError,
     APIStatusError,
     RateLimitError,
```

### Comparing `anthropic-0.8.1/src/anthropic/_base_client.py` & `anthropic-0.9.0/src/anthropic/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,26 @@
 from ._qs import Querystring
 from ._files import to_httpx_files, async_to_httpx_files
 from ._types import (
     NOT_GIVEN,
     Body,
     Omit,
     Query,
-    ModelT,
     Headers,
     Timeout,
     NotGiven,
     ResponseT,
     Transport,
     AnyMapping,
     PostParser,
     ProxiesTypes,
     RequestFiles,
+    HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
-    UnknownResponse,
     ModelBuilderProtocol,
     BinaryResponseContent,
 )
 from ._utils import is_dict, is_given, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import APIResponse
@@ -137,39 +136,39 @@
         url: URL | NotGiven = NOT_GIVEN,
         params: Query | NotGiven = NOT_GIVEN,
     ) -> None:
         self.url = url
         self.params = params
 
 
-class BasePage(GenericModel, Generic[ModelT]):
+class BasePage(GenericModel, Generic[_T]):
     """
     Defines the core interface for pagination.
 
     Type Args:
         ModelT: The pydantic model that represents an item in the response.
 
     Methods:
         has_next_page(): Check if there is another page available
         next_page_info(): Get the necessary information to make a request for the next page
     """
 
     _options: FinalRequestOptions = PrivateAttr()
-    _model: Type[ModelT] = PrivateAttr()
+    _model: Type[_T] = PrivateAttr()
 
     def has_next_page(self) -> bool:
         items = self._get_page_items()
         if not items:
             return False
         return self.next_page_info() is not None
 
     def next_page_info(self) -> Optional[PageInfo]:
         ...
 
-    def _get_page_items(self) -> Iterable[ModelT]:  # type: ignore[empty-body]
+    def _get_page_items(self) -> Iterable[_T]:  # type: ignore[empty-body]
         ...
 
     def _params_from_url(self, url: URL) -> httpx.QueryParams:
         # TODO: do we have to preprocess params here?
         return httpx.QueryParams(cast(Any, self._options.params)).merge(url.params)
 
     def _info_to_options(self, info: PageInfo) -> FinalRequestOptions:
@@ -186,36 +185,36 @@
             options.params = dict(url.params)
             options.url = str(url)
             return options
 
         raise ValueError("Unexpected PageInfo state")
 
 
-class BaseSyncPage(BasePage[ModelT], Generic[ModelT]):
+class BaseSyncPage(BasePage[_T], Generic[_T]):
     _client: SyncAPIClient = pydantic.PrivateAttr()
 
     def _set_private_attributes(
         self,
         client: SyncAPIClient,
-        model: Type[ModelT],
+        model: Type[_T],
         options: FinalRequestOptions,
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
 
     # Pydantic uses a custom `__iter__` method to support casting BaseModels
     # to dictionaries. e.g. dict(model).
     # As we want to support `for item in page`, this is inherently incompatible
     # with the default pydantic behaviour. It is not possible to support both
     # use cases at once. Fortunately, this is not a big deal as all other pydantic
     # methods should continue to work as expected as there is an alternative method
     # to cast a model to a dictionary, model.dict(), which is used internally
     # by pydantic.
-    def __iter__(self) -> Iterator[ModelT]:  # type: ignore
+    def __iter__(self) -> Iterator[_T]:  # type: ignore
         for page in self.iter_pages():
             for item in page._get_page_items():
                 yield item
 
     def iter_pages(self: SyncPageT) -> Iterator[SyncPageT]:
         page = self
         while True:
@@ -232,21 +231,21 @@
                 "No next page expected; please check `.has_next_page()` before calling `.get_next_page()`."
             )
 
         options = self._info_to_options(info)
         return self._client._request_api_list(self._model, page=self.__class__, options=options)
 
 
-class AsyncPaginator(Generic[ModelT, AsyncPageT]):
+class AsyncPaginator(Generic[_T, AsyncPageT]):
     def __init__(
         self,
         client: AsyncAPIClient,
         options: FinalRequestOptions,
         page_cls: Type[AsyncPageT],
-        model: Type[ModelT],
+        model: Type[_T],
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
         self._page_cls = page_cls
 
     def __await__(self) -> Generator[Any, None, AsyncPageT]:
@@ -261,38 +260,38 @@
             )
             return resp
 
         self._options.post_parser = _parser
 
         return await self._client.request(self._page_cls, self._options)
 
-    async def __aiter__(self) -> AsyncIterator[ModelT]:
+    async def __aiter__(self) -> AsyncIterator[_T]:
         # https://github.com/microsoft/pyright/issues/3464
         page = cast(
             AsyncPageT,
             await self,  # type: ignore
         )
         async for item in page:
             yield item
 
 
-class BaseAsyncPage(BasePage[ModelT], Generic[ModelT]):
+class BaseAsyncPage(BasePage[_T], Generic[_T]):
     _client: AsyncAPIClient = pydantic.PrivateAttr()
 
     def _set_private_attributes(
         self,
-        model: Type[ModelT],
+        model: Type[_T],
         client: AsyncAPIClient,
         options: FinalRequestOptions,
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
 
-    async def __aiter__(self) -> AsyncIterator[ModelT]:
+    async def __aiter__(self) -> AsyncIterator[_T]:
         async for page in self.iter_pages():
             for item in page._get_page_items():
                 yield item
 
     async def iter_pages(self: AsyncPageT) -> AsyncIterator[AsyncPageT]:
         page = self
         while True:
@@ -523,15 +522,15 @@
         data: object,
         cast_to: type[ResponseT],
         response: httpx.Response,
     ) -> ResponseT:
         if data is None:
             return cast(ResponseT, None)
 
-        if cast_to is UnknownResponse:
+        if cast_to is object:
             return cast(ResponseT, data)
 
         try:
             if inspect.isclass(cast_to) and issubclass(cast_to, ModelBuilderProtocol):
                 return cast(ResponseT, cast_to.build(response=response, data=data))
 
             if self._strict_response_validation:
@@ -869,19 +868,23 @@
     ) -> ResponseT | _StreamT:
         self._prepare_options(options)
 
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
         self._prepare_request(request)
 
+        kwargs: HttpxSendArgs = {}
+        if self.custom_auth is not None:
+            kwargs["auth"] = self.custom_auth
+
         try:
             response = self._client.send(
                 request,
-                auth=self.custom_auth,
                 stream=stream or self._should_stream_response_body(request=request),
+                **kwargs,
             )
         except httpx.TimeoutException as err:
             if retries > 0:
                 return self._retry_request(
                     options,
                     cast_to,
                     retries,
@@ -961,15 +964,15 @@
             remaining_retries=remaining,
             stream=stream,
             stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
-        model: Type[ModelT],
+        model: Type[object],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
     ) -> SyncPageT:
         def _parser(resp: SyncPageT) -> SyncPageT:
             resp._set_private_attributes(
                 client=self,
                 model=model,
@@ -1123,15 +1126,15 @@
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
         return self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
-        model: Type[ModelT],
+        model: Type[object],
         page: Type[SyncPageT],
         body: Body | None = None,
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
@@ -1331,19 +1334,23 @@
     ) -> ResponseT | _AsyncStreamT:
         await self._prepare_options(options)
 
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
         await self._prepare_request(request)
 
+        kwargs: HttpxSendArgs = {}
+        if self.custom_auth is not None:
+            kwargs["auth"] = self.custom_auth
+
         try:
             response = await self._client.send(
                 request,
-                auth=self.custom_auth,
                 stream=stream or self._should_stream_response_body(request=request),
+                **kwargs,
             )
         except httpx.TimeoutException as err:
             if retries > 0:
                 return await self._retry_request(
                     options,
                     cast_to,
                     retries,
@@ -1421,18 +1428,18 @@
             remaining_retries=remaining,
             stream=stream,
             stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
-        model: Type[ModelT],
+        model: Type[_T],
         page: Type[AsyncPageT],
         options: FinalRequestOptions,
-    ) -> AsyncPaginator[ModelT, AsyncPageT]:
+    ) -> AsyncPaginator[_T, AsyncPageT]:
         return AsyncPaginator(client=self, options=options, page_cls=page, model=model)
 
     @overload
     async def get(
         self,
         path: str,
         *,
@@ -1571,21 +1578,20 @@
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
         return await self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
-        # TODO: support paginating `str`
-        model: Type[ModelT],
+        model: Type[_T],
         page: Type[AsyncPageT],
         body: Body | None = None,
         options: RequestOptions = {},
         method: str = "get",
-    ) -> AsyncPaginator[ModelT, AsyncPageT]:
+    ) -> AsyncPaginator[_T, AsyncPageT]:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
 def make_request_options(
     *,
     query: Query | None = None,
```

### Comparing `anthropic-0.8.1/src/anthropic/_client.py` & `anthropic-0.9.0/src/anthropic/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,26 @@
     Timeout,
     NotGiven,
     Transport,
     ProxiesTypes,
     AsyncTransport,
     RequestOptions,
 )
-from ._utils import is_given, get_async_library
+from ._utils import (
+    is_given,
+    get_async_library,
+)
 from ._version import __version__
-from ._streaming import Stream as Stream
-from ._streaming import AsyncStream as AsyncStream
+from ._streaming import Stream as Stream, AsyncStream as AsyncStream
 from ._exceptions import APIStatusError
-from ._tokenizers import TokenizerType  # type: ignore[import]
-from ._tokenizers import sync_get_tokenizer, async_get_tokenizer
+from ._tokenizers import (
+    TokenizerType,  # type: ignore[import]
+    sync_get_tokenizer,
+    async_get_tokenizer,
+)
 from ._base_client import (
     DEFAULT_LIMITS,
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
     SyncHttpxClientWrapper,
     AsyncHttpxClientWrapper,
```

### Comparing `anthropic-0.8.1/src/anthropic/_compat.py` & `anthropic-0.9.0/src/anthropic/_compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,29 +39,31 @@
         ...
 
     def is_typeddict(type_: type[Any]) -> bool:  # noqa: ARG001
         ...
 
 else:
     if PYDANTIC_V2:
-        from pydantic.v1.typing import get_args as get_args
-        from pydantic.v1.typing import is_union as is_union
-        from pydantic.v1.typing import get_origin as get_origin
-        from pydantic.v1.typing import is_typeddict as is_typeddict
-        from pydantic.v1.typing import is_literal_type as is_literal_type
-        from pydantic.v1.datetime_parse import parse_date as parse_date
-        from pydantic.v1.datetime_parse import parse_datetime as parse_datetime
+        from pydantic.v1.typing import (
+            get_args as get_args,
+            is_union as is_union,
+            get_origin as get_origin,
+            is_typeddict as is_typeddict,
+            is_literal_type as is_literal_type,
+        )
+        from pydantic.v1.datetime_parse import parse_date as parse_date, parse_datetime as parse_datetime
     else:
-        from pydantic.typing import get_args as get_args
-        from pydantic.typing import is_union as is_union
-        from pydantic.typing import get_origin as get_origin
-        from pydantic.typing import is_typeddict as is_typeddict
-        from pydantic.typing import is_literal_type as is_literal_type
-        from pydantic.datetime_parse import parse_date as parse_date
-        from pydantic.datetime_parse import parse_datetime as parse_datetime
+        from pydantic.typing import (
+            get_args as get_args,
+            is_union as is_union,
+            get_origin as get_origin,
+            is_typeddict as is_typeddict,
+            is_literal_type as is_literal_type,
+        )
+        from pydantic.datetime_parse import parse_date as parse_date, parse_datetime as parse_datetime
 
 
 # refactored config
 if TYPE_CHECKING:
     from pydantic import ConfigDict as ConfigDict
 else:
     if PYDANTIC_V2:
@@ -167,7 +169,17 @@
             ...
 
     else:
         import pydantic.generics
 
         class GenericModel(pydantic.generics.GenericModel, pydantic.BaseModel):
             ...
+
+
+# cached properties
+if TYPE_CHECKING:
+    cached_property = property
+else:
+    try:
+        from functools import cached_property as cached_property
+    except ImportError:
+        from cached_property import cached_property as cached_property
```

### Comparing `anthropic-0.8.1/src/anthropic/_exceptions.py` & `anthropic-0.9.0/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_files.py` & `anthropic-0.9.0/src/anthropic/_files.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_models.py` & `anthropic-0.9.0/src/anthropic/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,19 @@
     ModelT,
     Headers,
     Timeout,
     NotGiven,
     AnyMapping,
     HttpxRequestFiles,
 )
-from ._utils import (
-    is_list,
-    is_given,
-    is_mapping,
-    parse_date,
-    parse_datetime,
-    strip_not_given,
-)
-from ._compat import PYDANTIC_V2, ConfigDict
-from ._compat import GenericModel as BaseGenericModel
+from ._utils import is_list, is_given, is_mapping, parse_date, parse_datetime, strip_not_given
 from ._compat import (
+    PYDANTIC_V2,
+    ConfigDict,
+    GenericModel as BaseGenericModel,
     get_args,
     is_union,
     parse_obj,
     get_origin,
     is_literal_type,
     get_model_config,
     get_model_fields,
```

### Comparing `anthropic-0.8.1/src/anthropic/_qs.py` & `anthropic-0.9.0/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_resource.py` & `anthropic-0.9.0/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_response.py` & `anthropic-0.9.0/src/anthropic/_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import functools
 from typing import TYPE_CHECKING, Any, Union, Generic, TypeVar, Callable, cast
 from typing_extensions import Awaitable, ParamSpec, override, get_origin
 
 import httpx
 
-from ._types import NoneType, UnknownResponse, BinaryResponseContent
+from ._types import NoneType, BinaryResponseContent
 from ._utils import is_given, extract_type_var_from_base
 from ._models import BaseModel, is_basemodel
 from ._constants import RAW_RESPONSE_HEADER
 from ._exceptions import APIResponseValidationError
 
 if TYPE_CHECKING:
     from ._models import FinalRequestOptions
@@ -158,15 +158,15 @@
         # which means we must return *exactly* what was input or transform it in a
         # way that retains the TypeVar state. As we cannot do that in this function
         # then we have to resort to using `cast`. At the time of writing, we know this
         # to be safe as we have handled all the types that could be bound to the
         # `ResponseT` TypeVar, however if that TypeVar is ever updated in the future, then
         # this function would become unsafe but a type checker would not report an error.
         if (
-            cast_to is not UnknownResponse
+            cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
             and not issubclass(origin, BaseModel)
         ):
             raise RuntimeError(
                 f"Invalid state, expected {cast_to} to be a subclass type of {BaseModel}, {dict}, {list} or {Union}."
```

### Comparing `anthropic-0.8.1/src/anthropic/_streaming.py` & `anthropic-0.9.0/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_tokenizers.py` & `anthropic-0.9.0/src/anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_types.py` & `anthropic-0.9.0/src/anthropic/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,17 @@
     TypeVar,
     Callable,
     Iterator,
     Optional,
     Sequence,
     AsyncIterator,
 )
-from typing_extensions import (
-    Literal,
-    Protocol,
-    TypeAlias,
-    TypedDict,
-    override,
-    runtime_checkable,
-)
+from typing_extensions import Literal, Protocol, TypeAlias, TypedDict, override, runtime_checkable
 
+import httpx
 import pydantic
 from httpx import URL, Proxy, Timeout, Response, BaseTransport, AsyncBaseTransport
 
 if TYPE_CHECKING:
     from ._models import BaseModel
 
 Transport = BaseTransport
@@ -260,19 +254,14 @@
     max_retries: int
     timeout: float | Timeout | None
     params: Query
     extra_json: AnyMapping
     idempotency_key: str
 
 
-# Sentinel class used when the response type is an object with an unknown schema
-class UnknownResponse:
-    ...
-
-
 # Sentinel class used until PEP 0661 is accepted
 class NotGiven:
     """
     A sentinel singleton class used to distinguish omitted keyword arguments
     from those passed in with the value None (which may have different behavior).
 
     For example:
@@ -341,15 +330,25 @@
         ...
 
 
 HeadersLike = Union[Headers, HeadersLikeProtocol]
 
 ResponseT = TypeVar(
     "ResponseT",
-    bound="Union[str, None, BaseModel, List[Any], Dict[str, Any], Response, UnknownResponse, ModelBuilderProtocol, BinaryResponseContent]",
+    bound=Union[
+        object,
+        str,
+        None,
+        "BaseModel",
+        List[Any],
+        Dict[str, Any],
+        Response,
+        ModelBuilderProtocol,
+        BinaryResponseContent,
+    ],
 )
 
 StrBytesIntFloat = Union[str, bytes, int, float]
 
 # Note: copied from Pydantic
 # https://github.com/pydantic/pydantic/blob/32ea570bf96e84234d2992e1ddf40ab8a565925a/pydantic/main.py#L49
 IncEx: TypeAlias = "set[int] | set[str] | dict[int, Any] | dict[str, Any] | None"
@@ -365,7 +364,11 @@
     """
 
     __orig_bases__: tuple[_GenericAlias]
 
 
 class _GenericAlias(Protocol):
     __origin__: type[object]
+
+
+class HttpxSendArgs(TypedDict, total=False):
+    auth: httpx.Auth
```

### Comparing `anthropic-0.8.1/src/anthropic/tokenizer.json` & `anthropic-0.9.0/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_utils/_logs.py` & `anthropic-0.9.0/src/anthropic/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_utils/_proxy.py` & `anthropic-0.9.0/src/anthropic/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_utils/_transform.py` & `anthropic-0.9.0/src/anthropic/_utils/_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 from typing import Any, Mapping, TypeVar, cast
 from datetime import date, datetime
 from typing_extensions import Literal, get_args, override, get_type_hints
 
 import pydantic
 
-from ._utils import is_list, is_mapping
+from ._utils import (
+    is_list,
+    is_mapping,
+)
 from ._typing import (
     is_list_type,
     is_union_type,
     extract_type_arg,
     is_required_type,
     is_annotated_type,
     strip_annotated_type,
```

### Comparing `anthropic-0.8.1/src/anthropic/_utils/_typing.py` & `anthropic-0.9.0/src/anthropic/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/_utils/_utils.py` & `anthropic-0.9.0/src/anthropic/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
 from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
-from .._compat import parse_date as parse_date
-from .._compat import parse_datetime as parse_datetime
+from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
```

### Comparing `anthropic-0.8.1/src/anthropic/lib/streaming/_messages.py` & `anthropic-0.9.0/src/anthropic/lib/streaming/_messages.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/resources/completions.py` & `anthropic-0.9.0/src/anthropic/resources/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Union, overload
+from typing import List, Union, overload
 from typing_extensions import Literal
 
 import httpx
 
 from ..types import Completion, completion_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import required_args, maybe_transform
+from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._streaming import Stream, AsyncStream
-from .._base_client import make_request_options
-
-if TYPE_CHECKING:
-    from .._client import Anthropic, AsyncAnthropic
+from .._base_client import (
+    make_request_options,
+)
 
 __all__ = ["Completions", "AsyncCompletions"]
 
 
 class Completions(SyncAPIResource):
-    with_raw_response: CompletionsWithRawResponse
-
-    def __init__(self, client: Anthropic) -> None:
-        super().__init__(client)
-        self.with_raw_response = CompletionsWithRawResponse(self)
+    @cached_property
+    def with_raw_response(self) -> CompletionsWithRawResponse:
+        return CompletionsWithRawResponse(self)
 
     @overload
     def create(
         self,
         *,
         max_tokens_to_sample: int,
         model: Union[str, Literal["claude-2.1", "claude-instant-1"]],
@@ -355,19 +353,17 @@
             cast_to=Completion,
             stream=stream or False,
             stream_cls=Stream[Completion],
         )
 
 
 class AsyncCompletions(AsyncAPIResource):
-    with_raw_response: AsyncCompletionsWithRawResponse
-
-    def __init__(self, client: AsyncAnthropic) -> None:
-        super().__init__(client)
-        self.with_raw_response = AsyncCompletionsWithRawResponse(self)
+    @cached_property
+    def with_raw_response(self) -> AsyncCompletionsWithRawResponse:
+        return AsyncCompletionsWithRawResponse(self)
 
     @overload
     async def create(
         self,
         *,
         max_tokens_to_sample: int,
         model: Union[str, Literal["claude-2.1", "claude-instant-1"]],
```

### Comparing `anthropic-0.8.1/src/anthropic/resources/beta/beta.py` & `anthropic-0.9.0/src/anthropic/resources/beta/beta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
-from .messages import (
-    Messages,
-    AsyncMessages,
-    MessagesWithRawResponse,
-    AsyncMessagesWithRawResponse,
-)
+from .messages import Messages, AsyncMessages, MessagesWithRawResponse, AsyncMessagesWithRawResponse
+from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 
-if TYPE_CHECKING:
-    from ..._client import Anthropic, AsyncAnthropic
-
 __all__ = ["Beta", "AsyncBeta"]
 
 
 class Beta(SyncAPIResource):
-    messages: Messages
-    with_raw_response: BetaWithRawResponse
-
-    def __init__(self, client: Anthropic) -> None:
-        super().__init__(client)
-        self.messages = Messages(client)
-        self.with_raw_response = BetaWithRawResponse(self)
+    @cached_property
+    def messages(self) -> Messages:
+        return Messages(self._client)
+
+    @cached_property
+    def with_raw_response(self) -> BetaWithRawResponse:
+        return BetaWithRawResponse(self)
 
 
 class AsyncBeta(AsyncAPIResource):
-    messages: AsyncMessages
-    with_raw_response: AsyncBetaWithRawResponse
-
-    def __init__(self, client: AsyncAnthropic) -> None:
-        super().__init__(client)
-        self.messages = AsyncMessages(client)
-        self.with_raw_response = AsyncBetaWithRawResponse(self)
+    @cached_property
+    def messages(self) -> AsyncMessages:
+        return AsyncMessages(self._client)
+
+    @cached_property
+    def with_raw_response(self) -> AsyncBetaWithRawResponse:
+        return AsyncBetaWithRawResponse(self)
 
 
 class BetaWithRawResponse:
     def __init__(self, beta: Beta) -> None:
         self.messages = MessagesWithRawResponse(beta.messages)
```

### Comparing `anthropic-0.8.1/src/anthropic/resources/beta/messages.py` & `anthropic-0.9.0/src/anthropic/resources/beta/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, overload
+from typing import List, overload
 from functools import partial
 from typing_extensions import Literal
 
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import required_args, maybe_transform
+from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._streaming import Stream, AsyncStream
-from ...types.beta import (
-    Message,
-    MessageParam,
-    MessageStreamEvent,
-    message_create_params,
+from ...types.beta import Message, MessageParam, MessageStreamEvent, message_create_params
+from ..._base_client import (
+    make_request_options,
 )
-from ..._base_client import make_request_options
 from ...lib.streaming import (
     MessageStream,
     MessageStreamT,
     AsyncMessageStream,
     AsyncMessageStreamT,
     MessageStreamManager,
     AsyncMessageStreamManager,
 )
 
-if TYPE_CHECKING:
-    from ..._client import Anthropic, AsyncAnthropic
-
 __all__ = ["Messages", "AsyncMessages"]
 
 
 class Messages(SyncAPIResource):
-    with_raw_response: MessagesWithRawResponse
-
-    def __init__(self, client: Anthropic) -> None:
-        super().__init__(client)
-        self.with_raw_response = MessagesWithRawResponse(self)
+    @cached_property
+    def with_raw_response(self) -> MessagesWithRawResponse:
+        return MessagesWithRawResponse(self)
 
     @overload
     def create(
         self,
         *,
         max_tokens: int,
         messages: List[MessageParam],
@@ -659,19 +652,17 @@
             stream=True,
             stream_cls=event_handler,
         )
         return MessageStreamManager(make_request)
 
 
 class AsyncMessages(AsyncAPIResource):
-    with_raw_response: AsyncMessagesWithRawResponse
-
-    def __init__(self, client: AsyncAnthropic) -> None:
-        super().__init__(client)
-        self.with_raw_response = AsyncMessagesWithRawResponse(self)
+    @cached_property
+    def with_raw_response(self) -> AsyncMessagesWithRawResponse:
+        return AsyncMessagesWithRawResponse(self)
 
     @overload
     async def create(
         self,
         *,
         max_tokens: int,
         messages: List[MessageParam],
```

### Comparing `anthropic-0.8.1/src/anthropic/types/completion.py` & `anthropic-0.9.0/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/types/completion_create_params.py` & `anthropic-0.9.0/src/anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/types/beta/__init__.py` & `anthropic-0.9.0/src/anthropic/types/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/types/beta/message.py` & `anthropic-0.9.0/src/anthropic/types/beta/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     role: Literal["assistant"]
     """Conversational role of the generated message.
 
     This will always be `"assistant"`.
     """
 
-    stop_reason: Optional[Literal["end_turn", "max_tokens", "stop_sequence"]]
+    stop_reason: Optional[Literal["end_turn", "max_tokens", "stop_sequence"]] = None
     """The reason that we stopped.
 
     This may be one the following values:
 
     - `"end_turn"`: the model reached a natural stopping point
     - `"max_tokens"`: we exceeded the requested `max_tokens` or the model's maximum
     - `"stop_sequence"`: one of your provided custom `stop_sequences` was generated
@@ -75,14 +75,14 @@
     Note that these values are different than those in `/v1/complete`, where
     `end_turn` and `stop_sequence` were not differentiated.
 
     In non-streaming mode this value is always non-null. In streaming mode, it is
     null in the `message_start` event and non-null otherwise.
     """
 
-    stop_sequence: Optional[str]
+    stop_sequence: Optional[str] = None
     """Which custom stop sequence was generated.
 
     This value will be non-null if one of your custom stop sequences was generated.
     """
 
     type: Literal["message"]
```

### Comparing `anthropic-0.8.1/src/anthropic/types/beta/message_create_params.py` & `anthropic-0.9.0/src/anthropic/types/beta/message_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/src/anthropic/types/beta/message_stream_event.py` & `anthropic-0.9.0/src/anthropic/types/beta/message_stream_event.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/LICENSE` & `anthropic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/README.md` & `anthropic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `anthropic-0.8.1/pyproject.toml` & `anthropic-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "anthropic"
-version = "0.8.1"
+version = "0.9.0"
 description = "The official Python library for the anthropic API"
 readme = "README.md"
 license = "MIT"
 authors = [
 { name = "Anthropic", email = "support@anthropic.com" },
 ]
 dependencies = [
     "httpx>=0.23.0, <1",
     "pydantic>=1.9.0, <3",
     "typing-extensions>=4.7, <5",
     "anyio>=3.5.0, <5",
     "distro>=1.7.0, <2",
     "sniffio",
+    "cached-property; python_version < '3.8'",
     "tokenizers >= 0.13.0"
 ]
 requires-python = ">= 3.7"
 classifiers = [
   "Typing :: Typed",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3.7",
@@ -49,28 +50,26 @@
 dev-dependencies = [
     "pyright",
     "mypy",
     "respx",
     "pytest",
     "pytest-asyncio",
     "ruff",
-    "isort",
     "time-machine",
     "nox",
     "dirty-equals>=0.6.0",
     "importlib-metadata>=6.7.0",
 
 ]
 
 [tool.rye.scripts]
 format = { chain = [
   "format:ruff",
   "format:docs",
   "fix:ruff",
-  "format:isort",
 ]}
 "format:black" = "black ."
 "format:docs" = "python bin/ruffen-docs.py README.md api.md"
 "format:ruff" = "ruff format"
 "format:isort" = "isort ."
 
 "check:ruff" = "ruff ."
@@ -123,24 +122,21 @@
 ]
 
 reportImplicitOverride = true
 
 reportImportCycles = false
 reportPrivateUsage = false
 
-[tool.isort]
-profile = "black"
-length_sort = true
-extra_standard_library = ["typing_extensions"]
-
 [tool.ruff]
 line-length = 120
 output-format = "grouped"
 target-version = "py37"
 select = [
+  # isort
+  "I",
   # bugbear rules
   "B",
   # remove unused imports
   "F401",
   # bare except statements
   "E722",
   # unused arguments
@@ -159,11 +155,18 @@
   "T203",
 ]
 ignore-init-module-imports = true
 
 [tool.ruff.format]
 docstring-code-format = true
 
+[tool.ruff.lint.isort]
+length-sort = true
+length-sort-straight = true
+combine-as-imports = true
+extra-standard-library = ["typing_extensions"]
+known-first-party = ["anthropic", "tests"]
+
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `anthropic-0.8.1/PKG-INFO` & `anthropic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.8.1
+Version: 0.9.0
 Summary: The official Python library for the anthropic API
 Project-URL: Homepage, https://github.com/anthropics/anthropic-sdk-python
 Project-URL: Repository, https://github.com/anthropics/anthropic-sdk-python
 Author-email: Anthropic <support@anthropic.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: anyio<5,>=3.5.0
+Requires-Dist: cached-property; python_version < '3.8'
 Requires-Dist: distro<2,>=1.7.0
 Requires-Dist: httpx<1,>=0.23.0
 Requires-Dist: pydantic<3,>=1.9.0
 Requires-Dist: sniffio
 Requires-Dist: tokenizers>=0.13.0
 Requires-Dist: typing-extensions<5,>=4.7
 Description-Content-Type: text/markdown
```

