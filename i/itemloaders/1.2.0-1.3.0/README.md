# Comparing `tmp/itemloaders-1.2.0.tar.gz` & `tmp/itemloaders-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemloaders-1.2.0.tar", last modified: Thu Apr 18 09:56:24 2024, max compression
+gzip compressed data, was "itemloaders-1.3.0.tar", last modified: Thu May 30 11:09:35 2024, max compression
```

## Comparing `itemloaders-1.2.0.tar` & `itemloaders-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-18 09:56:14.000000 itemloaders-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:56:14.000000 itemloaders-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-18 09:56:23.996741 itemloaders-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-18 09:56:14.000000 itemloaders-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/itemloaders/
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-18 09:56:14.000000 itemloaders-1.2.0/itemloaders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/itemloaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 09:56:23.000000 itemloaders-1.2.0/itemloaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 09:56:23.996741 itemloaders-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-18 09:56:14.000000 itemloaders-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:56:23.996741 itemloaders-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_base_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_loader_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_nested_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_nested_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_output_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_select_jmes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_selector_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-18 09:56:14.000000 itemloaders-1.2.0/tests/test_utils_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 11:09:20.000000 itemloaders-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 11:09:20.000000 itemloaders-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-30 11:09:35.991864 itemloaders-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 11:09:20.000000 itemloaders-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.987864 itemloaders-1.3.0/itemloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    22988 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/itemloaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 11:09:35.991864 itemloaders-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 11:09:20.000000 itemloaders-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_loader_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_nested_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_nested_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_output_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_select_jmes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_selector_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_utils_python.py
```

### Comparing `itemloaders-1.2.0/LICENSE` & `itemloaders-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itemloaders-1.2.0/PKG-INFO` & `itemloaders-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.2.0
+Version: 1.3.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.2.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.3.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `itemloaders-1.2.0/README.rst` & `itemloaders-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `itemloaders-1.2.0/itemloaders/__init__.py` & `itemloaders-1.3.0/itemloaders/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 """
 Item Loader
 
 See documentation in docs/topics/loaders.rst
 """
 
+from __future__ import annotations
+
 from contextlib import suppress
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    MutableMapping,
+    Optional,
+    Pattern,
+    Union,
+)
 
 from itemadapter import ItemAdapter
+from parsel import Selector
 from parsel.utils import extract_regex, flatten
 
 from itemloaders.common import wrap_loader_context
 from itemloaders.processors import Identity
 from itemloaders.utils import arg_to_iter
 
+if TYPE_CHECKING:
+    # typing.Self requires Python 3.11
+    from typing_extensions import Self
+
 
-def unbound_method(method):
+def unbound_method(method: Callable[..., Any]) -> Callable[..., Any]:
     """
     Allow to use single-argument functions as input or output processors
     (no need to define an unused first 'self' argument)
     """
     with suppress(AttributeError):
         if "." not in method.__qualname__:
-            return method.__func__
+            return method.__func__  # type: ignore[attr-defined, no-any-return]
     return method
 
 
 class ItemLoader:
     """
     Return a new Item Loader for populating the given item. If no item is
     given, one is instantiated automatically using the class in
@@ -92,140 +111,179 @@
         The :class:`~parsel.selector.Selector` object to extract data from.
         It's the selector given in the ``__init__`` method.
         This attribute is meant to be read-only.
 
     .. _parsel: https://parsel.readthedocs.io/en/latest/
     """
 
-    default_item_class = dict
-    default_input_processor = Identity()
-    default_output_processor = Identity()
-
-    def __init__(self, item=None, selector=None, parent=None, **context):
-        self.selector = selector
+    default_item_class: type = dict
+    default_input_processor: Callable[..., Any] = Identity()
+    default_output_processor: Callable[..., Any] = Identity()
+
+    def __init__(
+        self,
+        item: Any = None,
+        selector: Optional[Selector] = None,
+        parent: Optional[ItemLoader] = None,
+        **context: Any,
+    ):
+        self.selector: Optional[Selector] = selector
         context.update(selector=selector)
         if item is None:
             item = self.default_item_class()
         self._local_item = item
         context["item"] = item
-        self.context = context
-        self.parent = parent
-        self._local_values = {}
+        self.context: MutableMapping[str, Any] = context
+        self.parent: Optional[ItemLoader] = parent
+        self._local_values: Dict[str, List[Any]] = {}
         # values from initial item
         for field_name, value in ItemAdapter(item).items():
             self._values.setdefault(field_name, [])
             self._values[field_name] += arg_to_iter(value)
 
     @property
-    def _values(self):
+    def _values(self) -> Dict[str, List[Any]]:
         if self.parent is not None:
             return self.parent._values
         else:
             return self._local_values
 
     @property
-    def item(self):
+    def item(self) -> Any:
         if self.parent is not None:
             return self.parent.item
         else:
             return self._local_item
 
-    def nested_xpath(self, xpath, **context):
+    def nested_xpath(self, xpath: str, **context: Any) -> Self:
         """
         Create a nested loader with an xpath selector.
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
+        self._check_selector_method()
+        assert self.selector
         selector = self.selector.xpath(xpath)
         context.update(selector=selector)
         subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
-    def nested_css(self, css, **context):
+    def nested_css(self, css: str, **context: Any) -> Self:
         """
         Create a nested loader with a css selector.
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
+        self._check_selector_method()
+        assert self.selector
         selector = self.selector.css(css)
         context.update(selector=selector)
         subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
-    def add_value(self, field_name, value, *processors, re=None, **kw):
+    def add_value(
+        self,
+        field_name: Optional[str],
+        value: Any,
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Process and then add the given ``value`` for the given field.
 
         The value is first passed through :meth:`get_value` by giving the
         ``processors`` and ``kwargs``, and then passed through the
         :ref:`field input processor <processors>` and its result
         appended to the data collected for that field. If the field already
         contains collected data, the new data is added.
 
         The given ``field_name`` can be ``None``, in which case values for
         multiple fields may be added. And the processed value should be a dict
         with field_name mapped to values.
 
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         Examples::
 
             loader.add_value('name', 'Color TV')
             loader.add_value('colours', ['white', 'blue'])
             loader.add_value('length', '100')
             loader.add_value('name', 'name: foo', TakeFirst(), re='name: (.+)')
             loader.add_value(None, {'name': 'foo', 'sex': 'male'})
+
         """
         value = self.get_value(value, *processors, re=re, **kw)
         if value is None:
             return
         if not field_name:
             for k, v in value.items():
                 self._add_value(k, v)
         else:
             self._add_value(field_name, value)
+        return self
 
-    def replace_value(self, field_name, value, *processors, re=None, **kw):
+    def replace_value(
+        self,
+        field_name: Optional[str],
+        value: Any,
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`add_value` but replaces the collected data with the
         new value instead of adding it.
+
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
         """
         value = self.get_value(value, *processors, re=re, **kw)
         if value is None:
             return
         if not field_name:
             for k, v in value.items():
                 self._replace_value(k, v)
         else:
             self._replace_value(field_name, value)
+        return self
 
-    def _add_value(self, field_name, value):
+    def _add_value(self, field_name: str, value: Any) -> None:
         value = arg_to_iter(value)
         processed_value = self._process_input_value(field_name, value)
         if processed_value:
             self._values.setdefault(field_name, [])
             self._values[field_name] += arg_to_iter(processed_value)
 
-    def _replace_value(self, field_name, value):
+    def _replace_value(self, field_name: str, value: Any) -> None:
         self._values.pop(field_name, None)
         self._add_value(field_name, value)
 
-    def get_value(self, value, *processors, re=None, **kw):
+    def get_value(
+        self,
+        value: Any,
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Any:
         """
         Process the given ``value`` by the given ``processors`` and keyword
         arguments.
 
         Available keyword arguments:
 
         :param re: a regular expression to use for extracting data from the
             given value using :func:`~parsel.utils.extract_regex` method,
             applied before processors
-        :type re: str or typing.Pattern
+        :type re: str or typing.Pattern[str]
 
         Examples:
 
         >>> from itemloaders import ItemLoader
         >>> from itemloaders.processors import TakeFirst
         >>> loader = ItemLoader()
         >>> loader.get_value('name: foo', TakeFirst(), str.upper, re='name: (.+)')
@@ -245,29 +303,29 @@
             except Exception as e:
                 raise ValueError(
                     "Error with processor %s value=%r error='%s: %s'"
                     % (_proc.__class__.__name__, value, type(e).__name__, str(e))
                 ) from e
         return value
 
-    def load_item(self):
+    def load_item(self) -> Any:
         """
         Populate the item with the data collected so far, and return it. The
         data collected is first passed through the :ref:`output processors
         <processors>` to get the final value to assign to each item field.
         """
         adapter = ItemAdapter(self.item)
         for field_name in tuple(self._values):
             value = self.get_output_value(field_name)
             if value is not None:
                 adapter[field_name] = value
 
         return adapter.item
 
-    def get_output_value(self, field_name):
+    def get_output_value(self, field_name: str) -> Any:
         """
         Return the collected values parsed using the output processor, for the
         given field. This method doesn't populate or modify the item at all.
         """
         proc = self.get_output_processor(field_name)
         proc = wrap_loader_context(proc, self.context)
         value = self._values.get(field_name, [])
@@ -275,39 +333,41 @@
             return proc(value)
         except Exception as e:
             raise ValueError(
                 "Error with output processor: field=%r value=%r error='%s: %s'"
                 % (field_name, value, type(e).__name__, str(e))
             ) from e
 
-    def get_collected_values(self, field_name):
+    def get_collected_values(self, field_name: str) -> List[Any]:
         """Return the collected values for the given field."""
         return self._values.get(field_name, [])
 
-    def get_input_processor(self, field_name):
+    def get_input_processor(self, field_name: str) -> Callable[..., Any]:
         proc = getattr(self, "%s_in" % field_name, None)
         if not proc:
             proc = self._get_item_field_attr(
                 field_name, "input_processor", self.default_input_processor
             )
         return unbound_method(proc)
 
-    def get_output_processor(self, field_name):
+    def get_output_processor(self, field_name: str) -> Callable[..., Any]:
         proc = getattr(self, "%s_out" % field_name, None)
         if not proc:
             proc = self._get_item_field_attr(
                 field_name, "output_processor", self.default_output_processor
             )
         return unbound_method(proc)
 
-    def _get_item_field_attr(self, field_name, key, default=None):
+    def _get_item_field_attr(
+        self, field_name: str, key: Any, default: Any = None
+    ) -> Any:
         field_meta = ItemAdapter(self.item).get_field_meta(field_name)
         return field_meta.get(key, default)
 
-    def _process_input_value(self, field_name, value):
+    def _process_input_value(self, field_name: str, value: Any) -> Any:
         proc = self.get_input_processor(field_name)
         _proc = proc
         proc = wrap_loader_context(proc, self.context)
         try:
             return proc(value)
         except Exception as e:
             raise ValueError(
@@ -318,164 +378,249 @@
                     field_name,
                     value,
                     type(e).__name__,
                     str(e),
                 )
             ) from e
 
-    def _check_selector_method(self):
+    def _check_selector_method(self) -> None:
         if self.selector is None:
             raise RuntimeError(
                 "To use XPath or CSS selectors, %s "
                 "must be instantiated with a selector" % self.__class__.__name__
             )
 
-    def add_xpath(self, field_name, xpath, *processors, re=None, **kw):
+    def add_xpath(
+        self,
+        field_name: Optional[str],
+        xpath: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`ItemLoader.add_value` but receives an XPath instead of a
         value, which is used to extract a list of strings from the
         selector associated with this :class:`ItemLoader`.
 
         See :meth:`get_xpath` for ``kwargs``.
 
         :param xpath: the XPath to extract data from
         :type xpath: str
 
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.add_xpath('name', '//p[@class="product-name"]')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.add_xpath('price', '//p[@id="price"]', re='the price is (.*)')
 
         """
         values = self._get_xpathvalues(xpath, **kw)
-        self.add_value(field_name, values, *processors, re=re, **kw)
+        return self.add_value(field_name, values, *processors, re=re, **kw)
 
-    def replace_xpath(self, field_name, xpath, *processors, re=None, **kw):
+    def replace_xpath(
+        self,
+        field_name: Optional[str],
+        xpath: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`add_xpath` but replaces collected data instead of adding it.
+
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         """
         values = self._get_xpathvalues(xpath, **kw)
-        self.replace_value(field_name, values, *processors, re=re, **kw)
+        return self.replace_value(field_name, values, *processors, re=re, **kw)
 
-    def get_xpath(self, xpath, *processors, re=None, **kw):
+    def get_xpath(
+        self,
+        xpath: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Any:
         """
         Similar to :meth:`ItemLoader.get_value` but receives an XPath instead of a
         value, which is used to extract a list of unicode strings from the
         selector associated with this :class:`ItemLoader`.
 
         :param xpath: the XPath to extract data from
         :type xpath: str
 
         :param re: a regular expression to use for extracting data from the
             selected XPath region
-        :type re: str or typing.Pattern
+        :type re: str or typing.Pattern[str]
 
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.get_xpath('//p[@class="product-name"]')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.get_xpath('//p[@id="price"]', TakeFirst(), re='the price is (.*)')
 
         """
         values = self._get_xpathvalues(xpath, **kw)
         return self.get_value(values, *processors, re=re, **kw)
 
-    def _get_xpathvalues(self, xpaths, **kw):
+    def _get_xpathvalues(
+        self, xpaths: Union[str, Iterable[str]], **kw: Any
+    ) -> List[Any]:
         self._check_selector_method()
+        assert self.selector
         xpaths = arg_to_iter(xpaths)
         return flatten(self.selector.xpath(xpath, **kw).getall() for xpath in xpaths)
 
-    def add_css(self, field_name, css, *processors, re=None, **kw):
+    def add_css(
+        self,
+        field_name: Optional[str],
+        css: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`ItemLoader.add_value` but receives a CSS selector
         instead of a value, which is used to extract a list of unicode strings
         from the selector associated with this :class:`ItemLoader`.
 
         See :meth:`get_css` for ``kwargs``.
 
         :param css: the CSS selector to extract data from
         :type css: str
 
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.add_css('name', 'p.product-name')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.add_css('price', 'p#price', re='the price is (.*)')
+
         """
         values = self._get_cssvalues(css)
-        self.add_value(field_name, values, *processors, re=re, **kw)
+        return self.add_value(field_name, values, *processors, re=re, **kw)
 
-    def replace_css(self, field_name, css, *processors, re=None, **kw):
+    def replace_css(
+        self,
+        field_name: Optional[str],
+        css: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`add_css` but replaces collected data instead of adding it.
+
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         """
         values = self._get_cssvalues(css)
-        self.replace_value(field_name, values, *processors, re=re, **kw)
+        return self.replace_value(field_name, values, *processors, re=re, **kw)
 
-    def get_css(self, css, *processors, re=None, **kw):
+    def get_css(
+        self,
+        css: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Any:
         """
         Similar to :meth:`ItemLoader.get_value` but receives a CSS selector
         instead of a value, which is used to extract a list of unicode strings
         from the selector associated with this :class:`ItemLoader`.
 
         :param css: the CSS selector to extract data from
         :type css: str
 
         :param re: a regular expression to use for extracting data from the
             selected CSS region
-        :type re: str or typing.Pattern
+        :type re: str or typing.Pattern[str]
 
         Examples::
 
             # HTML snippet: <p class="product-name">Color TV</p>
             loader.get_css('p.product-name')
             # HTML snippet: <p id="price">the price is $1200</p>
             loader.get_css('p#price', TakeFirst(), re='the price is (.*)')
         """
         values = self._get_cssvalues(css)
         return self.get_value(values, *processors, re=re, **kw)
 
-    def _get_cssvalues(self, csss):
+    def _get_cssvalues(self, csss: Union[str, Iterable[str]]) -> List[Any]:
         self._check_selector_method()
+        assert self.selector
         csss = arg_to_iter(csss)
         return flatten(self.selector.css(css).getall() for css in csss)
 
-    def add_jmes(self, field_name, jmes, *processors, re=None, **kw):
+    def add_jmes(
+        self,
+        field_name: Optional[str],
+        jmes: str,
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`ItemLoader.add_value` but receives a JMESPath selector
         instead of a value, which is used to extract a list of unicode strings
         from the selector associated with this :class:`ItemLoader`.
 
         See :meth:`get_jmes` for ``kwargs``.
 
         :param jmes: the JMESPath selector to extract data from
         :type jmes: str
 
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
+
         Examples::
 
             # HTML snippet: {"name": "Color TV"}
             loader.add_jmes('name')
             # HTML snippet: {"price": the price is $1200"}
             loader.add_jmes('price', TakeFirst(), re='the price is (.*)')
         """
         values = self._get_jmesvalues(jmes)
-        self.add_value(field_name, values, *processors, re=re, **kw)
+        return self.add_value(field_name, values, *processors, re=re, **kw)
 
-    def replace_jmes(self, field_name, jmes, *processors, re=None, **kw):
+    def replace_jmes(
+        self,
+        field_name: Optional[str],
+        jmes: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Self:
         """
         Similar to :meth:`add_jmes` but replaces collected data instead of adding it.
+
+        :returns: The current ItemLoader instance for method chaining.
+        :rtype: ItemLoader
         """
         values = self._get_jmesvalues(jmes)
-        self.replace_value(field_name, values, *processors, re=re, **kw)
+        return self.replace_value(field_name, values, *processors, re=re, **kw)
 
-    def get_jmes(self, jmes, *processors, re=None, **kw):
+    def get_jmes(
+        self,
+        jmes: Union[str, Iterable[str]],
+        *processors: Callable[..., Any],
+        re: Union[str, Pattern[str], None] = None,
+        **kw: Any,
+    ) -> Any:
         """
         Similar to :meth:`ItemLoader.get_value` but receives a JMESPath selector
         instead of a value, which is used to extract a list of unicode strings
         from the selector associated with this :class:`ItemLoader`.
 
         :param jmes: the JMESPath selector to extract data from
         :type jmes: str
@@ -490,15 +635,16 @@
             loader.get_jmes('name')
             # HTML snippet: {"price": the price is $1200"}
             loader.get_jmes('price', TakeFirst(), re='the price is (.*)')
         """
         values = self._get_jmesvalues(jmes)
         return self.get_value(values, *processors, re=re, **kw)
 
-    def _get_jmesvalues(self, jmess):
+    def _get_jmesvalues(self, jmess: Union[str, Iterable[str]]) -> List[Any]:
         self._check_selector_method()
+        assert self.selector
         jmess = arg_to_iter(jmess)
         if not hasattr(self.selector, "jmespath"):
             raise AttributeError(
                 "Please install parsel >= 1.8.1 to get jmespath support"
             )
         return flatten(self.selector.jmespath(jmes).getall() for jmes in jmess)
```

### Comparing `itemloaders-1.2.0/itemloaders/processors.py` & `itemloaders-1.3.0/itemloaders/processors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module provides some commonly used processors for Item Loaders.
 
 See documentation in docs/topics/loaders.rst
 """
 
 from collections import ChainMap
+from typing import Any, Callable, Iterable, List, MutableMapping, Optional
 
 from itemloaders.common import wrap_loader_context
 from itemloaders.utils import arg_to_iter
 
 
 class MapCompose:
     """
@@ -50,27 +51,30 @@
     As with the Compose processor, functions can receive Loader contexts, and
     ``__init__`` method keyword arguments are used as default context values.
     See :class:`Compose` processor for more info.
 
     .. _`parsel selectors`: https://parsel.readthedocs.io/en/latest/parsel.html#parsel.selector.Selector.extract
     """  # noqa
 
-    def __init__(self, *functions, **default_loader_context):
+    def __init__(self, *functions: Callable[..., Any], **default_loader_context: Any):
         self.functions = functions
         self.default_loader_context = default_loader_context
 
-    def __call__(self, value, loader_context=None):
+    def __call__(
+        self, value: Any, loader_context: Optional[MutableMapping[str, Any]] = None
+    ) -> Iterable[Any]:
         values = arg_to_iter(value)
+        context: MutableMapping[str, Any]
         if loader_context:
             context = ChainMap(loader_context, self.default_loader_context)
         else:
             context = self.default_loader_context
         wrapped_funcs = [wrap_loader_context(f, context) for f in self.functions]
         for func in wrapped_funcs:
-            next_values = []
+            next_values: List[Any] = []
             for v in values:
                 try:
                     next_values += arg_to_iter(func(v))
                 except Exception as e:
                     raise ValueError(
                         "Error in MapCompose with "
                         "%s value=%r error='%s: %s'"
@@ -105,20 +109,23 @@
     The keyword arguments passed in the ``__init__`` method are used as the default
     Loader context values passed to each function call. However, the final
     Loader context values passed to functions are overridden with the currently
     active Loader context accessible through the :attr:`ItemLoader.context
     <itemloaders.ItemLoader.context>` attribute.
     """
 
-    def __init__(self, *functions, **default_loader_context):
+    def __init__(self, *functions: Callable[..., Any], **default_loader_context: Any):
         self.functions = functions
         self.stop_on_none = default_loader_context.get("stop_on_none", True)
         self.default_loader_context = default_loader_context
 
-    def __call__(self, value, loader_context=None):
+    def __call__(
+        self, value: Any, loader_context: Optional[MutableMapping[str, Any]] = None
+    ) -> Any:
+        context: MutableMapping[str, Any]
         if loader_context:
             context = ChainMap(loader_context, self.default_loader_context)
         else:
             context = self.default_loader_context
         wrapped_funcs = [wrap_loader_context(f, context) for f in self.functions]
         for func in wrapped_funcs:
             if value is None and self.stop_on_none:
@@ -144,15 +151,15 @@
 
     >>> from itemloaders.processors import TakeFirst
     >>> proc = TakeFirst()
     >>> proc(['', 'one', 'two', 'three'])
     'one'
     """
 
-    def __call__(self, values):
+    def __call__(self, values: Any) -> Any:
         for value in values:
             if value is not None and value != "":
                 return value
 
 
 class Identity:
     """
@@ -164,15 +171,15 @@
 
     >>> from itemloaders.processors import Identity
     >>> proc = Identity()
     >>> proc(['one', 'two', 'three'])
     ['one', 'two', 'three']
     """
 
-    def __call__(self, values):
+    def __call__(self, values: Any) -> Any:
         return values
 
 
 class SelectJmes:
     """
     Query the input string for the jmespath (given at instantiation), and return the answer
     Requires : jmespath(https://github.com/jmespath/jmespath)
@@ -194,21 +201,23 @@
     >>> proc_single_json_str('{"foo": "bar"}')
     'bar'
     >>> proc_json_list = Compose(json.loads, MapCompose(SelectJmes('foo')))
     >>> proc_json_list('[{"foo":"bar"}, {"baz":"tar"}]')
     ['bar']
     """
 
-    def __init__(self, json_path):
-        self.json_path = json_path
-        import jmespath
+    def __init__(self, json_path: str):
+        self.json_path: str = json_path
+        import jmespath.parser
+
+        self.compiled_path: jmespath.parser.ParsedResult = jmespath.compile(
+            self.json_path
+        )
 
-        self.compiled_path = jmespath.compile(self.json_path)
-
-    def __call__(self, value):
+    def __call__(self, value: Any) -> Any:
         """Query value for the jmespath query and return answer
         :param value: a data structure (dict, list) to extract from
         :return: Element extracted according to jmespath query
         """
         return self.compiled_path.search(value)
 
 
@@ -227,12 +236,12 @@
     >>> proc(['one', 'two', 'three'])
     'one two three'
     >>> proc = Join('<br>')
     >>> proc(['one', 'two', 'three'])
     'one<br>two<br>three'
     """
 
-    def __init__(self, separator=" "):
+    def __init__(self, separator: str = " "):
         self.separator = separator
 
-    def __call__(self, values):
+    def __call__(self, values: Any) -> str:
         return self.separator.join(values)
```

### Comparing `itemloaders-1.2.0/itemloaders/utils.py` & `itemloaders-1.3.0/itemloaders/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Copy/paste from scrapy source at the moment, to ensure tests are working.
 Refactoring to come later
 """
 
 import inspect
 from functools import partial
-from typing import Generator
+from typing import Any, Callable, Generator, Iterable, List
 
 
-def arg_to_iter(arg):
+def arg_to_iter(arg: Any) -> Iterable[Any]:
     """Return an iterable based on *arg*.
 
     If *arg* is a list, a tuple or a generator, it will be returned as is.
 
     If *arg* is ``None``, an empty list will be returned.
 
     If *arg* is anything else, a list will be returned with *arg* as its only
@@ -21,20 +21,20 @@
     if arg is None:
         return []
     if isinstance(arg, (list, tuple, Generator)):
         return arg
     return [arg]
 
 
-def get_func_args(func, stripself=False):
+def get_func_args(func: Callable[..., Any], stripself: bool = False) -> List[str]:
     """Return the argument name list of a callable object"""
     if not callable(func):
         raise TypeError(f"func must be callable, got {type(func).__name__!r}")
 
-    args = []
+    args: List[str] = []
     try:
         sig = inspect.signature(func)
     except ValueError:
         return args
 
     if isinstance(func, partial):
         partial_args = func.args
```

### Comparing `itemloaders-1.2.0/itemloaders.egg-info/PKG-INFO` & `itemloaders-1.3.0/itemloaders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.2.0
+Version: 1.3.0
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.2.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.3.0 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `itemloaders-1.2.0/itemloaders.egg-info/SOURCES.txt` & `itemloaders-1.3.0/itemloaders.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 itemloaders/__init__.py
 itemloaders/common.py
 itemloaders/processors.py
+itemloaders/py.typed
 itemloaders/utils.py
 itemloaders.egg-info/PKG-INFO
 itemloaders.egg-info/SOURCES.txt
 itemloaders.egg-info/dependency_links.txt
 itemloaders.egg-info/not-zip-safe
 itemloaders.egg-info/requires.txt
 itemloaders.egg-info/top_level.txt
```

### Comparing `itemloaders-1.2.0/setup.py` & `itemloaders-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="itemloaders",
-    version="1.2.0",
+    version="1.3.0",
     url="https://github.com/scrapy/itemloaders",
     project_urls={
         "Documentation": "https://itemloaders.readthedocs.io/",
         "Source": "https://github.com/scrapy/itemloaders",
     },
     description="Base library for scrapy's ItemLoader",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Zyte",
     author_email="opensource@zyte.com",
     license="BSD",
     packages=find_packages(exclude=("tests", "tests.*")),
+    package_data={
+        "itemadapter": ["py.typed"],
+    },
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
```

### Comparing `itemloaders-1.2.0/tests/test_base_loader.py` & `itemloaders-1.3.0/tests/test_base_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,25 +296,25 @@
         assert expected_exc_str in s, s
 
     def test_output_processor_using_classes(self):
         il = CustomItemLoader()
         il.add_value("name", ["mar", "ta"])
         self.assertEqual(il.get_output_value("name"), ["Mar", "Ta"])
 
-        class TakeFirstItemLoader(CustomItemLoader):
+        class TakeFirstItemLoader1(CustomItemLoader):
             name_out = Join()
 
-        il = TakeFirstItemLoader()
+        il = TakeFirstItemLoader1()
         il.add_value("name", ["mar", "ta"])
         self.assertEqual(il.get_output_value("name"), "Mar Ta")
 
-        class TakeFirstItemLoader(CustomItemLoader):
+        class TakeFirstItemLoader2(CustomItemLoader):
             name_out = Join("<br>")
 
-        il = TakeFirstItemLoader()
+        il = TakeFirstItemLoader2()
         il.add_value("name", ["mar", "ta"])
         self.assertEqual(il.get_output_value("name"), "Mar<br>Ta")
 
     def test_default_output_processor(self):
         il = CustomItemLoader()
         il.add_value("name", ["mar", "ta"])
         self.assertEqual(il.get_output_value("name"), ["Mar", "Ta"])
```

### Comparing `itemloaders-1.2.0/tests/test_loader_initialization.py` & `itemloaders-1.3.0/tests/test_loader_initialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,103 @@
 import unittest
+from typing import Any, Protocol
 
 from itemloaders import ItemLoader
 
 
+class InitializationTestProtocol(Protocol):
+    item_class: Any
+
+    def assertEqual(self, first: Any, second: Any, msg: Any = ...) -> None: ...
+
+    def assertIsInstance(self, obj: object, cls: type, msg: Any = None) -> None: ...
+
+
 class InitializationTestMixin:
-    item_class = None
+    item_class: Any = None
 
-    def test_keep_single_value(self):
+    def test_keep_single_value(self: InitializationTestProtocol) -> None:
         """Loaded item should contain values from the initial item"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo"]})
 
-    def test_keep_list(self):
+    def test_keep_list(self: InitializationTestProtocol) -> None:
         """Loaded item should contain values from the initial item"""
         input_item = self.item_class(name=["foo", "bar"])
         il = ItemLoader(item=input_item)
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo", "bar"]})
 
-    def test_add_value_singlevalue_singlevalue(self):
+    def test_add_value_singlevalue_singlevalue(
+        self: InitializationTestProtocol,
+    ) -> None:
         """Values added after initialization should be appended"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         il.add_value("name", "bar")
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo", "bar"]})
 
-    def test_add_value_singlevalue_list(self):
+    def test_add_value_singlevalue_list(self: InitializationTestProtocol) -> None:
         """Values added after initialization should be appended"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         il.add_value("name", ["item", "loader"])
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo", "item", "loader"]})
 
-    def test_add_value_list_singlevalue(self):
+    def test_add_value_list_singlevalue(self: InitializationTestProtocol) -> None:
         """Values added after initialization should be appended"""
         input_item = self.item_class(name=["foo", "bar"])
         il = ItemLoader(item=input_item)
         il.add_value("name", "qwerty")
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo", "bar", "qwerty"]})
 
-    def test_add_value_list_list(self):
+    def test_add_value_list_list(self: InitializationTestProtocol) -> None:
         """Values added after initialization should be appended"""
         input_item = self.item_class(name=["foo", "bar"])
         il = ItemLoader(item=input_item)
         il.add_value("name", ["item", "loader"])
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(dict(loaded_item), {"name": ["foo", "bar", "item", "loader"]})
 
-    def test_get_output_value_singlevalue(self):
+    def test_get_output_value_singlevalue(self: InitializationTestProtocol) -> None:
         """Getting output value must not remove value from item"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         self.assertEqual(il.get_output_value("name"), ["foo"])
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(loaded_item, {"name": ["foo"]})
 
-    def test_get_output_value_list(self):
+    def test_get_output_value_list(self: InitializationTestProtocol) -> None:
         """Getting output value must not remove value from item"""
         input_item = self.item_class(name=["foo", "bar"])
         il = ItemLoader(item=input_item)
         self.assertEqual(il.get_output_value("name"), ["foo", "bar"])
         loaded_item = il.load_item()
         self.assertIsInstance(loaded_item, self.item_class)
         self.assertEqual(loaded_item, {"name": ["foo", "bar"]})
 
-    def test_values_single(self):
+    def test_values_single(self: InitializationTestProtocol) -> None:
         """Values from initial item must be added to loader._values"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         self.assertEqual(il._values.get("name"), ["foo"])
 
-    def test_values_list(self):
+    def test_values_list(self: InitializationTestProtocol) -> None:
         """Values from initial item must be added to loader._values"""
         input_item = self.item_class(name=["foo", "bar"])
         il = ItemLoader(item=input_item)
         self.assertEqual(il._values.get("name"), ["foo", "bar"])
 
 
 class InitializationFromDictTest(InitializationTestMixin, unittest.TestCase):
```

### Comparing `itemloaders-1.2.0/tests/test_nested_items.py` & `itemloaders-1.3.0/tests/test_nested_items.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
+from typing import Any
 
 from itemloaders import ItemLoader
 
 
 class NestedItemTest(unittest.TestCase):
     """Test that adding items as values works as expected."""
 
-    def _test_item(self, item):
+    def _test_item(self, item: Any) -> None:
         il = ItemLoader()
         il.add_value("item_list", item)
         self.assertEqual(il.load_item(), {"item_list": [item]})
 
     def test_attrs(self):
         try:
             import attr
@@ -40,11 +41,12 @@
 
     def test_scrapy_item(self):
         try:
             from scrapy import Field, Item
         except ImportError:
             self.skipTest("Cannot import Field or Item from scrapy")
 
-        class TestItem(Item):
+        # needs py.typed in Scrapy
+        class TestItem(Item):  # type: ignore[misc]
             foo = Field()
 
         self._test_item(TestItem(foo="bar"))
```

### Comparing `itemloaders-1.2.0/tests/test_nested_loader.py` & `itemloaders-1.3.0/tests/test_nested_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     )
 
     def test_nested_xpath(self):
         loader = ItemLoader(selector=self.selector)
         nl = loader.nested_xpath("//header")
         nl.add_xpath("name", "div/text()")
         nl.add_css("name_div", "#id")
+        assert nl.selector
         nl.add_value("name_value", nl.selector.xpath('div[@id = "id"]/text()').getall())
 
         self.assertEqual(loader.get_output_value("name"), ["marta"])
         self.assertEqual(
             loader.get_output_value("name_div"), ['<div id="id">marta</div>']
         )
         self.assertEqual(loader.get_output_value("name_value"), ["marta"])
@@ -45,14 +46,15 @@
         )
 
     def test_nested_css(self):
         loader = ItemLoader(selector=self.selector)
         nl = loader.nested_css("header")
         nl.add_xpath("name", "div/text()")
         nl.add_css("name_div", "#id")
+        assert nl.selector
         nl.add_value("name_value", nl.selector.xpath('div[@id = "id"]/text()').getall())
 
         self.assertEqual(loader.get_output_value("name"), ["marta"])
         self.assertEqual(
             loader.get_output_value("name_div"), ['<div id="id">marta</div>']
         )
         self.assertEqual(loader.get_output_value("name_value"), ["marta"])
```

### Comparing `itemloaders-1.2.0/tests/test_output_processor.py` & `itemloaders-1.3.0/tests/test_output_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
+from typing import Any, Dict
 
 from itemloaders import ItemLoader
 from itemloaders.processors import Compose, Identity, TakeFirst
 
 
 class TestOutputProcessorDict(unittest.TestCase):
     def test_output_processor(self):
-        class TempDict(dict):
+        class TempDict(Dict[str, Any]):
             def __init__(self, *args, **kwargs):
                 super(TempDict, self).__init__(self, *args, **kwargs)
                 self.setdefault("temp", 0.3)
 
         class TempLoader(ItemLoader):
             default_item_class = TempDict
             default_input_processor = Identity()
@@ -24,13 +25,13 @@
 
 class TestOutputProcessorItem(unittest.TestCase):
     def test_output_processor(self):
         class TempLoader(ItemLoader):
             default_input_processor = Identity()
             default_output_processor = Compose(TakeFirst())
 
-        item = {}
+        item: Dict[str, Any] = {}
         item.setdefault("temp", 0.3)
         loader = TempLoader(item=item)
         item = loader.load_item()
         self.assertIsInstance(item, dict)
         self.assertEqual(dict(item), {"temp": 0.3})
```

### Comparing `itemloaders-1.2.0/tests/test_processors.py` & `itemloaders-1.3.0/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.2.0/tests/test_select_jmes.py` & `itemloaders-1.3.0/tests/test_select_jmes.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.2.0/tests/test_selector_loader.py` & `itemloaders-1.3.0/tests/test_selector_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,7 +269,23 @@
     def test_replace_jmes_re(self):
         loader = CustomItemLoader(selector=self.jmes_selector)
         self.assertTrue(loader.selector)
         loader.add_jmes("url", "website.url")
         self.assertEqual(loader.get_output_value("url"), ["http://www.scrapy.org"])
         loader.replace_jmes("url", "website.url", re=r"http://www\.(.+)")
         self.assertEqual(loader.get_output_value("url"), ["scrapy.org"])
+
+    def test_fluent_interface(self):
+        loader = ItemLoader(selector=self.selector)
+        item = (
+            loader.add_xpath("name", "//body/text()")
+            .replace_xpath("name", "//div/text()")
+            .add_css("description", "div::text")
+            .replace_css("description", "p::text")
+            .add_value("url", "http://example.com")
+            .replace_value("url", "http://foo")
+            .load_item()
+        )
+        self.assertEqual(
+            item,
+            {"name": ["marta"], "description": ["paragraph"], "url": ["http://foo"]},
+        )
```

### Comparing `itemloaders-1.2.0/tests/test_utils_misc.py` & `itemloaders-1.3.0/tests/test_utils_misc.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.2.0/tests/test_utils_python.py` & `itemloaders-1.3.0/tests/test_utils_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import operator
 import platform
 import unittest
+from typing import Any
 
 from itemloaders.utils import get_func_args
 
 
 class UtilsPythonTestCase(unittest.TestCase):
     def test_get_func_args(self):
         def f1(a, b, c):
@@ -14,15 +15,15 @@
         def f2(a, b=None, c=None):
             pass
 
         def f3(a, b=None, *, c=None):
             pass
 
         class A:
-            def __init__(self, a, b, c):
+            def __init__(self, a: Any, b: Any, c: Any):
                 pass
 
             def method(self, a, b, c):
                 pass
 
         class Callable:
             def __call__(self, a, b, c):
```

