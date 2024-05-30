# Comparing `tmp/dash_spread_grid-0.1.3.tar.gz` & `tmp/dash_spread_grid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_spread_grid-0.1.3.tar", last modified: Mon May 27 07:25:39 2024, max compression
+gzip compressed data, was "dash_spread_grid-0.1.4.tar", last modified: Wed May 29 17:33:56 2024, max compression
```

## Comparing `dash_spread_grid-0.1.3.tar` & `dash_spread_grid-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/LICENSE
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/MANIFEST.in
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.3/README.md
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/dash_spread_grid/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3288 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/DashSpreadGrid.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.3/dash_spread_grid/__init__.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/_imports_.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    55304 2024-05-27 07:25:37.000000 dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   216183 2024-05-27 07:25:37.000000 dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js.map
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6046 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid/metadata.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-27 07:25:38.000000 dash_spread_grid-0.1.3/dash_spread_grid/package-info.json
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-05-27 07:25:39.000000 dash_spread_grid-0.1.3/dash_spread_grid.egg-info/top_level.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-27 07:25:15.000000 dash_spread_grid-0.1.3/package.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-05-27 07:25:39.587835 dash_spread_grid-0.1.3/setup.cfg
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.3/setup.py
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-29 17:33:56.844204 dash_spread_grid-0.1.4/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.4/LICENSE
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.4/MANIFEST.in
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-29 17:33:56.844204 dash_spread_grid-0.1.4/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.4/README.md
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-29 17:33:56.844204 dash_spread_grid-0.1.4/dash_spread_grid/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3490 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid/DashSpreadGrid.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.4/dash_spread_grid/__init__.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid/_imports_.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    58495 2024-05-29 17:33:55.000000 dash_spread_grid-0.1.4/dash_spread_grid/dash_spread_grid.min.js
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   228893 2024-05-29 17:33:55.000000 dash_spread_grid-0.1.4/dash_spread_grid/dash_spread_grid.min.js.map
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6509 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid/metadata.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid/package-info.json
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-29 17:33:56.844204 dash_spread_grid-0.1.4/dash_spread_grid.egg-info/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-05-29 17:33:56.000000 dash_spread_grid-0.1.4/dash_spread_grid.egg-info/top_level.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-29 17:33:40.000000 dash_spread_grid-0.1.4/package.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-05-29 17:33:56.844204 dash_spread_grid-0.1.4/setup.cfg
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.4/setup.py
```

### Comparing `dash_spread_grid-0.1.3/README.md` & `dash_spread_grid-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/DashSpreadGrid.py` & `dash_spread_grid-0.1.4/dash_spread_grid/DashSpreadGrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 
 - borderWidth (number; default 1)
 
 - clicked_cell (dict; optional)
 
 - clicked_custom_cell (dict; optional)
 
-- columnWidths (list; optional)
+- column_widths (list; optional)
 
 - columns (list; default [{ "type": "DATA-BLOCK" }])
 
+- columns_order (list; optional)
+
 - data (boolean | number | string | dict | list; optional)
 
 - data_selector (string; default "data[row.id][column.id]")
 
 - edited_cells (list; optional)
 
 - filtering (list; optional)
@@ -45,32 +47,34 @@
 
 - pinned_left (number; default 0)
 
 - pinned_right (number; default 0)
 
 - pinned_top (number; default 0)
 
-- rowHeights (list; optional)
+- row_heights (list; optional)
 
 - rows (list; default [{ "type": "HEADER" }, { "type": "DATA-BLOCK" }])
 
+- rows_order (list; optional)
+
 - selected_cells (list; optional)
 
 - sort_by (list; optional)
 
 - sorting (list; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_spread_grid'
     _type = 'DashSpreadGrid'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, data=Component.UNDEFINED, columns=Component.UNDEFINED, rows=Component.UNDEFINED, formatting=Component.UNDEFINED, filtering=Component.UNDEFINED, sorting=Component.UNDEFINED, data_selector=Component.UNDEFINED, pinned_top=Component.UNDEFINED, pinned_bottom=Component.UNDEFINED, pinned_left=Component.UNDEFINED, pinned_right=Component.UNDEFINED, borderWidth=Component.UNDEFINED, focusedCell=Component.UNDEFINED, selected_cells=Component.UNDEFINED, highlightedCells=Component.UNDEFINED, edited_cells=Component.UNDEFINED, filters=Component.UNDEFINED, sort_by=Component.UNDEFINED, columnWidths=Component.UNDEFINED, rowHeights=Component.UNDEFINED, clicked_cell=Component.UNDEFINED, clicked_custom_cell=Component.UNDEFINED, active_columns=Component.UNDEFINED, active_rows=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selected_cells', 'sort_by', 'sorting']
+    def __init__(self, id=Component.UNDEFINED, data=Component.UNDEFINED, columns=Component.UNDEFINED, rows=Component.UNDEFINED, formatting=Component.UNDEFINED, filtering=Component.UNDEFINED, sorting=Component.UNDEFINED, data_selector=Component.UNDEFINED, pinned_top=Component.UNDEFINED, pinned_bottom=Component.UNDEFINED, pinned_left=Component.UNDEFINED, pinned_right=Component.UNDEFINED, borderWidth=Component.UNDEFINED, focusedCell=Component.UNDEFINED, selected_cells=Component.UNDEFINED, highlightedCells=Component.UNDEFINED, edited_cells=Component.UNDEFINED, filters=Component.UNDEFINED, sort_by=Component.UNDEFINED, column_widths=Component.UNDEFINED, row_heights=Component.UNDEFINED, columns_order=Component.UNDEFINED, rows_order=Component.UNDEFINED, clicked_cell=Component.UNDEFINED, clicked_custom_cell=Component.UNDEFINED, active_columns=Component.UNDEFINED, active_rows=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'column_widths', 'columns', 'columns_order', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'row_heights', 'rows', 'rows_order', 'selected_cells', 'sort_by', 'sorting']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selected_cells', 'sort_by', 'sorting']
+        self.available_properties = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'column_widths', 'columns', 'columns_order', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'row_heights', 'rows', 'rows_order', 'selected_cells', 'sort_by', 'sorting']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(DashSpreadGrid, self).__init__(**args)
```

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/__init__.py` & `dash_spread_grid-0.1.4/dash_spread_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js` & `dash_spread_grid-0.1.4/dash_spread_grid/dash_spread_grid.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 __webpack_require__.d(__webpack_exports__, {
                     Z: () => __WEBPACK_DEFAULT_EXPORT__
                 });
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(196),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(64),
                     prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
-                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(906);
+                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(317);
 
                 function _typeof(e) {
                     return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, _typeof(e)
@@ -42,28 +42,28 @@
                 }
 
                 function _iterableToArrayLimit(e, t) {
                     var o = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null != o) {
                         var n, r, i, l, s = [],
                             a = !0,
-                            c = !1;
+                            u = !1;
                         try {
                             if (i = (o = o.call(e)).next, 0 === t) {
                                 if (Object(o) !== o) return;
                                 a = !1
                             } else
                                 for (; !(a = (n = i.call(o)).done) && (s.push(n.value), s.length !== t); a = !0);
                         } catch (e) {
-                            c = !0, r = e
+                            u = !0, r = e
                         } finally {
                             try {
                                 if (!a && null != o.return && (l = o.return(), Object(l) !== l)) return
                             } finally {
-                                if (c) throw r
+                                if (u) throw r
                             }
                         }
                         return s
                     }
                 }
 
                 function _arrayWithHoles(e) {
@@ -158,90 +158,122 @@
                         o = (0, react__WEBPACK_IMPORTED_MODULE_0__.useRef)(0),
                         n = e.data,
                         r = e.columns,
                         i = e.rows,
                         l = useResolvedFormatting(e.formatting),
                         s = useResolvedFiltering(e.filtering),
                         a = useResolvedDataSelector(e.data_selector),
-                        c = e.pinned_top,
-                        u = e.pinned_bottom,
+                        u = e.pinned_top,
+                        c = e.pinned_bottom,
                         d = e.pinned_left,
                         p = e.pinned_right,
-                        f = e.filters,
-                        h = e.edited_cells,
-                        _ = e.selected_cells,
-                        m = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        f = e.selected_cells,
+                        h = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 selected_cells: e
                             })
                         }), [t]),
-                        g = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        _ = e.filters,
+                        m = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 filters: e
                             })
                         }), [t]),
+                        g = e.edited_cells,
                         y = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 edited_cells: e
                             })
                         }), [t]),
                         w = e.clicked_cell,
-                        b = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        E = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_cell: _objectSpread(_objectSpread({}, e), {}, {
                                     n: o.current++
                                 })
                             })
                         }), [t]),
-                        E = e.clicked_custom_cell,
-                        v = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        b = e.clicked_custom_cell,
+                        R = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_custom_cell: _objectSpread(_objectSpread({}, e), {}, {
                                     n: o.current++
                                 })
                             })
                         }), [t]),
-                        x = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        v = e.column_widths,
+                        C = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                column_widths: e
+                            })
+                        }), [t]),
+                        x = e.row_heights,
+                        A = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                row_heights: e
+                            })
+                        }), [t]),
+                        k = e.columns_order,
+                        I = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                columns_order: e
+                            })
+                        }), [t]),
+                        D = e.rows_order,
+                        O = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                rows_order: e
+                            })
+                        }), [t]),
+                        M = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 active_columns: e
                             })
                         }), [t]),
-                        R = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        T = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 active_rows: e
                             })
                         }), [t]),
-                        A = _slicedToArray((0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(null), 2),
-                        C = A[0],
-                        k = A[1];
-                    return C && (0, js_spread_grid__WEBPACK_IMPORTED_MODULE_2__.Z)(C, {
+                        P = _slicedToArray((0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(null), 2),
+                        L = P[0],
+                        B = P[1];
+                    return L && (0, js_spread_grid__WEBPACK_IMPORTED_MODULE_2__.Z)(L, {
                         data: n,
                         columns: r,
                         rows: i,
                         formatting: l,
                         filtering: s,
-                        pinnedTop: c,
-                        pinnedBottom: u,
+                        pinnedTop: u,
+                        pinnedBottom: c,
                         pinnedLeft: d,
                         pinnedRight: p,
-                        filters: f,
                         dataSelector: a,
-                        editedCells: h,
-                        selectedCells: _,
-                        onSelectedCellsChange: m,
+                        selectedCells: f,
+                        onSelectedCellsChange: h,
+                        editedCells: g,
                         onEditedCellsChange: y,
-                        onFiltersChange: g,
+                        filters: _,
+                        onFiltersChange: m,
+                        columnWidths: v,
+                        onColumnWidthsChange: C,
+                        rowHeights: x,
+                        onRowHeightsChange: A,
+                        columnsOrder: k,
+                        onColumnsOrderChange: I,
+                        rowsOrder: D,
+                        onRowsOrderChange: O,
                         clickedCell: w,
-                        onCellClick: b,
-                        clickedCustomCell: E,
-                        onCustomCellClick: v,
-                        onActiveColumnsChange: x,
-                        onActiveRowsChange: R
+                        onCellClick: E,
+                        clickedCustomCell: b,
+                        onCustomCellClick: R,
+                        onActiveColumnsChange: M,
+                        onActiveRowsChange: T
                     }), react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
-                        ref: k
+                        ref: B
                     })
                 }
                 DashSpreadGrid.propTypes = {
                     setProps: prop_types__WEBPACK_IMPORTED_MODULE_1___default().func,
                     id: prop_types__WEBPACK_IMPORTED_MODULE_1___default().string,
                     data: prop_types__WEBPACK_IMPORTED_MODULE_1___default().any,
                     columns: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
@@ -257,16 +289,18 @@
                     borderWidth: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     focusedCell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     selected_cells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     highlightedCells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     edited_cells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     filters: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     sort_by: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
-                    columnWidths: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
-                    rowHeights: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    column_widths: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    row_heights: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    columns_order: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    rows_order: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     clicked_cell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     clicked_custom_cell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     active_columns: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     active_rows: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array
                 }, DashSpreadGrid.defaultProps = {
                     data: [],
                     columns: [{
@@ -288,30 +322,32 @@
                     borderWidth: 1,
                     focusedCell: null,
                     selected_cells: [],
                     highlightedCells: [],
                     edited_cells: [],
                     filters: [],
                     sort_by: [],
-                    columnWidths: [],
-                    rowHeights: [],
+                    column_widths: [],
+                    row_heights: [],
+                    columns_order: [],
+                    rows_order: [],
                     clicked_cell: null,
                     clicked_custom_cell: null,
                     active_columns: [],
                     active_rows: []
                 };
                 const __WEBPACK_DEFAULT_EXPORT__ = DashSpreadGrid
             },
             64: e => {
                 e.exports = window.PropTypes
             },
             196: e => {
                 e.exports = window.React
             },
-            906: (e, t, o) => {
+            317: (e, t, o) => {
                 function n(e) {
                     return null === e ? "null" : Array.isArray(e) ? `[${e.map(n).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${n(t[e])}`)).join(",")}}`) : JSON.stringify(e);
                     var t
                 }
 
                 function r(e, t) {
                     return "FILTER" === e.type ^ "FILTER" === t.type ? "FILTER" : "DATA"
@@ -320,146 +356,146 @@
                 function i(e, t, o, i) {
                     return e.map((e => {
                         const l = n(e.columnId),
                             s = n(e.rowId);
                         if (!o.has(l)) return null;
                         if (!i.has(s)) return null;
                         const a = o.get(l),
-                            c = i.get(s);
+                            u = i.get(s);
                         return {
-                            edit: t.resolve(c, a).edit,
+                            edit: t.resolve(u, a).edit,
                             cell: e,
-                            type: r(a, c)
+                            type: r(a, u)
                         }
                     })).filter((e => e?.edit))
                 }
 
                 function l(e, t) {
                     return Math.round(e * t) / t
                 }
 
                 function s(e, t, o) {
                     const n = e.state,
                         r = e.canvases[`${t}-${o}`],
                         i = n.sections[t],
                         s = n.sections[o],
                         a = s.columns,
-                        c = i.rows;
-                    if (0 === c.length || 0 === a.length) return void(r.parentElement && r.parentElement.removeChild(r));
+                        u = i.rows;
+                    if (0 === u.length || 0 === a.length) return void(r.parentElement && r.parentElement.removeChild(r));
                     r.parentElement || e.element.appendChild(r);
-                    const u = r.getContext("2d", {
+                    const c = r.getContext("2d", {
                             alpha: !1
                         }),
                         d = n.scrollRect,
                         p = n.textResolver,
                         f = n.renderFormatResolver,
                         h = n.borderWidth,
                         _ = i.showTopBorder,
                         m = i.showBottomBorder,
                         g = s.showLeftBorder,
                         y = s.showRightBorder,
                         w = h / 2,
-                        b = c.length - 1 + (_ ? 1 : 0) + (m ? 1 : 0),
-                        E = a.length - 1 + (g ? 1 : 0) + (y ? 1 : 0),
-                        v = c.map((e => e.height)),
-                        x = a.map((e => e.width)),
-                        R = x.reduce(((e, t) => e + t), 0) + E * h,
-                        A = v.reduce(((e, t) => e + t), 0) + b * h,
-                        C = "center" === o ? d.left : 0,
+                        E = u.length - 1 + (_ ? 1 : 0) + (m ? 1 : 0),
+                        b = a.length - 1 + (g ? 1 : 0) + (y ? 1 : 0),
+                        R = u.map((e => e.height)),
+                        v = a.map((e => e.width)),
+                        C = v.reduce(((e, t) => e + t), 0) + b * h,
+                        x = R.reduce(((e, t) => e + t), 0) + E * h,
+                        A = "center" === o ? d.left : 0,
                         k = "middle" === t ? d.top : 0,
                         I = "center" === o ? d.width : s.width,
                         D = "middle" === t ? d.height : i.height,
-                        T = x.reduce(((e, t, o) => {
+                        O = v.reduce(((e, t, o) => {
                             const n = e[o] + t + h;
                             return e.push(n), e
                         }), [g ? h : 0]),
-                        M = v.reduce(((e, t, o) => {
+                        M = R.reduce(((e, t, o) => {
                             const n = e[o] + t + h;
                             return e.push(n), e
                         }), [_ ? h : 0]),
-                        O = T.slice(0, -1),
+                        T = O.slice(0, -1),
                         P = M.slice(0, -1),
-                        L = Math.max(O.findLastIndex((e => e <= C)), 0),
-                        B = O.findLastIndex((e => e <= C + I)),
+                        L = Math.max(T.findLastIndex((e => e <= A)), 0),
+                        B = T.findLastIndex((e => e <= A + I)),
                         S = Math.max(P.findLastIndex((e => e <= k)), 0),
                         K = P.findLastIndex((e => e <= k + D)),
                         W = Math.max(L, g ? 0 : 1),
                         F = B + (y ? 1 : 0),
                         z = Math.max(S, _ ? 0 : 1),
                         U = K + (m ? 1 : 0),
                         N = Array.from({
                             length: K - S + 1
                         }, ((e, t) => {
-                            const o = c[t + S];
+                            const o = u[t + S];
                             return Array.from({
                                 length: B - L + 1
                             }, ((e, t) => {
                                 const n = a[t + L];
                                 return f.resolve(o, n)
                             }))
                         })),
                         H = (e, t) => N[e - S][t - L];
-                    r.width = Math.round(I * devicePixelRatio), r.height = Math.round(D * devicePixelRatio), r.style.width = `${I}px`, r.style.height = `${D}px`, r.style.marginLeft = `${C}px`, r.style.marginTop = `${k}px`, r.style.marginRight = R - I - C + "px", r.style.marginBottom = A - D - k + "px", u.fillStyle = "#E9E9E9", u.fillRect(0, 0, r.width, r.height);
+                    r.width = Math.round(I * devicePixelRatio), r.height = Math.round(D * devicePixelRatio), r.style.width = `${I}px`, r.style.height = `${D}px`, r.style.marginLeft = `${A}px`, r.style.marginTop = `${k}px`, r.style.marginRight = C - I - A + "px", r.style.marginBottom = x - D - k + "px", c.fillStyle = "#E9E9E9", c.fillRect(0, 0, r.width, r.height);
                     const j = (e, t) => {
-                            u.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - C) * devicePixelRatio, (t - k) * devicePixelRatio)
+                            c.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - A) * devicePixelRatio, (t - k) * devicePixelRatio)
                         },
                         q = (e, t, o, n) => {
-                            u.beginPath(), u.rect(e, t, o, n), u.clip()
+                            c.beginPath(), c.rect(e, t, o, n), c.clip()
                         };
                     for (let e = L; e <= B; e++) {
-                        u.save(), j(T[e], 0), q(0, 0, x[e], A);
+                        c.save(), j(O[e], 0), q(0, 0, v[e], x);
                         for (let t = S; t <= K; t++) {
                             const o = H(t, e),
                                 n = o.style,
                                 r = M[t],
-                                i = T[e],
-                                s = x[e],
-                                a = v[t],
-                                c = o.text,
+                                i = O[e],
+                                s = v[e],
+                                a = R[t],
+                                u = o.text,
                                 d = n.textBaseline || "middle",
                                 f = o.padding;
-                            if (j(i, r), u.fillStyle = n.background || "white", u.fillRect(0, 0, s, a), "draw" in o && o.draw(u), n.highlight && (u.fillStyle = n.highlight, u.fillRect(0, 0, s, a)), n.corner && (u.fillStyle = n.corner, u.beginPath(), u.moveTo(s - 7, a), u.lineTo(s, a), u.lineTo(s, a - 7), u.fill()), c) {
-                                u.fillStyle = n.foreground || "black", u.font = o.font;
+                            if (j(i, r), c.fillStyle = n.background || "white", c.fillRect(0, 0, s, a), "draw" in o && o.draw(c), n.highlight && (c.fillStyle = n.highlight, c.fillRect(0, 0, s, a)), n.corner && (c.fillStyle = n.corner, c.beginPath(), c.moveTo(s - 7, a), c.lineTo(s, a), c.lineTo(s, a - 7), c.fill()), u) {
+                                c.fillStyle = n.foreground || "black", c.font = o.font;
                                 const e = p.getFontMetrics(o.font),
-                                    t = "center" == n.textAlign && p.measureWidth(c, o.font) > s - f.left - f.right ? "left" : n.textAlign || "left";
-                                u.textAlign = t;
+                                    t = "center" == n.textAlign && p.measureWidth(u, o.font) > s - f.left - f.right ? "left" : n.textAlign || "left";
+                                c.textAlign = t;
                                 const r = l("left" === t ? f.left : "center" === t ? s / 2 : "right" === t ? s - f.right : 0, devicePixelRatio),
                                     i = l("top" === d ? e.middle + e.topOffset + f.top : "middle" === d ? a / 2 + e.middle : "bottom" === d ? a + e.middle - e.bottomOffset - f.bottom : 0, devicePixelRatio);
-                                i - e.middle - e.topOffset >= 0 && i - e.middle + e.bottomOffset <= a ? u.fillText(c, r, i) : (u.strokeStyle = "#E9E9E9", u.lineWidth = h, u.beginPath(), u.moveTo(0, h + w), u.lineTo(s, h + w), u.moveTo(0, a - h - w), u.lineTo(s, a - h - w), u.stroke(), u.save(), q(0, 2 * h, s, a - 4 * h), u.fillText(c, r, i), u.restore())
+                                i - e.middle - e.topOffset >= 0 && i - e.middle + e.bottomOffset <= a ? c.fillText(u, r, i) : (c.strokeStyle = "#E9E9E9", c.lineWidth = h, c.beginPath(), c.moveTo(0, h + w), c.lineTo(s, h + w), c.moveTo(0, a - h - w), c.lineTo(s, a - h - w), c.stroke(), c.save(), q(0, 2 * h, s, a - 4 * h), c.fillText(u, r, i), c.restore())
                             }
                         }
-                        u.restore()
+                        c.restore()
                     }
                     j(0, 0);
                     const $ = (e, t, o, n, r) => {
                             if (!r) return;
                             if (0 === r.width) return;
                             const i = r.width / devicePixelRatio,
                                 l = t === n,
                                 s = e - (l ? i / 2 : 0),
                                 a = t - (l ? 0 : i / 2),
-                                c = o + (l ? i / 2 : 0),
+                                u = o + (l ? i / 2 : 0),
                                 d = n + (l ? 0 : i / 2);
-                            u.strokeStyle = r.color || "black", u.lineWidth = i, r.dash ? (u.setLineDash(r.dash.map((e => e / devicePixelRatio))), u.lineDashOffset = l ? s : a) : u.setLineDash([]), u.beginPath(), u.moveTo(s, a), u.lineTo(c, d), u.stroke()
+                            c.strokeStyle = r.color || "black", c.lineWidth = i, r.dash ? (c.setLineDash(r.dash.map((e => e / devicePixelRatio))), c.lineDashOffset = l ? s : a) : c.setLineDash([]), c.beginPath(), c.moveTo(s, a), c.lineTo(u, d), c.stroke()
                         },
                         V = (e, t) => e ? t ? e.index > t.index ? e : t : e : t;
                     for (let e = z; e <= U; e++) {
                         const t = e - 1,
                             o = e;
                         for (let e = L; e <= B; e++) {
                             const n = V(t >= S ? H(t, e).style.borderBottom : null, o <= K ? H(o, e).style.borderTop : null);
-                            $(T[e] - w, M[o] - w, T[e + 1] - w, M[o] - w, n)
+                            $(O[e] - w, M[o] - w, O[e + 1] - w, M[o] - w, n)
                         }
                     }
                     for (let e = W; e <= F; e++) {
                         const t = e - 1,
                             o = e;
                         for (let e = S; e <= K; e++) {
                             const n = V(t >= L ? H(e, t).style.borderRight : null, o <= B ? H(e, o).style.borderLeft : null);
-                            $(T[o] - w, M[e] - w, T[o] - w, M[e + 1] - w, n)
+                            $(O[o] - w, M[e] - w, O[o] - w, M[e + 1] - w, n)
                         }
                     }
                 }
 
                 function a(e) {
                     if (!e.error) try {
                         ! function(e) {
@@ -485,15 +521,15 @@
                                             preventScroll: !0
                                         })
                                     }
                                 }(e),
                                 function(e) {
                                     const t = e.element,
                                         o = e.state;
-                                    o.resizableColumn && o.resizableRow ? t.style.cursor = "nwse-resize" : o.resizableColumn ? t.style.cursor = "col-resize" : o.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
+                                    e.isReordering ? t.style.cursor = "move" : o.resizableColumn && o.resizableRow ? t.style.cursor = "nwse-resize" : o.resizableColumn ? t.style.cursor = "col-resize" : o.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
                                 }(e),
                                 function(e) {
                                     const t = e.element,
                                         o = e.tooltip,
                                         n = e.state.tooltip,
                                         r = e.state.tooltipPlacement;
                                     r ? (o.innerHTML = n, o.style.left = `${r.left}px`, o.style.top = `${r.top}px`, o.parentElement || (t.appendChild(o), o.showPopover())) : o.parentElement && o.parentElement.removeChild(o)
@@ -507,17 +543,17 @@
                         e.errorRendered = !0;
                         const t = e.element,
                             o = e.error;
                         t.style.backgroundColor = "#9f0000", t.style.color = "white", t.style.padding = "20px", t.style.display = "flex", t.style.flexDirection = "column", t.style.userSelect = "text", t.innerHTML = `\n        <div style="font-size: 16px;">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style="font-size: 20px; font-weight: bold; padding: 20px 0;">\n            ${o.message}\n        </div>\n        <div style="font-size: 16px; white-space: pre-wrap;">${o.stack}</div>\n    `
                     }(e)
                 }
                 o.d(t, {
-                    Z: () => Ye
+                    Z: () => Je
                 });
-                const c = {
+                const u = {
                     value: ({
                         newValue: e
                     }) => e || "",
                     text: ({
                         newValue: e
                     }) => e || "Search...",
                     edit: {
@@ -525,15 +561,15 @@
                         parse: ({
                             string: e
                         }) => e,
                         autoCommit: !0
                     }
                 };
 
-                function u(e, t, o) {
+                function c(e, t, o) {
                     return [{
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "HEADER"
                         },
@@ -569,23 +605,23 @@
                     }, {
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "FILTER"
                         },
-                        ...c
+                        ...u
                     }, {
                         column: {
                             type: "FILTER"
                         },
                         row: {
                             type: "DATA"
                         },
-                        ...c
+                        ...u
                     }, {
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "DATA"
                         },
@@ -626,29 +662,29 @@
                     return f(e, ["value", "text", "edit"])
                 }
 
                 function _(e, t) {
                     return t ? e + "99" : e + "33"
                 }
 
-                function m(e, t, o, r, i, l, s, a, c, u) {
-                    const d = o ? n(o.columnId) : null,
-                        p = o ? n(o.rowId) : null,
-                        f = null !== c,
-                        h = null !== a || f,
-                        m = u + 2,
-                        g = u + 4,
-                        y = (e, t, o, n) => {
+                function m(e, t, o, r, i, l, s, a, u, c, d, p, f) {
+                    const h = o ? n(o.columnId) : null,
+                        m = o ? n(o.rowId) : null,
+                        g = null !== u,
+                        y = null !== a || g,
+                        w = c + 2,
+                        E = c + 4,
+                        b = (e, t, o, n) => {
                             if (o < 0 || o >= e.length) return !1;
                             if (n < 0 || n >= t.length) return !1;
                             const i = e[o].key,
                                 l = t[n].key;
                             return r.isKeySelected(i, l)
                         },
-                        w = (e, t) => e ? [t] : [];
+                        R = (e, t) => e ? [t] : [];
                     return [{
                         column: {
                             type: "DATA"
                         },
                         row: {
                             type: "FILTER"
                         },
@@ -685,53 +721,53 @@
                         },
                         row: {
                             type: "HEADER"
                         },
                         style: {
                             background: "#F5F5F5",
                             border: {
-                                width: u,
+                                width: c,
                                 color: "gray"
                             }
                         }
                     }, {
                         column: {
                             type: "HEADER"
                         },
                         row: {
                             type: "ANY"
                         },
                         style: {
                             background: "#F5F5F5",
                             border: {
-                                width: u,
+                                width: c,
                                 color: "gray"
                             }
                         }
                     }, {
                         column: {
                             type: "HEADER"
                         },
                         row: {
                             type: "HEADER"
                         },
                         style: {
                             background: "#E0E0E0"
                         }
-                    }, ...e, ...w(t && !f, {
+                    }, ...e, ...R(t && !g, {
                         column: {
                             type: "ANY"
                         },
                         row: {
                             id: t?.rowId
                         },
                         style: {
                             highlight: "#81948133"
                         }
-                    }), ...w(t && !h, {
+                    }), ...R(t && !y, {
                         column: {
                             id: t?.columnId
                         },
                         row: {
                             id: t?.rowId
                         },
                         style: {
@@ -745,51 +781,51 @@
                             type: "ANY"
                         },
                         condition: ({
                             rows: e,
                             columns: t,
                             row: o,
                             column: n
-                        }) => y(e, t, o.index, n.index),
+                        }) => b(e, t, o.index, n.index),
                         style: ({
                             rows: e,
                             columns: t,
                             row: o,
                             column: n,
                             edit: r
                         }) => ({
-                            ...y(e, t, o.index - 1, n.index) ? {} : {
+                            ...b(e, t, o.index - 1, n.index) ? {} : {
                                 borderTop: {
-                                    width: m,
+                                    width: w,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, o.index + 1, n.index) ? {} : {
+                            ...b(e, t, o.index + 1, n.index) ? {} : {
                                 borderBottom: {
-                                    width: m,
+                                    width: w,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, o.index, n.index - 1) ? {} : {
+                            ...b(e, t, o.index, n.index - 1) ? {} : {
                                 borderLeft: {
-                                    width: m,
+                                    width: w,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...y(e, t, o.index, n.index + 1) ? {} : {
+                            ...b(e, t, o.index, n.index + 1) ? {} : {
                                 borderRight: {
-                                    width: m,
+                                    width: w,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            highlight: _(r ? "#798d9c" : "#819481", d !== n.key || p !== o.key)
+                            highlight: _(r ? "#798d9c" : "#819481", h !== n.key || m !== o.key)
                         })
                     }, {
                         column: {
                             type: "ANY"
                         },
                         row: {
                             type: "ANY"
@@ -798,17 +834,17 @@
                             row: e,
                             column: t
                         }) => i.isKeySelected(e.key, t.key),
                         style: ({
                             row: e,
                             column: t
                         }) => ({
-                            highlight: _("#93a8b8", d !== t.key || p !== e.key)
+                            highlight: _("#93a8b8", h !== t.key || m !== e.key)
                         })
-                    }, ...w(o, {
+                    }, ...R(o, {
                         column: {
                             id: o?.columnId
                         },
                         row: {
                             id: o?.rowId
                         },
                         style: {
@@ -851,110 +887,130 @@
                         condition: ({
                             row: e,
                             column: t
                         }) => l.hasValueByKey(e.key, t.key),
                         style: {
                             corner: "darkgreen"
                         }
-                    }, ...w(a, {
+                    }, ...R(a, {
                         column: {
                             id: a
                         },
                         row: {
                             type: "HEADER"
                         },
                         style: {
                             borderRight: {
-                                width: g,
+                                width: E,
                                 color: "cornflowerblue"
                             }
                         }
-                    }), ...w(c, {
+                    }), ...R(u, {
                         column: {
                             type: "HEADER"
                         },
                         row: {
-                            id: c
+                            id: u
                         },
                         style: {
                             borderBottom: {
-                                width: g,
+                                width: E,
                                 color: "cornflowerblue"
                             }
                         }
+                    }), ...R(d && p, {
+                        column: {
+                            id: p
+                        },
+                        row: {
+                            type: "ANY"
+                        },
+                        style: {
+                            highlight: "#3a74e055"
+                        }
+                    }), ...R(d && f, {
+                        column: {
+                            type: "ANY"
+                        },
+                        row: {
+                            id: f
+                        },
+                        style: {
+                            highlight: "#3a74e055"
+                        }
                     })]
                 }
 
                 function g(e, t) {
                     const o = t.filter((e => "BEGIN" === e.pinned)).length,
                         n = t.filter((e => "END" === e.pinned)).length,
                         r = t.length - o - n,
                         i = e.filter((e => "BEGIN" === e.pinned)).length,
                         l = e.filter((e => "END" === e.pinned)).length,
                         s = e.length - i - l,
                         a = t.slice(0, o),
-                        c = t.slice(t.length - n, t.length),
-                        u = t.slice(o, t.length - n),
+                        u = t.slice(t.length - n, t.length),
+                        c = t.slice(o, t.length - n),
                         d = e.slice(0, i),
                         p = e.slice(e.length - l, e.length),
                         f = e.slice(i, e.length - l),
                         h = o > 0,
                         _ = i > 0,
                         m = r > 0 || !h,
                         g = !h,
                         y = !(n > 0),
                         w = s > 0 || !_,
-                        b = !_,
-                        E = !(l > 0),
-                        v = (e, t, o) => {
+                        E = !_,
+                        b = !(l > 0),
+                        R = (e, t, o) => {
                             if (0 === e.length) return 0;
                             const n = t ? e.at(0).topWithBorder : e.at(0).top;
                             return (o ? e.at(-1).bottomWithBorder : e.at(-1).bottom) - n
                         },
-                        x = (e, t, o) => {
+                        v = (e, t, o) => {
                             if (0 === e.length) return 0;
                             const n = t ? e.at(0).leftWithBorder : e.at(0).left;
                             return (o ? e.at(-1).rightWithBorder : e.at(-1).right) - n
                         };
                     return {
                         top: {
                             rows: a,
                             showTopBorder: !0,
                             showBottomBorder: !0,
-                            height: v(a, !0, !0)
+                            height: R(a, !0, !0)
                         },
                         bottom: {
-                            rows: c,
+                            rows: u,
                             showTopBorder: m,
                             showBottomBorder: !0,
-                            height: v(c, m, !0)
+                            height: R(u, m, !0)
                         },
                         middle: {
-                            rows: u,
+                            rows: c,
                             showTopBorder: g,
                             showBottomBorder: y,
-                            height: v(u, g, y)
+                            height: R(c, g, y)
                         },
                         left: {
                             columns: d,
                             showLeftBorder: !0,
                             showRightBorder: !0,
-                            width: x(d, !0, !0)
+                            width: v(d, !0, !0)
                         },
                         right: {
                             columns: p,
                             showLeftBorder: w,
                             showRightBorder: !0,
-                            width: x(p, w, !0)
+                            width: v(p, w, !0)
                         },
                         center: {
                             columns: f,
-                            showLeftBorder: b,
-                            showRightBorder: E,
-                            width: x(f, b, E)
+                            showLeftBorder: E,
+                            showRightBorder: b,
+                            width: v(f, E, b)
                         }
                     }
                 }
 
                 function y(e, t) {
                     return [...e, ...t.map((e => ({
                         columnId: e.columnId,
@@ -980,18 +1036,18 @@
                         return this.hasValueByKey(n(e), n(t))
                     }
                     getValueById(e, t) {
                         return this.getValueByKey(n(e), n(t))
                     }
                 }
 
-                function b(e) {
+                function E(e) {
                     return new w(e)
                 }
-                class E {
+                class b {
                     constructor(e) {
                         this.lookup = new Map, e.forEach((e => {
                             const t = n(e.rowId),
                                 o = n(e.columnId);
                             this.lookup.has(t) || this.lookup.set(t, new Set), this.lookup.get(t).add(o)
                         }))
                     }
@@ -999,59 +1055,58 @@
                         return this.lookup.has(e) && this.lookup.get(e).has(t)
                     }
                     isIdSelected(e, t) {
                         return this.isKeySelected(n(e), n(t))
                     }
                 }
 
-                function v(e) {
-                    return new E(e)
+                function R(e) {
+                    return new b(e)
                 }
 
-                function x(e, t) {
+                function v(e, t) {
                     return "function" == typeof e ? e(t) : e
                 }
 
-                function R(e, t, o, n) {
+                function C(e, t, o, n) {
                     return e < o ? "BEGIN" : e >= t - n ? "END" : void 0
                 }
 
-                function A(e, t, o) {
+                function x(e, t, o) {
                     return e.map(((r, i) => {
                         const l = "id" in r ? r.id : r.type;
                         return {
                             ...r,
                             id: l,
                             type: r.type || "DATA",
-                            index: i,
                             key: n(l),
-                            pinned: R(i, e.length, t, o),
+                            pinned: C(i, e.length, t, o),
                             header: "header" in r ? r.header : l,
                             labels: r.labels || []
                         }
                     }))
                 }
 
-                function C(e, t, o, r) {
+                function A(e, t, o, r) {
                     const i = new Map(r.map((({
                         columnId: e,
                         width: t
                     }) => [n(e), t])));
-                    return A(e, t, o).map((e => ({
+                    return x(e, t, o).map((e => ({
                         ...e,
                         width: i.has(e.key) ? i.get(e.key) : "width" in e ? e.width : "fit"
                     })))
                 }
 
                 function k(e, t, o, r) {
                     const i = new Map(r.map((({
                         rowId: e,
                         height: t
                     }) => [n(e), t])));
-                    return A(e, t, o).map((e => ({
+                    return x(e, t, o).map((e => ({
                         ...e,
                         height: i.has(e.key) ? i.get(e.key) : "height" in e ? e.height : "fit"
                     })))
                 }
 
                 function I(e, t, o) {
                     let n = o;
@@ -1082,22 +1137,22 @@
                                 top: n,
                                 bottom: n + i,
                                 bottomWithBorder: n + i + o
                             };
                         return n += s.height + o, s
                     }))
                 }
-                const T = "12px Calibri",
+                const O = "12px Calibri",
                     M = {
                         top: 2,
                         right: 5,
                         bottom: 2,
                         left: 5
                     },
-                    O = {
+                    T = {
                         HEADER: ["HEADER"],
                         FILTER: ["FILTER"],
                         DATA: ["DATA"],
                         CUSTOM: ["CUSTOM"],
                         ANY: ["HEADER", "DATA", "FILTER", "CUSTOM"],
                         SPECIAL: ["HEADER", "FILTER", "CUSTOM"],
                         undefined: []
@@ -1122,24 +1177,24 @@
                             } : e : {
                                 type: "DATA"
                             }, t = t ? "id" in t ? {
                                 key: n(t.id)
                             } : t : {
                                 type: "DATA"
                             }, "key" in e && i(this.lookup.byKey, e.key), "index" in e && i(this.lookup.byIndex, e.index), "label" in e && i(this.lookup.byLabel, e.label);
-                            for (const t of O[e.type]) i(this.lookup.byType, t)
+                            for (const t of T[e.type]) i(this.lookup.byType, t)
                         }
 
                         function r(e, t) {
                             e.has(t) || e.set(t, []), e.get(t).push(o)
                         }
 
                         function i(e, o) {
                             e.has(o) || e.set(o, new P), "key" in t && r(e.get(o).byKey, t.key), "index" in t && r(e.get(o).byIndex, t.index), "label" in t && r(e.get(o).byLabel, t.label);
-                            for (const n of O[t.type]) r(e.get(o).byType, n)
+                            for (const n of T[t.type]) r(e.get(o).byType, n)
                         }
                     }
                     getRules(e, t) {
                         const o = [];
                         if (!this.hasRules) return o;
 
                         function n(e) {
@@ -1195,61 +1250,61 @@
                                 index: t
                             };
                             "condition" in o && (e.condition = o.condition), "style" in o && (e.style = "function" == typeof o.style ? o.style : () => o.style), "value" in o && (e.value = "function" == typeof o.value ? o.value : () => o.value), "text" in o && (e.text = "function" == typeof o.text ? o.text : () => o.text), "font" in o && (e.font = "function" == typeof o.font ? o.font : () => o.font), "padding" in o && (e.padding = "function" == typeof o.padding ? o.padding : () => o.padding), "edit" in o && (e.edit = o.edit), "tooltip" in o && (e.tooltip = "function" == typeof o.tooltip ? o.tooltip : () => o.tooltip), "draw" in o && (e.draw = o.draw), this.rulesLookup.addRule(o.column, o.row, e)
                         }
                     }
                     resolve(e, t, o, n, r, i) {
                         const l = this.rulesLookup.getRules(r, n).sort(((e, t) => e.index - t.index)).filter(((e, t, o) => e.index !== o[t - 1]?.index));
-                        let s, a, c = {
+                        let s, a, u = {
                                 data: e,
                                 rows: t,
                                 columns: o,
                                 row: n,
                                 column: r
                             },
-                            u = {},
+                            c = {},
                             d = M,
-                            p = T;
-                        i.hasValueByKey(n.key, r.key) && (c = {
-                            ...c,
+                            p = O;
+                        i.hasValueByKey(n.key, r.key) && (u = {
+                            ...u,
                             newValue: i.getValueByKey(n.key, r.key)
                         });
                         for (const e of l)
-                            if ((!("condition" in e) || e.condition(c)) && ("value" in e && (c = {
-                                    ...c,
-                                    value: e.value(c)
-                                }), "style" in e && (u = {
+                            if ((!("condition" in e) || e.condition(u)) && ("value" in e && (u = {
                                     ...u,
-                                    ...K(e.style(c), e.index)
-                                }), "text" in e && (c = {
+                                    value: e.value(u)
+                                }), "style" in e && (c = {
                                     ...c,
-                                    text: e.text(c)
-                                }), "font" in e && (p = e.font(c)), "padding" in e && (d = {
+                                    ...K(e.style(u), e.index)
+                                }), "text" in e && (u = {
+                                    ...u,
+                                    text: e.text(u)
+                                }), "font" in e && (p = e.font(u)), "padding" in e && (d = {
                                     ...d,
-                                    ...e.padding(c)
-                                }), "edit" in e && (c = {
-                                    ...c,
-                                    edit: W(e, c)
-                                }), "tooltip" in e && (a = e.tooltip(c)), "draw" in e)) {
-                                const t = c;
+                                    ...e.padding(u)
+                                }), "edit" in e && (u = {
+                                    ...u,
+                                    edit: W(e, u)
+                                }), "tooltip" in e && (a = e.tooltip(u)), "draw" in e)) {
+                                const t = u;
                                 s = o => e.draw({
                                     ...t,
                                     ctx: o
                                 })
                             } const f = function(e) {
                                 return "text" in e ? `${e.text}` : "newValue" in e ? `${e.newValue}` : void 0 !== e.value ? `${e.value}` : ""
-                            }(c),
+                            }(u),
                             h = {
-                                style: u,
+                                style: c,
                                 visible: !0,
                                 text: f,
                                 padding: d,
                                 font: p
                             };
-                        return "value" in c && (h.value = c.value), "edit" in c && void 0 !== c.edit && (h.edit = c.edit), void 0 !== a && (h.tooltip = a), void 0 !== s && (h.draw = s), h
+                        return "value" in u && (h.value = u.value), "edit" in u && void 0 !== u.edit && (h.edit = u.edit), void 0 !== a && (h.tooltip = a), void 0 !== s && (h.draw = s), h
                     }
                 }
 
                 function z(e) {
                     return new F(e)
                 }
                 class U {
@@ -1276,32 +1331,32 @@
                 }
 
                 function j(e, t, o, n, r, i, l) {
                     if (0 === e.length) return r;
                     const s = H(e, "columnId", "rowId"),
                         a = i.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? r : r.filter((e => {
-                        for (const c of a) {
-                            const a = o.resolve(n, r, i, e, c, l),
-                                u = s.get(c.key);
-                            if (!t.resolve(n, r, i, e, c, a.value, a.text, u)) return !1
+                        for (const u of a) {
+                            const a = o.resolve(n, r, i, e, u, l),
+                                c = s.get(u.key);
+                            if (!t.resolve(n, r, i, e, u, a.value, a.text, c)) return !1
                         }
                         return !0
                     }))
                 }
 
                 function q(e, t, o, n, r, i, l) {
                     if (0 === e.length) return i;
                     const s = H(e, "rowId", "columnId"),
                         a = r.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? i : i.filter((e => {
-                        for (const c of a) {
-                            const a = o.resolve(n, r, i, c, e, l),
-                                u = s.get(c.key);
-                            if (!t.resolve(n, r, i, c, e, a.value, a.text, u)) return !1
+                        for (const u of a) {
+                            const a = o.resolve(n, r, i, u, e, l),
+                                c = s.get(u.key);
+                            if (!t.resolve(n, r, i, u, e, a.value, a.text, c)) return !1
                         }
                         return !0
                     }))
                 }
 
                 function $(e, t, o, n) {
                     return {
@@ -1321,26 +1376,26 @@
                 class G {
                     constructor() {
                         this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.fontMetrics = new Map
                     }
                     measureWidth(e, t) {
                         if (!e) return 0;
                         const o = this.context;
-                        return o.font = t || T, o.measureText(e).width
+                        return o.font = t || O, o.measureText(e).width
                     }
                     measureHeight(e, t) {
                         let o = 1;
                         for (const t of e) "\n" === t && o++;
                         return o * this.getFontMetrics(t).height
                     }
                     getFontMetrics(e) {
                         const t = e;
                         if (this.fontMetrics.has(t)) return this.fontMetrics.get(t);
                         const o = this.context;
-                        o.font = e || T;
+                        o.font = e || O;
                         const n = o.measureText("X"),
                             r = (n.actualBoundingBoxDescent - n.actualBoundingBoxAscent) / 2,
                             i = {
                                 topOffset: r + n.fontBoundingBoxAscent,
                                 middle: -r,
                                 bottomOffset: n.fontBoundingBoxDescent - r,
                                 height: n.fontBoundingBoxAscent + n.fontBoundingBoxDescent
@@ -1404,42 +1459,42 @@
 
                 function re(e, t, o, n) {
                     const r = t.x,
                         i = t.y,
                         l = e.scrollLeft,
                         s = e.scrollTop,
                         a = e.clientWidth,
-                        c = e.clientHeight;
+                        u = e.clientHeight;
                     return {
                         x: r <= o.left ? r : r >= a ? r + l : r >= a - o.right ? n.width - a + r : r + l,
-                        y: i <= o.top ? i : i >= c ? i + s : i >= c - o.bottom ? n.height - c + i : i + s
+                        y: i <= o.top ? i : i >= u ? i + s : i >= u - o.bottom ? n.height - u + i : i + s
                     }
                 }
 
                 function ie(e) {
                     return e.reduce(((e, t) => e.set(t.key, t)), new Map)
                 }
 
                 function le(e, t, o, r, i, l, s, a) {
                     if (!e) return [];
-                    if (t) return [];
+                    if (!t) return [];
                     if (!r) return [];
                     if (!o) return [];
-                    const c = n(o.columnId),
-                        u = n(o.rowId),
+                    const u = n(o.columnId),
+                        c = n(o.rowId),
                         d = n(r.columnId),
                         p = n(r.rowId);
-                    if (!s.has(c)) return [];
-                    if (!a.has(u)) return [];
+                    if (!s.has(u)) return [];
+                    if (!a.has(c)) return [];
                     if (!s.has(d)) return [];
                     if (!a.has(p)) return [];
-                    const f = Math.min(s.get(c).index, s.get(d).index),
-                        h = Math.max(s.get(c).index, s.get(d).index),
-                        _ = Math.min(a.get(u).index, a.get(p).index),
-                        m = Math.max(a.get(u).index, a.get(p).index);
+                    const f = Math.min(s.get(u).index, s.get(d).index),
+                        h = Math.max(s.get(u).index, s.get(d).index),
+                        _ = Math.min(a.get(c).index, a.get(p).index),
+                        m = Math.max(a.get(c).index, a.get(p).index);
                     return i.slice(f, h + 1).flatMap((e => l.slice(_, m + 1).map((t => ({
                         rowId: t.id,
                         columnId: e.id
                     })))))
                 }
 
                 function se(e, t) {
@@ -1456,47 +1511,47 @@
                     if (!e) return null;
                     const i = n(e.columnId),
                         l = n(e.rowId);
                     if (!t.has(i)) return null;
                     if (!o.has(l)) return null;
                     const s = t.get(i),
                         a = o.get(l),
-                        c = {
+                        u = {
                             width: s.width,
                             height: a.height,
                             section: se(s, a)
                         };
                     switch (a.pinned) {
                         case "BEGIN":
-                            c.top = a.top;
+                            u.top = a.top;
                             break;
                         case "END":
-                            c.bottom = r.top.height + r.middle.height + r.bottom.height - a.top - a.height;
+                            u.bottom = r.top.height + r.middle.height + r.bottom.height - a.top - a.height;
                             break;
                         default:
-                            c.marginTop = a.top - r.top.height
+                            u.marginTop = a.top - r.top.height
                     }
                     switch (s.pinned) {
                         case "BEGIN":
-                            c.left = s.left;
+                            u.left = s.left;
                             break;
                         case "END":
-                            c.right = r.left.width + r.center.width + r.right.width - s.left - s.width;
+                            u.right = r.left.width + r.center.width + r.right.width - s.left - s.width;
                             break;
                         default:
-                            c.marginLeft = s.left - r.left.width
+                            u.marginLeft = s.left - r.left.width
                     }
-                    return c
+                    return u
                 }
 
-                function ce(e, t, o, n, r) {
+                function ue(e, t, o, n, r) {
                     return 0 === e.length ? null : ae(t, o, n, r)
                 }
 
-                function ue(e, t) {
+                function ce(e, t) {
                     return t.every((t => t.edit.validate({
                         string: e
                     })))
                 }
 
                 function de(e) {
                     return Array.isArray(e) ? e.map(((e, t) => t)) : Object.keys(e)
@@ -1563,27 +1618,27 @@
                     }
                     resolve(e, t, o, n, r, i, l, s) {
                         const a = this.rulesLookup.getRules(r, n);
                         if (0 === a.length) return "DATA" !== n.type || "DATA" !== r.type || !s.has('"FILTER"') || me({
                             text: l,
                             expression: s.get('"FILTER"')
                         });
-                        let c = {
+                        let u = {
                             data: e,
                             rows: t,
                             columns: o,
                             row: n,
                             column: r,
                             value: i,
                             text: l
                         };
                         for (const e of a) {
                             if (!s.has(e.by)) continue;
                             const t = {
-                                ...c,
+                                ...u,
                                 expression: s.get(e.by)
                             };
                             if (!e.condition(t)) return !1
                         }
                         return !0
                     }
                 }
@@ -1592,19 +1647,19 @@
                     return new ge(e)
                 }
 
                 function we(e) {
                     return f(e, ["value", "text"])
                 }
 
-                function be(e) {
+                function Ee(e) {
                     return f(e, ["value", "text", "font", "padding"])
                 }
 
-                function Ee(e, t, o, n, r, i) {
+                function be(e, t, o, n, r, i) {
                     if (e.every((e => "number" == typeof e.width))) return e;
                     const l = e => {
                         const i = e.width;
                         if ("number" == typeof i) return i;
                         if (r.has(e.key)) {
                             const t = r.get(e.key);
                             if ("fit-once" === i && !t.dataOnly) return t.width;
@@ -1613,31 +1668,31 @@
                         let l = 0;
                         for (const r of t) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
                             const t = n.resolve(r, e),
                                 s = t.text,
                                 a = t.font,
-                                c = t.padding.left + t.padding.right,
-                                u = o.measureWidth(s, a) + c;
-                            l = Math.max(l, u)
+                                u = t.padding.left + t.padding.right,
+                                c = o.measureWidth(s, a) + u;
+                            l = Math.max(l, c)
                         }
                         return r.set(e.key, {
                             width: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return e.map((e => ({
                         ...e,
                         width: l(e)
                     })))
                 }
 
-                function ve(e, t, o, n, r, i) {
+                function Re(e, t, o, n, r, i) {
                     if (t.every((e => "number" == typeof e.height))) return t;
                     const l = t => {
                         const i = t.height;
                         if ("number" == typeof i) return i;
                         if (r.has(t.key)) {
                             const e = r.get(t.key);
                             if ("fit-once" === i && !e.dataOnly) return e.height;
@@ -1646,62 +1701,62 @@
                         let l = 0;
                         for (const r of e) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
                             const e = n.resolve(t, r),
                                 s = e.text,
                                 a = e.font,
-                                c = e.padding.top + e.padding.bottom,
-                                u = o.measureHeight(s, a) + c;
-                            l = Math.max(l, u)
+                                u = e.padding.top + e.padding.bottom,
+                                c = o.measureHeight(s, a) + u;
+                            l = Math.max(l, c)
                         }
                         return r.set(t.key, {
                             height: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return t.map((e => ({
                         ...e,
                         height: l(e)
                     })))
                 }
 
-                function xe(e) {
+                function ve(e) {
                     return new Set(e.map((e => e.key)))
                 }
 
-                function Re(e) {
+                function Ce(e) {
                     return f(e, ["value", "text"])
                 }
 
-                function Ae(e, t) {
+                function xe(e, t) {
                     return null != e.value && (null == t.value || e.value < t.value)
                 }
 
-                function Ce(e, t) {
+                function Ae(e, t) {
                     return null != e.value && (null == t.value || e.value > t.value)
                 }
                 class ke {
                     constructor(e) {
                         this.rulesLookup = new L;
                         for (const t of e) {
-                            const e = t.comparator ? (e, o) => t.comparator(e, o) : (e, t) => Ae(e, t),
-                                o = t.comparator ? (e, o) => !t.comparator(e, o) : (e, t) => Ce(e, t),
+                            const e = t.comparator ? (e, o) => t.comparator(e, o) : (e, t) => xe(e, t),
+                                o = t.comparator ? (e, o) => !t.comparator(e, o) : (e, t) => Ae(e, t),
                                 r = {
                                     by: n("by" in t ? t.by : "HEADER"),
                                     comparatorAsc: e,
                                     comparatorDesc: o
                                 };
                             this.rulesLookup.addRule(t.column, t.row, r)
                         }
                     }
                     resolve(e, t, o) {
                         const n = this.rulesLookup.getRules(e, t);
-                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? Ae : Ce : null;
+                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? xe : Ae : null;
                         if (n.length > 1) throw new Error("Multiple sorting rules for the same cell");
                         const r = n[0];
                         return o.has(r.by) ? "ASC" === o.get(r.by) ? r.comparatorAsc : r.comparatorDesc : null
                     }
                 }
 
                 function Ie(e) {
@@ -1714,95 +1769,97 @@
                         const e = n(i[t]),
                             l = n(i[o]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.direction)
                     }
                     return r
                 }
 
-                function Te(e, t) {
+                function Oe(e, t) {
                     e.sort(((e, t) => {
                         const o = e.comparator(e.cell, t.cell);
                         return "number" == typeof o ? o : o ? -1 : 1
                     })), t.push(...e.map((e => e.entity))), e.length = 0
                 }
 
                 function Me(e, t, o, r, i, l, s) {
                     if (0 === e.length) return i;
                     const a = De(e, "columnId", "rowId"),
-                        c = new Map(l.map((e => [e.key, e]))),
-                        u = e.map((e => n(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
-                    if (0 === u.length) return i;
-                    for (const e of u) {
+                        u = new Map(l.map((e => [e.key, e]))),
+                        c = e.map((e => n(e.columnId))).filter((e => u.has(e))).map((e => u.get(e))).reverse();
+                    if (0 === c.length) return i;
+                    for (const e of c) {
                         const n = [],
-                            c = [];
-                        for (const u of i) {
-                            const d = t.resolve(e, u, a.get(e.key));
+                            u = [];
+                        for (const c of i) {
+                            const d = t.resolve(e, c, a.get(e.key));
                             if (!d) {
-                                Te(c, n), n.push(u);
+                                Oe(u, n), n.push(c);
                                 continue
                             }
                             const p = {
-                                entity: u,
+                                entity: c,
                                 comparator: d,
-                                cell: o.resolve(r, i, l, u, e, s)
+                                cell: o.resolve(r, i, l, c, e, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (Te(c, n), c.push(p)) : c.push(p)
+                            0 !== u.length && u[0].comparator !== d ? (Oe(u, n), u.push(p)) : u.push(p)
                         }
-                        Te(c, n), i = n
+                        Oe(u, n), i = n
                     }
                     return i
                 }
 
-                function Oe(e, t, o, r, i, l, s) {
+                function Te(e, t, o, r, i, l, s) {
                     if (0 === e.length) return l;
                     const a = De(e, "rowId", "columnId"),
-                        c = new Map(i.map((e => [e.key, e]))),
-                        u = e.map((e => n(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
-                    if (0 === u.length) return l;
-                    for (const e of u) {
+                        u = new Map(i.map((e => [e.key, e]))),
+                        c = e.map((e => n(e.rowId))).filter((e => u.has(e))).map((e => u.get(e))).reverse();
+                    if (0 === c.length) return l;
+                    for (const e of c) {
                         const n = [],
-                            c = [];
-                        for (const u of l) {
-                            const d = t.resolve(u, e, a.get(e.key));
+                            u = [];
+                        for (const c of l) {
+                            const d = t.resolve(c, e, a.get(e.key));
                             if (!d) {
-                                Te(c, n), n.push(u);
+                                Oe(u, n), n.push(c);
                                 continue
                             }
                             const p = {
-                                entity: u,
+                                entity: c,
                                 comparator: d,
-                                cell: o.resolve(r, i, l, e, u, s)
+                                cell: o.resolve(r, i, l, e, c, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (Te(c, n), c.push(p)) : c.push(p)
+                            0 !== u.length && u[0].comparator !== d ? (Oe(u, n), u.push(p)) : u.push(p)
                         }
-                        Te(c, n), l = n
+                        Oe(u, n), l = n
                     }
                     return l
                 }
                 const Pe = 5;
 
-                function Le(e, t, o, r, i, l, s, a) {
+                function Le(e, t, o, r, i, l, s, a, u) {
                     if (!r) return null;
+                    if (s) return null;
                     const c = t.get(n(r.columnId));
                     if ("HEADER" !== o.get(n(r.rowId)).type) return null;
-                    const u = re(i, l, s, a);
-                    if (!u) return null;
-                    const d = u.x;
-                    return d >= c.right - Pe && d <= c.right + Pe ? c.id : 0 === c.index || d < c.left - Pe || d > c.left + Pe ? null : e[c.index - 1].id
+                    const d = re(i, l, a, u);
+                    if (!d) return null;
+                    const p = d.x;
+                    return p >= c.right - Pe && p <= c.right + Pe ? c.id : 0 === c.index || p < c.left - Pe || p > c.left + Pe ? null : e[c.index - 1].id
                 }
 
-                function Be(e, t, o, r, i, l, s, a) {
+                function Be(e, t, o, r, i, l, s, a, u) {
                     if (!r) return null;
+                    if (s) return null;
                     const c = t.get(n(r.columnId)),
-                        u = o.get(n(r.rowId));
+                        d = o.get(n(r.rowId));
                     if ("HEADER" !== c.type) return null;
-                    const d = re(i, l, s, a);
-                    if (!d) return null;
-                    const p = d.y;
-                    return p >= u.bottom - Pe && p <= u.bottom + Pe ? u.id : 0 === u.index || p < u.top - Pe || p > u.top + Pe ? null : e[u.index - 1].id
+                    const p = re(i, l, a, u);
+                    if (!p) return null;
+                    const f = p.y;
+                    return f >= d.bottom - Pe && f <= d.bottom + Pe ? d.id : 0 === d.index || f < d.top - Pe || f > d.top + Pe ? null : e[d.index - 1].id
                 }
 
                 function Se(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "HEADER",
                         rowId: "rowId" in e ? e.rowId : "HEADER",
                         direction: e.direction
@@ -1845,14 +1902,28 @@
                     return i ? {
                         top: i.top,
                         left: i.left
                     } : null
                 }
 
                 function Ne(e) {
+                    return e.map((e => n(e)))
+                }
+
+                function He(e, t) {
+                    if (!t) return e;
+                    const o = new Map;
+                    for (const t of e) o.set(t.key, t);
+                    const n = [];
+                    for (const e of t) o.has(e) && (n.push(o.get(e)), o.delete(e));
+                    for (const t of e) o.has(t.key) && n.push(o.get(t.key));
+                    return [...n.filter((e => "BEGIN" === e.pinned)), ...n.filter((e => !e.pinned)), ...n.filter((e => "END" === e.pinned))]
+                }
+
+                function je(e) {
                     const t = {
                             ...e.localOptions,
                             ...e.externalOptions
                         },
                         o = e.memory,
                         n = e.state,
                         r = e.element;
@@ -1862,57 +1933,61 @@
                         return r && !n.some(((e, t) => e !== r[t])) || (o[e] = {
                             value: t(...n),
                             dependencies: n
                         }), o[e].value
                     }
                     const s = window.devicePixelRatio,
                         a = t.borderWidth / s,
-                        c = t.data,
+                        u = t.data,
                         d = e.input.value,
                         p = l("sortBy", Se, [t.sortBy]),
                         f = l("filters", Ke, [t.filters]),
                         _ = l("textResolver", Y, []),
-                        w = l("dataFormatting", u, [t.formatting, t.dataSelector, p]),
-                        E = l("editedCellsAndFilters", y, [t.editedCells, f]),
-                        R = l("edition", b, [E]),
-                        A = l("invokedColumns", x, [t.columns, c]),
-                        T = l("invokedRows", x, [t.rows, c]),
-                        M = l("unfoldedColumns", he, [A, c]),
-                        O = l("unfoldedRows", _e, [T, c]),
-                        P = l("unfilteredColumns", C, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
-                        L = l("unfilteredRows", k, [O, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
-                        B = l("unfilteredColumnKeys", xe, [P]),
-                        S = l("unfilteredRowKeys", xe, [L]),
-                        K = l("filterFormatting", we, [w]),
-                        W = l("filterFormattingRules", z, [K]),
-                        F = l("filteringRules", ye, [t.filtering]),
-                        U = l("filteredColumns", q, [f, F, W, c, L, P, R]),
-                        H = l("filteredRows", j, [f, F, W, c, L, P, R]),
-                        G = l("sortingFormatting", Re, [w]),
-                        se = l("sortingFormattingRules", z, [G]),
-                        ae = l("sortingRules", Ie, [t.sorting]),
-                        de = l("sortedColumns", Oe, [p, ae, se, c, H, U, R]),
-                        pe = l("sortedRows", Me, [p, ae, se, c, H, U, R]),
-                        fe = l("measureFormatting", be, [w]),
-                        me = l("measureFormattingRules", z, [fe]),
-                        ge = l("measureFormatResolver", N, [me, c, pe, de, R]),
-                        Ae = e.columnWidthCache,
-                        Ce = e.rowHeightCache,
-                        ke = l("measuredColumns", Ee, [de, pe, _, ge, Ae, B]),
-                        De = l("measuredRows", ve, [de, pe, _, ge, Ce, S]),
-                        Te = l("columns", I, [ke, s, a]),
-                        Pe = l("rows", D, [De, s, a]),
-                        Ne = l("columnLookup", ie, [Te]),
-                        He = l("rowLookup", ie, [Pe]),
-                        je = t.focusedCell,
-                        qe = l("sections", g, [Te, Pe]),
-                        $e = t.selectedCells,
-                        Ve = l("fixedSize", $, [qe.top.height, qe.bottom.height, qe.left.width, qe.right.width]),
-                        Ge = l("totalSize", V, [Te, Pe]),
-                        Ye = function(e, t, o, n, r, i) {
+                        w = l("dataFormatting", c, [t.formatting, t.dataSelector, p]),
+                        b = l("editedCellsAndFilters", y, [t.editedCells, f]),
+                        C = l("edition", E, [b]),
+                        x = l("invokedColumns", v, [t.columns, u]),
+                        O = l("invokedRows", v, [t.rows, u]),
+                        M = l("unfoldedColumns", he, [x, u]),
+                        T = l("unfoldedRows", _e, [O, u]),
+                        P = l("unfilteredColumns", A, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
+                        L = l("unfilteredRows", k, [T, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
+                        B = l("unfilteredColumnKeys", ve, [P]),
+                        S = l("unfilteredRowKeys", ve, [L]),
+                        K = l("columnsOrder", Ne, [t.columnsOrder]),
+                        W = l("rowsOrder", Ne, [t.rowsOrder]),
+                        F = l("orderedColumns", He, [P, K]),
+                        U = l("orderedRows", He, [L, W]),
+                        H = l("filterFormatting", we, [w]),
+                        G = l("filterFormattingRules", z, [H]),
+                        se = l("filteringRules", ye, [t.filtering]),
+                        ae = l("filteredColumns", q, [f, se, G, u, U, F, C]),
+                        de = l("filteredRows", j, [f, se, G, u, U, F, C]),
+                        pe = l("sortingFormatting", Ce, [w]),
+                        fe = l("sortingFormattingRules", z, [pe]),
+                        me = l("sortingRules", Ie, [t.sorting]),
+                        ge = l("sortedColumns", Te, [p, me, fe, u, de, ae, C]),
+                        xe = l("sortedRows", Me, [p, me, fe, u, de, ae, C]),
+                        Ae = l("measureFormatting", Ee, [w]),
+                        ke = l("measureFormattingRules", z, [Ae]),
+                        De = l("measureFormatResolver", N, [ke, u, xe, ge, C]),
+                        Oe = e.columnWidthCache,
+                        Pe = e.rowHeightCache,
+                        je = l("measuredColumns", be, [ge, xe, _, De, Oe, B]),
+                        qe = l("measuredRows", Re, [ge, xe, _, De, Pe, S]),
+                        $e = l("columns", I, [je, s, a]),
+                        Ve = l("rows", D, [qe, s, a]),
+                        Ge = l("columnLookup", ie, [$e]),
+                        Ye = l("rowLookup", ie, [Ve]),
+                        Xe = t.focusedCell,
+                        Ze = l("sections", g, [$e, Ve]),
+                        Je = t.selectedCells,
+                        Qe = l("fixedSize", $, [Ze.top.height, Ze.bottom.height, Ze.left.width, Ze.right.width]),
+                        et = l("totalSize", V, [$e, Ve]),
+                        tt = function(e, t, o, n, r, i) {
                             if (!t) return null;
                             if (t.x < 0 || t.y < 0 || t.x > i.width || t.y > i.height) return null;
                             const l = re(e, t, r, i),
                                 s = function(e, t) {
                                     if (0 === e.length) return -1;
                                     if (t < e[0].topWithBorder) return -1;
                                     if (t > e[e.length - 1].bottomWithBorder) return -1;
@@ -1944,35 +2019,36 @@
                                     }
                                     return -1
                                 }(n, l.x);
                             return -1 === s || -1 === a ? null : {
                                 rowId: o[s].id,
                                 columnId: n[a].id
                             }
-                        }(r, e.mousePosition, Pe, Te, Ve, Ge),
-                        Xe = e.resizingColumn || l("resizableColumn", Le, [Te, Ne, He, Ye, r, e.mousePosition, Ve, Ge]),
-                        Ze = e.resizingRow || l("resizableRow", Be, [Pe, Ne, He, Ye, r, e.mousePosition, Ve, Ge]),
-                        Je = l("highlightedCells", le, [e.isMouseDown, !!Xe || !!Ze, je, Ye, Te, Pe, Ne, He]),
-                        Qe = l("selection", v, [$e]),
-                        et = l("highlight", v, [Je]),
-                        tt = l("renderFormatting", m, [w, Ye, je, Qe, et, R, p, Xe, Ze, t.borderWidth]),
-                        ot = l("renderFormattingRules", z, [tt]),
-                        nt = l("renderFormatResolver", N, [ot, c, Pe, Te, R]),
-                        rt = l("inputFormatting", h, [w]),
-                        it = l("inputFormattingRules", z, [rt]),
-                        lt = l("inputFormatResolver", N, [it, c, Pe, Te, R]),
-                        st = l("editableCells", i, [$e, lt, Ne, He]),
-                        at = l("inputPlacement", ce, [st, je, Ne, He, qe]),
-                        ct = l("isTextValid", ue, [d, st]),
-                        ut = l("contextFormatting", Fe, [w]),
-                        dt = l("contextFormattingRules", z, [ut]),
-                        pt = l("contextFormatResolver", N, [dt, c, Pe, Te, R]),
-                        ft = l("tooltip", ze, [Ye, pt, Ne, He]),
-                        ht = l("tooltipPlacement", Ue, [ft, Ye, Ne, He, qe]),
-                        _t = function(e, t, o, n) {
+                        }(r, e.mousePosition, Ve, $e, Qe, et),
+                        ot = e.isReordering,
+                        nt = e.resizingColumn || l("resizableColumn", Le, [$e, Ge, Ye, tt, r, e.mousePosition, ot, Qe, et]),
+                        rt = e.resizingRow || l("resizableRow", Be, [Ve, Ge, Ye, tt, r, e.mousePosition, ot, Qe, et]),
+                        it = l("highlightedCells", le, [e.isMouseDown, !nt && !rt && !e.didReorder, Xe, tt, $e, Ve, Ge, Ye]),
+                        lt = l("selection", R, [Je]),
+                        st = l("highlight", R, [it]),
+                        at = l("renderFormatting", m, [w, tt, Xe, lt, st, C, p, nt, rt, t.borderWidth, ot, e.reorderedColumn, e.reorderedRow]),
+                        ut = l("renderFormattingRules", z, [at]),
+                        ct = l("renderFormatResolver", N, [ut, u, Ve, $e, C]),
+                        dt = l("inputFormatting", h, [w]),
+                        pt = l("inputFormattingRules", z, [dt]),
+                        ft = l("inputFormatResolver", N, [pt, u, Ve, $e, C]),
+                        ht = l("editableCells", i, [Je, ft, Ge, Ye]),
+                        _t = l("inputPlacement", ue, [ht, Xe, Ge, Ye, Ze]),
+                        mt = l("isTextValid", ce, [d, ht]),
+                        gt = l("contextFormatting", Fe, [w]),
+                        yt = l("contextFormattingRules", z, [gt]),
+                        wt = l("contextFormatResolver", N, [yt, u, Ve, $e, C]),
+                        Et = l("tooltip", ze, [tt, wt, Ge, Ye]),
+                        bt = l("tooltipPlacement", Ue, [Et, tt, Ge, Ye, Ze]),
+                        Rt = function(e, t, o, n) {
                             const r = {
                                     width: n.getBoundingClientRect().width,
                                     height: n.getBoundingClientRect().height
                                 },
                                 i = {
                                     left: n.scrollLeft,
                                     top: n.scrollTop
@@ -1983,90 +2059,99 @@
                                     top: 0,
                                     ...t
                                 }, o),
                                 a = ee({
                                     ...i,
                                     ...r
                                 }, o),
-                                c = Z(s, J(a, te)),
-                                u = Z(s, J(a, oe));
-                            return X(s, l) && X(l, c) ? Q(l) > 2 * Q(u) ? u : l : u
-                        }(n?.scrollRect, Ge, Ve, r);
-                    l("activeColumns", We, [Te, t.onActiveColumnsChange]), l("activeRows", We, [Pe, t.onActiveRowsChange]), e.state = {
+                                u = Z(s, J(a, te)),
+                                c = Z(s, J(a, oe));
+                            return X(s, l) && X(l, u) ? Q(l) > 2 * Q(c) ? c : l : c
+                        }(n?.scrollRect, et, Qe, r);
+                    l("activeColumns", We, [$e, t.onActiveColumnsChange]), l("activeRows", We, [Ve, t.onActiveRowsChange]), e.state = {
                         options: t,
                         devicePixelRatio: s,
                         borderWidth: a,
-                        data: c,
-                        edition: R,
-                        filteredColumns: U,
-                        filteredRows: H,
-                        columns: Te,
-                        rows: Pe,
-                        sections: qe,
-                        selectedCells: $e,
-                        selection: Qe,
-                        highlight: et,
-                        hoveredCell: Ye,
-                        focusedCell: je,
-                        renderFormatting: tt,
-                        renderFormatResolver: nt,
-                        inputFormatting: rt,
-                        inputFormatResolver: lt,
-                        fixedSize: Ve,
-                        totalSize: Ge,
+                        data: u,
+                        edition: C,
+                        filteredColumns: ae,
+                        filteredRows: de,
+                        columns: $e,
+                        rows: Ve,
+                        sections: Ze,
+                        selectedCells: Je,
+                        selection: lt,
+                        highlight: st,
+                        hoveredCell: tt,
+                        focusedCell: Xe,
+                        renderFormatting: at,
+                        renderFormatResolver: ct,
+                        inputFormatting: dt,
+                        inputFormatResolver: ft,
+                        fixedSize: Qe,
+                        totalSize: et,
                         textResolver: _,
-                        scrollRect: _t,
-                        highlightedCells: Je,
-                        inputPlacement: at,
-                        columnLookup: Ne,
-                        rowLookup: He,
+                        scrollRect: Rt,
+                        highlightedCells: it,
+                        inputPlacement: _t,
+                        columnLookup: Ge,
+                        rowLookup: Ye,
                         text: d,
-                        isTextValid: ct,
-                        resizableColumn: Xe,
-                        resizableRow: Ze,
-                        tooltip: ft,
-                        tooltipPlacement: ht
+                        isTextValid: mt,
+                        resizableColumn: nt,
+                        resizableRow: rt,
+                        tooltip: Et,
+                        tooltipPlacement: bt
                     }
                 }
 
-                function He(e) {
+                function qe(e) {
                     if (!e.error) try {
-                        Ne(e)
+                        je(e)
                     } catch (t) {
                         e.error = t
                     }
                 }
 
-                function je(e, t) {
-                    const o = new E(t);
+                function $e(e, t) {
+                    const o = new b(t);
                     return [...t, ...e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))]
                 }
 
-                function qe(e, t) {
-                    const o = new E(t);
+                function Ve(e, t) {
+                    const o = new b(t);
                     return e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))
                 }
 
-                function $e(e) {
+                function Ge(e) {
                     const t = e.currentTarget.getBoundingClientRect();
                     return {
                         x: e.clientX - t.left,
                         y: e.clientY - t.top
                     }
                 }
 
-                function Ve(e, t) {
+                function Ye(e, t) {
                     return e.map((e => ({
                         ...e,
                         columnId: "id" in e ? e.id : t,
                         rowId: "id" in e ? e.id : t
                     })))
                 }
 
-                function Ge(e) {
+                function Xe(e, t, o) {
+                    const r = n(t),
+                        i = n(o);
+                    if (r === i) return null;
+                    const l = e.findIndex((e => e.key === r)),
+                        s = e.findIndex((e => e.key === i));
+                    return -1 === l || -1 === s || l === s ? null : [l, s]
+                }
+
+                function Ze(e) {
                     if ("spread-grid-context" in e) return;
                     const t = {
                             "top-left": document.createElement("canvas"),
                             "top-center": document.createElement("canvas"),
                             "top-right": document.createElement("canvas"),
                             "middle-left": document.createElement("canvas"),
                             "middle-center": document.createElement("canvas"),
@@ -2089,15 +2174,15 @@
                         renderRequested: !1,
                         mousePosition: null,
                         isMouseDown: !1,
                         columnWidthCache: new Map,
                         rowHeightCache: new Map,
                         requestNewRender: () => {
                             s.renderRequested || (s.renderRequested = !0, requestAnimationFrame((() => {
-                                s.renderRequested = !1, He(s), a(s)
+                                s.renderRequested = !1, qe(s), a(s)
                             })))
                         },
                         addEventListener: (e, t, o) => {
                             e.addEventListener(t, (e => {
                                 try {
                                     o(e)
                                 } catch (e) {
@@ -2156,66 +2241,74 @@
                         onColumnWidthsChange: e => {
                             s.localOptions.columnWidths = e, s.requestNewRender()
                         },
                         rowHeights: [],
                         onRowHeightsChange: e => {
                             s.localOptions.rowHeights = e, s.requestNewRender()
                         },
+                        columnsOrder: [],
+                        onColumnsOrderChange: e => {
+                            s.localOptions.columnsOrder = e, s.requestNewRender()
+                        },
+                        rowsOrder: [],
+                        onRowsOrderChange: e => {
+                            s.localOptions.rowsOrder = e, s.requestNewRender()
+                        },
                         onActiveColumnsChange: () => {},
                         onActiveRowsChange: () => {}
                     }, e["spread-grid-context"] = s;
-                    const c = e => {
+                    const u = e => {
                             o.value = e, o.dispatchEvent(new Event("input"))
                         },
-                        u = e => {
+                        c = e => {
                             const t = s.state.options.selectedCells,
                                 o = s.state.inputFormatResolver,
                                 n = s.state.columnLookup,
                                 r = s.state.rowLookup,
                                 l = s.state.text,
                                 a = s.state.isTextValid,
-                                u = s.state.options.onEditedCellsChange,
+                                c = s.state.options.onEditedCellsChange,
                                 d = s.state.options.onFiltersChange,
                                 p = i(t, o, n, r);
                             if ("" === l) return;
                             if (!a) return;
                             if (e && !p.every((e => e.edit.autoCommit))) return;
                             const f = p.filter((e => "DATA" === e.type)),
                                 h = p.filter((e => "FILTER" === e.type));
                             var _;
                             _ = f.map((e => ({
                                 ...e.cell,
                                 value: e.edit.parse({
                                     string: l
                                 })
-                            }))), u(je(s.state.options.editedCells, _)), (e => {
-                                d(je(Ve(s.state.options.filters, "FILTER"), e))
+                            }))), c($e(s.state.options.editedCells, _)), (e => {
+                                d($e(Ye(s.state.options.filters, "FILTER"), e))
                             })(h.map((e => ({
                                 ...e.cell,
                                 expression: e.edit.parse({
                                     string: l
                                 })
-                            })))), e || c("")
+                            })))), e || u("")
                         },
                         d = e => {
                             const t = s.state.options.selectedCells,
                                 o = s.state.options.onEditedCellsChange,
                                 n = s.state.options.onFiltersChange,
                                 r = i(t, s.state.inputFormatResolver, s.state.columnLookup, s.state.rowLookup);
                             var l;
-                            e && !r.every((e => e.edit.autoCommit)) || (l = t, o(qe(s.state.options.editedCells, l)), (e => {
-                                n(qe(Ve(s.state.options.filters, "FILTER"), e))
+                            e && !r.every((e => e.edit.autoCommit)) || (l = t, o(Ve(s.state.options.editedCells, l)), (e => {
+                                n(Ve(Ye(s.state.options.filters, "FILTER"), e))
                             })(t))
                         };
                     s.addEventListener(e, "scroll", (e => {
                         s.requestNewRender()
                     })), s.addEventListener(e, "mouseenter", (e => {
-                        s.mousePosition = $e(e), s.requestNewRender()
+                        s.mousePosition = Ge(e), s.requestNewRender()
                     })), s.addEventListener(e, "mousemove", (t => {
-                        if (s.mousePosition = $e(t), s.resizingColumn) {
+                        if (s.mousePosition = Ge(t), s.resizingColumn) {
                             const t = s.state.columnLookup.get(n(s.resizingColumn)),
                                 o = t.width,
                                 r = t.right,
                                 i = re(e, s.mousePosition, s.state.fixedSize, s.state.totalSize),
                                 l = Math.max(10, i.x - r + o),
                                 a = s.state.options.columnWidths.filter((e => n(e.columnId) !== t.key)).concat([{
                                     columnId: t.id,
@@ -2231,93 +2324,134 @@
                                 l = Math.max(10, i.y - r + o),
                                 a = s.state.options.rowHeights.filter((e => n(e.rowId) !== t.key)).concat([{
                                     rowId: t.id,
                                     height: l
                                 }]);
                             s.state.options.onRowHeightsChange(a)
                         }
+                        if (s.reorderedColumn) {
+                            const t = s.state.columns,
+                                o = s.state.hoveredCell,
+                                n = re(e, s.mousePosition, s.state.fixedSize, s.state.totalSize),
+                                r = function(e, t, o, n) {
+                                    if (!o) return null;
+                                    const r = Xe(e, t, o.columnId);
+                                    if (!r) return null;
+                                    const [i, l] = r, s = l <= i ? n.x < e[l].leftWithBorder + e[i].width ? l : l + 1 : n.x > e[l].rightWithBorder - e[i].width ? l : l - 1;
+                                    if (s === i) return null;
+                                    const a = e.map((e => e.id));
+                                    return a.splice(i, 1), a.splice(s, 0, t), a
+                                }(t, s.reorderedColumn, o, n);
+                            r && (s.didReorder = !0, s.isReordering = !0, s.state.options.onColumnsOrderChange(r))
+                        }
+                        if (s.reorderedRow) {
+                            const t = s.state.rows,
+                                o = s.state.hoveredCell,
+                                n = re(e, s.mousePosition, s.state.fixedSize, s.state.totalSize),
+                                r = function(e, t, o, n) {
+                                    if (!o) return null;
+                                    const r = Xe(e, t, o.rowId);
+                                    if (!r) return null;
+                                    const [i, l] = r, s = l <= i ? n.y < e[l].topWithBorder + e[i].height ? l : l + 1 : n.y > e[l].bottomWithBorder - e[i].height ? l : l - 1;
+                                    if (s === i) return null;
+                                    const a = e.map((e => e.id));
+                                    return a.splice(i, 1), a.splice(s, 0, t), a
+                                }(t, s.reorderedRow, o, n);
+                            r && (s.didReorder = !0, s.isReordering = !0, s.state.options.onRowsOrderChange(r))
+                        }
                         s.requestNewRender()
                     })), s.addEventListener(e, "mouseleave", (() => {
                         s.mousePosition = null, s.requestNewRender()
                     })), s.addEventListener(e, "mousedown", (e => {
-                        He(s), c(""), s.isMouseDown = !0, s.mouseDownPosition = s.mousePosition, s.mouseDownCell = s.state.hoveredCell, s.state.resizableColumn && (s.resizingColumn = s.state.resizableColumn), s.state.resizableRow && (s.resizingRow = s.state.resizableRow), s.state.resizableColumn || s.state.resizableRow || s.state.options.onFocusedCellChange(s.state.hoveredCell), e.ctrlKey || s.state.options.onSelectedCellsChange([]), s.requestNewRender()
+                        qe(s), u("");
+                        const t = s.state.hoveredCell;
+                        if (s.isMouseDown = !0, s.didReorder = !1, s.mouseDownPosition = s.mousePosition, s.mouseDownCell = t, s.state.resizableColumn && (s.resizingColumn = s.state.resizableColumn), s.state.resizableRow && (s.resizingRow = s.state.resizableRow), !s.resizingColumn && t) {
+                            const e = s.state.rowLookup.get(n(t.rowId));
+                            s.reorderedColumn = "HEADER" === e.type ? t.columnId : null
+                        }
+                        if (!s.resizingRow && t) {
+                            const e = s.state.columnLookup.get(n(t.columnId));
+                            s.reorderedRow = "HEADER" === e.type ? t.rowId : null
+                        }
+                        s.resizingColumn || s.resizingRow || s.state.options.onFocusedCellChange(t), e.ctrlKey || s.state.options.onSelectedCellsChange([]), s.requestNewRender()
                     })), s.addEventListener(e, "mouseup", (e => {
-                        He(s), s.isMouseDown = !1, s.resizingColumn = null, s.resizingRow = null, s.state.options.onSelectedCellsChange(je(s.state.options.selectedCells, s.state.highlightedCells)), s.requestNewRender()
+                        qe(s), s.isMouseDown = !1, s.isReordering = !1, s.resizingColumn = null, s.resizingRow = null, s.reorderedColumn = null, s.reorderedRow = null, s.state.options.onSelectedCellsChange($e(s.state.options.selectedCells, s.state.highlightedCells)), s.requestNewRender()
                     })), s.addEventListener(e, "pointerdown", (e => {
                         s.element.setPointerCapture(e.pointerId)
                     })), s.addEventListener(e, "pointerup", (e => {
                         s.element.releasePointerCapture(e.pointerId)
                     })), s.addEventListener(e, "click", (e => {
-                        He(s);
+                        qe(s);
                         const t = s.state.hoveredCell,
                             o = s.mouseDownCell;
                         if (s.state.resizableColumn || s.state.resizableRow) return;
+                        if (s.didReorder) return;
                         if (null === t) return;
                         if (n(t.columnId) !== n(o.columnId)) return;
                         if (n(t.rowId) !== n(o.rowId)) return;
                         const i = s.state.columnLookup.get(n(t.columnId)),
                             l = s.state.rowLookup.get(n(t.rowId)),
                             a = s.state.options.sortBy,
-                            c = s.state.inputFormatResolver.resolve(l, i),
-                            u = {
+                            u = s.state.inputFormatResolver.resolve(l, i),
+                            c = {
                                 ctrlKey: e.ctrlKey,
                                 shiftKey: e.shiftKey,
                                 button: e.button,
                                 buttons: e.buttons
                             };
-                        if (c.edit?.toggle) {
+                        if (u.edit?.toggle) {
                             const e = function(e, t, o, n) {
                                     const r = n.hasValueByKey(o.key, t.key) ? n.getValueByKey(o.key, t.key) : e.value,
                                         i = e.edit.toggle;
                                     return "function" == typeof i ? i({
                                         value: r
                                     }) : i[(i.indexOf(r) + 1) % i.length]
-                                }(c, i, l, s.state.edition),
+                                }(u, i, l, s.state.edition),
                                 o = r(i, l);
-                            "DATA" === o && s.state.options.onEditedCellsChange(je(s.state.options.editedCells, [{
+                            "DATA" === o && s.state.options.onEditedCellsChange($e(s.state.options.editedCells, [{
                                 ...t,
                                 value: e
-                            }])), "FILTER" === o && s.state.options.onFiltersChange(je(s.state.options.filters, [{
+                            }])), "FILTER" === o && s.state.options.onFiltersChange($e(s.state.options.filters, [{
                                 ...t,
                                 expression: e
                             }]))
                         } else if ("DATA" === i.type && "DATA" === l.type) s.state.options.onCellClick({
                             ...s.state.hoveredCell,
-                            ...u
+                            ...c
                         });
                         else if ("CUSTOM" === i.type || "CUSTOM" === l.type) s.state.options.onCustomCellClick({
                             ...s.state.hoveredCell,
-                            ...u
+                            ...c
                         });
                         else if ("HEADER" === i.type || "HEADER" === l.type) {
                             const t = function(e, t, o, r) {
                                 function i(e) {
                                     const r = "columnId" in e ? e.columnId : "HEADER",
                                         i = "rowId" in e ? e.rowId : "HEADER";
                                     return t.key === n(r) && o.key === n(i)
                                 }
                                 const l = ["ASC", "DESC", void 0],
                                     s = e.find(i),
                                     a = l.indexOf(s?.direction),
-                                    c = l[(a + 1) % l.length],
-                                    u = e.indexOf(s) === e.length - 1;
-                                return [...!r || !u && s ? e.filter((e => ! function(e) {
+                                    u = l[(a + 1) % l.length],
+                                    c = e.indexOf(s) === e.length - 1;
+                                return [...!r || !c && s ? e.filter((e => ! function(e) {
                                     const r = "columnId" in e ? e.columnId : "HEADER",
                                         i = "rowId" in e ? e.rowId : "HEADER";
                                     return "HEADER" === t.type && t.key === n(r) || "HEADER" === o.type && o.key === n(i)
-                                }(e))) : e.filter((e => !i(e))), ...c ? [{
+                                }(e))) : e.filter((e => !i(e))), ...u ? [{
                                     columnId: t.id,
                                     rowId: o.id,
-                                    direction: c
+                                    direction: u
                                 }] : []]
                             }(a, i, l, e.ctrlKey);
                             s.state.options.onSortByChange(t), s.state.options.onSelectedCellsChange([])
                         }
                     })), s.addEventListener(e, "dblclick", (e => {
-                        if (He(s), s.state.resizableColumn) {
+                        if (qe(s), s.state.resizableColumn) {
                             const e = n(s.state.resizableColumn),
                                 t = s.state.options.columnWidths.filter((t => n(t.columnId) !== e));
                             s.state.options.onColumnWidthsChange(t), s.columnWidthCache.delete(e)
                         }
                         if (s.state.resizableRow) {
                             const e = n(s.state.resizableRow),
                                 t = s.state.options.rowHeights.filter((t => n(t.rowId) !== e));
@@ -2325,90 +2459,90 @@
                         }
                         const t = s.state.focusedCell;
                         if (null === t) return;
                         const r = n(t.columnId),
                             i = n(t.rowId),
                             l = s.state.columnLookup,
                             a = s.state.rowLookup,
-                            u = s.state.inputFormatResolver;
+                            c = s.state.inputFormatResolver;
                         if (!l.has(r)) return;
                         if (!a.has(i)) return;
                         const d = l.get(r),
                             p = a.get(i),
-                            f = u.resolve(p, d),
+                            f = c.resolve(p, d),
                             h = f.text;
-                        f.edit && (f.edit.toggle || (c(h), o?.select()))
+                        f.edit && (f.edit.toggle || (u(h), o?.select()))
                     })), s.addEventListener(e, "focus", (() => {
                         o.parentElement && o.focus({
                             preventScroll: !0
                         })
                     })), s.addEventListener(e, "keydown", (e => {
-                        He(s);
+                        qe(s);
                         const t = s.state.focusedCell,
                             o = s.state.columnLookup,
                             r = s.state.rowLookup,
                             i = s.state.options.selectedCells,
                             l = s.state.options.onSelectedCellsChange,
                             a = s.state.options.onFocusedCellChange,
                             p = s.state.options.editedCells,
                             f = s.state.options.onEditedCellsChange,
                             h = s.state.columns,
                             _ = s.state.rows,
                             m = s.state.text,
                             g = s.state.inputFormatResolver,
                             y = (e, t) => {
-                                a(e), t.shiftKey ? l(je(i, [e])) : l([e])
+                                a(e), t.shiftKey ? l($e(i, [e])) : l([e])
                             },
                             w = (e, r) => {
                                 if (!t) return;
                                 const i = n(t.columnId);
                                 if (!o.has(i)) return;
                                 const l = o.get(i).index,
                                     s = Math.max(0, Math.min(h.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: t.rowId,
                                     columnId: h[s].id
                                 };
                                 y(a, r)
                             },
-                            b = (e, o) => {
+                            E = (e, o) => {
                                 if (!t) return;
                                 const i = n(t.rowId);
                                 if (!r.has(i)) return;
                                 const l = r.get(i).index,
                                     s = Math.max(0, Math.min(_.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: _[s].id,
                                     columnId: t.columnId
                                 };
                                 y(a, o)
                             },
-                            v = () => {
+                            R = () => {
                                 e.preventDefault(), e.stopPropagation()
                             };
                         switch (e.key) {
                             case "Escape":
-                                "" !== m ? c("") : i.length > 1 ? l([t]) : p.length > 0 ? f([]) : (a(null), l([]));
+                                "" !== m ? u("") : i.length > 1 ? l([t]) : p.length > 0 ? f([]) : (a(null), l([]));
                                 break;
                             case "Enter":
-                                u();
+                                c();
                                 break;
                             case "ArrowUp":
-                                v(), b(e.ctrlKey ? -_.length : -1, e);
+                                R(), E(e.ctrlKey ? -_.length : -1, e);
                                 break;
                             case "ArrowDown":
-                                v(), b(e.ctrlKey ? _.length : 1, e);
+                                R(), E(e.ctrlKey ? _.length : 1, e);
                                 break;
                             case "ArrowLeft":
-                                v(), w(e.ctrlKey ? -h.length : -1, e);
+                                R(), w(e.ctrlKey ? -h.length : -1, e);
                                 break;
                             case "ArrowRight":
-                                v(), w(e.ctrlKey ? h.length : 1, e);
+                                R(), w(e.ctrlKey ? h.length : 1, e);
                                 break;
                             case "Delete":
                             case "Backspace":
                                 d();
                                 break;
                             case "c":
                                 (e => {
@@ -2417,31 +2551,31 @@
                                         const i = new Map(t.map((e => [e.key, e]))),
                                             l = new Map(o.map((e => [e.key, e]))),
                                             s = e.map((e => ({
                                                 columnKey: n(e.columnId),
                                                 rowKey: n(e.rowId)
                                             }))).filter((e => i.has(e.columnKey) && l.has(e.rowKey))),
                                             a = new Set(s.map((e => e.columnKey))),
-                                            c = new Set(s.map((e => e.rowKey)));
+                                            u = new Set(s.map((e => e.rowKey)));
                                         if (0 === s.length) return "";
-                                        const u = new E(e),
+                                        const c = new b(e),
                                             d = Math.min(...s.map((e => i.get(e.columnKey).index))),
                                             p = Math.max(...s.map((e => i.get(e.columnKey).index))),
                                             f = Math.min(...s.map((e => l.get(e.rowKey).index))),
                                             h = Math.max(...s.map((e => l.get(e.rowKey).index))),
                                             _ = [];
                                         for (let e = f; e <= h; e++) {
                                             const n = o[e],
                                                 i = n.key;
-                                            if (c.has(i)) {
+                                            if (u.has(i)) {
                                                 for (let e = d; e <= p; e++) {
                                                     const o = t[e],
                                                         l = o.key;
                                                     if (a.has(l)) {
-                                                        if (u.isKeySelected(i, l)) {
+                                                        if (c.isKeySelected(i, l)) {
                                                             const e = r.resolve(n, o).text;
                                                             _.push(e)
                                                         }
                                                         e < p && _.push("\t")
                                                     }
                                                 }
                                                 e < h && _.push("\n")
@@ -2455,15 +2589,15 @@
                                         e.value = t, document.body.appendChild(e), e.select(), document.execCommand("copy"), document.body.removeChild(e)
                                     }
                                 })(e)
                         }
                     })), new ResizeObserver((() => {
                         s.requestNewRender()
                     })).observe(e), s.addEventListener(o, "input", (e => {
-                        He(s), e.target.value ? (u(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && d(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
+                        qe(s), e.target.value ? (c(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && d(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
                     })), s.addEventListener(o, "click", (e => {
                         e.stopPropagation()
                     })), s.addEventListener(o, "dblclick", (e => {
                         e.stopPropagation()
                     })), s.addEventListener(o, "mousedown", (e => {
                         e.stopPropagation()
                     })), s.addEventListener(o, "keydown", (e => {
@@ -2481,18 +2615,18 @@
                                 break;
                             default:
                                 e.stopPropagation(), s.requestNewRender()
                         }
                     }))
                 }
 
-                function Ye(e, t) {
-                    Ge(e);
+                function Je(e, t) {
+                    Ze(e);
                     const o = e["spread-grid-context"];
-                    o.externalOptions = t, null === o.state ? (He(o), a(o)) : o.requestNewRender()
+                    o.externalOptions = t, null === o.state ? (qe(o), a(o)) : o.requestNewRender()
                 }
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
@@ -2542,15 +2676,15 @@
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
                 o = isLocalScript(t),
                 n = __jsonpScriptSrc__(e);
             if (!o) return n;
             var r = n.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_1_3m1716794736"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_1_4m1717004035"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     var __webpack_exports__ = {};
     (() => {
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
             DashSpreadGrid: () => e.Z
         });
```

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/dash_spread_grid.min.js.map` & `dash_spread_grid-0.1.4/dash_spread_grid/dash_spread_grid.min.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9045506594014057%*

 * *Differences: {"'mappings'": "'2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,yEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAkBpB,GAhBI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_spread_grid.min.js",
-    "mappings": "2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,yEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAkBpB,GAhBI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC,WAAWO,MAAQhB,SAASQ,KAAKQ,OAASH,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKQ,MAAK,MAAOR,KAAKQ,OACzF,YAAaR,OACbC,WAAWQ,QAAUjB,SAASQ,KAAKS,SAAWJ,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKS,QAAO,MAAOT,KAAKS,SAC/F,SAAUT,OACVC,WAAWS,KAAOL,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKU,KAAI,OACpD,SAAUV,KACV,GAAIA,KAAKW,KAAM,CACX,IAAMC,WAAa,CAAC,EAChB,aAAcZ,KAAKW,OACnBC,WAAWC,SAAWR,KAAK,kBAADC,OAAmBN,KAAKW,KAAKE,SAAQ,OAC/D,UAAWb,KAAKW,OAChBC,WAAWE,MAAQT,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKW,KAAKG,MAAK,OAC3D,gBAAiBd,KAAKW,OACtBC,WAAWG,WAAaf,KAAKW,KAAKK,aAClC,WAAYhB,KAAKW,OACjBC,WAAWK,OAASjB,KAAKW,KAAKM,QAClChB,WAAWU,KAAOC,UACtB,MAEIX,WAAWU,KAAOX,KAAKW,KAG/B,OAAOV,UACX,GACJ,GAAG,CAACL,YACR,CAEA,SAASsB,qBAAqBC,WAC1B,OAAOtB,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,8DAEhB,OAAOqB,UAAUpB,KAAI,SAAAC,MACjB,IAAMC,WAAa,CAAC,EASpB,MAPI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAE3DH,UACX,GACJ,GAAG,CAACkB,WACR,CAEA,SAASC,wBAAwBC,cAC7B,OAAOxB,EAAAA,mCAAAA,UAAQ,WACX,OAAOQ,KAAK,6BAADC,OAA8Be,aAAY,KACzD,GAAG,CAACA,cACR,CAIA,SAASC,eAAeC,GAGpB,IAAMC,EAAWD,EAAMC,SACjBC,GAAUC,EAAAA,mCAAAA,QAAO,GAEjBC,EAAOJ,EAAMI,KACbC,EAAUL,EAAMK,QAChBC,EAAON,EAAMM,KACbjC,EAAaD,sBAAsB4B,EAAM3B,YACzCuB,EAAYD,qBAAqBK,EAAMJ,WACvCE,EAAeD,wBAAwBG,EAAMO,eAC7CC,EAAYR,EAAMS,WAClBC,EAAeV,EAAMW,cACrBC,EAAaZ,EAAMa,YACnBC,EAAcd,EAAMe,aACpBC,EAAUhB,EAAMgB,QAChBC,EAAcjB,EAAMkB,aACpBC,EAAgBnB,EAAMoB,eACtBC,GAAwBC,EAAAA,mCAAAA,cAAY,SAACH,GACvClB,EAAS,CAAEmB,eAAgBD,GAC/B,GAAG,CAAClB,IACEsB,GAAkBD,EAAAA,mCAAAA,cAAY,SAACN,GACjCf,EAAS,CAAEe,QAAAA,GACf,GAAG,CAACf,IACEuB,GAAsBF,EAAAA,mCAAAA,cAAY,SAACL,GACrChB,EAAS,CAAEiB,aAAcD,GAC7B,GAAG,CAAChB,IACEwB,EAAczB,EAAM0B,aACpBC,GAAcL,EAAAA,mCAAAA,cAAY,SAACM,GAC7B3B,EAAS,CAAEyB,aAAYG,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAG5B,EAAQ6B,aACnD,GAAG,CAAC9B,IACE+B,EAAoBhC,EAAMiC,oBAC1BC,GAAoBZ,EAAAA,mCAAAA,cAAY,SAACM,GACnC3B,EAAS,CAAEgC,oBAAmBJ,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAG5B,EAAQ6B,aAC1D,GAAG,CAAC9B,IACEkC,GAAwBb,EAAAA,mCAAAA,cAAY,SAACc,GACvCnC,EAAS,CAAEoC,eAAgBD,GAC/B,GAAG,CAACnC,IACEqC,GAAqBhB,EAAAA,mCAAAA,cAAY,SAACiB,GACpCtC,EAAS,CAAEuC,YAAaD,GAC5B,GAAG,CAACtC,IAEwCwC,EAAAC,gBAAdC,EAAAA,mCAAAA,UAAS,MAAK,GAArCC,EAAOH,EAAA,GAAEI,EAAUJ,EAAA,GA4B1B,OA1BIG,IACAE,EAAAA,4CAAAA,GAAWF,EAAS,CAChBxC,KAAAA,EACAC,QAAAA,EACAC,KAAAA,EACAjC,WAAAA,EACAuB,UAAAA,EACAY,UAAAA,EACAE,aAAAA,EACAE,WAAAA,EACAE,YAAAA,EACAE,QAAAA,EACAlB,aAAAA,EACAmB,YAAAA,EACAE,cAAAA,EACAE,sBAAAA,EACAG,oBAAAA,EACAD,gBAAAA,EACAE,YAAAA,EACAE,YAAAA,EACAK,kBAAAA,EACAE,kBAAAA,EACAC,sBAAAA,EACAG,mBAAAA,IAGDS,6CAAAA,cAAoB,MAAO,CAAEC,IAAKH,GAC7C,CAIA9C,eAAekD,UAAY,CAEvBhD,SAAUiD,kDAAAA,KAEVC,GAAID,kDAAAA,OAEJ9C,KAAM8C,kDAAAA,IAEN7C,QAAS6C,kDAAAA,MAET5C,KAAM4C,kDAAAA,MAEN7E,WAAY6E,kDAAAA,MAEZtD,UAAWsD,kDAAAA,MAEXE,QAASF,kDAAAA,MAET3C,cAAe2C,kDAAAA,OAEfzC,WAAYyC,kDAAAA,OAEZvC,cAAeuC,kDAAAA,OAEfrC,YAAaqC,kDAAAA,OAEbnC,aAAcmC,kDAAAA,OAEdG,YAAaH,kDAAAA,OAEbI,YAAaJ,kDAAAA,OAEb9B,eAAgB8B,kDAAAA,MAEhBK,iBAAkBL,kDAAAA,MAElBhC,aAAcgC,kDAAAA,MAEdlC,QAASkC,kDAAAA,MAETM,QAASN,kDAAAA,MAETO,aAAcP,kDAAAA,MAEdQ,WAAYR,kDAAAA,MAEZxB,aAAcwB,kDAAAA,OAEdjB,oBAAqBiB,kDAAAA,OAErBb,eAAgBa,kDAAAA,MAEhBV,YAAaU,kDAAAA,OAGjBnD,eAAe4D,aAAe,CAC1BvD,KAAM,GACNC,QAAS,CAAC,CAAE,KAAQ,eACpBC,KAAM,CAAC,CAAE,KAAQ,UAAY,CAAE,KAAQ,eACvCjC,WAAY,GACZuB,UAAW,GACXwD,QAAS,GACT7C,cAAe,0BACfE,WAAY,EACZE,cAAe,EACfE,YAAa,EACbE,aAAc,EACdsC,YAAa,EACbC,YAAa,KACblC,eAAgB,GAChBmC,iBAAkB,GAClBrC,aAAc,GACdF,QAAS,GACTwC,QAAS,GACTC,aAAc,GACdC,WAAY,GACZhC,aAAc,KACdO,oBAAqB,KACrBI,eAAgB,GAChBG,YAAa,IAGjB,+C,SChPAoB,EAAOC,QAAUC,OAAkB,S,UCAnCF,EAAOC,QAAUC,OAAc,K,gBCehB,SAASC,EAAYC,GAChC,OAAY,OAARA,EACO,OAEPC,MAAMC,QAAQF,GAPX,IAQmBA,EAVAxF,IAAIuF,GAEPI,KAAK,QAUT,iBAARH,GAtBUI,EAuBMJ,EAjBpB,IALMK,OAAOC,KAAKF,GAAQG,OACR/F,KAAIwF,GAClB,GAAGA,KAAOD,EAAYK,EAAOJ,QAGjBG,KAAK,SAmBrBK,KAAKC,UAAUT,GAhB1B,IATyBI,CA0BzB,CC1Be,SAASM,EAAgB/F,EAAQC,GAC5C,MAAoB,WAAhBD,EAAOgG,KAAiC,WAAb/F,EAAI+F,KACxB,SACJ,MACX,CCDe,SAASC,EAAiBzD,EAAe0D,EAAgBC,EAAcC,GAClF,OAAO5D,EAAc3C,KAAIoD,IACrB,MAAMoD,EAAYjB,EAAYnC,EAAKqD,UAC7BC,EAASnB,EAAYnC,EAAKuD,OAEhC,IAAKL,EAAaM,IAAIJ,GAClB,OAAO,KACX,IAAKD,EAAUK,IAAIF,GACf,OAAO,KAEX,MAAMvG,EAASmG,EAAaO,IAAIL,GAC1BpG,EAAMmG,EAAUM,IAAIH,GAE1B,MAAO,CACH9F,KAAMyF,EAAeS,QAAQ1G,EAAKD,GAAQS,KAC1CwC,KAAMA,EACN+C,KAAMD,EAAgB/F,EAAQC,GAClC,IACD2G,QAAO3D,GAAQA,GAAMxC,MAC5B,CCtBe,SAASoG,EAActH,EAAOuH,GACzC,OAAOC,KAAKC,MAAMzH,EAAQuH,GAAoBA,CAClD,CCAA,SAASG,EAAcrH,EAASsH,EAAUC,GACtC,MAAMC,EAAQxH,EAAQwH,MAChBC,EAASzH,EAAQ0H,SAAS,GAAGJ,KAAYC,KACzCI,EAAkBH,EAAMI,SAASN,GACjCO,EAAoBL,EAAMI,SAASL,GACnCzF,EAAU+F,EAAkB/F,QAC5BC,EAAO4F,EAAgB5F,KAE7B,GAAoB,IAAhBA,EAAK+F,QAAmC,IAAnBhG,EAAQgG,OAG7B,YAFIL,EAAOM,eACPN,EAAOM,cAAcC,YAAYP,IAIpCA,EAAOM,eACR/H,EAAQqE,QAAQ4D,YAAYR,GAOhC,MAAMS,EAAMT,EAAOU,WAAW,KAAM,CAAEC,OAAO,IAEvCC,EAAab,EAAMa,WACnBC,EAAed,EAAMc,aAErBhC,EAAiBkB,EAAMe,qBACvBzD,EAAc0C,EAAM1C,YACpB0D,EACGb,EAAgBc,cADnBD,EAEMb,EAAgBe,iBAFtBF,EAGIX,EAAkBc,eAHtBH,EAIKX,EAAkBe,gBAEvBC,EAAe/D,EAAc,EAG7BgE,EAFW/G,EAAK+F,OAEmB,GAAKU,EAAqB,EAAI,IAAMA,EAAwB,EAAI,GACnGO,EAFcjH,EAAQgG,OAEc,GAAKU,EAAsB,EAAI,IAAMA,EAAuB,EAAI,GACpGrD,EAAapD,EAAK9B,KAAII,GAAOA,EAAI2I,SACjC9D,EAAepD,EAAQ7B,KAAIG,GAAUA,EAAO6I,QAC5CC,EAAahE,EAAaiE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKN,EAAsBjE,EAC7EwE,EAAcnE,EAAWgE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKP,EAAwBhE,EAE9EyE,EAAsB,WAAfhC,EACPc,EAAWkB,KACX,EACAC,EAAmB,WAAblC,EACNe,EAAWmB,IACX,EACAP,EAAuB,WAAf1B,EACRc,EAAWY,MACXpB,EAAkBoB,MAClBD,EAAsB,WAAb1B,EACTe,EAAWW,OACXrB,EAAgBqB,OAGhBS,EAAoBvE,EAAaiE,QAAO,CAACO,EAAKT,EAAOU,KACvD,MACMC,EADaF,EAAIC,GACKV,EAAQnE,EAEpC,OADA4E,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAClB,EAAsB1D,EAAc,IAClCgF,EAAkB3E,EAAWgE,QAAO,CAACO,EAAKV,EAAQW,KACpD,MACMC,EADaF,EAAIC,GACKX,EAASlE,EAErC,OADA4E,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAClB,EAAqB1D,EAAc,IAEjCiF,EAAgBN,EAAkBO,MAAM,GAAI,GAC5CC,EAAaH,EAAgBE,MAAM,GAAI,GAEvCE,EAAwB/C,KAAKgD,IAAIJ,EAAcK,eAAcR,GAAUA,GAAUL,IAAO,GACxFc,EAAwBN,EAAcK,eAAcR,GAAUA,GAAUL,EAAON,IAC/EqB,EAAqBnD,KAAKgD,IAAIF,EAAWG,eAAcR,GAAUA,GAAUJ,IAAM,GACjFe,EAAqBN,EAAWG,eAAcR,GAAUA,GAAUJ,EAAMR,IAExEwB,EAAgCrD,KAAKgD,IAAID,EAAuB1B,EAAsB,EAAI,GAC1FiC,EAAgCJ,GAAyB7B,EAAuB,EAAI,GACpFkC,EAAkCvD,KAAKgD,IAAIG,EAAoB9B,EAAqB,EAAI,GACxFmC,EAAkCJ,GAAsB/B,EAAwB,EAAI,GAEpFoC,EAAQlF,MAAMmF,KAAK,CAAE/C,OAAQyC,EAAqBD,EAAqB,IAAK,CAACQ,EAAGC,KAClF,MAAM1K,EAAM0B,EAAKgJ,EAAWT,GAC5B,OAAO5E,MAAMmF,KAAK,CAAE/C,OAAQuC,EAAwBH,EAAwB,IAAK,CAACY,EAAGE,KACjF,MAAM5K,EAAS0B,EAAQkJ,EAAcd,GACrC,OAAO5D,EAAeS,QAAQ1G,EAAKD,EAAO,GAC5C,IAEA6K,EAAU,CAACF,EAAUC,IAAgBJ,EAAMG,EAAWT,GAAoBU,EAAcd,GAE9FzC,EAAOwB,MAAQ9B,KAAKC,MAAM6B,EAAQ/B,kBAClCO,EAAOuB,OAAS7B,KAAKC,MAAM4B,EAAS9B,kBACpCO,EAAO/G,MAAMuI,MAAQ,GAAGA,MACxBxB,EAAO/G,MAAMsI,OAAS,GAAGA,MACzBvB,EAAO/G,MAAMwK,WAAa,GAAG3B,MAC7B9B,EAAO/G,MAAMyK,UAAY,GAAG3B,MAC5B/B,EAAO/G,MAAM0K,YAAiBlC,EAAaD,EAAQM,EAAxB,KAC3B9B,EAAO/G,MAAM2K,aAAkB/B,EAAcN,EAASQ,EAA1B,KAE5BtB,EAAIoD,UAAY,UAChBpD,EAAIqD,SAAS,EAAG,EAAG9D,EAAOwB,MAAOxB,EAAOuB,QAExC,MAAMwC,EAAe,CAACC,EAAGC,KACrBxD,EAAIsD,aAAatE,iBAAkB,EAAG,EAAGA,kBAAmBuE,EAAIlC,GAAQrC,kBAAmBwE,EAAIlC,GAAOtC,iBAAiB,EAErHyE,EAAU,CAACF,EAAGC,EAAGzC,EAAOD,KAC1Bd,EAAI0D,YACJ1D,EAAI2D,KAAKJ,EAAGC,EAAGzC,EAAOD,GACtBd,EAAI4D,MAAM,EAId,IAAK,IAAId,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F9C,EAAI6D,OACJP,EAAa/B,EAAkBuB,GAAc,GAC7CW,EAAQ,EAAG,EAAGzG,EAAa8F,GAAc1B,GAEzC,IAAK,IAAIyB,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAAM1H,EAAO4H,EAAQF,EAAUC,GACzBtK,EAAQ2C,EAAK3C,MACbsL,EAAUlC,EAAgBiB,GAC1BkB,EAAWxC,EAAkBuB,GAC7BkB,EAAYhH,EAAa8F,GACzBmB,EAAahH,EAAW4F,GACxBtK,EAAO4C,EAAK5C,KACZ2L,EAAe1L,EAAM0L,cAAgB,SACrCzL,EAAU0C,EAAK1C,QAwBrB,GAtBA6K,EAAaS,EAAUD,GAEvB9D,EAAIoD,UAAY5K,EAAM2L,YAAc,QACpCnE,EAAIqD,SAAS,EAAG,EAAGW,EAAWC,GAE1B,SAAU9I,GACVA,EAAKzC,KAAKsH,GAEVxH,EAAM4L,YACNpE,EAAIoD,UAAY5K,EAAM4L,UACtBpE,EAAIqD,SAAS,EAAG,EAAGW,EAAWC,IAG9BzL,EAAM6L,SACNrE,EAAIoD,UAAY5K,EAAM6L,OACtBrE,EAAI0D,YACJ1D,EAAIsE,OAAON,EAAY,EAAGC,GAC1BjE,EAAIuE,OAAOP,EAAWC,GACtBjE,EAAIuE,OAAOP,EAAWC,EAAa,GACnCjE,EAAIwE,QAGJjM,EAAM,CACNyH,EAAIoD,UAAY5K,EAAMiM,YAAc,QACpCzE,EAAI0E,KAAOvJ,EAAKuJ,KAEhB,MAAMC,EAAcvE,EAAawE,eAAezJ,EAAKuJ,MAE/CG,EAAgC,UAAnBrM,EAAMqM,WAAyBzE,EAAa0E,aAAavM,EAAM4C,EAAKuJ,MAAQV,EAAYvL,EAAQ4I,KAAO5I,EAAQsM,MAC5H,OACAvM,EAAMqM,WAAa,OACzB7E,EAAI6E,UAAYA,EAGhB,MAAMG,EAAQjG,EACI,SAAd8F,EAAuBpM,EAAQ4I,KACb,WAAdwD,EAAyBb,EAAY,EACnB,UAAda,EAAwBb,EAAYvL,EAAQsM,MACxC,EACZ/F,kBAGEiG,EAAQlG,EACO,QAAjBmF,EAAyBS,EAAYO,OAASP,EAAYQ,UAAY1M,EAAQ6I,IACzD,WAAjB4C,EAA4BD,EAAa,EAAIU,EAAYO,OACpC,WAAjBhB,EAA4BD,EAAaU,EAAYO,OAASP,EAAYS,aAAe3M,EAAQ4M,OAC7F,EACZrG,kBAGmBiG,EAAQN,EAAYO,OAASP,EAAYQ,WAAa,GAAKF,EAAQN,EAAYO,OAASP,EAAYS,cAAgBnB,EAGvIjE,EAAIsF,SAAS/M,EAAMyM,EAAOC,IAI1BjF,EAAIuF,YAAc,UAClBvF,EAAIwF,UAAY5I,EAEhBoD,EAAI0D,YACJ1D,EAAIsE,OAAO,EAAG1H,EAAc+D,GAC5BX,EAAIuE,OAAOP,EAAWpH,EAAc+D,GACpCX,EAAIsE,OAAO,EAAGL,EAAarH,EAAc+D,GACzCX,EAAIuE,OAAOP,EAAWC,EAAarH,EAAc+D,GACjDX,EAAIyF,SAEJzF,EAAI6D,OACJJ,EAAQ,EAAG,EAAI7G,EAAaoH,EAAWC,EAAa,EAAIrH,GAExDoD,EAAIsF,SAAS/M,EAAMyM,EAAOC,GAE1BjF,EAAI0F,UAEZ,CACJ,CAEA1F,EAAI0F,SACR,CAEApC,EAAa,EAAG,GAMhB,MAAMqC,EAAa,CAACC,EAAIC,EAAIC,EAAIC,EAAIvN,KAChC,IAAKA,EACD,OACJ,GAAoB,IAAhBA,EAAMuI,MACN,OAEJ,MAAMA,EAAQvI,EAAMuI,MAAQ/B,iBAEtBgH,EAAeH,IAAOE,EAGtBE,EAAKL,GAAMI,EAAejF,EAAQ,EAAI,GACtCmF,EAAKL,GAAOG,EAA2B,EAAZjF,EAAQ,GACnCoF,EAAKL,GAAME,EAAejF,EAAQ,EAAI,GACtCqF,EAAKL,GAAOC,EAA2B,EAAZjF,EAAQ,GAEzCf,EAAIuF,YAAc/M,EAAM6N,OAAS,QACjCrG,EAAIwF,UAAYzE,EAEZvI,EAAM8N,MACNtG,EAAIuG,YAAY/N,EAAM8N,KAAKvO,KAAIN,GAASA,EAAQuH,oBAChDgB,EAAIwG,eAAkBR,EAAeC,EAAKC,GAG1ClG,EAAIuG,YAAY,IAGpBvG,EAAI0D,YACJ1D,EAAIsE,OAAO2B,EAAIC,GACflG,EAAIuE,OAAO4B,EAAIC,GACfpG,EAAIyF,QAAQ,EAGVgB,EAAe,CAACC,EAAcC,IAC3BD,EAGAC,EAGDD,EAAajF,MAAQkF,EAAalF,MAC3BiF,EAEJC,EALID,EAHAC,EAYf,IAAK,IAAIC,EAAwBpE,EAAiCoE,GAAyBnE,EAAiCmE,IAAyB,CACjJ,MAAMC,EAAcD,EAAwB,EACtCE,EAAiBF,EAEvB,IAAK,IAAI9D,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F,MAGMiE,EAAcN,EAHGI,GAAezE,EAAqBW,EAAQ8D,EAAa/D,GAAatK,MAAMwO,aAAe,KACxFF,GAAkBzE,EAAqBU,EAAQ+D,EAAgBhE,GAAatK,MAAMyO,UAAY,MAIxHtB,EACIpE,EAAkBuB,GAAenC,EACjCiB,EAAgBkF,GAAkBnG,EAClCY,EAAkBuB,EAAc,GAAKnC,EACrCiB,EAAgBkF,GAAkBnG,EAClCoG,EACR,CACJ,CAEA,IAAK,IAAIG,EAAsB5E,EAA+B4E,GAAuB3E,EAA+B2E,IAAuB,CACvI,MAAMC,EAAkBD,EAAsB,EACxCE,EAAmBF,EAEzB,IAAK,IAAIrE,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAGMkE,EAAcN,EAHIU,GAAmBnF,EAAwBe,EAAQF,EAAUsE,GAAiB3O,MAAM6O,YAAc,KACjGD,GAAoBjF,EAAwBY,EAAQF,EAAUuE,GAAkB5O,MAAM8O,WAAa,MAI5H3B,EACIpE,EAAkB6F,GAAoBzG,EACtCiB,EAAgBiB,GAAYlC,EAC5BY,EAAkB6F,GAAoBzG,EACtCiB,EAAgBiB,EAAW,GAAKlC,EAChCoG,EACR,CACJ,CACJ,CAsHe,SAASQ,EAAOzP,GAC3B,IAAKA,EAAQ0P,MACT,KA5CR,SAAwB1P,GACpBqH,EAAcrH,EAAS,MAAO,QAC9BqH,EAAcrH,EAAS,MAAO,UAC9BqH,EAAcrH,EAAS,MAAO,SAC9BqH,EAAcrH,EAAS,SAAU,QACjCqH,EAAcrH,EAAS,SAAU,UACjCqH,EAAcrH,EAAS,SAAU,SACjCqH,EAAcrH,EAAS,SAAU,QACjCqH,EAAcrH,EAAS,SAAU,UACjCqH,EAAcrH,EAAS,SAAU,SAnFrC,SAAqBA,GACjB,MAAMqE,EAAUrE,EAAQqE,QAClBsL,EAAQ3P,EAAQ2P,MAChBnI,EAAQxH,EAAQwH,MAChBoI,EAAiBpI,EAAMoI,eAE7B,IAAKA,EAAgB,CACjB,GAAID,EAAM5H,cAAe,CACrB,MAAM8H,EAAWC,SAASC,gBAAkBJ,EAC5CA,EAAM5H,cAAcC,YAAY2H,GAC5BE,GACAxL,EAAQ2L,MAAM,CAAEC,eAAe,GACvC,CACA,MACJ,CAEA,MAAMxI,EAASzH,EAAQ0H,SAASkI,EAAeM,SAc/C,GAZAP,EAAMjP,MAAM6I,KAAO,SAAUqG,EAAiB,GAAGA,EAAerG,SAAW,IAC3EoG,EAAMjP,MAAM8I,IAAM,QAASoG,EAAiB,GAAGA,EAAepG,QAAU,IACxEmG,EAAMjP,MAAMuM,MAAQ,UAAW2C,EAAiB,GAAGA,EAAe3C,UAAY,IAC9E0C,EAAMjP,MAAM6M,OAAS,WAAYqC,EAAiB,GAAGA,EAAerC,WAAa,IACjFoC,EAAMjP,MAAMwK,WAAa,eAAgB0E,EAAiB,GAAGA,EAAe1E,eAAiB,IAC7FyE,EAAMjP,MAAMyK,UAAY,cAAeyE,EAAiB,GAAGA,EAAezE,cAAgB,IAC1FwE,EAAMjP,MAAMuI,MAAQ,GAAG2G,EAAe3G,UACtC0G,EAAMjP,MAAMsI,OAAS,GAAG4G,EAAe5G,WACvC2G,EAAMjP,MAAMyP,SAAW1I,EAAO/G,MAAMyP,SACpCR,EAAMjP,MAAM0P,OAAS3I,EAAO/G,MAAM0P,OAClCT,EAAMjP,MAAM2P,gBAAkB7I,EAAM8I,YAAc,QAAU,WAEvDX,EAAM5H,cAAe,CACtB,MAAM8H,EAAWC,SAASC,gBAAkB1L,EAC5CA,EAAQ4D,YAAY0H,GAChBE,GACAF,EAAMK,MAAM,CAAEC,eAAe,GACrC,CACJ,CAiDIM,CAAYvQ,GA/ChB,SAAsBA,GAClB,MAAMqE,EAAUrE,EAAQqE,QAClBmD,EAAQxH,EAAQwH,MAElBA,EAAMgJ,iBAAmBhJ,EAAMiJ,aAC/BpM,EAAQ3D,MAAMgQ,OAAS,cAClBlJ,EAAMgJ,gBACXnM,EAAQ3D,MAAMgQ,OAAS,aAClBlJ,EAAMiJ,aACXpM,EAAQ3D,MAAMgQ,OAAS,aAEvBrM,EAAQ3D,MAAMgQ,OAAS,SAC/B,CAoCIC,CAAa3Q,GAlCjB,SAAuBA,GACnB,MAAMqE,EAAUrE,EAAQqE,QAClBuM,EAAU5Q,EAAQ4Q,QAClBC,EAAU7Q,EAAQwH,MAAMoJ,QACxBE,EAAY9Q,EAAQwH,MAAMuJ,iBAE3BD,GAMLF,EAAQI,UAAYH,EACpBD,EAAQlQ,MAAM6I,KAAO,GAAGuH,EAAUvH,SAClCqH,EAAQlQ,MAAM8I,IAAM,GAAGsH,EAAUtH,QAE5BoH,EAAQ7I,gBACT1D,EAAQ4D,YAAY2I,GACpBA,EAAQK,gBAXJL,EAAQ7I,eACR6I,EAAQ7I,cAAcC,YAAY4I,EAY9C,CAeIM,CAAclR,EAClB,CA+BYmR,CAAenR,EACnB,CACA,MAAO0P,GACH1P,EAAQ0P,MAAQA,CACpB,CAGA1P,EAAQ0P,OApChB,SAAqB1P,GACjB,GAAIA,EAAQoR,cACR,OAEJpR,EAAQoR,eAAgB,EAExB,MAAM/M,EAAUrE,EAAQqE,QAClBqL,EAAQ1P,EAAQ0P,MAEtBrL,EAAQ3D,MAAM2P,gBAAkB,UAChChM,EAAQ3D,MAAM6N,MAAQ,QACtBlK,EAAQ3D,MAAMC,QAAU,OACxB0D,EAAQ3D,MAAM2Q,QAAU,OACxBhN,EAAQ3D,MAAM4Q,cAAgB,SAC9BjN,EAAQ3D,MAAM6Q,WAAa,OAC3BlN,EAAQ2M,UAAY,0OAKVtB,EAAM8B,yFAE2C9B,EAAM+B,mBAErE,CAaQC,CAAY1R,EACpB,C,kBClbA,MAAM2R,EAAa,CACfhS,MAAO,EAAGiS,cAAeA,GAAY,GACrCnR,KAAM,EAAGmR,cAAeA,GAAY,YACpC/Q,KAAM,CACFE,SAAU,KAAM,EAChBC,MAAO,EAAG6Q,YAAaA,EACvB5Q,YAAY,IAIL,SAAS6Q,EAAkBhS,EAAYyB,EAAcwQ,GAChE,MAAO,CACH,CACI3R,OAAQ,CAAEgG,KAAM,QAChB/F,IAAK,CAAE+F,KAAM,UACbzG,MAAO,EAAGS,iBAA+B4R,IAAlB5R,EAAO6R,OAAuB7R,EAAOwE,GAAKxE,EAAO6R,QAE5E,CACI7R,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,QACbzG,MAAO,EAAGU,cAAyB2R,IAAf3R,EAAI4R,OAAuB5R,EAAIuE,GAAKvE,EAAI4R,QAEhE,CACI7R,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,WACbzG,MAAO,IAEX,CACIS,OAAQ,CAAEgG,KAAM,WAChB/F,IAAK,CAAE+F,KAAM,UACbzG,MAAO,IAEX,CACIS,OAAQ,CAAEgG,KAAM,QAChB/F,IAAK,CAAE+F,KAAM,aACVuL,GAEP,CACIvR,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,WACVuL,GAEP,CACIvR,OAAQ,CAAEgG,KAAM,QAChB/F,IAAK,CAAE+F,KAAM,QACbzG,MAAO4B,MAERzB,KAEAiS,EAAO9R,KAAI,EAAGyG,WAAUE,QAAOsL,aAAavI,KAAU,CACrDvJ,OAAQ,CAAEwE,GAAI8B,GACdrG,IAAK,CAAEuE,GAAIgC,GACXnG,KAAM,EAAGd,QAAOc,UAAW,GAAGsR,EAAOjK,OAAS,EAAI6B,EAAQ,EAAI,KAAmB,QAAduI,EAAsB,IAAM,OAAOzR,GAAQd,QAG1H,CCvDA,MAAMwS,EAAe,CAAC,SAAU,MAAO,aAWvC,SAASC,EAAUlS,GAIf,OAHgB4F,OAAOC,KAAK7F,GAAM4H,OACfhC,OAAOC,KAAK7F,GAAM8G,QAAOvB,GAAO0M,EAAaE,SAAS5M,KAAMqC,MAGnF,CAEe,SAASwK,EAAqBxS,EAAYyS,GACrD,MAAMC,EAAiB,IAAIL,KAAiBI,GAE5C,OAAOzS,EAAWG,KAAIC,GAnB1B,SAAgBA,EAAMqS,GAClB,MAAME,EAAc,CAAC,EACrB,IAAK,MAAMC,KAASH,EACZG,KAASxS,IACTuS,EAAYC,GAASxS,EAAKwS,IAElC,OAAOD,CACX,CAYkCtJ,CAAOjJ,EAAMsS,KAAiBxL,OAAOoL,EACvE,CCpBe,SAASO,EAAmB7S,GACvC,OAAOwS,EAAqBxS,EAAY,CAAC,QAAS,OAAQ,QAC9D,CCFA,SAAS8S,EAAkBC,EAAWC,GAClC,OAAIA,EACOD,EAAY,KAEZA,EAAY,IAC3B,CAEe,SAASE,EAAoBjT,EAAYkT,EAAajO,EAAakO,EAAW3G,EAAW4G,EAASnB,EAAQvB,EAAiBC,EAAc3L,GACpJ,MAAMqO,EAAmBpO,EAAcS,EAAYT,EAAY2B,UAAY,KACrE0M,EAAgBrO,EAAcS,EAAYT,EAAY6B,OAAS,KAE/DyM,EAAiC,OAAjB5C,EAChB6C,EAFuC,OAApB9C,GAEc6C,EACjCE,EAAuBzO,EAAc,EACrC0O,EAAuB1O,EAAc,EAErC2O,EAAa,CAAC1R,EAAMD,EAASiJ,EAAUC,KACzC,GAAID,EAAW,GAAKA,GAAYhJ,EAAK+F,OACjC,OAAO,EACX,GAAIkD,EAAc,GAAKA,GAAelJ,EAAQgG,OAC1C,OAAO,EAEX,MAAMnB,EAAS5E,EAAKgJ,GAAUtF,IACxBgB,EAAY3E,EAAQkJ,GAAavF,IAEvC,OAAOwN,EAAUS,cAAc/M,EAAQF,EAAU,EAG/CkN,EAAW,CAACrT,EAAWI,IACrBJ,EACO,CAACI,GAED,GAGf,MAAO,CACH,CACIN,OAAQ,CAAEgG,KAAM,QAChB/F,IAAK,CAAE+F,KAAM,UACb1F,MAAO,EAAGkR,eAAe,CAAGvF,WAAY,UAAWM,WAAYiF,EAAW,QAAU,UAAWgC,OAAQ,CAAE3K,MAAO,EAAGsF,MAAO,WAE9H,CACInO,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,QACb1F,MAAO,EAAGkR,eAAe,CAAGvF,WAAY,UAAWM,WAAYiF,EAAW,QAAU,UAAWgC,OAAQ,CAAE3K,MAAO,EAAGsF,MAAO,WAE9H,CACInO,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAE+F,KAAM,UACb1F,MAAO,CAAE2L,WAAY,UAAWuH,OAAQ,CAAE3K,MAAOnE,EAAayJ,MAAO,UAEzE,CACInO,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,OACb1F,MAAO,CAAE2L,WAAY,UAAWuH,OAAQ,CAAE3K,MAAOnE,EAAayJ,MAAO,UAEzE,CACInO,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAE+F,KAAM,UACb1F,MAAO,CAAE2L,WAAY,eAEtBvM,KAOA6T,EAASX,IAAgBK,EAAe,CACvCjT,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAEuE,GAAIoO,GAAapM,OACxBlG,MAAO,CAAE4L,UAAW,kBAErBqH,EAASX,IAAgBM,EAAY,CACpClT,OAAQ,CAAEwE,GAAIoO,GAAatM,UAC3BrG,IAAK,CAAEuE,GAAIoO,GAAapM,OACxBlG,MAAO,CAAE4L,UAAW,eAExB,CACIlM,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAE+F,KAAM,OACb9F,UAAW,EAAGyB,OAAMD,UAASzB,MAAKD,YAAaqT,EAAW1R,EAAMD,EAASzB,EAAIsJ,MAAOvJ,EAAOuJ,OAC3FjJ,MAAO,EAAGqB,OAAMD,UAASzB,MAAKD,SAAQS,WAAW,IACxC4S,EAAW1R,EAAMD,EAASzB,EAAIsJ,MAAQ,EAAGvJ,EAAOuJ,OAA4G,CAAC,EAApG,CAAEwF,UAAW,CAAElG,MAAOsK,EAAsBhF,MAAO,UAAW5E,MAAOkK,OAAOC,sBACrIL,EAAW1R,EAAMD,EAASzB,EAAIsJ,MAAQ,EAAGvJ,EAAOuJ,OAA+G,CAAC,EAAvG,CAAEuF,aAAc,CAAEjG,MAAOsK,EAAsBhF,MAAO,UAAW5E,MAAOkK,OAAOC,sBACxIL,EAAW1R,EAAMD,EAASzB,EAAIsJ,MAAOvJ,EAAOuJ,MAAQ,GAAyG,CAAC,EAArG,CAAE6F,WAAY,CAAEvG,MAAOsK,EAAsBhF,MAAO,UAAW5E,MAAOkK,OAAOC,sBACtIL,EAAW1R,EAAMD,EAASzB,EAAIsJ,MAAOvJ,EAAOuJ,MAAQ,GAA0G,CAAC,EAAtG,CAAE4F,YAAa,CAAEtG,MAAOsK,EAAsBhF,MAAO,UAAW5E,MAAOkK,OAAOC,mBAC5IxH,UAAWsG,EAAkB/R,EAAO,UAAY,UAAWsS,IAAqB/S,EAAOqF,KAAO2N,IAAkB/S,EAAIoF,QAG5H,CACIrF,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAE+F,KAAM,OACb9F,UAAW,EAAGD,MAAKD,YAAakM,EAAUoH,cAAcrT,EAAIoF,IAAKrF,EAAOqF,KACxE/E,MAAO,EAAGL,MAAKD,aAAa,CACxBkM,UAAWsG,EAAkB,UAAWO,IAAqB/S,EAAOqF,KAAO2N,IAAkB/S,EAAIoF,WAGtGkO,EAAS5O,EAAa,CACrB3E,OAAQ,CAAEwE,GAAIG,GAAa2B,UAC3BrG,IAAK,CAAEuE,GAAIG,GAAa6B,OACxBlG,MAAO,CAAE4L,UAAW,kBAErByF,EAAO9R,KAAI,EAAGyG,WAAUE,QAAOsL,aAAavI,KAAU,CACrDvJ,OAAQ,CAAEwE,GAAI8B,GACdrG,IAAK,CAAEuE,GAAIgC,GACXlG,MAAO,CAAE4L,UAAW,iBAExB,CACIlM,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAE+F,KAAM,OACb9F,UAAW,EAAGO,UAAWA,EACzBH,MAAO,CAAE6L,OAAQ,cAErB,CACInM,OAAQ,CAAEgG,KAAM,OAChB/F,IAAK,CAAE+F,KAAM,OACb9F,UAAW,EAAGD,MAAKD,YAAa8S,EAAQa,cAAc1T,EAAIoF,IAAKrF,EAAOqF,KACtE/E,MAAO,CAAE6L,OAAQ,iBAElBoH,EAASnD,EAAiB,CACzBpQ,OAAQ,CAAEwE,GAAI4L,GACdnQ,IAAK,CAAE+F,KAAM,UACb1F,MAAO,CAAE6O,YAAa,CAAEtG,MAAOuK,EAAsBjF,MAAO,wBAE7DoF,EAASlD,EAAc,CACtBrQ,OAAQ,CAAEgG,KAAM,UAChB/F,IAAK,CAAEuE,GAAI6L,GACX/P,MAAO,CAAEwO,aAAc,CAAEjG,MAAOuK,EAAsBjF,MAAO,qBAGzE,CCrIe,SAASyF,EAAYlS,EAASC,GACzC,MAAMkS,EAAYlS,EAAKiF,QAAO3G,GAAsB,UAAfA,EAAI6T,SAAoBpM,OACvDqM,EAAepS,EAAKiF,QAAO3G,GAAsB,QAAfA,EAAI6T,SAAkBpM,OACxDsM,EAAerS,EAAK+F,OAASmM,EAAYE,EACzCE,EAAavS,EAAQkF,QAAO5G,GAA4B,UAAlBA,EAAO8T,SAAoBpM,OACjEwM,EAAcxS,EAAQkF,QAAO5G,GAA4B,QAAlBA,EAAO8T,SAAkBpM,OAChEyM,EAAezS,EAAQgG,OAASuM,EAAaC,EAE7CE,EAAUzS,EAAKiI,MAAM,EAAGiK,GACxBQ,EAAa1S,EAAKiI,MAAMjI,EAAK+F,OAASqM,EAAcpS,EAAK+F,QACzD4M,EAAa3S,EAAKiI,MAAMiK,EAAWlS,EAAK+F,OAASqM,GACjDQ,EAAc7S,EAAQkI,MAAM,EAAGqK,GAC/BO,EAAe9S,EAAQkI,MAAMlI,EAAQgG,OAASwM,EAAaxS,EAAQgG,QACnE+M,EAAgB/S,EAAQkI,MAAMqK,EAAYvS,EAAQgG,OAASwM,GAE3DQ,EAAab,EAAY,EAGzBc,EAAiBV,EAAa,EAM9BW,EAPgBZ,EAAe,IAOSU,EAExCG,GAAuBH,EACvBI,IAXgBf,EAAe,GAc/BgB,EAVmBZ,EAAe,IAUSQ,EAE3CK,GAAwBL,EACxBM,IAdkBf,EAAc,GAgBhCgB,EAAY,CAACvT,EAAM0G,EAAeC,KACpC,GAAoB,IAAhB3G,EAAK+F,OACL,OAAO,EAEX,MAAM0B,EAAMf,EAAgB1G,EAAKwT,GAAG,GAAGC,cAAgBzT,EAAKwT,GAAG,GAAG/L,IAGlE,OAFed,EAAmB3G,EAAKwT,IAAI,GAAGE,iBAAmB1T,EAAKwT,IAAI,GAAGhI,QAE7D/D,CAAG,EAGjBkM,EAAW,CAAC5T,EAAS6G,EAAgBC,KACvC,GAAuB,IAAnB9G,EAAQgG,OACR,OAAO,EAEX,MAAMyB,EAAOZ,EAAiB7G,EAAQyT,GAAG,GAAGI,eAAiB7T,EAAQyT,GAAG,GAAGhM,KAG3E,OAFcX,EAAkB9G,EAAQyT,IAAI,GAAGK,gBAAkB9T,EAAQyT,IAAI,GAAGtI,OAEjE1D,CAAI,EAUvB,MAAO,CACHC,IAAK,CACDzH,KAAMyS,EACN/L,eA3CiB,EA4CjBC,kBA3CoB,EA4CpBM,OAZUsM,EAAUd,GAjCH,GACG,IA8CxBjH,OAAQ,CACJxL,KAAM0S,EACNhM,cAAeuM,EACftM,kBA/CuB,EAgDvBM,OAjBasM,EAAUb,EAAYO,GA/BZ,IAkD3B5H,OAAQ,CACJrL,KAAM2S,EACNjM,cAAewM,EACfvM,iBAAkBwM,EAClBlM,OAtBasM,EAAUZ,EAAYO,EAAqBC,IAwB5D3L,KAAM,CACFzH,QAAS6S,EACThM,gBAvDmB,EAwDnBC,iBAvDoB,EAwDpBK,MA3BUyM,EAASf,GA9BA,GACC,IA0DxB1H,MAAO,CACHnL,QAAS8S,EACTjM,eAAgBwM,EAChBvM,iBA3DqB,EA4DrBK,MAhCWyM,EAASd,EAAcO,GA5Bb,IA8DzBU,OAAQ,CACJ/T,QAAS+S,EACTlM,eAAgByM,EAChBxM,gBAAiByM,EACjBpM,MArCYyM,EAASb,EAAeO,EAAsBC,IAwCtE,CCnGe,SAASS,EAAyBpT,EAAaD,GAC1D,MAAO,IAAIC,KAAgBD,EAAQxC,KAAI+G,IAAU,CAAGN,SAAUM,EAAON,SAAUE,MAAOI,EAAOJ,MAAOjH,MAAOqH,EAAO+O,eACtH,CCAe,MAAMC,EACjB,WAAAC,CAAYvT,GACRwT,KAAKC,OAAS,IAAIC,IAElB1T,EAAY2T,SAAQhT,IAChB,MAAMsD,EAASnB,EAAYnC,EAAKuD,OAC1BH,EAAYjB,EAAYnC,EAAKqD,UAE9BwP,KAAKC,OAAOtP,IAAIF,IACjBuP,KAAKC,OAAOG,IAAI3P,EAAQ,IAAIyP,KAEhCF,KAAKC,OAAOrP,IAAIH,GAAQ2P,IAAI7P,EAAWpD,EAAK1D,MAAM,GAE1D,CAEA,aAAAoU,CAAcpN,EAAQF,GAClB,OAAOyP,KAAKC,OAAOtP,IAAIF,IAAWuP,KAAKC,OAAOrP,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,aAAA8P,CAAc5P,EAAQF,GAClB,GAAKyP,KAAKnC,cAAcpN,EAAQF,GAGhC,OAAOyP,KAAKC,OAAOrP,IAAIH,GAAQG,IAAIL,EACvC,CAEA,YAAA+P,CAAa5P,EAAOF,GAChB,OAAOwP,KAAKnC,cAAcvO,EAAYoB,GAAQpB,EAAYkB,GAC9D,CAEA,YAAA+P,CAAa7P,EAAOF,GAChB,OAAOwP,KAAKK,cAAc/Q,EAAYoB,GAAQpB,EAAYkB,GAC9D,EChCW,SAASgQ,EAAWC,GAC/B,OAAO,IAAIX,EAAQW,EACvB,CCHe,MAAMC,EACjB,WAAAX,CAAYrT,GACRsT,KAAKC,OAAS,IAAIC,IAElBxT,EAAcyT,SAAQhT,IAClB,MAAMsD,EAASnB,EAAYnC,EAAKuD,OAC1BH,EAAYjB,EAAYnC,EAAKqD,UAE9BwP,KAAKC,OAAOtP,IAAIF,IACjBuP,KAAKC,OAAOG,IAAI3P,EAAQ,IAAIkQ,KAEhCX,KAAKC,OAAOrP,IAAIH,GAAQmQ,IAAIrQ,EAAU,GAE9C,CAEA,aAAAiN,CAAc/M,EAAQF,GAClB,OAAOyP,KAAKC,OAAOtP,IAAIF,IAAWuP,KAAKC,OAAOrP,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,YAAAsQ,CAAanQ,EAAOF,GAChB,OAAOwP,KAAKxC,cAAclO,EAAYoB,GAAQpB,EAAYkB,GAC9D,ECrBW,SAASsQ,EAAapU,GACjC,OAAO,IAAIgU,EAAUhU,EACzB,CCJe,SAASqU,EAAWC,EAAerV,GAC9C,MAAgC,mBAAlBqV,EACRA,EAAcrV,GACdqV,CACV,CCHe,SAASC,EAAUxN,EAAO7B,EAAQsP,EAAaC,GAC1D,OAAI1N,EAAQyN,EACD,QACPzN,GAAS7B,EAASuP,EACX,WADX,CAGJ,CCJA,SAASC,EAAYC,EAAUH,EAAaC,GACxC,OAAOE,EAAStX,KAAI,CAACoE,EAASsF,KAC1B,MAAM/E,EAAK,OAAQP,EAAUA,EAAQO,GAAKP,EAAQ+B,KAClD,MAAO,IACA/B,EACHO,GAAIA,EACJwB,KAAM/B,EAAQ+B,MAAQ,OACtBuD,MAAOA,EACPlE,IAAKD,EAAYZ,GACjBsP,OAAQiD,EAAUxN,EAAO4N,EAASzP,OAAQsP,EAAaC,GACvDpF,OAAQ,WAAY5N,EAAUA,EAAQ4N,OAASrN,EAC/C4S,OAAQnT,EAAQmT,QAAU,GAC7B,GAET,CAEO,SAASC,EAAmB3V,EAASsV,EAAaC,EAAWnS,GAChE,MAAMwS,EAAe,IAAItB,IAAIlR,EAAajF,KAAI,EAAGyG,WAAUuC,WAAY,CAACzD,EAAYkB,GAAWuC,MAG/F,OAFwBqO,EAAYxV,EAASsV,EAAaC,GAEnCpX,KAAIG,IAAU,IAC9BA,EACH6I,MAAOyO,EAAa7Q,IAAIzG,EAAOqF,KACzBiS,EAAa5Q,IAAI1G,EAAOqF,KACxB,UAAWrF,EACPA,EAAO6I,MACP,SAElB,CAEO,SAAS0O,EAAgB5V,EAAMqV,EAAaC,EAAWlS,GAC1D,MAAMyS,EAAgB,IAAIxB,IAAIjR,EAAWlF,KAAI,EAAG2G,QAAOoC,YAAa,CAACxD,EAAYoB,GAAQoC,MAGzF,OAFqBsO,EAAYvV,EAAMqV,EAAaC,GAEhCpX,KAAII,IAAO,IACxBA,EACH2I,OAAQ4O,EAAc/Q,IAAIxG,EAAIoF,KACxBmS,EAAc9Q,IAAIzG,EAAIoF,KACtB,WAAYpF,EACRA,EAAI2I,OACJ,SAElB,CC3CO,SAAS6O,EAAiB/V,EAASoF,EAAkBpC,GACxD,IAAIyE,EAAOzE,EAEX,OAAOhD,EAAQ7B,KAAI,CAACG,EAAQuJ,KACxB,MACMV,EAAQhC,EADQ,UAAW7G,EAASA,EAAO6I,MAAQ,IACd/B,GACrC4Q,EAAY,IACX1X,EACHuJ,MAAOA,EACPV,MAAOA,EACP0M,eAAgBpM,EAAOzE,EACvByE,KAAMA,EACN0D,MAAO1D,EAAON,EACd2M,gBAAiBrM,EAAON,EAAQnE,GAKpC,OAFAyE,GAAQuO,EAAU7O,MAAQnE,EAEnBgT,CAAS,GAExB,CAEO,SAASC,EAAchW,EAAMmF,EAAkBpC,GAClD,IAAI0E,EAAM1E,EAEV,OAAO/C,EAAK9B,KAAI,CAACI,EAAKsJ,KAClB,MACMX,EAAS/B,EADQ,WAAY5G,EAAMA,EAAI2I,OAAS,GACT9B,GACvC8Q,EAAS,IACR3X,EACHsJ,MAAOA,EACPX,OAAQA,EACRwM,cAAehM,EAAM1E,EACrB0E,IAAKA,EACL+D,OAAQ/D,EAAMR,EACdyM,iBAAkBjM,EAAMR,EAASlE,GAKrC,OAFA0E,GAAOwO,EAAOhP,OAASlE,EAEhBkT,CAAM,GAErB,CC5CA,MAAMC,EAAc,eACdC,EAAiB,CAAE1O,IAAK,EAAGyD,MAAO,EAAGM,OAAQ,EAAGhE,KAAM,GCCtD4O,EAAc,CAChB,OAAU,CAAC,UACX,OAAU,CAAC,UACX,KAAQ,CAAC,QACT,OAAU,CAAC,UACX,IAAO,CAAC,SAAU,OAAQ,SAAU,UACpC,QAAW,CAAC,SAAU,SAAU,UAChCnG,UAAW,IAGf,MAAMoG,EACFC,MAAQ,IAAIjC,IACZkC,QAAU,IAAIlC,IACdmC,QAAU,IAAInC,IACdoC,OAAS,IAAIpC,IAGF,MAAMqC,EACjBtC,OAAS,IAAIiC,EACbM,UAAW,EAEX,OAAAC,CAAQvY,EAAQC,EAAKH,GAGjB,GAFAgW,KAAKwC,UAAW,EAEZhT,MAAMC,QAAQvF,GACd,IAAK,MAAMwY,KAAKxY,EACZ8V,KAAKyC,QAAQC,EAAGvY,EAAKH,QAI7B,GAAIwF,MAAMC,QAAQtF,GACd,IAAK,MAAMwY,KAAKxY,EACZ6V,KAAKyC,QAAQvY,EAAQyY,EAAG3Y,OAFhC,CAMAE,EAASA,EACH,OAAQA,EACJ,CAAEqF,IAAKD,EAAYpF,EAAOwE,KAC1BxE,EACJ,CAAEgG,KAAM,QACd/F,EAAMA,EACA,OAAQA,EACJ,CAAEoF,IAAKD,EAAYnF,EAAIuE,KACvBvE,EACJ,CAAE+F,KAAM,QAuBV,QAAShG,GACT0Y,EAAc5C,KAAKC,OAAOkC,MAAOjY,EAAOqF,KACxC,UAAWrF,GACX0Y,EAAc5C,KAAKC,OAAOmC,QAASlY,EAAOuJ,OAC1C,UAAWvJ,GACX0Y,EAAc5C,KAAKC,OAAOoC,QAASnY,EAAO2Y,OAC9C,IAAK,MAAM3S,KAAQ+R,EAAY/X,EAAOgG,MAClC0S,EAAc5C,KAAKC,OAAOqC,OAAQpS,EAzCtC,CAaA,SAAS4S,EAAW7C,EAAQ1Q,GACnB0Q,EAAOtP,IAAIpB,IACZ0Q,EAAOG,IAAI7Q,EAAK,IAEpB0Q,EAAOrP,IAAIrB,GAAKoE,KAAK3J,EACzB,CAEA,SAAS4Y,EAAc3C,EAAQ1Q,GACtB0Q,EAAOtP,IAAIpB,IACZ0Q,EAAOG,IAAI7Q,EAAK,IAAI2S,GAEpB,QAAS/X,GACT2Y,EAAW7C,EAAOrP,IAAIrB,GAAK4S,MAAOhY,EAAIoF,KACtC,UAAWpF,GACX2Y,EAAW7C,EAAOrP,IAAIrB,GAAK6S,QAASjY,EAAIsJ,OACxC,UAAWtJ,GACX2Y,EAAW7C,EAAOrP,IAAIrB,GAAK8S,QAASlY,EAAI0Y,OAC5C,IAAK,MAAM3S,KAAQ+R,EAAY9X,EAAI+F,MAC/B4S,EAAW7C,EAAOrP,IAAIrB,GAAK+S,OAAQpS,EAC3C,CAUJ,CAEA,QAAA6S,CAAS7Y,EAAQC,GACb,MAAM6Y,EAAQ,GAEd,IAAKhD,KAAKwC,SACN,OAAOQ,EAEX,SAASC,EAAYC,GACjB,IAAK,MAAMlZ,KAAQkZ,EACfF,EAAMrP,KAAK3J,EACnB,CAEA,SAASmZ,EAAelD,GAChBA,EAAOkC,MAAMxR,IAAIxG,EAAIoF,MACrB0T,EAAYhD,EAAOkC,MAAMvR,IAAIzG,EAAIoF,MACjC0Q,EAAOmC,QAAQzR,IAAIxG,EAAIsJ,QACvBwP,EAAYhD,EAAOmC,QAAQxR,IAAIzG,EAAIsJ,QACnCwM,EAAOqC,OAAO3R,IAAIxG,EAAI+F,OACtB+S,EAAYhD,EAAOqC,OAAO1R,IAAIzG,EAAI+F,OACtC,IAAK,MAAM2S,KAAS1Y,EAAImX,OAChBrB,EAAOoC,QAAQ1R,IAAIkS,IACnBI,EAAYhD,EAAOoC,QAAQzR,IAAIiS,GAE3C,CAEI7C,KAAKC,OAAOkC,MAAMxR,IAAIzG,EAAOqF,MAC7B4T,EAAenD,KAAKC,OAAOkC,MAAMvR,IAAI1G,EAAOqF,MAC5CyQ,KAAKC,OAAOmC,QAAQzR,IAAIzG,EAAOuJ,QAC/B0P,EAAenD,KAAKC,OAAOmC,QAAQxR,IAAI1G,EAAOuJ,QAC9CuM,KAAKC,OAAOqC,OAAO3R,IAAIzG,EAAOgG,OAC9BiT,EAAenD,KAAKC,OAAOqC,OAAO1R,IAAI1G,EAAOgG,OACjD,IAAK,MAAM2S,KAAS3Y,EAAOoX,OACnBtB,KAAKC,OAAOoC,QAAQ1R,IAAIkS,IACxBM,EAAenD,KAAKC,OAAOoC,QAAQzR,IAAIiS,IAG/C,OAAOG,CACX,ECjHJ,MAAMI,EAAc,CAAC,YAAa,cAAe,eAAgB,cAE3DC,EAAc,CAAExY,SAAU,KAAM,EAAMC,MAAO,EAAG6Q,YAAaA,GAGnE,SAAS2H,EAAa9Y,EAAOiJ,GACzB,MAAM8P,EAAW,IAAK/Y,GAEtB,GAAI,WAAY+Y,EAAU,CACtB,IAAK,MAAMC,KAAcJ,EACrBG,EAASC,GAAcD,EAAS7F,cAC7B6F,EAAS7F,MACpB,CAEA,IAAK,MAAM8F,KAAcJ,EACjBI,KAAcD,IACdA,EAASC,GAAc,IAAKD,EAASC,GAAa/P,UAE1D,OAAO8P,CACX,CAYA,SAASE,EAAQzZ,EAAMF,GACnB,IAAkB,IAAdE,EAAKW,KAET,OAAkB,IAAdX,EAAKW,KACE,SAAUb,EAAUA,EAAQa,KAAO0Y,EAC1C,SAAUvZ,EACH,IAAKA,EAAQa,QAASX,EAAKW,MAC/B,IAAK0Y,KAAgBrZ,EAAKW,KACrC,CAMe,MAAM+Y,EACjB,WAAA3D,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAO9O,EAAOzJ,KAASgZ,EAAMY,UAAW,CACzC,MAAMC,EAAQ,CAAEpQ,SAGZ,cAAezJ,IACf6Z,EAAMzZ,UAAYJ,EAAKI,WACvB,UAAWJ,IACX6Z,EAAMrZ,MAA8B,mBAAfR,EAAKQ,MAAuBR,EAAKQ,MAAQ,IAAMR,EAAKQ,OACzE,UAAWR,IACX6Z,EAAMpa,MAA8B,mBAAfO,EAAKP,MAAuBO,EAAKP,MAAQ,IAAMO,EAAKP,OACzE,SAAUO,IACV6Z,EAAMtZ,KAA4B,mBAAdP,EAAKO,KAAsBP,EAAKO,KAAO,IAAMP,EAAKO,MACtE,SAAUP,IACV6Z,EAAMnN,KAA4B,mBAAd1M,EAAK0M,KAAsB1M,EAAK0M,KAAO,IAAM1M,EAAK0M,MACtE,YAAa1M,IACb6Z,EAAMpZ,QAAkC,mBAAjBT,EAAKS,QAAyBT,EAAKS,QAAU,IAAMT,EAAKS,SAC/E,SAAUT,IACV6Z,EAAMlZ,KAAOX,EAAKW,MAClB,YAAaX,IACb6Z,EAAMnJ,QAAkC,mBAAjB1Q,EAAK0Q,QAAyB1Q,EAAK0Q,QAAU,IAAM1Q,EAAK0Q,SAC/E,SAAU1Q,IACV6Z,EAAMnZ,KAAOV,EAAKU,MAEtBsV,KAAK2D,YAAYlB,QAAQzY,EAAKE,OAAQF,EAAKG,IAAK0Z,EACpD,CACJ,CAEA,OAAAhT,CAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQ8S,GACtC,MAAMgG,EAAQhD,KAAK2D,YACdZ,SAAS7Y,EAAQC,GACjB2F,MAAK,CAACoD,EAAGC,IAAMD,EAAEO,MAAQN,EAAEM,QAC3B3C,QAAO,CAACrH,EAAOgK,EAAOqQ,IAAUra,EAAMgK,QAAUqQ,EAAMrQ,EAAQ,IAAIA,QAEvE,IAEI/I,EAIAgQ,EANA5Q,EAAU,CAAE6B,OAAME,OAAMD,UAASzB,MAAKD,UACtCM,EAAQ,CAAC,EAGTC,EAAUuX,EACVtL,EAAOqL,EAGP/E,EAAQa,cAAc1T,EAAIoF,IAAKrF,EAAOqF,OACtCzF,EAAU,IAAKA,EAAS4R,SAAUsB,EAAQqD,cAAclW,EAAIoF,IAAKrF,EAAOqF,OAE5E,IAAK,MAAMvF,KAAQgZ,EACf,MAAI,cAAehZ,IAASA,EAAKI,UAAUN,MAIvC,UAAWE,IACXF,EAAU,IAAKA,EAASL,MAAOO,EAAKP,MAAMK,KAC1C,UAAWE,IACXQ,EAAQ,IAAKA,KAAU8Y,EAAatZ,EAAKQ,MAAMV,GAAUE,EAAKyJ,SAC9D,SAAUzJ,IACVF,EAAU,IAAKA,EAASS,KAAMP,EAAKO,KAAKT,KACxC,SAAUE,IACV0M,EAAO1M,EAAK0M,KAAK5M,IACjB,YAAaE,IACbS,EAAU,IAAKA,KAAYT,EAAKS,QAAQX,KACxC,SAAUE,IACVF,EAAU,IAAKA,EAASa,KAAM8Y,EAAQzZ,EAAMF,KAC5C,YAAaE,IACb0Q,EAAU1Q,EAAK0Q,QAAQ5Q,IACvB,SAAUE,GAAM,CAChB,MAAM+Z,EAAiBja,EACvBY,EAAQsH,GAAQhI,EAAKU,KAAK,IAAKqZ,EAAgB/R,OACnD,CAKJ,MAAMzH,EAnGd,SAAiBT,GACb,MAAI,SAAUA,EACH,GAAGA,EAAQS,OAClB,aAAcT,EACP,GAAGA,EAAQ4R,gBACAI,IAAlBhS,EAAQL,MACD,GAAGK,EAAQL,QACf,EACX,CA2FqBua,CAAQla,GACfma,EAAS,CACXzZ,QACA0Z,SAtCU,EAuCV3Z,OACAE,UACAiM,QAYJ,MATI,UAAW5M,IACXma,EAAOxa,MAAQK,EAAQL,OACvB,SAAUK,QAA4BgS,IAAjBhS,EAAQa,OAC7BsZ,EAAOtZ,KAAOb,EAAQa,WACVmR,IAAZpB,IACAuJ,EAAOvJ,QAAUA,QACRoB,IAATpR,IACAuZ,EAAOvZ,KAAOA,GAEXuZ,CACX,EC5IW,SAASE,EAAmBva,GACvC,OAAO,IAAI8Z,EAAgB9Z,EAC/B,CCJe,MAAMwa,EACjB,WAAArE,CAAYsE,EAAiB1Y,EAAME,EAAMD,EAASoR,GAC9CgD,KAAKqE,gBAAkBA,EACvBrE,KAAKrU,KAAOA,EACZqU,KAAKnU,KAAOA,EACZmU,KAAKpU,QAAUA,EACfoU,KAAKhD,QAAUA,CACnB,CAEA,OAAAnM,CAAQ1G,EAAKD,GACT,OAAO8V,KAAKqE,gBAAgBxT,QACxBmP,KAAKrU,KACLqU,KAAKnU,KACLmU,KAAKpU,QACLzB,EACAD,EACA8V,KAAKhD,QACb,ECfW,SAASsH,EAAkBD,EAAiB1Y,EAAME,EAAMD,EAASoR,GAC5E,OAAO,IAAIoH,EAAeC,EAAiB1Y,EAAME,EAAMD,EAASoR,EACpE,CCFA,SAASuH,EAAgBhY,EAASiY,EAAYC,GAC1C,MAAMC,EAAe,IAAIxE,IACzB,IAAK,MAAM/S,KAAQZ,EAAS,CACxB,MAAMoY,EAAUrV,EAAYnC,EAAKqX,IAC3BI,EAAYtV,EAAYnC,EAAKsX,IAE9BC,EAAa/T,IAAIgU,IAClBD,EAAatE,IAAIuE,EAAS,IAAIzE,KAElCwE,EAAa9T,IAAI+T,GAASvE,IAAIwE,EAAWzX,EAAK0S,WAClD,CACA,OAAO6E,CACX,CAEO,SAASG,EAAgBtY,EAASuY,EAAgBT,EAAiB1Y,EAAME,EAAMD,EAASoR,GAC3F,GAAuB,IAAnBzQ,EAAQqF,OACR,OAAO/F,EAEX,MAAM6Y,EAAeH,EAAgBhY,EAAS,WAAY,SACpDwY,EAAkBnZ,EAAQkF,QAAO5G,GAA0B,WAAhBA,EAAOgG,MAAqBwU,EAAa/T,IAAIzG,EAAOqF,OAErG,OAA+B,IAA3BwV,EAAgBnT,OACT/F,EAEJA,EAAKiF,QAAO3G,IACf,IAAK,MAAMD,KAAU6a,EAAiB,CAClC,MAAM5X,EAAOkX,EAAgBxT,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQ8S,GACjEgI,EAAgBN,EAAa9T,IAAI1G,EAAOqF,KAG9C,IAFgBuV,EAAejU,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQiD,EAAK1D,MAAO0D,EAAK5C,KAAMya,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CAEO,SAASC,EAAmB1Y,EAASuY,EAAgBT,EAAiB1Y,EAAME,EAAMD,EAASoR,GAC9F,GAAuB,IAAnBzQ,EAAQqF,OACR,OAAOhG,EAEX,MAAM8Y,EAAeH,EAAgBhY,EAAS,QAAS,YACjD2Y,EAAerZ,EAAKiF,QAAO3G,GAAoB,WAAbA,EAAI+F,MAAqBwU,EAAa/T,IAAIxG,EAAIoF,OAEtF,OAA4B,IAAxB2V,EAAatT,OACNhG,EAEJA,EAAQkF,QAAO5G,IAClB,IAAK,MAAMC,KAAO+a,EAAc,CAC5B,MAAM/X,EAAOkX,EAAgBxT,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQ8S,GACjEmI,EAAaT,EAAa9T,IAAIzG,EAAIoF,KAGxC,IAFgBuV,EAAejU,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQiD,EAAK1D,MAAO0D,EAAK5C,KAAM4a,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CC5De,SAASC,EAAa9R,EAAK+D,EAAQhE,EAAM0D,GACpD,MAAO,CACHzD,IAAKA,EACL+D,OAAQA,EACRhE,KAAMA,EACN0D,MAAOA,EAEf,CCPe,SAASsO,EAAazZ,EAASC,GAC1C,MAAO,CACHkH,MAAOnH,EAAQgG,OAAShG,EAAQyT,IAAI,GAAGK,gBAAkB,EACzD5M,OAAQjH,EAAK+F,OAAS/F,EAAKwT,IAAI,GAAGE,iBAAmB,EAE7D,CCHe,MAAM+F,EACjB,WAAAvF,GACIC,KAAKzO,OAASqI,SAAS2L,cAAc,UACrCvF,KAAKlW,QAAUkW,KAAKzO,OAAOU,WAAW,MACtC+N,KAAKrJ,YAAc,IAAIuJ,GAC3B,CAEA,YAAApJ,CAAavM,EAAMmM,GACf,IAAKnM,EACD,OAAO,EAEX,MAAMyH,EAAMgO,KAAKlW,QAIjB,OAHAkI,EAAI0E,KAAOA,GAAQqL,EACC/P,EAAIwT,YAAYjb,GAEjBwI,KACvB,CAEA,aAAA0S,CAAclb,EAAMmM,GAChB,IAAIgP,EAAQ,EACZ,IAAK,MAAMC,KAAQpb,EACF,OAATob,GACAD,IAGR,OAAOA,EAAQ1F,KAAKpJ,eAAeF,GAAM5D,MAC7C,CAEA,cAAA8D,CAAeF,GACX,MAAMnH,EAAMmH,EAEZ,GAAIsJ,KAAKrJ,YAAYhG,IAAIpB,GACrB,OAAOyQ,KAAKrJ,YAAY/F,IAAIrB,GAEhC,MAAMyC,EAAMgO,KAAKlW,QAGjBkI,EAAI0E,KAAOA,GAAQqL,EAEnB,MAAM6D,EAAc5T,EAAIwT,YAAY,KAE9BtO,GAAU0O,EAAYC,yBAA2BD,EAAYE,yBAA2B,EAKxFnP,EAAc,CAChBQ,UALcD,EAAS0O,EAAYG,sBAMnC7O,QAASA,EACTE,aANiBwO,EAAYI,uBAAyB9O,EAOtDpE,OANW8S,EAAYG,sBAAwBH,EAAYI,wBAW/D,OAFAhG,KAAKrJ,YAAYyJ,IAAI7Q,EAAKoH,GAEnBA,CACX,ECxDW,SAASsP,IACpB,OAAO,IAAIX,CACf,CCJO,SAASY,EAASC,EAAQxQ,GAC7B,OACIA,EAAKrC,KAAO6S,EAAO7S,KACnBqC,EAAKtC,MAAQ8S,EAAO9S,MACpBsC,EAAKrC,IAAMqC,EAAK7C,QAAUqT,EAAO7S,IAAM6S,EAAOrT,QAC9C6C,EAAKtC,KAAOsC,EAAK5C,OAASoT,EAAO9S,KAAO8S,EAAOpT,KAEvD,CAEO,SAAS6C,EAAKuQ,EAAQxQ,GACzB,MAAMyQ,EAAU,CACZ9S,IAAKrC,KAAKgD,IAAIkS,EAAO7S,IAAKqC,EAAKrC,KAC/BD,KAAMpC,KAAKgD,IAAIkS,EAAO9S,KAAMsC,EAAKtC,MACjCN,MAAO9B,KAAKoV,IAAIF,EAAO9S,KAAO8S,EAAOpT,MAAO4C,EAAKtC,KAAOsC,EAAK5C,OAAS9B,KAAKgD,IAAIkS,EAAO9S,KAAMsC,EAAKtC,MACjGP,OAAQ7B,KAAKoV,IAAIF,EAAO7S,IAAM6S,EAAOrT,OAAQ6C,EAAKrC,IAAMqC,EAAK7C,QAAU7B,KAAKgD,IAAIkS,EAAO7S,IAAKqC,EAAKrC,MAGrG,OAAI8S,EAAQrT,OAAS,GAAKqT,EAAQtT,QAAU,EACjCsT,EAEJ,CACH9S,IAAK6S,EAAO7S,IACZD,KAAM8S,EAAO9S,KACbN,MAAO,EACPD,OAAQ,EAEhB,CAEO,SAASwT,EAAO3Q,EAAM4Q,GACzB,MAAO,CACHjT,IAAKqC,EAAKrC,IAAMiT,EAChBlT,KAAMsC,EAAKtC,KAAOkT,EAClBxT,MAAO4C,EAAK5C,MAAiB,EAATwT,EACpBzT,OAAQ6C,EAAK7C,OAAkB,EAATyT,EAE9B,CAEO,SAAS,EAAK5Q,GACjB,OAAOA,EAAK5C,MAAQ4C,EAAK7C,MAC7B,CAEO,SAAS0T,GAAS7Q,EAAM4Q,GAC3B,MAAO,CACHjT,IAAKqC,EAAKrC,IACVD,KAAMsC,EAAKtC,KACXN,MAAO9B,KAAKgD,IAAI,EAAG0B,EAAK5C,MAAQwT,EAAOlT,KAAOkT,EAAOxP,OACrDjE,OAAQ7B,KAAKgD,IAAI,EAAG0B,EAAK7C,OAASyT,EAAOjT,IAAMiT,EAAOlP,QAE9D,CC9CA,MAAMoP,GAAiB,IACjBC,GAAkB,IAClBC,GAAY,CACdtT,KAAM,EACNC,IAAK,EACLP,MAAO,EACPD,OAAQ,GCRG,SAAS8T,GAAoBzY,EAAS0Y,EAAUC,EAAWC,GAExE,MAAMxR,EAAIsR,EAAStR,EACbC,EAAIqR,EAASrR,EAEbwR,EACE7Y,EAAQ8Y,WADVD,EAEC7Y,EAAQ+Y,UAGTC,EACGhZ,EAAQiZ,YADXD,EAEIhZ,EAAQkZ,aAGlB,MAAO,CACL9R,EAAGA,GAAKuR,EAAUzT,KACdkC,EACAA,GAAK4R,EACH5R,EAAIyR,EACJzR,GAAK4R,EAAmBL,EAAU/P,MAChCgQ,EAAUhU,MAAQoU,EAAmB5R,EACrCA,EAAIyR,EACZxR,EAAGA,GAAKsR,EAAUxT,IACdkC,EACAA,GAAK2R,EACH3R,EAAIwR,EACJxR,GAAK2R,EAAoBL,EAAUzP,OACjC0P,EAAUjU,OAASqU,EAAoB3R,EACvCA,EAAIwR,EAEhB,CC/Be,SAASM,GAAUjG,GAC9B,OAAOA,EAASpO,QAAO,CAACgN,EAAQ9R,IAAY8R,EAAOG,IAAIjS,EAAQoB,IAAKpB,IAAU,IAAI+R,IACtF,CCAe,SAASqH,GAAoBC,EAAapK,EAAYvO,EAAaiO,EAAalR,EAASC,EAAMwE,EAAcC,GACxH,IAAKkX,EACD,MAAO,GACX,GAAIpK,EACA,MAAO,GACX,IAAKN,EACD,MAAO,GACX,IAAKjO,EACD,MAAO,GAEX,MAAMoO,EAAmB3N,EAAYT,EAAY2B,UAC3C0M,EAAgB5N,EAAYT,EAAY6B,OACxC+W,EAAmBnY,EAAYwN,EAAYtM,UAC3CkX,EAAgBpY,EAAYwN,EAAYpM,OAE9C,IAAKL,EAAaM,IAAIsM,GAClB,MAAO,GACX,IAAK3M,EAAUK,IAAIuM,GACf,MAAO,GACX,IAAK7M,EAAaM,IAAI8W,GAClB,MAAO,GACX,IAAKnX,EAAUK,IAAI+W,GACf,MAAO,GAEX,MAAMC,EAAiB1W,KAAKoV,IAAIhW,EAAaO,IAAIqM,GAAkBxJ,MAAOpD,EAAaO,IAAI6W,GAAkBhU,OACvGmU,EAAiB3W,KAAKgD,IAAI5D,EAAaO,IAAIqM,GAAkBxJ,MAAOpD,EAAaO,IAAI6W,GAAkBhU,OACvGoU,EAAc5W,KAAKoV,IAAI/V,EAAUM,IAAIsM,GAAezJ,MAAOnD,EAAUM,IAAI8W,GAAejU,OACxFqU,EAAc7W,KAAKgD,IAAI3D,EAAUM,IAAIsM,GAAezJ,MAAOnD,EAAUM,IAAI8W,GAAejU,OAE9F,OAAO7H,EAAQkI,MAAM6T,EAAgBC,EAAiB,GAAGG,SAAQ7d,GACtD2B,EAAKiI,MAAM+T,EAAaC,EAAc,GAAG/d,KAAII,IACzC,CACHuG,MAAOvG,EAAIuE,GACX8B,SAAUtG,EAAOwE,QAIjC,CCvBe,SAASsZ,GAAe9d,EAAQC,GAC3C,MAAMsH,EAjBV,SAA4BtH,GACxB,MAAmB,UAAfA,EAAI6T,OACG,MACQ,QAAf7T,EAAI6T,OACG,SACJ,QACX,CAW4BiK,CAAmB9d,GACrCwH,EAVV,SAA8BzH,GAC1B,MAAsB,UAAlBA,EAAO8T,OACA,OACW,QAAlB9T,EAAO8T,OACA,QACJ,QACX,CAI8BkK,CAAqBhe,GAE/C,MAAO,GAAGuH,KAAmBE,GACjC,CClBe,SAASwW,GAAkBhb,EAAMkD,EAAcC,EAAWoB,GACrE,IAAKvE,EACD,OAAO,KAEX,MAAMoD,EAAYjB,EAAYnC,EAAKqD,UAC7BC,EAASnB,EAAYnC,EAAKuD,OAEhC,IAAKL,EAAaM,IAAIJ,GAClB,OAAO,KACX,IAAKD,EAAUK,IAAIF,GACf,OAAO,KAEX,MAAMvG,EAASmG,EAAaO,IAAIL,GAC1BpG,EAAMmG,EAAUM,IAAIH,GAEpBoW,EAAW,CACb9T,MAAO7I,EAAO6I,MACdD,OAAQ3I,EAAI2I,OACZkH,QAASgO,GAAe9d,EAAQC,IAGpC,OAAQA,EAAI6T,QACR,IAAK,QACD6I,EAASvT,IAAMnJ,EAAImJ,IACnB,MACJ,IAAK,MACDuT,EAASxP,OAAS3F,EAAS4B,IAAIR,OAASpB,EAASwF,OAAOpE,OAASpB,EAAS2F,OAAOvE,OAAS3I,EAAImJ,IAAMnJ,EAAI2I,OACxG,MACJ,QACI+T,EAAS5R,UAAY9K,EAAImJ,IAAM5B,EAAS4B,IAAIR,OAGpD,OAAQ5I,EAAO8T,QACX,IAAK,QACD6I,EAASxT,KAAOnJ,EAAOmJ,KACvB,MACJ,IAAK,MACDwT,EAAS9P,MAAQrF,EAAS2B,KAAKN,MAAQrB,EAASiO,OAAO5M,MAAQrB,EAASqF,MAAMhE,MAAQ7I,EAAOmJ,KAAOnJ,EAAO6I,MAC3G,MACJ,QACI8T,EAAS7R,WAAa9K,EAAOmJ,KAAO3B,EAAS2B,KAAKN,MAG1D,OAAO8T,CACX,CC7Ce,SAAS,GAAkBuB,EAAevZ,EAAawB,EAAcC,EAAWoB,GAC3F,OAA6B,IAAzB0W,EAAcxW,OACP,KAEJ,GAAiB/C,EAAawB,EAAcC,EAAWoB,EAClE,CCPe,SAAS2W,GAAe9d,EAAM6d,GACzC,OAAOA,EAAcE,OAAMnb,GAAQA,EAAKxC,KAAKE,SAAS,CAAE8Q,OAAQpR,KACpE,CCFA,SAASge,GAAclH,GACnB,OAAK7R,MAAMC,QAAQ4R,GAGZA,EAAStX,KAAI,CAAC6K,EAAGnB,IAAUA,IAFvB7D,OAAOC,KAAKwR,EAG3B,CAEA,SAASmH,GAAiB7c,GACtB,OAAO4c,GAAc5c,EACzB,CAEA,SAAS8c,GAAoB9c,GACzB,MAAMkE,EAAO,IAAI8Q,IAEjB,GAAInR,MAAMC,QAAQ9D,GACd,IAAK,MAAMwC,KAAWxC,EAClB,IAAK,MAAM+C,KAAM6Z,GAAcpa,GAC3B0B,EAAK+Q,IAAIlS,QAGjB,IAAK,MAAMa,KAAO5D,EACd,IAAK,MAAM+C,KAAM6Z,GAAc5c,EAAK4D,IAChCM,EAAK+Q,IAAIlS,GAIrB,MAAO,IAAImB,EACf,CAEO,SAAS6Y,GAAmB9c,EAASD,GAGxC,IAFsBC,EAAQ+c,MAAKze,GAA0B,eAAhBA,EAAOgG,OAGhD,OAAOtE,EAEX,MAAMgd,EAAkB,GAExB,IAAK,MAAM1e,KAAU0B,EACjB,GAAoB,eAAhB1B,EAAOgG,KAAuB,CAC9B,MAAM2Y,EAAM,aAAc3e,EACpBA,EAAO4e,SAASnd,GAChB8c,GAAoB9c,GAE1B,IAAK,MAAM+C,KAAMma,EACbD,EAAgBjV,KAAK,IACdzJ,EACHwE,KACAwB,KAAM,QAGlB,MACI0Y,EAAgBjV,KAAKzJ,GAI7B,OAAO0e,CACX,CAEO,SAASG,GAAgBld,EAAMF,GAGlC,IAFsBE,EAAK8c,MAAKxe,GAAoB,eAAbA,EAAI+F,OAGvC,OAAOrE,EAEX,MAAMmd,EAAe,GAErB,IAAK,MAAM7e,KAAO0B,EACd,GAAiB,eAAb1B,EAAI+F,KAAuB,CAC3B,MAAM2Y,EAAM,aAAc1e,EACpBA,EAAI2e,SAASnd,GACb6c,GAAiB7c,GAEvB,IAAK,MAAM+C,KAAMma,EACbG,EAAarV,KAAK,IACXxJ,EACHuE,KACAwB,KAAM,QAGlB,MACI8Y,EAAarV,KAAKxJ,GAI1B,OAAO6e,CACX,CClFA,MAAMC,GAAmB,EAAG1e,OAAMsV,gBAAiBtV,EAAK4R,SAAS0D,GAElD,MAAMqJ,GACjB,WAAAnJ,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAMvY,KAAQgZ,EAAO,CACtB,MAAMa,EAAQ,CACVsF,GAAI7Z,EAAY,OAAQtF,EAAOA,EAAKmf,GAAK,UACzC/e,UAAWJ,EAAKI,WAAa6e,IAGjCjJ,KAAK2D,YAAYlB,QAAQzY,EAAKE,OAAQF,EAAKG,IAAK0Z,EACpD,CACJ,CAEA,OAAAhT,CAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQT,EAAOc,EAAMma,GACnD,MAAM1B,EAAQhD,KAAK2D,YAAYZ,SAAS7Y,EAAQC,GAEhD,GAAqB,IAAjB6Y,EAAMpR,OACN,MAAiB,SAAbzH,EAAI+F,MAEY,SAAhBhG,EAAOgG,OAENwU,EAAa/T,IAAI,aAGfsY,GAAiB,CAAE1e,OAAMsV,WAAY6E,EAAa9T,IAAI,cAGjE,IAAI9G,EAAU,CAAE6B,OAAME,OAAMD,UAASzB,MAAKD,SAAQT,QAAOc,QAEzD,IAAK,MAAMP,KAAQgZ,EAAO,CACtB,IAAK0B,EAAa/T,IAAI3G,EAAKmf,IACvB,SAEJ,MAAMC,EAAgB,IAAKtf,EAAS+V,WAAY6E,EAAa9T,IAAI5G,EAAKmf,KAEtE,IAAKnf,EAAKI,UAAUgf,GAChB,OAAO,CACf,CAEA,OAAO,CACX,EC5CW,SAASC,GAAkBle,GACtC,OAAO,IAAI+d,GAAe/d,EAC9B,CCFe,SAASme,GAAoB1f,GACxC,OAAOwS,EAAqBxS,EAAY,CAAC,QAAS,QACtD,CCFe,SAAS2f,GAAqB3f,GACzC,OAAOwS,EAAqBxS,EAAY,CAAC,QAAS,OAAQ,OAAQ,WACtE,CCAO,SAAS4f,GAAmB5d,EAASC,EAAMuG,EAAchC,EAAgBqZ,EAAgBC,GAC5F,GAAI9d,EAAQ0c,OAAMpe,GAAkC,iBAAjBA,EAAO6I,QACtC,OAAOnH,EAEX,MAAM+d,EAAgBzf,IAClB,MAAM0f,EAAiB1f,EAAO6I,MAE9B,GAA8B,iBAAnB6W,EACP,OAAOA,EAEX,GAAIH,EAAe9Y,IAAIzG,EAAOqF,KAAM,CAChC,MAAMsa,EAASJ,EAAe7Y,IAAI1G,EAAOqF,KAEzC,GAAuB,aAAnBqa,IAAkCC,EAAOC,SACzC,OAAOD,EAAO9W,MAClB,GAAuB,kBAAnB6W,GAAsCC,EAAOC,SAC7C,OAAOD,EAAO9W,KACtB,CAEA,IAAIA,EAAQ,EACZ,IAAK,MAAM5I,KAAO0B,EAAM,CACpB,GAAiB,SAAb1B,EAAI+F,MAAsC,kBAAnB0Z,EACvB,SACJ,GAAiB,SAAbzf,EAAI+F,MAAsC,aAAnB0Z,EACvB,SAEJ,MAAMzc,EAAOiD,EAAeS,QAAQ1G,EAAKD,GACnCK,EAAO4C,EAAK5C,KACZmM,EAAOvJ,EAAKuJ,KACZjM,EAAU0C,EAAK1C,QAAQ4I,KAAOlG,EAAK1C,QAAQsM,MAE3Cf,EAAY5D,EAAa0E,aAAavM,EAAMmM,GAAQjM,EAE1DsI,EAAQ9B,KAAKgD,IAAIlB,EAAOiD,EAC5B,CAOA,OALAyT,EAAerJ,IAAIlW,EAAOqF,IAAK,CAC3BwD,QACA+W,SAA6B,kBAAnBF,IAGP7W,CAAK,EAGhB,IAAK,MAAMxD,KAAOka,EAAe5Z,OACxB6Z,EAAY/Y,IAAIpB,IACjBka,EAAeM,OAAOxa,GAG9B,OAAO3D,EAAQ7B,KAAIG,IAAU,IACtBA,EACH6I,MAAO4W,EAAczf,MAE7B,CAEO,SAAS8f,GAAgBpe,EAASC,EAAMuG,EAAchC,EAAgBqZ,EAAgBC,GACzF,GAAI7d,EAAKyc,OAAMne,GAA6B,iBAAfA,EAAI2I,SAC7B,OAAOjH,EAEX,MAAMoe,EAAa9f,IACf,MAAM+f,EAAkB/f,EAAI2I,OAE5B,GAA+B,iBAApBoX,EACP,OAAOA,EAEX,GAAIT,EAAe9Y,IAAIxG,EAAIoF,KAAM,CAC7B,MAAMsa,EAASJ,EAAe7Y,IAAIzG,EAAIoF,KAEtC,GAAwB,aAApB2a,IAAmCL,EAAOC,SAC1C,OAAOD,EAAO/W,OAClB,GAAwB,kBAApBoX,GAAuCL,EAAOC,SAC9C,OAAOD,EAAO/W,MACtB,CAEA,IAAIA,EAAS,EACb,IAAK,MAAM5I,KAAU0B,EAAS,CAC1B,GAAoB,SAAhB1B,EAAOgG,MAAuC,kBAApBga,EAC1B,SACJ,GAAoB,SAAhBhgB,EAAOgG,MAAuC,aAApBga,EAC1B,SAEJ,MAAM/c,EAAOiD,EAAeS,QAAQ1G,EAAKD,GACnCK,EAAO4C,EAAK5C,KACZmM,EAAOvJ,EAAKuJ,KACZjM,EAAU0C,EAAK1C,QAAQ6I,IAAMnG,EAAK1C,QAAQ4M,OAE1CpB,EAAa7D,EAAaqT,cAAclb,EAAMmM,GAAQjM,EAE5DqI,EAAS7B,KAAKgD,IAAInB,EAAQmD,EAC9B,CAOA,OALAwT,EAAerJ,IAAIjW,EAAIoF,IAAK,CACxBuD,SACAgX,SAA8B,kBAApBI,IAGPpX,CAAM,EAGjB,IAAK,MAAMvD,KAAOka,EAAe5Z,OACxB6Z,EAAY/Y,IAAIpB,IACjBka,EAAeM,OAAOxa,GAG9B,OAAO1D,EAAK9B,KAAII,IAAO,IAChBA,EACH2I,OAAQmX,EAAW9f,MAE3B,CChHe,SAASggB,GAAQvG,GAC5B,OAAO,IAAIjD,IAAIiD,EAAQ7Z,KAAI8Z,GAASA,EAAMtU,MAC9C,CCAe,SAAS6a,GAAqBxgB,GACzC,OAAOwS,EAAqBxS,EAAY,CAAC,QAAS,QACtD,CCDA,SAASygB,GAAqBC,EAAKC,GAC/B,OAAiBzO,MAAbwO,EAAI7gB,QAESqS,MAAbyO,EAAI9gB,OAED6gB,EAAI7gB,MAAQ8gB,EAAI9gB,MAC3B,CAEA,SAAS+gB,GAAsBF,EAAKC,GAChC,OAAiBzO,MAAbwO,EAAI7gB,QAESqS,MAAbyO,EAAI9gB,OAED6gB,EAAI7gB,MAAQ8gB,EAAI9gB,MAC3B,CAEe,MAAMghB,GACjB,WAAA1K,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAMvY,KAAQgZ,EAAO,CACtB,MAAM0H,EAAgB1gB,EAAK2gB,WACrB,CAACL,EAAKC,IAAQvgB,EAAK2gB,WAAWL,EAAKC,GACnC,CAACD,EAAKC,IAAQF,GAAqBC,EAAKC,GACxCK,EAAiB5gB,EAAK2gB,WACtB,CAACL,EAAKC,KAASvgB,EAAK2gB,WAAWL,EAAKC,GACpC,CAACD,EAAKC,IAAQC,GAAsBF,EAAKC,GAEzC1G,EAAQ,CACVsF,GAAI7Z,EAAY,OAAQtF,EAAOA,EAAKmf,GAAK,UACzCuB,cAAeA,EACfE,eAAgBA,GAGpB5K,KAAK2D,YAAYlB,QAAQzY,EAAKE,OAAQF,EAAKG,IAAK0Z,EACpD,CACJ,CAEA,OAAAhT,CAAQ3G,EAAQC,EAAK0gB,GACjB,MAAM7H,EAAQhD,KAAK2D,YAAYZ,SAAS7Y,EAAQC,GAEhD,GAAqB,IAAjB6Y,EAAMpR,OACN,MAAiB,SAAbzH,EAAI+F,MAEY,SAAhBhG,EAAOgG,KADA,KAGN2a,EAAala,IAAI,YAGkB,QAAjCka,EAAaja,IAAI,YAClByZ,GACAG,GAJK,KAOf,GAAIxH,EAAMpR,OAAS,EACf,MAAM,IAAIkZ,MAAM,4CAEpB,MAAM9gB,EAAOgZ,EAAM,GAEnB,OAAK6H,EAAala,IAAI3G,EAAKmf,IAGU,QAA9B0B,EAAaja,IAAI5G,EAAKmf,IACvBnf,EAAK0gB,cACL1gB,EAAK4gB,eAJA,IAKf,EClEW,SAASG,GAAgBpc,GACpC,OAAO,IAAI8b,GAAa9b,EAC5B,CCFA,SAASqc,GAAgBnP,EAAQ2I,EAAYC,GACzC,MAAMoG,EAAe,IAAI3K,IACzB,IAAK,MAAM/S,KAAQ0O,EAAQ,CACvB,MAAM8I,EAAUrV,EAAYnC,EAAKqX,IAC3BI,EAAYtV,EAAYnC,EAAKsX,IAE9BoG,EAAala,IAAIgU,IAClBkG,EAAazK,IAAIuE,EAAS,IAAIzE,KAElC2K,EAAaja,IAAI+T,GAASvE,IAAIwE,EAAWzX,EAAK6O,UAClD,CACA,OAAO6O,CACX,CAEA,SAASI,GAAMC,EAAMjH,GACjBiH,EAAKpb,MAAK,CAACwa,EAAKC,KACZ,MAAMtG,EAASqG,EAAIK,WAAWL,EAAInd,KAAMod,EAAIpd,MAC5C,MAAsB,iBAAX8W,EACAA,EACJA,GAAU,EAAI,CAAC,IAE1BA,EAAOtQ,QAAQuX,EAAKnhB,KAAI8Z,GAASA,EAAMsH,UACvCD,EAAKtZ,OAAS,CAClB,CAEO,SAASwZ,GAAcvP,EAAQwP,EAAchH,EAAiB1Y,EAAME,EAAMD,EAASoR,GACtF,GAAsB,IAAlBnB,EAAOjK,OACP,OAAO/F,EAEX,MAAMgf,EAAeG,GAAgBnP,EAAQ,WAAY,SACnDxL,EAAe,IAAI6P,IAAItU,EAAQ7B,KAAIG,GAAU,CAACA,EAAOqF,IAAKrF,MAC1DohB,EAAgBzP,EACjB9R,KAAIoD,GAAQmC,EAAYnC,EAAKqD,YAC7BM,QAAOvB,GAAOc,EAAaM,IAAIpB,KAC/BxF,KAAIwF,GAAOc,EAAaO,IAAIrB,KAC5Bgc,UAEL,GAA6B,IAAzBD,EAAc1Z,OACd,OAAO/F,EAEX,IAAK,MAAM3B,KAAUohB,EAAe,CAChC,MAAMrH,EAAS,GACTiH,EAAO,GAEb,IAAK,MAAM/gB,KAAO0B,EAAM,CACpB,MAAM8e,EAAaU,EAAaxa,QAAQ3G,EAAQC,EAAK0gB,EAAaja,IAAI1G,EAAOqF,MAE7E,IAAKob,EAAY,CACbM,GAAMC,EAAMjH,GACZA,EAAOtQ,KAAKxJ,GACZ,QACJ,CAEA,MACM0Z,EAAQ,CAAEsH,OAAQhhB,EAAKwgB,aAAYxd,KAD5BkX,EAAgBxT,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQ8S,IAGnD,IAAhBkO,EAAKtZ,QAKLsZ,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAMjH,GACZiH,EAAKvX,KAAKkQ,IAVNqH,EAAKvX,KAAKkQ,EAWlB,CAEAoH,GAAMC,EAAMjH,GACZpY,EAAOoY,CACX,CAEA,OAAOpY,CACX,CAEO,SAAS2f,GAAiB3P,EAAQwP,EAAchH,EAAiB1Y,EAAME,EAAMD,EAASoR,GACzF,GAAsB,IAAlBnB,EAAOjK,OACP,OAAOhG,EAEX,MAAMif,EAAeG,GAAgBnP,EAAQ,QAAS,YAChDvL,EAAY,IAAI4P,IAAIrU,EAAK9B,KAAII,GAAO,CAACA,EAAIoF,IAAKpF,MAC9CshB,EAAa5P,EACd9R,KAAIoD,GAAQmC,EAAYnC,EAAKuD,SAC7BI,QAAOvB,GAAOe,EAAUK,IAAIpB,KAC5BxF,KAAIwF,GAAOe,EAAUM,IAAIrB,KACzBgc,UAEL,GAA0B,IAAtBE,EAAW7Z,OACX,OAAOhG,EAEX,IAAK,MAAMzB,KAAOshB,EAAY,CAC1B,MAAMxH,EAAS,GACTiH,EAAO,GAEb,IAAK,MAAMhhB,KAAU0B,EAAS,CAC1B,MAAM+e,EAAaU,EAAaxa,QAAQ3G,EAAQC,EAAK0gB,EAAaja,IAAIzG,EAAIoF,MAE1E,IAAKob,EAAY,CACbM,GAAMC,EAAMjH,GACZA,EAAOtQ,KAAKzJ,GACZ,QACJ,CAEA,MACM2Z,EAAQ,CAAEsH,OAAQjhB,EAAQygB,aAAYxd,KAD/BkX,EAAgBxT,QAAQlF,EAAME,EAAMD,EAASzB,EAAKD,EAAQ8S,IAGnD,IAAhBkO,EAAKtZ,QAKLsZ,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAMjH,GACZiH,EAAKvX,KAAKkQ,IAVNqH,EAAKvX,KAAKkQ,EAWlB,CAEAoH,GAAMC,EAAMjH,GACZrY,EAAUqY,CACd,CAEA,OAAOrY,CACX,CC9HA,MAAM8f,GAAa,EAIZ,SAASC,GAAmB/f,EAASyE,EAAcC,EAAWwM,EAAa3O,EAASyd,EAAe9E,EAAWC,GACjH,IAAKjK,EACD,OAAO,KAEX,MAAM5S,EAASmG,EAAaO,IAAItB,EAAYwN,EAAYtM,WAGxD,GAAiB,WAFLF,EAAUM,IAAItB,EAAYwN,EAAYpM,QAE1CR,KACJ,OAAO,KAEX,MAAM2b,EAAmBjF,GAAoBzY,EAASyd,EAAe9E,EAAWC,GAChF,IAAK8E,EACD,OAAO,KACX,MAAMtW,EAAIsW,EAAiBtW,EAE3B,OAAIA,GAAKrL,EAAO6M,MAAQ2U,IAAcnW,GAAKrL,EAAO6M,MAAQ2U,GAC/CxhB,EAAOwE,GAEG,IAAjBxE,EAAOuJ,OAEP8B,EAAIrL,EAAOmJ,KAAOqY,IAAcnW,EAAIrL,EAAOmJ,KAAOqY,GAD3C,KAIJ9f,EAAQ1B,EAAOuJ,MAAQ,GAAG/E,EACrC,CAEO,SAASod,GAAgBjgB,EAAMwE,EAAcC,EAAWwM,EAAa3O,EAASyd,EAAe9E,EAAWC,GAC3G,IAAKjK,EACD,OAAO,KAEX,MAAM5S,EAASmG,EAAaO,IAAItB,EAAYwN,EAAYtM,WAClDrG,EAAMmG,EAAUM,IAAItB,EAAYwN,EAAYpM,QAElD,GAAoB,WAAhBxG,EAAOgG,KACP,OAAO,KAEX,MAAM2b,EAAmBjF,GAAoBzY,EAASyd,EAAe9E,EAAWC,GAChF,IAAK8E,EACD,OAAO,KACX,MAAMrW,EAAIqW,EAAiBrW,EAE3B,OAAIA,GAAKrL,EAAIkN,OAASqU,IAAclW,GAAKrL,EAAIkN,OAASqU,GAC3CvhB,EAAIuE,GAEG,IAAdvE,EAAIsJ,OAEJ+B,EAAIrL,EAAImJ,IAAMoY,IAAclW,EAAIrL,EAAImJ,IAAMoY,GADnC,KAIJ7f,EAAK1B,EAAIsJ,MAAQ,GAAG/E,EAC/B,CCzDe,SAASqd,GAAkBlQ,GACtC,OAAOA,EAAO9R,KAAI+F,IAAQ,CACtBU,SAAU,aAAcV,EAAOA,EAAKU,SAAW,SAC/CE,MAAO,UAAWZ,EAAOA,EAAKY,MAAQ,SACtCsL,UAAWlM,EAAKkM,aAExB,CCNe,SAASgQ,GAAmBzf,GACvC,OAAOA,EAAQxC,KAAI+G,IAAU,CACzBN,SAAU,aAAcM,EAASA,EAAON,SAAW,SACnDE,MAAO,UAAWI,EAASA,EAAOJ,MAAQ,SAC1CmP,WAAY/O,EAAO+O,cAE3B,CCIO,SAASoM,GAAiBrgB,EAASsgB,GACtC,OAXJ,SAAmBtI,EAASsI,GACxB,MAAMrD,EAAMjF,EACP9S,QAAO+S,GAAwB,SAAfA,EAAM3T,OACtBnG,KAAI8Z,GAASA,EAAMnV,KAIxB,OAFAwd,EAASrD,GAEFA,CACX,CAGWsD,CAAUvgB,EAASsgB,EAC9B,CCVe,SAASE,GAAqBxiB,GACzC,OAAOwS,EAAqBxS,EAAY,CAAC,QAAS,OAAQ,WAC9D,CCFe,SAASyiB,GAAWvP,EAAa1M,EAAgBC,EAAcC,GAC1E,IAAKwM,EACD,OAAO,KAEX,MAAMvM,EAAYjB,EAAYwN,EAAYtM,UACpCC,EAASnB,EAAYwN,EAAYpM,OAEvC,IAAKL,EAAaM,IAAIJ,GAClB,OAAO,KACX,IAAKD,EAAUK,IAAIF,GACf,OAAO,KAEX,MAAMtG,EAAMmG,EAAUM,IAAIH,GACpBvG,EAASmG,EAAaO,IAAIL,GAEhC,OAAOH,EAAeS,QAAQ1G,EAAKD,GAAQwQ,OAC/C,CChBe,SAAS4R,GAAoB5R,EAAS7L,EAAawB,EAAcC,EAAWoB,GACvF,IAAKgJ,EACD,OAAO,KAEX,MAAM6R,EAAgB,GAAiB1d,EAAawB,EAAcC,EAAWoB,GAE7E,OAAK6a,EAGE,CACHjZ,IAAKiZ,EAAcjZ,IACnBD,KAAMkZ,EAAclZ,MAJb,IAMf,CC0BA,SAASmZ,GAAoB1iB,GAGzB,MAAM2iB,EAAU,IAAK3iB,EAAQ4iB,gBAAiB5iB,EAAQ6iB,iBAChDC,EAAS9iB,EAAQ8iB,OACjBC,EAAgB/iB,EAAQwH,MACxBnD,EAAUrE,EAAQqE,QAGxB,SAAS2e,EAAMvd,EAAKwd,EAAMC,GACtB,MAAMC,EAAuBL,EAAOrd,IAAQqd,EAAOrd,GAAKyd,aAGxD,OAFKC,IAAwBD,EAAarE,MAAK,CAACuE,EAAYzZ,IAAUyZ,IAAeD,EAAqBxZ,OACtGmZ,EAAOrd,GAAO,CAAE9F,MAAOsjB,KAAQC,GAAeA,iBAC3CJ,EAAOrd,GAAK9F,KACvB,CAEA,MAAMuH,EAAmB3B,OAAO2B,iBAC1BpC,EAAc6d,EAAQ7d,YAAcoC,EACpCrF,EAAO8gB,EAAQ9gB,KACfpB,EAAOT,EAAQ2P,MAAMhQ,MACrBoS,EAASiR,EAAM,SAAUf,GAAmB,CAACU,EAAQ5Q,SACrDtP,EAAUugB,EAAM,UAAWd,GAAoB,CAACS,EAAQlgB,UACxD6F,EAAe0a,EAAM,eAAgB7G,EAAiB,IACtDkH,EAAiBL,EAAM,iBAAkBlR,EAAmB,CAAC6Q,EAAQ7iB,WAAY6iB,EAAQphB,aAAcwQ,IACvG4E,EAAwBqM,EAAM,wBAAyBlN,EAA0B,CAAC6M,EAAQjgB,YAAaD,IACvGyQ,EAAU8P,EAAM,UAAWtM,EAAY,CAACC,IACxC2M,EAAiBN,EAAM,iBAAkB/L,EAAY,CAAC0L,EAAQ7gB,QAASD,IACvE0hB,EAAcP,EAAM,cAAe/L,EAAY,CAAC0L,EAAQ5gB,KAAMF,IAG9Did,EAAkBkE,EAAM,kBAAmBpE,GAAoB,CAAC0E,EAAgBzhB,IAChFqd,EAAe8D,EAAM,eAAgB/D,GAAiB,CAACsE,EAAa1hB,IACpE2hB,EAAoBR,EAAM,oBAAqBvL,EAAoB,CAACqH,EAAiB6D,EAAQtgB,WAAYsgB,EAAQpgB,YAAaogB,EAAQzd,eACtIue,EAAiBT,EAAM,iBAAkBrL,EAAiB,CAACuH,EAAcyD,EAAQ1gB,UAAW0gB,EAAQxgB,aAAcwgB,EAAQxd,aAC1Hue,EAAuBV,EAAM,uBAAwB3C,GAAS,CAACmD,IAC/DG,EAAoBX,EAAM,oBAAqB3C,GAAS,CAACoD,IAGzDG,EAAmBZ,EAAM,mBAAoBxD,GAAqB,CAAC6D,IACnEQ,EAAwBb,EAAM,wBAAyB3I,EAAoB,CAACuJ,IAC5E5I,EAAiBgI,EAAM,iBAAkBzD,GAAmB,CAACoD,EAAQthB,YACrE4Z,EAAkB+H,EAAM,kBAAmB7H,EAAoB,CAAC1Y,EAASuY,EAAgB6I,EAAuBhiB,EAAM4hB,EAAgBD,EAAmBtQ,IACzJkI,EAAe4H,EAAM,eAAgBjI,EAAiB,CAACtY,EAASuY,EAAgB6I,EAAuBhiB,EAAM4hB,EAAgBD,EAAmBtQ,IAGhJ4Q,EAAoBd,EAAM,oBAAqB1C,GAAsB,CAAC+C,IACtEU,GAAyBf,EAAM,yBAA0B3I,EAAoB,CAACyJ,IAC9EvC,GAAeyB,EAAM,eAAgB/B,GAAiB,CAAC0B,EAAQ9d,UAK/Dmf,GAJgBhB,EAAM,gBAAiBtB,GAAkB,CAAC3P,EAAQwP,GAAcwC,GAAwBliB,EAAMuZ,EAAcH,EAAiB/H,IAK7I+Q,GAJajB,EAAM,aAAc1B,GAAe,CAACvP,EAAQwP,GAAcwC,GAAwBliB,EAAMuZ,EAAcH,EAAiB/H,IAOpIgR,GAAoBlB,EAAM,oBAAqBvD,GAAsB,CAAC4D,IACtEc,GAAyBnB,EAAM,yBAA0B3I,EAAoB,CAAC6J,KAC9EE,GAAwBpB,EAAM,wBAAyBxI,EAAmB,CAAC2J,GAAwBtiB,EAAMoiB,GAAYD,GAAe9Q,IACpImR,GAAmBrkB,EAAQqkB,iBAC3BC,GAAiBtkB,EAAQskB,eACzBC,GAAkBvB,EAAM,kBAAmBtD,GAAoB,CAACsE,GAAeC,GAAY3b,EAAc8b,GAAuBC,GAAkBX,IAClJc,GAAexB,EAAM,eAAgB9C,GAAiB,CAAC8D,GAAeC,GAAY3b,EAAc8b,GAAuBE,GAAgBX,IAGvI7hB,GAAUkhB,EAAM,UAAWnL,EAAkB,CAAC0M,GAAiBrd,EAAkBpC,IACjF/C,GAAOihB,EAAM,OAAQjL,EAAe,CAACyM,GAActd,EAAkBpC,IACrEyB,GAAeyc,EAAM,eAAgBxF,GAAW,CAAC1b,KACjD0E,GAAYwc,EAAM,YAAaxF,GAAW,CAACzb,KAC3CgD,GAAc4d,EAAQ5d,YACtB6C,GAAWob,EAAM,WAAYhP,EAAa,CAAClS,GAASC,KACpDa,GAAgB+f,EAAQ/f,cACxBoa,GAAYgG,EAAM,YAAa1H,EAAc,CAAC1T,GAAS4B,IAAIR,OAAQpB,GAAS2F,OAAOvE,OAAQpB,GAAS2B,KAAKN,MAAOrB,GAASqF,MAAMhE,QAC/HgU,GAAY+F,EAAM,YAAazH,EAAc,CAACzZ,GAASC,KAEvDiR,GChHK,SAAwB3O,EAASyd,EAAe/f,EAAMD,EAASkb,EAAWC,GACrF,IAAK6E,EACD,OAAO,KACX,GAAIA,EAAcrW,EAAI,GAAKqW,EAAcpW,EAAI,GAAKoW,EAAcrW,EAAIwR,EAAUhU,OAAS6Y,EAAcpW,EAAIuR,EAAUjU,OAC/G,OAAO,KAEX,MAAM+Y,EAAmBjF,GAAoBzY,EAASyd,EAAe9E,EAAWC,GAC1EwH,ECXK,SAAqB1iB,EAAM2J,GACtC,GAAoB,IAAhB3J,EAAK+F,OACL,OAAQ,EACZ,GAAI4D,EAAI3J,EAAK,GAAGyT,cACZ,OAAQ,EACZ,GAAI9J,EAAI3J,EAAKA,EAAK+F,OAAS,GAAG2N,iBAC1B,OAAQ,EAEZ,IAAIiP,EAAQ,EACRC,EAAQ5iB,EAAK+F,OAAS,EAE1B,KAAO4c,GAASC,GAAO,CACnB,MAAMC,EAAQzd,KAAK0d,OAAOH,EAAQC,GAAS,GAE3C,GAAIjZ,EAAI3J,EAAK6iB,GAAOpP,cAChBmP,EAAQC,EAAQ,MACf,MAAIlZ,EAAI3J,EAAK6iB,GAAOnP,kBAIrB,OAAOmP,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CDb0BE,CAAY/iB,EAAMggB,EAAiBrW,GACnDqZ,EEZK,SAAwBjjB,EAAS2J,GAC5C,GAAuB,IAAnB3J,EAAQgG,OACR,OAAQ,EACZ,GAAI2D,EAAI3J,EAAQ,GAAG6T,eACf,OAAQ,EACZ,GAAIlK,EAAI3J,EAAQA,EAAQgG,OAAS,GAAG8N,gBAChC,OAAQ,EAEZ,IAAI8O,EAAQ,EACRC,EAAQ7iB,EAAQgG,OAAS,EAE7B,KAAO4c,GAASC,GAAO,CACnB,MAAMC,EAAQzd,KAAK0d,OAAOH,EAAQC,GAAS,GAE3C,GAAIlZ,EAAI3J,EAAQ8iB,GAAOjP,eACnBgP,EAAQC,EAAQ,MACf,MAAInZ,EAAI3J,EAAQ8iB,GAAOhP,iBAIxB,OAAOgP,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CFZ6BI,CAAeljB,EAASigB,EAAiBtW,GAElE,OAAuB,IAAnBgZ,IAA8C,IAAtBM,EACjB,KAEJ,CACHne,MAAO7E,EAAK0iB,GAAe7f,GAC3B8B,SAAU5E,EAAQijB,GAAkBngB,GAE5C,CD+FwBqgB,CAAe5gB,EAASrE,EAAQ8hB,cAAe/f,GAAMD,GAASkb,GAAWC,IACvFzM,GAAkBxQ,EAAQklB,gBAAkBlC,EAAM,kBAAmBnB,GAAoB,CAAC/f,GAASyE,GAAcC,GAAWwM,GAAa3O,EAASrE,EAAQ8hB,cAAe9E,GAAWC,KACpLxM,GAAezQ,EAAQmlB,aAAenC,EAAM,eAAgBhB,GAAiB,CAACjgB,GAAMwE,GAAcC,GAAWwM,GAAa3O,EAASrE,EAAQ8hB,cAAe9E,GAAWC,KAGrKjY,GAAmBge,EAAM,mBAAoBvF,GAAqB,CAFpDzd,EAAQ0d,cACPlN,MAAqBC,GACwD1L,GAAaiO,GAAalR,GAASC,GAAMwE,GAAcC,KACnJyM,GAAY+P,EAAM,YAAahM,EAAc,CAACpU,KAC9C0J,GAAY0W,EAAM,YAAahM,EAAc,CAAChS,KAE9CogB,GAAmBpC,EAAM,mBAAoBjQ,EAAqB,CAACsQ,EAAgBrQ,GAAajO,GAAakO,GAAW3G,GAAW4G,EAASnB,EAAQvB,GAAiBC,GAAckS,EAAQ7d,cAC3LugB,GAAwBrC,EAAM,wBAAyB3I,EAAoB,CAAC+K,KAC5E7c,GAAuBya,EAAM,uBAAwBxI,EAAmB,CAAC6K,GAAuBxjB,EAAME,GAAMD,GAASoR,IACrHoS,GAAkBtC,EAAM,kBAAmBrQ,EAAoB,CAAC0Q,IAChEkC,GAAuBvC,EAAM,uBAAwB3I,EAAoB,CAACiL,KAC1EE,GAAsBxC,EAAM,sBAAuBxI,EAAmB,CAAC+K,GAAsB1jB,EAAME,GAAMD,GAASoR,IAClHoL,GAAgB0E,EAAM,gBAAiB3c,EAAkB,CAACzD,GAAe4iB,GAAqBjf,GAAcC,KAC5GoJ,GAAiBoT,EAAM,iBAAkB,GAAmB,CAAC1E,GAAevZ,GAAawB,GAAcC,GAAWoB,KAClH0I,GAAc0S,EAAM,cAAezE,GAAgB,CAAC9d,EAAM6d,KAC1DmH,GAAoBzC,EAAM,oBAAqBV,GAAsB,CAACe,IACtEqC,GAAyB1C,EAAM,yBAA0B3I,EAAoB,CAACoL,KAC9EE,GAAwB3C,EAAM,wBAAyBxI,EAAmB,CAACkL,GAAwB7jB,EAAME,GAAMD,GAASoR,IACxHtC,GAAUoS,EAAM,UAAWT,GAAY,CAACvP,GAAa2S,GAAuBpf,GAAcC,KAC1FuK,GAAmBiS,EAAM,mBAAoBR,GAAqB,CAAC5R,GAASoC,GAAazM,GAAcC,GAAWoB,KAGlHS,G1BlIK,SAAuBud,EAAU3I,EAAWD,EAAW3Y,GAElE,MAAMwhB,EAAO,CACT5c,MAAO5E,EAAQyhB,wBAAwB7c,MACvCD,OAAQ3E,EAAQyhB,wBAAwB9c,QAEtCkU,EAAe,CACjB3T,KAAMlF,EAAQ8Y,WACd3T,IAAKnF,EAAQ+Y,WAGX2I,EAAiBH,GAAY/I,GAG7BR,EAASK,GADG,CAAEnT,KAAM,EAAGC,IAAK,KAAMyT,GACLD,GAC7B3U,EAAaqU,GAAS,IAAKQ,KAAiB2I,GAAQ7I,GACpDgJ,EAAqBla,EAAKuQ,EAAQG,EAAOnU,EAAYsU,KACrDsJ,EAAsBna,EAAKuQ,EAAQG,EAAOnU,EAAYuU,KAE5D,OAAKR,EAASC,EAAQ0J,IAGjB3J,EAAS2J,EAAgBC,GAG1B,EAAKD,GAAkB,EAAI,EAAKE,GACzBA,EAEJF,EARIE,CASf,C0BqGuBC,CAAcnD,GAAe1a,WAAY4U,GAAWD,GAAW3Y,GAGlF2e,EAAM,gBAAiBb,GAAkB,CAACrgB,GAAS6gB,EAAQ/e,wBAC3Dof,EAAM,aAAcb,GAAkB,CAACpgB,GAAM4gB,EAAQ5e,qBAErD/D,EAAQwH,MAAQ,CACZmb,UACAzb,mBACApC,cACAjD,OACAqR,UACA+H,kBACAG,eACAtZ,WACAC,QACA6F,YACAhF,iBACAqQ,aACA3G,aACA0G,eACAjO,eACAqgB,oBACA7c,wBACA+c,mBACAE,uBACAxI,aACAC,aACA3U,eACAD,cACArD,oBACA4K,kBACArJ,gBACAC,aACA/F,OACA6P,eACAE,mBACAC,gBACAG,WACAG,oBAER,CAEe,SAASoV,GAAYnmB,GAChC,IAAKA,EAAQ0P,MACT,IACIgT,GAAoB1iB,EACxB,CAAE,MAAO0P,GACL1P,EAAQ0P,MAAQA,CACpB,CAER,CI9Le,SAAS0W,GAAiBC,EAAeC,GACpD,MAAMrT,EAAY,IAAI2D,EAAU0P,GAChC,MAAO,IAAIA,KAAaD,EAAcrf,QAAO3D,IAAS4P,EAAU8D,aAAa1T,EAAKuD,MAAOvD,EAAKqD,YAClG,CCHe,SAAS6f,GAAgBF,EAAeG,GACnD,MAAMvT,EAAY,IAAI2D,EAAU4P,GAChC,OAAOH,EAAcrf,QAAO3D,IAAS4P,EAAU8D,aAAa1T,EAAKuD,MAAOvD,EAAKqD,WACjF,CCLe,SAAS+f,GAAiBC,GACrC,MACM7a,EADU6a,EAAMC,cACDb,wBACrB,MAAO,CACHra,EAAGib,EAAME,QAAU/a,EAAKtC,KACxBmC,EAAGgb,EAAMG,QAAUhb,EAAKrC,IAEhC,CCPO,SAASsd,GAAiBlc,EAAOmc,GACpC,OAAOnc,EAAM3K,KAAIoD,IAAQ,IAClBA,EACHqD,SAAU,OAAQrD,EAAOA,EAAKuB,GAAKmiB,EACnCngB,MAAO,OAAQvD,EAAOA,EAAKuB,GAAKmiB,KAExC,CCQA,SAASC,GAAW3iB,GAChB,GAAI,wBAAyBA,EAAS,OAItC,MAAMqD,EAAW,CACb,WAAYoI,SAAS2L,cAAc,UACnC,aAAc3L,SAAS2L,cAAc,UACrC,YAAa3L,SAAS2L,cAAc,UACpC,cAAe3L,SAAS2L,cAAc,UACtC,gBAAiB3L,SAAS2L,cAAc,UACxC,eAAgB3L,SAAS2L,cAAc,UACvC,cAAe3L,SAAS2L,cAAc,UACtC,gBAAiB3L,SAAS2L,cAAc,UACxC,eAAgB3L,SAAS2L,cAAc,WAErC9L,EAAQG,SAAS2L,cAAc,SAC/B7K,EAAUd,SAAS2L,cAAc,OAEvCpX,EAAQ4iB,aAAa,WAAY,KACjC5iB,EAAQ4iB,aAAa,QAAS,oQAC9B5iB,EAAQ6iB,UAAUpQ,IAAI,eACtBpP,EAAS,YAAYuf,aAAa,QAAS,+EAC3Cvf,EAAS,cAAcuf,aAAa,QAAS,sEAC7Cvf,EAAS,aAAauf,aAAa,QAAS,gFAC5Cvf,EAAS,eAAeuf,aAAa,QAAS,uEAC9Cvf,EAAS,iBAAiBuf,aAAa,QAAS,4CAChDvf,EAAS,gBAAgBuf,aAAa,QAAS,wEAC/Cvf,EAAS,eAAeuf,aAAa,QAAS,kFAC9Cvf,EAAS,iBAAiBuf,aAAa,QAAS,yEAChDvf,EAAS,gBAAgBuf,aAAa,QAAS,mFAC/CtX,EAAMsX,aAAa,QAAS,0NAC5BrW,EAAQqW,aAAa,QAAS,uGAC9BrW,EAAQqW,aAAa,UAAW,IAEhC,MAAMjnB,EAAU,CACZ6iB,gBAAiB,CAAC,EAClBrb,MAAO,KACPsb,OAAQ,CAAC,EACTze,QAASA,EACTqD,SAAUA,EACViI,MAAOA,EACPiB,QAASA,EACTuW,iBAAiB,EACjBrF,cAAe,KACfpE,aAAa,EACb2G,iBAAkB,IAAIjO,IACtBkO,eAAgB,IAAIlO,IAGxBpW,iBAA2B,KACnBA,EAAQmnB,kBACZnnB,EAAQmnB,iBAAkB,EAC1BC,uBAAsB,KAClBpnB,EAAQmnB,iBAAkB,EAC1BhB,GAAYnmB,GACZyP,EAAOzP,EAAQ,IACjB,EAGNA,iBAA2B,CAACqE,EAAS+B,EAAMihB,KACvChjB,EAAQijB,iBAAiBlhB,GAAOsgB,IAC5B,IACIW,EAASX,EACb,CACA,MAAOhX,GACHA,EAAM8B,QAAU,IAAIpL,aAAgBsJ,EAAM8B,UAC1CxR,EAAQ0P,MAAQA,EAChB1P,EAAQunB,kBACZ,IACF,GAGNvnB,EAAQ4iB,aAAe,CACnB/gB,KAAM,GACNC,QAAS,CAAC,CAAEsE,KAAM,eAClBrE,KAAM,CAAC,CAAEqE,KAAM,UAAY,CAAEA,KAAM,eACnCtG,WAAY,GACZuB,UAAW,GACXwD,QAAS,GACTtD,aAAc,EAAGM,OAAMxB,MAAKD,YAAayB,IAAOxB,EAAIuE,MAAMxE,EAAOwE,IACjE3C,UAAW,EACXE,aAAc,EACdE,WAAY,EACZE,YAAa,EACbuC,YAAa,EACbC,YAAa,KACbyiB,oBAAsBziB,IAClB/E,EAAQ4iB,aAAa7d,YAAcA,EACnC/E,EAAQunB,kBAAkB,EAE9B3kB,cAAe,GACfE,sBAAwBF,IACpB5C,EAAQ4iB,aAAahgB,cAAgBA,EACrC5C,EAAQunB,kBAAkB,EAE9BviB,iBAAkB,GAClBtC,YAAa,GACbO,oBAAsBP,IAElB1C,EAAQ4iB,aAAalgB,YAAcA,EACnC1C,EAAQunB,kBAAkB,EAE9B9kB,QAAS,GACTO,gBAAkBP,IACdzC,EAAQ4iB,aAAangB,QAAUA,EAC/BzC,EAAQunB,kBAAkB,EAE9BxV,OAAQ,GACR0V,eAAiB1V,IACb/R,EAAQ4iB,aAAa7Q,OAASA,EAC9B/R,EAAQunB,kBAAkB,EAE9BnkB,YAAa,OACbO,kBAAmB,OACnBuB,aAAc,GACdwiB,qBAAuBxiB,IACnBlF,EAAQ4iB,aAAa1d,aAAeA,EACpClF,EAAQunB,kBAAkB,EAE9BpiB,WAAY,GACZwiB,mBAAqBxiB,IACjBnF,EAAQ4iB,aAAazd,WAAaA,EAClCnF,EAAQunB,kBAAkB,EAE9B3jB,sBAAuB,OACvBG,mBAAoB,QAGxBM,EAAQ,uBAAyBrE,EAEjC,MAAM4nB,EAAWnnB,IACbkP,EAAMhQ,MAAQc,EACdkP,EAAMkY,cAAc,IAAIC,MAAM,SAAS,EAGrCC,EAAU9mB,IACZ,MAAM2B,EAAgB5C,EAAQwH,MAAMmb,QAAQ/f,cACtC0D,EAAiBtG,EAAQwH,MAAMge,oBAC/Bjf,EAAevG,EAAQwH,MAAMjB,aAC7BC,EAAYxG,EAAQwH,MAAMhB,UAC1B/F,EAAOT,EAAQwH,MAAM/G,KACrB6P,EAActQ,EAAQwH,MAAM8I,YAC5B0X,EAAiBhoB,EAAQwH,MAAMmb,QAAQ1f,oBACvCglB,EAAajoB,EAAQwH,MAAMmb,QAAQ3f,gBAGnCsb,EAAgBjY,EAAiBzD,EAAe0D,EAAgBC,EAAcC,GAEpF,GAAa,KAAT/F,EACA,OACJ,IAAK6P,EACD,OACJ,GAAIrP,IAAeqd,EAAcE,OAAMnb,GAAQA,EAAKxC,KAAKI,aACrD,OAEJ,MAAMinB,EAAY5J,EAActX,QAAO3D,GAAsB,SAAdA,EAAK+C,OAC9C+hB,EAAc7J,EAActX,QAAO3D,GAAsB,WAAdA,EAAK+C,OAZ/B,IAACwE,IAcTsd,EAAUjoB,KAAIoD,IAAQ,IAAMA,EAAKA,KAAM1D,MAAO0D,EAAKxC,KAAKG,MAAM,CAAE6Q,OAAQpR,QAdrDunB,EAAe5B,GAAiBpmB,EAAQwH,MAAMmb,QAAQjgB,YAAakI,IAClF,CAACA,IAAUqd,EAAW7B,GAAiBU,GAAiB9mB,EAAQwH,MAAMmb,QAAQlgB,QAAS,UAAWmI,GAAO,EAc5Hwd,CAAWD,EAAYloB,KAAIoD,IAAQ,IAAMA,EAAKA,KAAM0S,WAAY1S,EAAKxC,KAAKG,MAAM,CAAE6Q,OAAQpR,SAErFQ,GACD2mB,EAAQ,GAAG,EAGbS,EAASpnB,IACX,MAAM2B,EAAgB5C,EAAQwH,MAAMmb,QAAQ/f,cACtColB,EAAiBhoB,EAAQwH,MAAMmb,QAAQ1f,oBACvCglB,EAAajoB,EAAQwH,MAAMmb,QAAQ3f,gBAMnCsb,EAAgBjY,EAAiBzD,EAHhB5C,EAAQwH,MAAMge,oBAChBxlB,EAAQwH,MAAMjB,aACjBvG,EAAQwH,MAAMhB,WAJN,IAACoE,EAOvB3J,IAAeqd,EAAcE,OAAMnb,GAAQA,EAAKxC,KAAKI,eAP9B2J,EAUThI,EAVmBolB,EAAezB,GAAgBvmB,EAAQwH,MAAMmb,QAAQjgB,YAAakI,IACjF,CAACA,IAAUqd,EAAW1B,GAAgBO,GAAiB9mB,EAAQwH,MAAMmb,QAAQlgB,QAAS,UAAWmI,GAAO,EAU9H0d,CAAc1lB,GAAc,EAKhC5C,EAAQsnB,iBAAiBjjB,EAAS,UAAWqiB,IAKzC1mB,EAAQunB,kBAAkB,IAG9BvnB,EAAQsnB,iBAAiBjjB,EAAS,cAAeqiB,IAC7C1mB,EAAQ8hB,cAAgB2E,GAAiBC,GACzC1mB,EAAQunB,kBAAkB,IAG9BvnB,EAAQsnB,iBAAiBjjB,EAAS,aAAcqiB,IAG5C,GAFA1mB,EAAQ8hB,cAAgB2E,GAAiBC,GAErC1mB,EAAQklB,eAAgB,CACxB,MAAM9kB,EAASJ,EAAQwH,MAAMjB,aAAaO,IAAItB,EAAYxF,EAAQklB,iBAC5DqD,EAAcnoB,EAAO6I,MACrBuf,EAAcpoB,EAAO6M,MACrB8U,EAAmBjF,GAAoBzY,EAASrE,EAAQ8hB,cAAe9hB,EAAQwH,MAAMwV,UAAWhd,EAAQwH,MAAMyV,WAC9GwL,EAAiBthB,KAAKgD,IAAI,GAAI4X,EAAiBtW,EAAI+c,EAAcD,GAEjEG,EADuB1oB,EAAQwH,MAAMmb,QAAQzd,aAE9C8B,QAAOuhB,GAAe/iB,EAAY+iB,EAAY7hB,YAActG,EAAOqF,MACnEjF,OAAO,CAAC,CAAEkG,SAAUtG,EAAOwE,GAAIqE,MAAOwf,KAC3CzoB,EAAQwH,MAAMmb,QAAQ+E,qBAAqBgB,EAC/C,CACA,GAAI1oB,EAAQmlB,YAAa,CACrB,MAAM9kB,EAAML,EAAQwH,MAAMhB,UAAUM,IAAItB,EAAYxF,EAAQmlB,cACtDwD,EAAYtoB,EAAI2I,OAChB4f,EAAYvoB,EAAIkN,OAChBwU,EAAmBjF,GAAoBzY,EAASrE,EAAQ8hB,cAAe9hB,EAAQwH,MAAMwV,UAAWhd,EAAQwH,MAAMyV,WAC9G4L,EAAe1hB,KAAKgD,IAAI,GAAI4X,EAAiBrW,EAAIkd,EAAYD,GAE7DG,EADqB9oB,EAAQwH,MAAMmb,QAAQxd,WAE5C6B,QAAO2hB,GAAanjB,EAAYmjB,EAAU/hB,SAAWvG,EAAIoF,MACzDjF,OAAO,CAAC,CAAEoG,MAAOvG,EAAIuE,GAAIoE,OAAQ6f,KACtC7oB,EAAQwH,MAAMmb,QAAQgF,mBAAmBmB,EAC7C,CAGA9oB,EAAQunB,kBAAkB,IAG9BvnB,EAAQsnB,iBAAiBjjB,EAAS,cAAc,KAC5CrE,EAAQ8hB,cAAgB,KACxB9hB,EAAQunB,kBAAkB,IAK9BvnB,EAAQsnB,iBAAiBjjB,EAAS,aAAcqiB,IAC5CP,GAAYnmB,GACZ4nB,EAAQ,IAER5nB,EAAQ0d,aAAc,EACtB1d,EAAQ+oB,kBAAoB/oB,EAAQ8hB,cACpC9hB,EAAQgpB,cAAgBhpB,EAAQwH,MAAMwL,YAElChT,EAAQwH,MAAMgJ,kBACdxQ,EAAQklB,eAAiBllB,EAAQwH,MAAMgJ,iBAEvCxQ,EAAQwH,MAAMiJ,eACdzQ,EAAQmlB,YAAcnlB,EAAQwH,MAAMiJ,cAEnCzQ,EAAQwH,MAAMgJ,iBAAoBxQ,EAAQwH,MAAMiJ,cACjDzQ,EAAQwH,MAAMmb,QAAQ6E,oBAAoBxnB,EAAQwH,MAAMwL,aAGvD0T,EAAMuC,SACPjpB,EAAQwH,MAAMmb,QAAQ7f,sBAAsB,IAEhD9C,EAAQunB,kBAAkB,IAG9BvnB,EAAQsnB,iBAAiBjjB,EAAS,WAAYqiB,IAC1CP,GAAYnmB,GAEZA,EAAQ0d,aAAc,EACtB1d,EAAQklB,eAAiB,KACzBllB,EAAQmlB,YAAc,KAEtBnlB,EAAQwH,MAAMmb,QAAQ7f,sBAAsBsjB,GAAiBpmB,EAAQwH,MAAMmb,QAAQ/f,cAAe5C,EAAQwH,MAAMxC,mBAChHhF,EAAQunB,kBAAkB,IAG9BvnB,EAAQsnB,iBAAiBjjB,EAAS,eAAgBqiB,IAC9C1mB,EAAQqE,QAAQ6kB,kBAAkBxC,EAAMyC,UAAU,IAGtDnpB,EAAQsnB,iBAAiBjjB,EAAS,aAAcqiB,IAC5C1mB,EAAQqE,QAAQ+kB,sBAAsB1C,EAAMyC,UAAU,IAG1DnpB,EAAQsnB,iBAAiBjjB,EAAS,SAAUqiB,IACxCP,GAAYnmB,GAEZ,MAAMqD,EAAOrD,EAAQwH,MAAMwL,YACrBgW,EAAgBhpB,EAAQgpB,cAE9B,GAAIhpB,EAAQwH,MAAMgJ,iBAAmBxQ,EAAQwH,MAAMiJ,aAC/C,OACJ,GAAa,OAATpN,EACA,OACJ,GAAImC,EAAYnC,EAAKqD,YAAclB,EAAYwjB,EAActiB,UACzD,OACJ,GAAIlB,EAAYnC,EAAKuD,SAAWpB,EAAYwjB,EAAcpiB,OACtD,OAEJ,MAAMxG,EAASJ,EAAQwH,MAAMjB,aAAaO,IAAItB,EAAYnC,EAAKqD,WACzDrG,EAAML,EAAQwH,MAAMhB,UAAUM,IAAItB,EAAYnC,EAAKuD,QACnDmL,EAAS/R,EAAQwH,MAAMmb,QAAQ5Q,OAE/BsX,EADiBrpB,EAAQwH,MAAMge,oBACLze,QAAQ1G,EAAKD,GACvCkpB,EAAkB,CACpBL,QAASvC,EAAMuC,QACfM,SAAU7C,EAAM6C,SAChBC,OAAQ9C,EAAM8C,OACdC,QAAS/C,EAAM+C,SAGnB,GAAIJ,EAASxoB,MAAMM,OAAQ,CACvB,MACMyQ,ECpUH,SAAyBvO,EAAMjD,EAAQC,EAAK6S,GACvD,MAAMvT,EAAQuT,EAAQa,cAAc1T,EAAIoF,IAAKrF,EAAOqF,KAC9CyN,EAAQqD,cAAclW,EAAIoF,IAAKrF,EAAOqF,KACtCpC,EAAK1D,MACLwB,EAASkC,EAAKxC,KAAKM,OAEzB,MAAsB,mBAAXA,EACAA,EAAO,CAACxB,UAEZwB,GAAQA,EAAOuoB,QAAQ/pB,GAAS,GAAKwB,EAAO2G,OACvD,CD0T6B6hB,CAAgBN,EAAUjpB,EAAQC,EADnCL,EAAQwH,MAAM0L,SAExB0W,EAAWzjB,EAAgB/F,EAAQC,GACxB,SAAbupB,GACA5pB,EAAQwH,MAAMmb,QAAQ1f,oBAAoBmjB,GAAiBpmB,EAAQwH,MAAMmb,QAAQjgB,YAAa,CAAC,IAAKW,EAAM1D,MAAOiS,MACpG,WAAbgY,GACA5pB,EAAQwH,MAAMmb,QAAQ3f,gBAAgBojB,GAAiBpmB,EAAQwH,MAAMmb,QAAQlgB,QAAS,CAAC,IAAKY,EAAM0S,WAAYnE,KACtH,MAAO,GAAoB,SAAhBxR,EAAOgG,MAAgC,SAAb/F,EAAI+F,KACrCpG,EAAQwH,MAAMmb,QAAQvf,YAAY,IAAKpD,EAAQwH,MAAMwL,eAAgBsW,SAClE,GAAoB,WAAhBlpB,EAAOgG,MAAkC,WAAb/F,EAAI+F,KACvCpG,EAAQwH,MAAMmb,QAAQhf,kBAAkB,IAAK3D,EAAQwH,MAAMwL,eAAgBsW,SACxE,GAAoB,WAAhBlpB,EAAOgG,MAAkC,WAAb/F,EAAI+F,KAAmB,CAC1D,MAAMyjB,EE7UH,SAAsB9X,EAAQ3R,EAAQC,EAAK4oB,GAGtD,SAASa,EAAc5pB,GACnB,MAAMwG,EAAW,aAAcxG,EAAOA,EAAKwG,SAAW,SAChDE,EAAQ,UAAW1G,EAAOA,EAAK0G,MAAQ,SAE7C,OAAOxG,EAAOqF,MAAQD,EAAYkB,IAAarG,EAAIoF,MAAQD,EAAYoB,EAC3E,CAUA,MAAMmjB,EAAgB,CAAC,MAAO,YAAQ/X,GAChCgY,EAAcjY,EAAOkY,KAAKH,GAC1BI,EAAiBH,EAAcL,QAAQM,GAAa9X,WACpDiY,EAAeJ,GAAeG,EAAiB,GAAKH,EAAcjiB,QAClEsiB,EAAarY,EAAO2X,QAAQM,KAAiBjY,EAAOjK,OAAS,EAOnE,MAAO,KANemhB,IAAYmB,GAAeJ,EAG3CjY,EAAO/K,QAAO9G,IAhBpB,SAAsCA,GAClC,MAAMwG,EAAW,aAAcxG,EAAOA,EAAKwG,SAAW,SAChDE,EAAQ,UAAW1G,EAAOA,EAAK0G,MAAQ,SAE7C,MAAuB,WAAhBxG,EAAOgG,MAAqBhG,EAAOqF,MAAQD,EAAYkB,IAC1C,WAAbrG,EAAI+F,MAAqB/F,EAAIoF,MAAQD,EAAYoB,EAC5D,CAU6ByjB,CAA6BnqB,KADpD6R,EAAO/K,QAAO9G,IAAS4pB,EAAc5pB,QAE1BiqB,EAAe,CAAC,CAAEzjB,SAAUtG,EAAOwE,GAAIgC,MAAOvG,EAAIuE,GAAIsN,UAAWiY,IAAkB,GAGxG,CF+S8BG,CAAavY,EAAQ3R,EAAQC,EAAKqmB,EAAMuC,SAC1DjpB,EAAQwH,MAAMmb,QAAQ8E,eAAeoC,GACrC7pB,EAAQwH,MAAMmb,QAAQ7f,sBAAsB,GAChD,KAGJ9C,EAAQsnB,iBAAiBjjB,EAAS,YAAaqiB,IAG3C,GAFAP,GAAYnmB,GAERA,EAAQwH,MAAMgJ,gBAAiB,CAC/B,MAAM+Z,EAAqB/kB,EAAYxF,EAAQwH,MAAMgJ,iBAC/CkY,EAAkB1oB,EAAQwH,MAAMmb,QAAQzd,aAAa8B,QAAOuhB,GAAe/iB,EAAY+iB,EAAY7hB,YAAc6jB,IACvHvqB,EAAQwH,MAAMmb,QAAQ+E,qBAAqBgB,GAC3C1oB,EAAQqkB,iBAAiBpE,OAAOsK,EACpC,CACA,GAAIvqB,EAAQwH,MAAMiJ,aAAc,CAC5B,MAAM+Z,EAAkBhlB,EAAYxF,EAAQwH,MAAMiJ,cAC5CqY,EAAgB9oB,EAAQwH,MAAMmb,QAAQxd,WAAW6B,QAAO2hB,GAAanjB,EAAYmjB,EAAU/hB,SAAW4jB,IAC5GxqB,EAAQwH,MAAMmb,QAAQgF,mBAAmBmB,GACzC9oB,EAAQskB,eAAerE,OAAOuK,EAClC,CAEA,MAAMzlB,EAAc/E,EAAQwH,MAAMzC,YAClC,GAAoB,OAAhBA,EACA,OAEJ,MAAMoO,EAAmB3N,EAAYT,EAAY2B,UAC3C0M,EAAgB5N,EAAYT,EAAY6B,OACxCL,EAAevG,EAAQwH,MAAMjB,aAC7BC,EAAYxG,EAAQwH,MAAMhB,UAC1BF,EAAiBtG,EAAQwH,MAAMge,oBAErC,IAAKjf,EAAaM,IAAIsM,GAClB,OACJ,IAAK3M,EAAUK,IAAIuM,GACf,OAEJ,MAAMhT,EAASmG,EAAaO,IAAIqM,GAC1B9S,EAAMmG,EAAUM,IAAIsM,GACpB/P,EAAOiD,EAAeS,QAAQ1G,EAAKD,GACnCK,EAAO4C,EAAK5C,KAEb4C,EAAKxC,OAENwC,EAAKxC,KAAKM,SAGdymB,EAAQnnB,GACRkP,GAAO8a,UAAQ,IAGnBzqB,EAAQsnB,iBAAiBjjB,EAAS,SAAS,KACnCsL,EAAM5H,eACN4H,EAAMK,MAAM,CAAEC,eAAe,GAAO,IAG5CjQ,EAAQsnB,iBAAiBjjB,EAAS,WAAYqiB,IAE1CP,GAAYnmB,GAEZ,MAAM+E,EAAc/E,EAAQwH,MAAMzC,YAC5BwB,EAAevG,EAAQwH,MAAMjB,aAC7BC,EAAYxG,EAAQwH,MAAMhB,UAC1B5D,EAAgB5C,EAAQwH,MAAMmb,QAAQ/f,cACtC8nB,EAAmB1qB,EAAQwH,MAAMmb,QAAQ7f,sBAEzC6nB,EAAiB3qB,EAAQwH,MAAMmb,QAAQ6E,oBACvC9kB,EAAc1C,EAAQwH,MAAMmb,QAAQjgB,YACpCslB,EAAiBhoB,EAAQwH,MAAMmb,QAAQ1f,oBACvCnB,EAAU9B,EAAQwH,MAAM1F,QACxBC,EAAO/B,EAAQwH,MAAMzF,KACrBtB,EAAOT,EAAQwH,MAAM/G,KACrB+kB,EAAsBxlB,EAAQwH,MAAMge,oBAEpCoF,EAAU,CAACvnB,EAAMqjB,KACnBiE,EAAetnB,GAEXqjB,EAAM6C,SAZsBmB,EAAiBtE,GAAiBxjB,EAa7C,CAACS,KAElBqnB,EAAiB,CAACrnB,GAAM,EAG1BwnB,EAAoB,CAACjhB,EAAQ8c,KAC/B,IAAK3hB,EACD,OAEJ,MAAMoO,EAAmB3N,EAAYT,EAAY2B,UACjD,IAAKH,EAAaM,IAAIsM,GAClB,OAEJ,MAAM2X,EAAqBvkB,EAAaO,IAAIqM,GAAkBxJ,MACxDohB,EAAiB5jB,KAAKgD,IAAI,EAAGhD,KAAKoV,IAAIza,EAAQgG,OAAS,EAAGgjB,EAAqBlhB,IACrF,GAAImhB,IAAmBD,EACnB,OAEJ,MAAME,EAAiB,CAAEpkB,MAAO7B,EAAY6B,MAAOF,SAAU5E,EAAQipB,GAAgBnmB,IAErFgmB,EAAQI,EAAgBtE,EAAM,EAG5BuE,EAAkB,CAACrhB,EAAQ8c,KAC7B,IAAK3hB,EACD,OAEJ,MAAMqO,EAAgB5N,EAAYT,EAAY6B,OAC9C,IAAKJ,EAAUK,IAAIuM,GACf,OAEJ,MAAM8X,EAAkB1kB,EAAUM,IAAIsM,GAAezJ,MAC/CwhB,EAAchkB,KAAKgD,IAAI,EAAGhD,KAAKoV,IAAIxa,EAAK+F,OAAS,EAAGojB,EAAkBthB,IAC5E,GAAIuhB,IAAgBD,EAChB,OAEJ,MAAMF,EAAiB,CAAEpkB,MAAO7E,EAAKopB,GAAavmB,GAAI8B,SAAU3B,EAAY2B,UAE5EkkB,EAAQI,EAAgBtE,EAAM,EAG5B0E,EAAiB,KACnB1E,EAAM0E,iBACN1E,EAAM2E,iBAAiB,EAqC3B,OAAQ3E,EAAMjhB,KACV,IAAK,SAlCQ,KAAThF,EACAmnB,EAAQ,IAEHhlB,EAAckF,OAAS,EAC5B4iB,EAAiB,CAAC3lB,IAEbrC,EAAYoF,OAAS,EAC1BkgB,EAAe,KAGf2C,EAAe,MACfD,EAAiB,KAyBjB,MACJ,IAAK,QACD3C,IACA,MACJ,IAAK,UAGDqD,IACAH,EAAgBvE,EAAMuC,SAAWlnB,EAAK+F,QAAU,EAAG4e,GACnD,MACJ,IAAK,YACD0E,IACAH,EAAgBvE,EAAMuC,QAAUlnB,EAAK+F,OAAS,EAAG4e,GACjD,MACJ,IAAK,YACD0E,IACAP,EAAkBnE,EAAMuC,SAAWnnB,EAAQgG,QAAU,EAAG4e,GACxD,MACJ,IAAK,aACD0E,IACAP,EAAkBnE,EAAMuC,QAAUnnB,EAAQgG,OAAS,EAAG4e,GACtD,MACJ,IAAK,SACL,IAAK,YACD2B,IACA,MACJ,IAAK,IA/Ce,CAAC3B,IACrB,IAAKA,EAAMuC,QACP,OAEJ,MAAMqC,EG5dH,SAA0B1oB,EAAed,EAASC,EAAMuE,GACnE,MAAMC,EAAe,IAAI6P,IAAItU,EAAQ7B,KAAIG,GAAU,CAACA,EAAOqF,IAAKrF,MAC1DoG,EAAY,IAAI4P,IAAIrU,EAAK9B,KAAII,GAAO,CAACA,EAAIoF,IAAKpF,MAC9CkrB,EAAmB3oB,EAAc3C,KAAIoD,IAAQ,CAC/CoD,UAAWjB,EAAYnC,EAAKqD,UAC5BC,OAAQnB,EAAYnC,EAAKuD,WACzBI,QAAO3D,GAAQkD,EAAaM,IAAIxD,EAAKoD,YAAcD,EAAUK,IAAIxD,EAAKsD,UACpE6kB,EAAkB,IAAI3U,IAAI0U,EAAiBtrB,KAAIoD,GAAQA,EAAKoD,aAC5DglB,EAAe,IAAI5U,IAAI0U,EAAiBtrB,KAAIoD,GAAQA,EAAKsD,UAE/D,GAAgC,IAA5B4kB,EAAiBzjB,OACjB,MAAO,GAEX,MAAMmL,EAAY,IAAI2D,EAAUhU,GAC1Bib,EAAiB1W,KAAKoV,OAAOgP,EAAiBtrB,KAAIoD,GAAQkD,EAAaO,IAAIzD,EAAKoD,WAAWkD,SAC3FmU,EAAiB3W,KAAKgD,OAAOohB,EAAiBtrB,KAAIoD,GAAQkD,EAAaO,IAAIzD,EAAKoD,WAAWkD,SAC3FoU,EAAc5W,KAAKoV,OAAOgP,EAAiBtrB,KAAIoD,GAAQmD,EAAUM,IAAIzD,EAAKsD,QAAQgD,SAClFqU,EAAc7W,KAAKgD,OAAOohB,EAAiBtrB,KAAIoD,GAAQmD,EAAUM,IAAIzD,EAAKsD,QAAQgD,SAElF+hB,EAAgB,GAEtB,IAAK,IAAI3gB,EAAWgT,EAAahT,GAAYiT,EAAajT,IAAY,CAClE,MAAM1K,EAAM0B,EAAKgJ,GACXpE,EAAStG,EAAIoF,IAEnB,GAAKgmB,EAAa5kB,IAAIF,GAAtB,CAGA,IAAK,IAAIqE,EAAc6S,EAAgB7S,GAAe8S,EAAgB9S,IAAe,CACjF,MAAM5K,EAAS0B,EAAQkJ,GACjBvE,EAAYrG,EAAOqF,IAEzB,GAAK+lB,EAAgB3kB,IAAIJ,GAAzB,CAGA,GAAIwM,EAAUS,cAAc/M,EAAQF,GAAY,CAC5C,MAAM4iB,EAAW/iB,EAAeS,QAAQ1G,EAAKD,GAAQK,KACrDirB,EAAc7hB,KAAKwf,EACvB,CAEIre,EAAc8S,GACd4N,EAAc7hB,KAAK,KARX,CAShB,CAEIkB,EAAWiT,GACX0N,EAAc7hB,KAAK,KAnBX,CAoBhB,CAEA,OAAO6hB,EAAc9lB,KAAK,GAC9B,CH2akC+lB,CAAiB/oB,EAAed,EAASC,EAAMyjB,GAErE,GAAIoG,UAAUC,UACVD,UAAUC,UAAUC,UAAUR,OAC3B,CACH,MAAMS,EAAWjc,SAAS2L,cAAc,YACxCsQ,EAASpsB,MAAQ2rB,EACjBxb,SAASkc,KAAK/jB,YAAY8jB,GAC1BA,EAAStB,SACT3a,SAASmc,YAAY,QACrBnc,SAASkc,KAAKhkB,YAAY+jB,EAC9B,GAiCIG,CAAgBxF,GAIxB,IAGJ,IAAIyF,gBAAe,KACfnsB,EAAQunB,kBAAkB,IAC3B6E,QAAQ/nB,GAEXrE,EAAQsnB,iBAAiB3X,EAAO,SAAU+W,IAEtCP,GAAYnmB,GAER0mB,EAAM2F,OAAO1sB,OACbooB,GAAO,GAEPpY,EAAMjP,MAAM4rB,QAAU,EACtB3c,EAAMjP,MAAM6rB,cAAgB,SAGxB7F,EAAM8F,WACNnE,GAAM,GAEV1Y,EAAMjP,MAAM4rB,QAAU,EACtB3c,EAAMjP,MAAM6rB,cAAgB,OAChC,IAGJvsB,EAAQsnB,iBAAiB3X,EAAO,SAAU+W,IACtCA,EAAM2E,iBAAiB,IAG3BrrB,EAAQsnB,iBAAiB3X,EAAO,YAAa+W,IACzCA,EAAM2E,iBAAiB,IAG3BrrB,EAAQsnB,iBAAiB3X,EAAO,aAAc+W,IAC1CA,EAAM2E,iBAAiB,IAG3BrrB,EAAQsnB,iBAAiB3X,EAAO,WAAY+W,IACxC,OAAQA,EAAMjhB,KACV,IAAK,QACL,IAAK,SACD,MACJ,IAAK,SACL,IAAK,YACL,IAAK,UACL,IAAK,YACL,IAAK,YACL,IAAK,aACmB,KAAhBkK,EAAMhQ,QACN+mB,EAAM2E,kBACNrrB,EAAQunB,oBAEZ,MACJ,QACIb,EAAM2E,kBAENrrB,EAAQunB,mBAEhB,GAER,CAEe,SAAShjB,GAAWF,EAASse,GAGxCqE,GAAW3iB,GAEX,MAAMrE,EAAUqE,EAAQ,uBACxBrE,EAAQ6iB,gBAAkBF,EAEJ,OAAlB3iB,EAAQwH,OACR2e,GAAYnmB,GAEZyP,EAAOzP,IAGPA,EAAQunB,kBAEhB,C,GI7lBIkF,yBAA2B,CAAC,EAGhC,SAASC,oBAAoBC,GAE5B,IAAIC,EAAeH,yBAAyBE,GAC5C,QAAqB3a,IAAjB4a,EACH,OAAOA,EAAatnB,QAGrB,IAAID,EAASonB,yBAAyBE,GAAY,CAGjDrnB,QAAS,CAAC,GAOX,OAHAunB,oBAAoBF,GAAUtnB,EAAQA,EAAOC,QAASonB,qBAG/CrnB,EAAOC,OACf,CCrBAonB,oBAAoBnpB,EAAK8B,IACxB,IAAIynB,EAASznB,GAAUA,EAAO0nB,WAC7B,IAAO1nB,EAAiB,QACxB,IAAM,EAEP,OADAqnB,oBAAoBM,EAAEF,EAAQ,CAAE1jB,EAAG0jB,IAC5BA,CAAM,ECLdJ,oBAAoBM,EAAI,CAAC1nB,EAAS2nB,KACjC,IAAI,IAAIxnB,KAAOwnB,EACXP,oBAAoBQ,EAAED,EAAYxnB,KAASinB,oBAAoBQ,EAAE5nB,EAASG,IAC5EK,OAAOqnB,eAAe7nB,EAASG,EAAK,CAAE2nB,YAAY,EAAMtmB,IAAKmmB,EAAWxnB,IAE1E,ECNDinB,oBAAoBQ,EAAI,CAACG,EAAKC,IAAUxnB,OAAOynB,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFZ,oBAAoB7T,EAAKvT,IACH,oBAAXooB,QAA0BA,OAAOC,aAC1C7nB,OAAOqnB,eAAe7nB,EAASooB,OAAOC,YAAa,CAAEhuB,MAAO,WAE7DmG,OAAOqnB,eAAe7nB,EAAS,aAAc,CAAE3F,OAAO,GAAO,ECL9D,IAAIiuB,iBAAmB,WACnB,IAAIC,EAAS/d,SAASge,cACtB,IAAKD,EAAQ,CAOT,IAHA,IAAIE,EAAcje,SAASke,qBAAqB,UAC5CC,EAAU,GAELC,EAAI,EAAGA,EAAIH,EAAYjmB,OAAQomB,IACpCD,EAAQpkB,KAAKkkB,EAAYG,IAI7BL,GADAI,EAAUA,EAAQjnB,QAAO,SAASmnB,GAAK,OAAQA,EAAEC,QAAUD,EAAE1tB,OAAS0tB,EAAEE,WAAa,KACpErkB,OAAO,GAAG,EAC/B,CAEA,OAAO6jB,CACX,EAEIS,cAAgB,SAAST,GACzB,MAAO,6BAA6BU,KAAKV,EAAOW,IACpD,EAMYC,IAQZ,GAZA3oB,OAAOqnB,eAAeT,oBAAqB,IAAK,CAC5C5lB,KAGQ2nB,IAFSb,mBAEIY,IAAIE,MAAM,KAAK1kB,MAAM,GAAI,GAAGpE,KAAK,KAAO,IAElD,WACH,OAAO6oB,GACX,KAIsB,oBAAnBE,eAAgC,CACvC,IAAIC,mBAAqBD,eACzBA,eAAiB,SAASE,GACtB,IAAIhB,EAASD,mBACTkB,EAAUR,cAAcT,GAExBW,EAAMI,mBAAmBC,GAE7B,IAAIC,EACA,OAAON,EAGX,IAAIO,EAAeP,EAAIE,MAAM,KACzBM,EAAgBD,EAAa/kB,OAAO,GAAG,GAAG0kB,MAAM,KAKpD,OAHAM,EAAcC,OAAO,EAAG,EAAG,qBAC3BF,EAAaE,QAAQ,EAAG,EAAGD,EAAcppB,KAAK,MAEvCmpB,EAAanpB,KAAK,IAC7B,CACJ,C",
+    "mappings": "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",
     "names": [
         "isString",
         "value",
         "String",
         "useResolvedFormatting",
         "formatting",
         "useMemo",
@@ -45,33 +45,45 @@
         "pinned_top",
         "pinnedBottom",
         "pinned_bottom",
         "pinnedLeft",
         "pinned_left",
         "pinnedRight",
         "pinned_right",
-        "filters",
-        "editedCells",
-        "edited_cells",
         "selectedCells",
         "selected_cells",
         "onSelectedCellsChange",
         "useCallback",
+        "filters",
         "onFiltersChange",
+        "editedCells",
+        "edited_cells",
         "onEditedCellsChange",
         "clickedCell",
         "clicked_cell",
         "onCellClick",
         "cell",
         "_objectSpread",
         "n",
         "current",
         "clickedCustomCell",
         "clicked_custom_cell",
         "onCustomCellClick",
+        "columnWidths",
+        "column_widths",
+        "onColumnWidthsChange",
+        "rowHeights",
+        "row_heights",
+        "onRowHeightsChange",
+        "columnsOrder",
+        "columns_order",
+        "onColumnsOrderChange",
+        "rowsOrder",
+        "rows_order",
+        "onRowsOrderChange",
         "onActiveColumnsChange",
         "activeColumns",
         "active_columns",
         "onActiveRowsChange",
         "activeRows",
         "active_rows",
         "_useState2",
@@ -86,16 +98,14 @@
         "PropTypes",
         "id",
         "sorting",
         "borderWidth",
         "focusedCell",
         "highlightedCells",
         "sort_by",
-        "columnWidths",
-        "rowHeights",
         "defaultProps",
         "module",
         "exports",
         "window",
         "stringifyId",
         "key",
         "Array",
@@ -268,17 +278,18 @@
         "preventScroll",
         "section",
         "gridArea",
         "zIndex",
         "backgroundColor",
         "isTextValid",
         "renderInput",
+        "isReordering",
+        "cursor",
         "resizableColumn",
         "resizableRow",
-        "cursor",
         "renderCursor",
         "tooltip",
         "content",
         "placement",
         "tooltipPlacement",
         "innerHTML",
         "showPopover",
@@ -311,14 +322,16 @@
         "getHighlightColor",
         "baseColor",
         "isStrong",
         "getRenderFormatting",
         "hoveredCell",
         "selection",
         "edition",
+        "reorderedColumn",
+        "reorderedRow",
         "focusedColumnKey",
         "focusedRowKey",
         "isResizingRow",
         "isResizing",
         "selectionBorderWidth",
         "resizableBorderWidth",
         "isSelected",
@@ -479,14 +492,15 @@
         "scrollTop",
         "clientSize",
         "clientWidth",
         "clientHeight",
         "getLookup",
         "getHighlightedCells",
         "isMouseDown",
+        "canHighlight",
         "hoveredColumnKey",
         "hoveredRowKey",
         "minColumnIndex",
         "maxColumnIndex",
         "minRowIndex",
         "maxRowIndex",
         "flatMap",
@@ -558,14 +572,18 @@
         "getActiveColumns",
         "callback",
         "getActive",
         "getContextFormatting",
         "getTooltip",
         "getTooltipPlacement",
         "cellPlacement",
+        "getOrder",
+        "order",
+        "getOrdered",
+        "mixedResult",
         "updateStateInternal",
         "options",
         "localOptions",
         "externalOptions",
         "memory",
         "previousState",
         "cache",
@@ -576,14 +594,16 @@
         "dataFormatting",
         "invokedColumns",
         "invokedRows",
         "unfilteredColumns",
         "unfilteredRows",
         "unfilteredColumnKeys",
         "unfilteredRowKeys",
+        "orderedColumns",
+        "orderedRows",
         "filterFormatting",
         "filterFormattingRules",
         "sortingFormatting",
         "sortingFormattingRules",
         "shapedColumns",
         "shapedRows",
         "measureFormatting",
@@ -600,14 +620,15 @@
         "floor",
         "getRowIndex",
         "hoverColumnIndex",
         "getColumnIndex",
         "getHoveredCell",
         "resizingColumn",
         "resizingRow",
+        "didReorder",
         "renderFormatting",
         "renderFormattingRules",
         "inputFormatting",
         "inputFormattingRules",
         "inputFormatResolver",
         "contextFormatting",
         "contextFormattingRules",
@@ -628,26 +649,32 @@
         "getMousePosition",
         "event",
         "currentTarget",
         "clientX",
         "clientY",
         "getWithAssumedId",
         "defaultId",
+        "findMove",
+        "focusedId",
+        "hoveredId",
+        "focusedKey",
+        "hoveredKey",
+        "focusedIndex",
+        "findIndex",
+        "hoveredIndex",
         "initialize",
         "setAttribute",
         "classList",
         "renderRequested",
         "requestAnimationFrame",
         "listener",
         "addEventListener",
         "requestNewRender",
         "onFocusedCellChange",
         "onSortByChange",
-        "onColumnWidthsChange",
-        "onRowHeightsChange",
         "setText",
         "dispatchEvent",
         "Event",
         "accept",
         "setEditedCells",
         "setFilters",
         "dataCells",
@@ -659,14 +686,23 @@
         "columnRight",
         "newColumnWidth",
         "newColumnWidths",
         "rowHeight",
         "rowBottom",
         "newRowHeight",
         "newRowHeights",
+        "reorderedColumns",
+        "move",
+        "to",
+        "adjustedTo",
+        "reordered",
+        "splice",
+        "getReorderedColumns",
+        "reorderedRows",
+        "getReorderedRows",
         "mouseDownPosition",
         "mouseDownCell",
         "ctrlKey",
         "setPointerCapture",
         "pointerId",
         "releasePointerCapture",
         "cellData",
@@ -756,16 +792,15 @@
         "url",
         "split",
         "jsonpScriptSrc",
         "__jsonpScriptSrc__",
         "chunkId",
         "isLocal",
         "srcFragments",
-        "fileFragments",
-        "splice"
+        "fileFragments"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/components/DashSpreadGrid.jsx",
         "webpack:///external window \"PropTypes\"",
         "webpack:///external window \"React\"",
         "webpack:///../lib/src/core-utils/stringifyId.js",
@@ -821,55 +856,58 @@
         "webpack:///../lib/src/state-utils/getResizable.js",
         "webpack:///../lib/src/state-utils/getResolvedSortBy.js",
         "webpack:///../lib/src/state-utils/getResolvedFilters.js",
         "webpack:///../lib/src/state-utils/getActive.js",
         "webpack:///../lib/src/state-utils/getContextFormatting.js",
         "webpack:///../lib/src/state-utils/getTooltip.js",
         "webpack:///../lib/src/state-utils/getTooltipPlacement.js",
+        "webpack:///../lib/src/state-utils/getOrder.js",
+        "webpack:///../lib/src/state-utils/getOrdered.js",
         "webpack:///../lib/src/core/state.js",
         "webpack:///../lib/src/state-utils/getHoveredCell.js",
         "webpack:///../lib/src/state-utils/getRowIndex.js",
         "webpack:///../lib/src/state-utils/getColumnIndex.js",
         "webpack:///../lib/src/state-utils/getCombinedCells.js",
         "webpack:///../lib/src/state-utils/getReducedCells.js",
         "webpack:///../lib/src/state-utils/getMousePosition.js",
         "webpack:///../lib/src/state-utils/getWithAssumedId.js",
+        "webpack:///../lib/src/state-utils/getReordered.js",
         "webpack:///../lib/src/index.js",
         "webpack:///../lib/src/state-utils/getToggledValue.js",
         "webpack:///../lib/src/state-utils/getNewSortBy.js",
         "webpack:///../lib/src/state-utils/getClipboardData.js",
         "webpack:///webpack/bootstrap",
         "webpack:///webpack/runtime/compat get default export",
         "webpack:///webpack/runtime/define property getters",
         "webpack:///webpack/runtime/hasOwnProperty shorthand",
         "webpack:///webpack/runtime/make namespace object",
         "webpack:///webpack/runtime/compat"
     ],
     "sourcesContent": [
-        "/* eslint-disable import/prefer-default-export */\n\nimport React, { useCallback, useMemo, useRef, useState } from 'react';\nimport PropTypes from 'prop-types';\nimport createGrid from 'js-spread-grid';\n\nfunction isString(value) {\n    return typeof value === 'string' || value instanceof String;\n}\n\nfunction useResolvedFormatting(formatting) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, newValue, text, string, ctx}';\n\n        return formatting.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n            if ('value' in rule)\n                mappedRule.value = eval(`(${context})=> (${rule.value})`);\n            if ('text' in rule)\n                mappedRule.text = eval(`(${context}) => (${rule.text})`);\n            if ('style' in rule)\n                mappedRule.style = isString(rule.style) ? eval(`(${context}) => (${rule.style})`) : rule.style;\n            if ('padding' in rule)\n                mappedRule.padding = isString(rule.padding) ? eval(`(${context}) => (${rule.padding})`) : rule.padding;\n            if ('draw' in rule)\n                mappedRule.draw = eval(`(${context}) => {${rule.draw}}`);\n            if ('edit' in rule)\n                if (rule.edit) {\n                    const mappedEdit = {};\n                    if ('validate' in rule.edit)\n                        mappedEdit.validate = eval(`({string}) => (${rule.edit.validate})`);\n                    if ('parse' in rule.edit)\n                        mappedEdit.parse = eval(`(${context}) => (${rule.edit.parse})`);\n                    if ('auto_commit' in rule.edit)\n                        mappedEdit.autoCommit = rule.edit.auto_commit;\n                    if ('toggle' in rule.edit)\n                        mappedEdit.toggle = rule.edit.toggle;\n                    mappedRule.edit = mappedEdit;\n                }\n                else {\n                    mappedRule.edit = rule.edit;\n                }\n\n            return mappedRule;\n        });\n    }, [formatting]);\n}\n\nfunction useResolvedFiltering(filtering) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, text, expression}';\n\n        return filtering.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n\n            return mappedRule;\n        });\n    }, [filtering]);\n}\n\nfunction useResolvedDataSelector(dataSelector) {\n    return useMemo(() => {\n        return eval(`({data, row, column}) => (${dataSelector})`);\n    }, [dataSelector]);\n}\n\n// TODO: Write description\n// TODO: Rename to DashSpreadGrid\nfunction DashSpreadGrid(props) {\n    // console.count('render DashSpreadGrid');\n\n    const setProps = props.setProps;\n    const counter = useRef(0);\n\n    const data = props.data;\n    const columns = props.columns;\n    const rows = props.rows;\n    const formatting = useResolvedFormatting(props.formatting);\n    const filtering = useResolvedFiltering(props.filtering);\n    const dataSelector = useResolvedDataSelector(props.data_selector);\n    const pinnedTop = props.pinned_top;\n    const pinnedBottom = props.pinned_bottom;\n    const pinnedLeft = props.pinned_left;\n    const pinnedRight = props.pinned_right;\n    const filters = props.filters;\n    const editedCells = props.edited_cells;\n    const selectedCells = props.selected_cells;\n    const onSelectedCellsChange = useCallback((selectedCells) => {\n        setProps({ selected_cells: selectedCells });\n    }, [setProps]);\n    const onFiltersChange = useCallback((filters) => {\n        setProps({ filters });\n    }, [setProps]);\n    const onEditedCellsChange = useCallback((editedCells) => {\n        setProps({ edited_cells: editedCells });\n    }, [setProps]);\n    const clickedCell = props.clicked_cell;\n    const onCellClick = useCallback((cell) => {\n        setProps({ clicked_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const clickedCustomCell = props.clicked_custom_cell;\n    const onCustomCellClick = useCallback((cell) => {\n        setProps({ clicked_custom_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const onActiveColumnsChange = useCallback((activeColumns) => {\n        setProps({ active_columns: activeColumns });\n    }, [setProps]);\n    const onActiveRowsChange = useCallback((activeRows) => {\n        setProps({ active_rows: activeRows });\n    }, [setProps]);\n\n    const [element, setElement] = useState(null);\n\n    if (element)\n        createGrid(element, {\n            data,\n            columns,\n            rows,\n            formatting,\n            filtering,\n            pinnedTop,\n            pinnedBottom,\n            pinnedLeft,\n            pinnedRight,\n            filters,\n            dataSelector,\n            editedCells,\n            selectedCells,\n            onSelectedCellsChange,\n            onEditedCellsChange,\n            onFiltersChange,\n            clickedCell,\n            onCellClick,\n            clickedCustomCell,\n            onCustomCellClick,\n            onActiveColumnsChange,\n            onActiveRowsChange\n        });\n\n    return React.createElement(\"div\", { ref: setElement });\n};\n\n// TODO: add descriptions\n// TODO: Fix types\nDashSpreadGrid.propTypes = {\n    // _\n    setProps: PropTypes.func,\n    // _\n    id: PropTypes.string,\n    // _\n    data: PropTypes.any,\n    // _\n    columns: PropTypes.array,\n    // _\n    rows: PropTypes.array,\n    // _\n    formatting: PropTypes.array,\n    // _\n    filtering: PropTypes.array,\n    // _\n    sorting: PropTypes.array,\n    // _\n    data_selector: PropTypes.string,\n    // _\n    pinned_top: PropTypes.number,\n    // _\n    pinned_bottom: PropTypes.number,\n    // _\n    pinned_left: PropTypes.number,\n    // _\n    pinned_right: PropTypes.number,\n    // _\n    borderWidth: PropTypes.number,\n    // _\n    focusedCell: PropTypes.object,\n    // _\n    selected_cells: PropTypes.array,\n    // _\n    highlightedCells: PropTypes.array,\n    // _\n    edited_cells: PropTypes.array,\n    // _\n    filters: PropTypes.array,\n    // _\n    sort_by: PropTypes.array,\n    // _\n    columnWidths: PropTypes.array,\n    // _\n    rowHeights: PropTypes.array,\n    // _\n    clicked_cell: PropTypes.object,\n    // _\n    clicked_custom_cell: PropTypes.object,\n    // _\n    active_columns: PropTypes.array,\n    // _\n    active_rows: PropTypes.array\n};\n\nDashSpreadGrid.defaultProps = {\n    data: [],\n    columns: [{ \"type\": \"DATA-BLOCK\" }],\n    rows: [{ \"type\": \"HEADER\" }, { \"type\": \"DATA-BLOCK\" }],\n    formatting: [],\n    filtering: [],\n    sorting: [],\n    data_selector: \"data[row.id][column.id]\",\n    pinned_top: 0,\n    pinned_bottom: 0,\n    pinned_left: 0,\n    pinned_right: 0,\n    borderWidth: 1,\n    focusedCell: null,\n    selected_cells: [],\n    highlightedCells: [],\n    edited_cells: [],\n    filters: [],\n    sort_by: [],\n    columnWidths: [],\n    rowHeights: [],\n    clicked_cell: null,\n    clicked_custom_cell: null,\n    active_columns: [],\n    active_rows: []\n};\n\nexport default DashSpreadGrid;\n",
+        "/* eslint-disable import/prefer-default-export */\n\nimport React, { useCallback, useMemo, useRef, useState } from 'react';\nimport PropTypes from 'prop-types';\nimport createGrid from 'js-spread-grid';\n\nfunction isString(value) {\n    return typeof value === 'string' || value instanceof String;\n}\n\nfunction useResolvedFormatting(formatting) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, newValue, text, string, ctx}';\n\n        return formatting.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n            if ('value' in rule)\n                mappedRule.value = eval(`(${context})=> (${rule.value})`);\n            if ('text' in rule)\n                mappedRule.text = eval(`(${context}) => (${rule.text})`);\n            if ('style' in rule)\n                mappedRule.style = isString(rule.style) ? eval(`(${context}) => (${rule.style})`) : rule.style;\n            if ('padding' in rule)\n                mappedRule.padding = isString(rule.padding) ? eval(`(${context}) => (${rule.padding})`) : rule.padding;\n            if ('draw' in rule)\n                mappedRule.draw = eval(`(${context}) => {${rule.draw}}`);\n            if ('edit' in rule)\n                if (rule.edit) {\n                    const mappedEdit = {};\n                    if ('validate' in rule.edit)\n                        mappedEdit.validate = eval(`({string}) => (${rule.edit.validate})`);\n                    if ('parse' in rule.edit)\n                        mappedEdit.parse = eval(`(${context}) => (${rule.edit.parse})`);\n                    if ('auto_commit' in rule.edit)\n                        mappedEdit.autoCommit = rule.edit.auto_commit;\n                    if ('toggle' in rule.edit)\n                        mappedEdit.toggle = rule.edit.toggle;\n                    mappedRule.edit = mappedEdit;\n                }\n                else {\n                    mappedRule.edit = rule.edit;\n                }\n\n            return mappedRule;\n        });\n    }, [formatting]);\n}\n\nfunction useResolvedFiltering(filtering) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, text, expression}';\n\n        return filtering.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n\n            return mappedRule;\n        });\n    }, [filtering]);\n}\n\nfunction useResolvedDataSelector(dataSelector) {\n    return useMemo(() => {\n        return eval(`({data, row, column}) => (${dataSelector})`);\n    }, [dataSelector]);\n}\n\n// TODO: Write description\n// TODO: Rename to DashSpreadGrid\nfunction DashSpreadGrid(props) {\n    // console.count('render DashSpreadGrid');\n\n    const setProps = props.setProps;\n    const counter = useRef(0);\n\n    const data = props.data;\n    const columns = props.columns;\n    const rows = props.rows;\n    const formatting = useResolvedFormatting(props.formatting);\n    const filtering = useResolvedFiltering(props.filtering);\n    const dataSelector = useResolvedDataSelector(props.data_selector);\n    const pinnedTop = props.pinned_top;\n    const pinnedBottom = props.pinned_bottom;\n    const pinnedLeft = props.pinned_left;\n    const pinnedRight = props.pinned_right;\n    const selectedCells = props.selected_cells;\n    const onSelectedCellsChange = useCallback((selectedCells) => {\n        setProps({ selected_cells: selectedCells });\n    }, [setProps]);\n    const filters = props.filters;\n    const onFiltersChange = useCallback((filters) => {\n        setProps({ filters });\n    }, [setProps]);\n    const editedCells = props.edited_cells;\n    const onEditedCellsChange = useCallback((editedCells) => {\n        setProps({ edited_cells: editedCells });\n    }, [setProps]);\n    const clickedCell = props.clicked_cell;\n    const onCellClick = useCallback((cell) => {\n        setProps({ clicked_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const clickedCustomCell = props.clicked_custom_cell;\n    const onCustomCellClick = useCallback((cell) => {\n        setProps({ clicked_custom_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const columnWidths = props.column_widths;\n    const onColumnWidthsChange = useCallback((columnWidths) => {\n        setProps({ column_widths: columnWidths });\n    }, [setProps]);\n    const rowHeights = props.row_heights;\n    const onRowHeightsChange = useCallback((rowHeights) => {\n        setProps({ row_heights: rowHeights });\n    }, [setProps]);\n    const columnsOrder = props.columns_order;\n    const onColumnsOrderChange = useCallback((columnsOrder) => {\n        setProps({ columns_order: columnsOrder });\n    }, [setProps]);\n    const rowsOrder = props.rows_order;\n    const onRowsOrderChange = useCallback((rowsOrder) => {\n        setProps({ rows_order: rowsOrder });\n    }, [setProps]);\n    const onActiveColumnsChange = useCallback((activeColumns) => {\n        setProps({ active_columns: activeColumns });\n    }, [setProps]);\n    const onActiveRowsChange = useCallback((activeRows) => {\n        setProps({ active_rows: activeRows });\n    }, [setProps]);\n\n    const [element, setElement] = useState(null);\n\n    if (element)\n        createGrid(element, {\n            data,\n            columns,\n            rows,\n            formatting,\n            filtering,\n            pinnedTop,\n            pinnedBottom,\n            pinnedLeft,\n            pinnedRight,\n            dataSelector,\n            selectedCells,\n            onSelectedCellsChange,\n            editedCells,\n            onEditedCellsChange,\n            filters,\n            onFiltersChange,\n            columnWidths,\n            onColumnWidthsChange,\n            rowHeights,\n            onRowHeightsChange,\n            columnsOrder,\n            onColumnsOrderChange,\n            rowsOrder,\n            onRowsOrderChange,\n            clickedCell,\n            onCellClick,\n            clickedCustomCell,\n            onCustomCellClick,\n            onActiveColumnsChange,\n            onActiveRowsChange\n        });\n\n    return React.createElement(\"div\", { ref: setElement });\n};\n\n// TODO: add descriptions\n// TODO: Fix types\nDashSpreadGrid.propTypes = {\n    // _\n    setProps: PropTypes.func,\n    // _\n    id: PropTypes.string,\n    // _\n    data: PropTypes.any,\n    // _\n    columns: PropTypes.array,\n    // _\n    rows: PropTypes.array,\n    // _\n    formatting: PropTypes.array,\n    // _\n    filtering: PropTypes.array,\n    // _\n    sorting: PropTypes.array,\n    // _\n    data_selector: PropTypes.string,\n    // _\n    pinned_top: PropTypes.number,\n    // _\n    pinned_bottom: PropTypes.number,\n    // _\n    pinned_left: PropTypes.number,\n    // _\n    pinned_right: PropTypes.number,\n    // _\n    borderWidth: PropTypes.number,\n    // _\n    focusedCell: PropTypes.object,\n    // _\n    selected_cells: PropTypes.array,\n    // _\n    highlightedCells: PropTypes.array,\n    // _\n    edited_cells: PropTypes.array,\n    // _\n    filters: PropTypes.array,\n    // _\n    sort_by: PropTypes.array,\n    // _\n    column_widths: PropTypes.array,\n    // _\n    row_heights: PropTypes.array,\n    // _\n    columns_order: PropTypes.array,\n    // _\n    rows_order: PropTypes.array,\n    // _\n    clicked_cell: PropTypes.object,\n    // _\n    clicked_custom_cell: PropTypes.object,\n    // _\n    active_columns: PropTypes.array,\n    // _\n    active_rows: PropTypes.array\n};\n\nDashSpreadGrid.defaultProps = {\n    data: [],\n    columns: [{ \"type\": \"DATA-BLOCK\" }],\n    rows: [{ \"type\": \"HEADER\" }, { \"type\": \"DATA-BLOCK\" }],\n    formatting: [],\n    filtering: [],\n    sorting: [],\n    data_selector: \"data[row.id][column.id]\",\n    pinned_top: 0,\n    pinned_bottom: 0,\n    pinned_left: 0,\n    pinned_right: 0,\n    borderWidth: 1,\n    focusedCell: null,\n    selected_cells: [],\n    highlightedCells: [],\n    edited_cells: [],\n    filters: [],\n    sort_by: [],\n    column_widths: [],\n    row_heights: [],\n    columns_order: [],\n    rows_order: [],\n    clicked_cell: null,\n    clicked_custom_cell: null,\n    active_columns: [],\n    active_rows: []\n};\n\nexport default DashSpreadGrid;\n",
         "module.exports = window[\"PropTypes\"];",
         "module.exports = window[\"React\"];",
         "function stringifyObject(object) {\n    const keys = Object.keys(object).sort();\n    const stringified = keys.map(key => {\n        return `${key}:${stringifyId(object[key])}`\n    });\n\n    return `{${stringified.join(',')}}`;\n}\n\nfunction stringifyArray(array) {\n    const stringified = array.map(stringifyId);\n\n    return `[${stringified.join(',')}]`;\n}\n\nexport default function stringifyId(key) {\n    if (key === null)\n        return 'null'\n\n    if (Array.isArray(key))\n        return stringifyArray(key)\n\n    if (typeof key === 'object')\n        return stringifyObject(key)\n\n    return JSON.stringify(key)\n}",
         "export default function getCellEditType(column, row) {\n    if (column.type === 'FILTER' ^ row.type === 'FILTER')\n        return 'FILTER';\n    return 'DATA';\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellEditType from \"./getCellEditType.js\";\n\nexport default function getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup) {\n    return selectedCells.map(cell => {\n        const columnKey = stringifyId(cell.columnId);\n        const rowKey = stringifyId(cell.rowId);\n\n        if (!columnLookup.has(columnKey))\n            return null;\n        if (!rowLookup.has(rowKey))\n            return null;\n\n        const column = columnLookup.get(columnKey);\n        const row = rowLookup.get(rowKey);\n\n        return {\n            edit: formatResolver.resolve(row, column).edit,\n            cell: cell,\n            type: getCellEditType(column, row)\n        }\n    }).filter(cell => cell?.edit);\n}",
         "export default function roundToPixels(value, devicePixelRatio) {\n    return Math.round(value * devicePixelRatio) / devicePixelRatio;\n}",
-        "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    // console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            if (text) {\n                ctx.fillStyle = style.foreground || 'black';\n                ctx.font = cell.font;\n\n                const fontMetrics = textResolver.getFontMetrics(cell.font);\n\n                const textAlign = (style.textAlign == 'center' && textResolver.measureWidth(text, cell.font) > cellWidth - padding.left - padding.right)\n                    ? 'left'\n                    : style.textAlign || 'left';\n                ctx.textAlign = textAlign;\n\n                // TODO: Make sure that values are rounded using devicePixelRatio\n                const textX = roundToPixels(\n                    textAlign === 'left' ? padding.left :\n                        textAlign === 'center' ? cellWidth / 2 :\n                            textAlign === 'right' ? cellWidth - padding.right :\n                                0,\n                    devicePixelRatio\n                );\n\n                const textY = roundToPixels(\n                    textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                        textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                            textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                                0,\n                    devicePixelRatio\n                );\n\n                const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n                if (fitsVertically) {\n                    ctx.fillText(text, textX, textY);\n                }\n                else {\n                    // TODO: Clip if the text is too high (and draw some indicator if you do)\n                    ctx.strokeStyle = '#E9E9E9';\n                    ctx.lineWidth = borderWidth;\n\n                    ctx.beginPath();\n                    ctx.moveTo(0, borderWidth + borderOffset);\n                    ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                    ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                    ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                    ctx.stroke();\n\n                    ctx.save();\n                    setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                    ctx.fillText(text, textX, textY);\n\n                    ctx.restore();\n                }\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n        if (style.width === 0)\n            return;\n\n        const width = style.width / devicePixelRatio\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderTooltip(context) {\n    const element = context.element;\n    const tooltip = context.tooltip;\n    const content = context.state.tooltip;\n    const placement = context.state.tooltipPlacement;\n\n    if (!placement) {\n        if (tooltip.parentElement)\n            tooltip.parentElement.removeChild(tooltip);\n        return;\n    }\n\n    tooltip.innerHTML = content;\n    tooltip.style.left = `${placement.left}px`;\n    tooltip.style.top = `${placement.top}px`;\n\n    if (!tooltip.parentElement) {\n        element.appendChild(tooltip);\n        tooltip.showPopover();\n    }\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n    renderTooltip(context);\n}\n\nfunction renderError(context) {\n    if (context.errorRendered)\n        return;\n\n    context.errorRendered = true;\n\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.style.userSelect = 'text';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
+        "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    // console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            if (text) {\n                ctx.fillStyle = style.foreground || 'black';\n                ctx.font = cell.font;\n\n                const fontMetrics = textResolver.getFontMetrics(cell.font);\n\n                const textAlign = (style.textAlign == 'center' && textResolver.measureWidth(text, cell.font) > cellWidth - padding.left - padding.right)\n                    ? 'left'\n                    : style.textAlign || 'left';\n                ctx.textAlign = textAlign;\n\n                // TODO: Make sure that values are rounded using devicePixelRatio\n                const textX = roundToPixels(\n                    textAlign === 'left' ? padding.left :\n                        textAlign === 'center' ? cellWidth / 2 :\n                            textAlign === 'right' ? cellWidth - padding.right :\n                                0,\n                    devicePixelRatio\n                );\n\n                const textY = roundToPixels(\n                    textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                        textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                            textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                                0,\n                    devicePixelRatio\n                );\n\n                const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n                if (fitsVertically) {\n                    ctx.fillText(text, textX, textY);\n                }\n                else {\n                    // TODO: Clip if the text is too high (and draw some indicator if you do)\n                    ctx.strokeStyle = '#E9E9E9';\n                    ctx.lineWidth = borderWidth;\n\n                    ctx.beginPath();\n                    ctx.moveTo(0, borderWidth + borderOffset);\n                    ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                    ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                    ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                    ctx.stroke();\n\n                    ctx.save();\n                    setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                    ctx.fillText(text, textX, textY);\n\n                    ctx.restore();\n                }\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n        if (style.width === 0)\n            return;\n\n        const width = style.width / devicePixelRatio\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (context.isReordering)\n        element.style.cursor = 'move';\n    else if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderTooltip(context) {\n    const element = context.element;\n    const tooltip = context.tooltip;\n    const content = context.state.tooltip;\n    const placement = context.state.tooltipPlacement;\n\n    if (!placement) {\n        if (tooltip.parentElement)\n            tooltip.parentElement.removeChild(tooltip);\n        return;\n    }\n\n    tooltip.innerHTML = content;\n    tooltip.style.left = `${placement.left}px`;\n    tooltip.style.top = `${placement.top}px`;\n\n    if (!tooltip.parentElement) {\n        element.appendChild(tooltip);\n        tooltip.showPopover();\n    }\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n    renderTooltip(context);\n}\n\nfunction renderError(context) {\n    if (context.errorRendered)\n        return;\n\n    context.errorRendered = true;\n\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.style.userSelect = 'text';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
         "const filterRule = {\n    value: ({ newValue }) => newValue || '',\n    text: ({ newValue }) => newValue || 'Search...', // TODO: Move to render formatting?\n    edit: {\n        validate: () => true,\n        parse: ({ string }) => string,\n        autoCommit: true\n    }\n};\n\nexport default function getDataFormatting(formatting, dataSelector, sortBy) {\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'HEADER' },\n            value: ({ column }) => column.header === undefined ? column.id : column.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'DATA' },\n            value: ({ row }) => row.header === undefined ? row.id : row.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'SPECIAL' },\n            value: ''\n        },\n        {\n            column: { type: 'SPECIAL' },\n            row: { type: 'HEADER' },\n            value: ''\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            ...filterRule\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            ...filterRule\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'DATA' },\n            value: dataSelector\n        },\n        ...formatting,\n        // TODO: Fix headers of sorted rows\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            text: ({ value, text }) => `${sortBy.length > 1 ? index + 1 : ''}${direction === 'ASC' ? '\u21e3' : '\u21e1'} ${text || value}`\n        })),\n    ];\n}",
         "const commonFields = ['column', 'row', 'condition'];\n\nfunction reduce(rule, fields) {\n    const reducedRule = {};\n    for (const field of fields) {\n        if (field in rule)\n            reducedRule[field] = rule[field];\n    }\n    return reducedRule;\n}\n\nfunction hasImpact(rule) {\n    const allKeys = Object.keys(rule).length;\n    const commonKeys = Object.keys(rule).filter(key => commonFields.includes(key)).length;\n\n    return allKeys > commonKeys;\n}\n\nexport default function getReducedFormatting(formatting, fields) {\n    const acceptedFields = [...commonFields, ...fields];\n\n    return formatting.map(rule => reduce(rule, acceptedFields)).filter(hasImpact);\n}",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getInputFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'edit']);\n}",
-        "import stringifyId from '../core-utils/stringifyId.js';\n\nfunction getHighlightColor(baseColor, isStrong) {\n    if (isStrong)\n        return baseColor + '99';\n    else\n        return baseColor + '33';\n}\n\nexport default function getRenderFormatting(formatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, borderWidth) {\n    const focusedColumnKey = focusedCell ? stringifyId(focusedCell.columnId) : null;\n    const focusedRowKey = focusedCell ? stringifyId(focusedCell.rowId) : null;\n    const isResizingColumn = resizableColumn !== null;\n    const isResizingRow = resizableRow !== null;\n    const isResizing = isResizingColumn || isResizingRow;\n    const selectionBorderWidth = borderWidth + 2;\n    const resizableBorderWidth = borderWidth + 4;\n\n    const isSelected = (rows, columns, rowIndex, columnIndex) => {\n        if (rowIndex < 0 || rowIndex >= rows.length)\n            return false;\n        if (columnIndex < 0 || columnIndex >= columns.length)\n            return false;\n\n        const rowKey = rows[rowIndex].key;\n        const columnKey = columns[columnIndex].key;\n\n        return selection.isKeySelected(rowKey, columnKey);\n    };\n\n    const optional = (condition, style) => {\n        if (condition)\n            return [style];\n        else\n            return [];\n    }\n\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'HEADER' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'ANY' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'HEADER' },\n            style: { background: '#E0E0E0' }\n        },\n        ...formatting,\n        // TODO: optionally re-enable\n        // ...optional(hoveredCell && !isResizingColumn, {\n        //     column: { id: hoveredCell?.columnId },\n        //     row: { type: 'ANY' },\n        //     style: { highlight: '#81948133' },\n        // }),\n        ...optional(hoveredCell && !isResizingRow, {\n            column: { type: 'ANY' },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948133' },\n        }),\n        ...optional(hoveredCell && !isResizing, {\n            column: { id: hoveredCell?.columnId },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948188' },\n        }),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ rows, columns, row, column }) => isSelected(rows, columns, row.index, column.index),\n            style: ({ rows, columns, row, column, edit }) => ({\n                ...(!isSelected(rows, columns, row.index - 1, column.index) ? { borderTop: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index + 1, column.index) ? { borderBottom: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index - 1) ? { borderLeft: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index + 1) ? { borderRight: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                highlight: getHighlightColor(edit ? '#798d9c' : '#819481', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            }),\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => highlight.isKeySelected(row.key, column.key),\n            style: ({ row, column }) => ({\n                highlight: getHighlightColor('#93a8b8', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            })\n        },\n        ...optional(focusedCell, {\n            column: { id: focusedCell?.columnId },\n            row: { id: focusedCell?.rowId },\n            style: { highlight: '#ffffffaa' }\n        }),\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            style: { highlight: '#0377fc44' }\n        })),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ edit }) => edit,\n            style: { corner: '#77777720' },\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => edition.hasValueByKey(row.key, column.key),\n            style: { corner: 'darkgreen' },\n        },\n        ...optional(resizableColumn, {\n            column: { id: resizableColumn },\n            row: { type: 'HEADER' },\n            style: { borderRight: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n        ...optional(resizableRow, {\n            column: { type: 'HEADER' },\n            row: { id: resizableRow },\n            style: { borderBottom: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n    ];\n}",
+        "import stringifyId from '../core-utils/stringifyId.js';\n\nfunction getHighlightColor(baseColor, isStrong) {\n    if (isStrong)\n        return baseColor + '99';\n    else\n        return baseColor + '33';\n}\n\nexport default function getRenderFormatting(formatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, borderWidth, isReordering, reorderedColumn, reorderedRow) {\n    const focusedColumnKey = focusedCell ? stringifyId(focusedCell.columnId) : null;\n    const focusedRowKey = focusedCell ? stringifyId(focusedCell.rowId) : null;\n    const isResizingColumn = resizableColumn !== null;\n    const isResizingRow = resizableRow !== null;\n    const isResizing = isResizingColumn || isResizingRow;\n    const selectionBorderWidth = borderWidth + 2;\n    const resizableBorderWidth = borderWidth + 4;\n\n    const isSelected = (rows, columns, rowIndex, columnIndex) => {\n        if (rowIndex < 0 || rowIndex >= rows.length)\n            return false;\n        if (columnIndex < 0 || columnIndex >= columns.length)\n            return false;\n\n        const rowKey = rows[rowIndex].key;\n        const columnKey = columns[columnIndex].key;\n\n        return selection.isKeySelected(rowKey, columnKey);\n    };\n\n    const optional = (condition, style) => {\n        if (condition)\n            return [style];\n        else\n            return [];\n    }\n\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'HEADER' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'ANY' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'HEADER' },\n            style: { background: '#E0E0E0' }\n        },\n        ...formatting,\n        // TODO: optionally re-enable\n        // ...optional(hoveredCell && !isResizingColumn, {\n        //     column: { id: hoveredCell?.columnId },\n        //     row: { type: 'ANY' },\n        //     style: { highlight: '#81948133' },\n        // }),\n        ...optional(hoveredCell && !isResizingRow, {\n            column: { type: 'ANY' },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948133' },\n        }),\n        ...optional(hoveredCell && !isResizing, {\n            column: { id: hoveredCell?.columnId },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948188' },\n        }),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ rows, columns, row, column }) => isSelected(rows, columns, row.index, column.index),\n            style: ({ rows, columns, row, column, edit }) => ({\n                ...(!isSelected(rows, columns, row.index - 1, column.index) ? { borderTop: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index + 1, column.index) ? { borderBottom: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index - 1) ? { borderLeft: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index + 1) ? { borderRight: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                highlight: getHighlightColor(edit ? '#798d9c' : '#819481', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            }),\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => highlight.isKeySelected(row.key, column.key),\n            style: ({ row, column }) => ({\n                highlight: getHighlightColor('#93a8b8', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            })\n        },\n        ...optional(focusedCell, {\n            column: { id: focusedCell?.columnId },\n            row: { id: focusedCell?.rowId },\n            style: { highlight: '#ffffffaa' }\n        }),\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            style: { highlight: '#0377fc44' }\n        })),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ edit }) => edit,\n            style: { corner: '#77777720' },\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => edition.hasValueByKey(row.key, column.key),\n            style: { corner: 'darkgreen' },\n        },\n        ...optional(resizableColumn, {\n            column: { id: resizableColumn },\n            row: { type: 'HEADER' },\n            style: { borderRight: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n        ...optional(resizableRow, {\n            column: { type: 'HEADER' },\n            row: { id: resizableRow },\n            style: { borderBottom: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n        ...optional(isReordering && reorderedColumn, {\n            column: { id: reorderedColumn },\n            row: { type: 'ANY' },\n            style: { highlight: '#3a74e055' },\n        }),\n        ...optional(isReordering && reorderedRow, {\n            column: { type: 'ANY' },\n            row: { id: reorderedRow },\n            style: { highlight: '#3a74e055' },\n        }),\n    ];\n}",
         "export default function getSections(columns, rows) {\n    const topLength = rows.filter(row => row.pinned === 'BEGIN').length; // TODO: optimize\n    const bottomLength = rows.filter(row => row.pinned === 'END').length;\n    const middleLength = rows.length - topLength - bottomLength;\n    const leftLength = columns.filter(column => column.pinned === 'BEGIN').length;\n    const rightLength = columns.filter(column => column.pinned === 'END').length;\n    const centerLength = columns.length - leftLength - rightLength;\n\n    const topRows = rows.slice(0, topLength);\n    const bottomRows = rows.slice(rows.length - bottomLength, rows.length);\n    const middleRows = rows.slice(topLength, rows.length - bottomLength);\n    const leftColumns = columns.slice(0, leftLength);\n    const rightColumns = columns.slice(columns.length - rightLength, columns.length);\n    const centerColumns = columns.slice(leftLength, columns.length - rightLength);\n\n    const hasTopRows = topLength > 0;\n    const hasBottomRows = bottomLength > 0;\n    const hasMiddleRows = middleLength > 0;\n    const hasLeftColumns = leftLength > 0;\n    const hasRightColumns = rightLength > 0;\n    const hasCenterColumns = centerLength > 0;\n\n    const topShowTopBorder = true;\n    const topShowBottomBorder = true;\n    const bottomShowTopBorder = hasMiddleRows || !hasTopRows;\n    const bottomShowBottomBorder = true;\n    const middleShowTopBorder = !hasTopRows;\n    const middleShowBottomBorder = !hasBottomRows;\n    const leftShowLeftBorder = true;\n    const leftShowRightBorder = true;\n    const rightShowLeftBorder = hasCenterColumns || !hasLeftColumns;\n    const rightShowRightBorder = true;\n    const centerShowLeftBorder = !hasLeftColumns;\n    const centerShowRightBorder = !hasRightColumns;\n\n    const getHeight = (rows, showTopBorder, showBottomBorder) => {\n        if (rows.length === 0)\n            return 0;\n\n        const top = showTopBorder ? rows.at(0).topWithBorder : rows.at(0).top;\n        const bottom = showBottomBorder ? rows.at(-1).bottomWithBorder : rows.at(-1).bottom;\n\n        return bottom - top;\n    }\n\n    const getWidth = (columns, showLeftBorder, showRightBorder) => {\n        if (columns.length === 0)\n            return 0;\n\n        const left = showLeftBorder ? columns.at(0).leftWithBorder : columns.at(0).left;\n        const right = showRightBorder ? columns.at(-1).rightWithBorder : columns.at(-1).right;\n\n        return right - left;\n    }\n\n    const topHeight = getHeight(topRows, topShowTopBorder, topShowBottomBorder);\n    const bottomHeight = getHeight(bottomRows, bottomShowTopBorder, bottomShowBottomBorder);\n    const middleHeight = getHeight(middleRows, middleShowTopBorder, middleShowBottomBorder);\n    const leftWidth = getWidth(leftColumns, leftShowLeftBorder, leftShowRightBorder);\n    const rightWidth = getWidth(rightColumns, rightShowLeftBorder, rightShowRightBorder);\n    const centerWidth = getWidth(centerColumns, centerShowLeftBorder, centerShowRightBorder);\n\n    return {\n        top: {\n            rows: topRows,\n            showTopBorder: topShowTopBorder,\n            showBottomBorder: topShowBottomBorder,\n            height: topHeight\n        },\n        bottom: {\n            rows: bottomRows,\n            showTopBorder: bottomShowTopBorder,\n            showBottomBorder: bottomShowBottomBorder,\n            height: bottomHeight\n        },\n        middle: {\n            rows: middleRows,\n            showTopBorder: middleShowTopBorder,\n            showBottomBorder: middleShowBottomBorder,\n            height: middleHeight\n        },\n        left: {\n            columns: leftColumns,\n            showLeftBorder: leftShowLeftBorder,\n            showRightBorder: leftShowRightBorder,\n            width: leftWidth\n        },\n        right: {\n            columns: rightColumns,\n            showLeftBorder: rightShowLeftBorder,\n            showRightBorder: rightShowRightBorder,\n            width: rightWidth\n        },\n        center: {\n            columns: centerColumns,\n            showLeftBorder: centerShowLeftBorder,\n            showRightBorder: centerShowRightBorder,\n            width: centerWidth\n        }\n    };\n}",
         "// TODO: Move\nexport default function getEditedCellsAndFilters(editedCells, filters) {\n    return [...editedCells, ...filters.map(filter => ({ columnId: filter.columnId, rowId: filter.rowId, value: filter.expression }))];\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\n// TODO: write unit tests\nexport default class Edition {\n    constructor(editedCells) {\n        this.lookup = new Map();\n\n        editedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Map());\n\n            this.lookup.get(rowKey).set(columnKey, cell.value);\n        });\n    }\n\n    hasValueByKey(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    getValueByKey(rowKey, columnKey) {\n        if (!this.hasValueByKey(rowKey, columnKey))\n            return undefined;\n\n        return this.lookup.get(rowKey).get(columnKey);\n    }\n\n    hasValueById(rowId, columnId) {\n        return this.hasValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n\n    getValueById(rowId, columnId) {\n        return this.getValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Edition from \"../types/Edition.js\";\n\n// TODO: Move\nexport default function getEdition(editedCellsAndFilters) {\n    return new Edition(editedCellsAndFilters);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default class Selection {\n    constructor(selectedCells) {\n        this.lookup = new Map();\n\n        selectedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Set());\n\n            this.lookup.get(rowKey).add(columnKey);\n        });\n    }\n\n    isKeySelected(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    isIdSelected(rowId, columnId) {\n        return this.isKeySelected(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getSelection(selectedCells) {\n    return new Selection(selectedCells);\n}\n",
         "export default function getInvoked(columnsOrRows, data) {\n    return typeof columnsOrRows === 'function'\n        ? columnsOrRows(data)\n        : columnsOrRows;\n}\n",
         "// TODO: Move\nexport default function getPinned(index, length, pinnedBegin, pinnedEnd) {\n    if (index < pinnedBegin)\n        return \"BEGIN\";\n    if (index >= length - pinnedEnd)\n        return \"END\";\n    return undefined;\n}\n",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            index: index,\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : 'width' in column\n                ? column.width\n                : 'fit'\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : 'height' in row\n                ? row.height\n                : 'fit'\n    }));\n}\n",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : 'width' in column\n                ? column.width\n                : 'fit'\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : 'height' in row\n                ? row.height\n                : 'fit'\n    }));\n}\n",
         "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nexport function getPlacedColumns(columns, devicePixelRatio, borderWidth) {\n    let left = borderWidth;\n\n    return columns.map((column, index) => {\n        const assignedWidth = 'width' in column ? column.width : 100;\n        const width = roundToPixels(assignedWidth, devicePixelRatio);\n        const newColumn = {\n            ...column,\n            index: index,\n            width: width,\n            leftWithBorder: left - borderWidth,\n            left: left,\n            right: left + width,\n            rightWithBorder: left + width + borderWidth\n        };\n\n        left += newColumn.width + borderWidth;\n\n        return newColumn;\n    });\n}\n\nexport function getPlacedRows(rows, devicePixelRatio, borderWidth) {\n    let top = borderWidth;\n\n    return rows.map((row, index) => {\n        const assignedHeight = 'height' in row ? row.height : 20;\n        const height = roundToPixels(assignedHeight, devicePixelRatio);\n        const newRow = {\n            ...row,\n            index: index,\n            height: height,\n            topWithBorder: top - borderWidth,\n            top: top,\n            bottom: top + height,\n            bottomWithBorder: top + height + borderWidth\n        };\n\n        top += newRow.height + borderWidth;\n\n        return newRow;\n    });\n}\n",
         "const defaultFont = '12px Calibri';\nconst defaultPadding = { top: 2, right: 5, bottom: 2, left: 5 };\n\nexport { defaultFont, defaultPadding };",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst typeMapping = {\n    'HEADER': ['HEADER'],\n    'FILTER': ['FILTER'],\n    'DATA': ['DATA'],\n    'CUSTOM': ['CUSTOM'],\n    'ANY': ['HEADER', 'DATA', 'FILTER', 'CUSTOM'],\n    'SPECIAL': ['HEADER', 'FILTER', 'CUSTOM'],\n    undefined: []\n};\n\nclass Lookup {\n    byKey = new Map();\n    byIndex = new Map(); // TODO: Should this be removed?\n    byLabel = new Map();\n    byType = new Map();\n}\n\nexport default class RulesLookup {\n    lookup = new Lookup();\n    hasRules = false;\n\n    addRule(column, row, rule) {\n        this.hasRules = true;\n\n        if (Array.isArray(column)) {\n            for (const c of column)\n                this.addRule(c, row, rule);\n            return;\n        }\n\n        if (Array.isArray(row)) {\n            for (const r of row)\n                this.addRule(column, r, rule);\n            return;\n        }\n\n        column = column\n            ? 'id' in column\n                ? { key: stringifyId(column.id) }\n                : column\n            : { type: 'DATA' };\n        row = row\n            ? 'id' in row\n                ? { key: stringifyId(row.id) }\n                : row\n            : { type: 'DATA' };\n\n        function addRowRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, []);\n\n            lookup.get(key).push(rule);\n        }\n\n        function addColumnRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, new Lookup());\n\n            if ('key' in row)\n                addRowRule(lookup.get(key).byKey, row.key);\n            if ('index' in row)\n                addRowRule(lookup.get(key).byIndex, row.index);\n            if ('label' in row)\n                addRowRule(lookup.get(key).byLabel, row.label);\n            for (const type of typeMapping[row.type])\n                addRowRule(lookup.get(key).byType, type);\n        }\n\n        if ('key' in column)\n            addColumnRule(this.lookup.byKey, column.key);\n        if ('index' in column)\n            addColumnRule(this.lookup.byIndex, column.index);\n        if ('label' in column)\n            addColumnRule(this.lookup.byLabel, column.label);\n        for (const type of typeMapping[column.type])\n            addColumnRule(this.lookup.byType, type);\n    }\n\n    getRules(column, row) {\n        const rules = [];\n\n        if (!this.hasRules)\n            return rules;\n\n        function gatherRules(newRules) {\n            for (const rule of newRules)\n                rules.push(rule);\n        }\n\n        function gatherRowRules(lookup) {\n            if (lookup.byKey.has(row.key))\n                gatherRules(lookup.byKey.get(row.key));\n            if (lookup.byIndex.has(row.index))\n                gatherRules(lookup.byIndex.get(row.index));\n            if (lookup.byType.has(row.type))\n                gatherRules(lookup.byType.get(row.type));\n            for (const label of row.labels) {\n                if (lookup.byLabel.has(label))\n                    gatherRules(lookup.byLabel.get(label));\n            }\n        }\n\n        if (this.lookup.byKey.has(column.key))\n            gatherRowRules(this.lookup.byKey.get(column.key));\n        if (this.lookup.byIndex.has(column.index))\n            gatherRowRules(this.lookup.byIndex.get(column.index));\n        if (this.lookup.byType.has(column.type))\n            gatherRowRules(this.lookup.byType.get(column.type));\n        for (const label of column.labels) {\n            if (this.lookup.byLabel.has(label))\n                gatherRowRules(this.lookup.byLabel.get(label));\n        }\n\n        return rules;\n    }\n};",
         "import { defaultFont, defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: ({ string }) => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return `${context.text}`;\n    if ('newValue' in context)\n        return `${context.newValue}`;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\nfunction getEdit(rule, context) {\n    if (rule.edit === false)\n        return undefined;\n    if (rule.edit === true)\n        return 'edit' in context ? context.edit : defaultEdit;\n    if ('edit' in context)\n        return { ...context.edit, ...rule.edit };\n    return { ...defaultEdit, ...rule.edit };\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated type rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            // TODO: Mark which rules are actually present and only check those in resolve\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('font' in rule)\n                entry.font = typeof rule.font === 'function' ? rule.font : () => rule.font;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('tooltip' in rule)\n                entry.tooltip = typeof rule.tooltip === 'function' ? rule.tooltip : () => rule.tooltip;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n        let font = defaultFont;\n        let tooltip = undefined;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('font' in rule)\n                font = rule.font(context);\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: getEdit(rule, context) };\n            if ('tooltip' in rule)\n                tooltip = rule.tooltip(context);\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding,\n            font\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context && context.edit !== undefined)\n            result.edit = context.edit;\n        if (tooltip !== undefined)\n            result.tooltip = tooltip;\n        if (draw !== undefined)\n            result.draw = draw;\n\n        return result;\n    }\n}",
         "import FormattingRules from \"../types/FormattingRules.js\";\n\nexport default function getFormattingRules(formatting) {\n    return new FormattingRules(formatting);\n}\n",
         "export default class FormatResolver {\n    constructor(formattingRules, data, rows, columns, edition) {\n        this.formattingRules = formattingRules;\n        this.data = data;\n        this.rows = rows;\n        this.columns = columns;\n        this.edition = edition;\n    }\n\n    resolve(row, column) {\n        return this.formattingRules.resolve(\n            this.data,\n            this.rows,\n            this.columns,\n            row,\n            column,\n            this.edition);\n    }\n}",
         "import FormatResolver from \"../types/FormatResolver.js\";\n\nexport default function getFormatResolver(formattingRules, data, rows, columns, edition) {\n    return new FormatResolver(formattingRules, data, rows, columns, edition);\n}\n",
@@ -878,15 +916,15 @@
         "export default function getTotalSize(columns, rows) {\n    return {\n        width: columns.length ? columns.at(-1).rightWithBorder : 0,\n        height: rows.length ? rows.at(-1).bottomWithBorder : 0\n    };\n}\n",
         "import { defaultFont } from \"../core-utils/defaults.js\";\n\nexport default class TextResolver {\n    constructor() {\n        this.canvas = document.createElement('canvas');\n        this.context = this.canvas.getContext('2d');\n        this.fontMetrics = new Map();\n    }\n\n    measureWidth(text, font) {\n        if (!text)\n            return 0;\n\n        const ctx = this.context;\n        ctx.font = font || defaultFont;\n        const textMetrics = ctx.measureText(text);\n\n        return textMetrics.width;\n    }\n\n    measureHeight(text, font) {\n        let lines = 1;\n        for (const char of text) {\n            if (char === '\\n')\n                lines++;\n        }\n\n        return lines * this.getFontMetrics(font).height;\n    }\n\n    getFontMetrics(font) {\n        const key = font;\n\n        if (this.fontMetrics.has(key))\n            return this.fontMetrics.get(key);\n\n        const ctx = this.context;\n\n        // TODO: Set other font properties\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText('X');\n\n        const middle = (textMetrics.actualBoundingBoxDescent - textMetrics.actualBoundingBoxAscent) / 2;\n        const topOffset = middle + textMetrics.fontBoundingBoxAscent;\n        const bottomOffset = textMetrics.fontBoundingBoxDescent - middle;\n        const height = textMetrics.fontBoundingBoxAscent + textMetrics.fontBoundingBoxDescent;\n\n        const fontMetrics = {\n            topOffset: topOffset,\n            middle: -middle,\n            bottomOffset: bottomOffset,\n            height: height\n        };\n\n        this.fontMetrics.set(key, fontMetrics);\n\n        return fontMetrics;\n    }\n}",
         "import TextResolver from \"../types/TextResolver.js\";\n\nexport default function getTextResolver() {\n    return new TextResolver();\n}\n",
         "export function contains(bounds, rect) {\n    return (\n        rect.top >= bounds.top &&\n        rect.left >= bounds.left &&\n        rect.top + rect.height <= bounds.top + bounds.height &&\n        rect.left + rect.width <= bounds.left + bounds.width\n    );\n}\n\nexport function clip(bounds, rect) {\n    const newRect = {\n        top: Math.max(bounds.top, rect.top),\n        left: Math.max(bounds.left, rect.left),\n        width: Math.min(bounds.left + bounds.width, rect.left + rect.width) - Math.max(bounds.left, rect.left),\n        height: Math.min(bounds.top + bounds.height, rect.top + rect.height) - Math.max(bounds.top, rect.top)\n    };\n\n    if (newRect.width >= 0 && newRect.height >= 0)\n        return newRect;\n\n    return {\n        top: bounds.top,\n        left: bounds.left,\n        width: 0,\n        height: 0\n    }\n}\n\nexport function expand(rect, margin) {\n    return {\n        top: rect.top - margin,\n        left: rect.left - margin,\n        width: rect.width + margin * 2,\n        height: rect.height + margin * 2\n    };\n}\n\nexport function area(rect) {\n    return rect.width * rect.height;\n}\n\nexport function subtract(rect, margin) {\n    return {\n        top: rect.top,\n        left: rect.left,\n        width: Math.max(0, rect.width - margin.left - margin.right),\n        height: Math.max(0, rect.height - margin.top - margin.bottom)\n    };\n}",
         "import { area, clip, contains, expand, subtract } from \"../core-utils/rect.js\";\n\nconst requiredMargin = 200;\nconst preloadedMargin = 400;\nconst emptyRect = {\n    left: 0,\n    top: 0,\n    width: 0,\n    height: 0\n};\n\nexport default function getScrollRect(previous, totalSize, fixedSize, element) {\n    // TODO: Is it optimal to use getBoundingClientRect()?\n    const size = {\n        width: element.getBoundingClientRect().width,\n        height: element.getBoundingClientRect().height\n    };\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const prevScrollRect = previous || emptyRect;\n\n    const totalRect = { left: 0, top: 0, ...totalSize };\n    const bounds = subtract(totalRect, fixedSize);\n    const scrollRect = subtract({ ...scrollOffset, ...size }, fixedSize);\n    const requiredScrollRect = clip(bounds, expand(scrollRect, requiredMargin));\n    const preloadedScrollRect = clip(bounds, expand(scrollRect, preloadedMargin));\n\n    if (!contains(bounds, prevScrollRect))\n        return preloadedScrollRect;\n\n    if (!contains(prevScrollRect, requiredScrollRect))\n        return preloadedScrollRect;\n\n    if (area(prevScrollRect) > 2 * area(preloadedScrollRect))\n        return preloadedScrollRect;\n\n    return prevScrollRect;\n}\n",
         "export default function getInternalPosition(element, position, fixedSize, totalSize) {\n  // TODO: sometimes mousePosition is outside of bounds and it crashes the click events\n  const x = position.x;\n  const y = position.y;\n\n  const scrollOffset = {\n    left: element.scrollLeft,\n    top: element.scrollTop\n  };\n\n  const clientSize = {\n    width: element.clientWidth,\n    height: element.clientHeight\n  };\n\n  return {\n    x: x <= fixedSize.left\n      ? x\n      : x >= clientSize.width // TODO: This will not work for resizing columns pinned to the right\n        ? x + scrollOffset.left\n        : x >= clientSize.width - fixedSize.right\n          ? totalSize.width - clientSize.width + x\n          : x + scrollOffset.left,\n    y: y <= fixedSize.top\n      ? y\n      : y >= clientSize.height // TODO: This will not work for resizing rows pinned to the bottom\n        ? y + scrollOffset.top\n        : y >= clientSize.height - fixedSize.bottom\n          ? totalSize.height - clientSize.height + y\n          : y + scrollOffset.top\n  };\n}",
         "export default function getLookup(elements) {\n    return elements.reduce((lookup, element) => lookup.set(element.key, element), new Map());\n}\n",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getHighlightedCells(isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup) {\n    if (!isMouseDown)\n        return [];\n    if (isResizing)\n        return [];\n    if (!hoveredCell)\n        return [];\n    if (!focusedCell)\n        return [];\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n    const hoveredColumnKey = stringifyId(hoveredCell.columnId);\n    const hoveredRowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return [];\n    if (!rowLookup.has(focusedRowKey))\n        return [];\n    if (!columnLookup.has(hoveredColumnKey))\n        return [];\n    if (!rowLookup.has(hoveredRowKey))\n        return [];\n\n    const minColumnIndex = Math.min(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const maxColumnIndex = Math.max(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const minRowIndex = Math.min(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n    const maxRowIndex = Math.max(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n\n    return columns.slice(minColumnIndex, maxColumnIndex + 1).flatMap(column => {\n        return rows.slice(minRowIndex, maxRowIndex + 1).map(row => {\n            return {\n                rowId: row.id,\n                columnId: column.id\n            };\n        });\n    });\n}\n",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getHighlightedCells(isMouseDown, canHighlight, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup) {\n    if (!isMouseDown)\n        return [];\n    if (!canHighlight)\n        return [];\n    if (!hoveredCell)\n        return [];\n    if (!focusedCell)\n        return [];\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n    const hoveredColumnKey = stringifyId(hoveredCell.columnId);\n    const hoveredRowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return [];\n    if (!rowLookup.has(focusedRowKey))\n        return [];\n    if (!columnLookup.has(hoveredColumnKey))\n        return [];\n    if (!rowLookup.has(hoveredRowKey))\n        return [];\n\n    const minColumnIndex = Math.min(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const maxColumnIndex = Math.max(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const minRowIndex = Math.min(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n    const maxRowIndex = Math.max(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n\n    return columns.slice(minColumnIndex, maxColumnIndex + 1).flatMap(column => {\n        return rows.slice(minRowIndex, maxRowIndex + 1).map(row => {\n            return {\n                rowId: row.id,\n                columnId: column.id\n            };\n        });\n    });\n}\n",
         "function getVerticalSection(row) {\n    if (row.pinned === \"BEGIN\")\n        return \"top\";\n    if (row.pinned === \"END\")\n        return \"bottom\";\n    return \"middle\";\n}\n\nfunction getHorizontalSection(column) {\n    if (column.pinned === \"BEGIN\")\n        return \"left\";\n    if (column.pinned === \"END\")\n        return \"right\";\n    return \"center\";\n}\n\nexport default function getCellSection(column, row) {\n    const verticalSection = getVerticalSection(row);\n    const horizontalSection = getHorizontalSection(column);\n\n    return `${verticalSection}-${horizontalSection}`;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellSection from \"./getCellSection.js\";\n\nexport default function getInputPlacement(cell, columnLookup, rowLookup, sections) {\n    if (!cell)\n        return null;\n\n    const columnKey = stringifyId(cell.columnId);\n    const rowKey = stringifyId(cell.rowId);\n\n    if (!columnLookup.has(columnKey))\n        return null;\n    if (!rowLookup.has(rowKey))\n        return null;\n\n    const column = columnLookup.get(columnKey);\n    const row = rowLookup.get(rowKey);\n\n    const position = {\n        width: column.width,\n        height: row.height,\n        section: getCellSection(column, row)\n    };\n\n    switch (row.pinned) {\n        case \"BEGIN\":\n            position.top = row.top;\n            break;\n        case \"END\":\n            position.bottom = sections.top.height + sections.middle.height + sections.bottom.height - row.top - row.height;\n            break;\n        default:\n            position.marginTop = row.top - sections.top.height;\n    }\n\n    switch (column.pinned) {\n        case \"BEGIN\":\n            position.left = column.left;\n            break;\n        case \"END\":\n            position.right = sections.left.width + sections.center.width + sections.right.width - column.left - column.width;\n            break;\n        default:\n            position.marginLeft = column.left - sections.left.width;\n    }\n\n    return position;\n}\n",
         "import getCellPlacement from \"./getCellPlacement.js\";\n\nexport default function getInputPlacement(editableCells, focusedCell, columnLookup, rowLookup, sections) {\n    if (editableCells.length === 0)\n        return null;\n\n    return getCellPlacement(focusedCell, columnLookup, rowLookup, sections);\n}\n",
         "export default function getIsTextValid(text, editableCells) {\n    return editableCells.every(cell => cell.edit.validate({ string: text }));\n}\n",
         "function getDefaultIds(elements) {\n    if (!Array.isArray(elements))\n        return Object.keys(elements);\n\n    return elements.map((_, index) => index);\n}\n\nfunction getDefaultRowIds(data) {\n    return getDefaultIds(data);\n}\n\nfunction getDefaultColumnIds(data) {\n    const keys = new Set();\n\n    if (Array.isArray(data)) {\n        for (const element of data) {\n            for (const id of getDefaultIds(element))\n                keys.add(id);\n        }\n    } else {\n        for (const key in data) {\n            for (const id of getDefaultIds(data[key]))\n                keys.add(id);\n        }\n    }\n\n    return [...keys];\n}\n\nexport function getUnfoldedColumns(columns, data) {\n    const hasDataBlocks = columns.some(column => column.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return columns;\n\n    const unfoldedColumns = [];\n\n    for (const column of columns) {\n        if (column.type === 'DATA-BLOCK') {\n            const ids = 'selector' in column\n                ? column.selector(data)\n                : getDefaultColumnIds(data);\n\n            for (const id of ids) {\n                unfoldedColumns.push({\n                    ...column,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedColumns.push(column);\n        }\n    }\n\n    return unfoldedColumns;\n}\n\nexport function getUnfoldedRows(rows, data) {\n    const hasDataBlocks = rows.some(row => row.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return rows;\n\n    const unfoldedRows = [];\n\n    for (const row of rows) {\n        if (row.type === 'DATA-BLOCK') {\n            const ids = 'selector' in row\n                ? row.selector(data)\n                : getDefaultRowIds(data);\n\n            for (const id of ids) {\n                unfoldedRows.push({\n                    ...row,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedRows.push(row);\n        }\n    }\n\n    return unfoldedRows;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst defaultCondition = ({ text, expression }) => text.includes(expression);\n\nexport default class FilteringRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'FILTER'),\n                condition: rule.condition || defaultCondition\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, value, text, filterLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return true;\n            if (column.type !== 'DATA')\n                return true;\n            if (!filterLookup.has('\"FILTER\"'))\n                return true;\n\n            return defaultCondition({ text, expression: filterLookup.get('\"FILTER\"') });\n        }\n\n        let context = { data, rows, columns, row, column, value, text };\n\n        for (const rule of rules) {\n            if (!filterLookup.has(rule.by))\n                continue;\n\n            const filterContext = { ...context, expression: filterLookup.get(rule.by) };\n\n            if (!rule.condition(filterContext))\n                return false;\n        }\n\n        return true;\n    }\n}",
         "import FilteringRules from \"../types/FilteringRules.js\";\n\nexport default function getFilteringRules(filtering) {\n    return new FilteringRules(filtering);\n}",
@@ -894,35 +932,38 @@
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getMeasureFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'font', 'padding']);\n}",
         "import { defaultPadding } from \"../core-utils/defaults.js\";\n\n// TODO: add expand and expand-data\n\nexport function getMeasuredColumns(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (columns.every(column => typeof column.width === 'number'))\n        return columns;\n\n    const measureColumn = column => {\n        const requestedWidth = column.width;\n\n        if (typeof requestedWidth === 'number')\n            return requestedWidth;\n\n        if (measuringCache.has(column.key)) {\n            const cached = measuringCache.get(column.key);\n\n            if (requestedWidth === 'fit-once' && !cached.dataOnly)\n                return cached.width;\n            if (requestedWidth === 'fit-data-once' && cached.dataOnly)\n                return cached.width;\n        }\n\n        let width = 0;\n        for (const row of rows) {\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data-once')\n                continue;\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.left + cell.padding.right;\n\n            const cellWidth = textResolver.measureWidth(text, font) + padding;\n\n            width = Math.max(width, cellWidth);\n        }\n\n        measuringCache.set(column.key, {\n            width,\n            dataOnly: requestedWidth === 'fit-data-once'\n        });\n\n        return width;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return columns.map(column => ({\n        ...column,\n        width: measureColumn(column)\n    }));\n}\n\nexport function getMeasuredRows(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (rows.every(row => typeof row.height === 'number'))\n        return rows;\n\n    const measureRow = row => {\n        const requestedHeight = row.height;\n\n        if (typeof requestedHeight === 'number')\n            return requestedHeight;\n\n        if (measuringCache.has(row.key)) {\n            const cached = measuringCache.get(row.key);\n\n            if (requestedHeight === 'fit-once' && !cached.dataOnly)\n                return cached.height;\n            if (requestedHeight === 'fit-data-once' && cached.dataOnly)\n                return cached.height;\n        }\n\n        let height = 0;\n        for (const column of columns) {\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data-once')\n                continue;\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.top + cell.padding.bottom;\n\n            const cellHeight = textResolver.measureHeight(text, font) + padding;\n\n            height = Math.max(height, cellHeight);\n        }\n\n        measuringCache.set(row.key, {\n            height,\n            dataOnly: requestedHeight === 'fit-data-once'\n        });\n\n        return height;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return rows.map(row => ({\n        ...row,\n        height: measureRow(row)\n    }));\n}",
         "export default function getKeys(entries) {\n    return new Set(entries.map(entry => entry.key));\n}\n",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getSortingFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text']);\n}",
         "import RulesLookup from \"./RulesLookup.js\";\nimport stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction defaultComparatorAsc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value < rhs.value;\n}\n\nfunction defaultComparatorDesc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value > rhs.value;\n}\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const comparatorAsc = rule.comparator\n                ? (lhs, rhs) => rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorAsc(lhs, rhs);\n            const comparatorDesc = rule.comparator\n                ? (lhs, rhs) => !rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorDesc(lhs, rhs);\n\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: comparatorAsc,\n                comparatorDesc: comparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        if (!sortByLookup.has(rule.by))\n            return null;\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
         "import SortingRules from \"../types/SortingRules.js\";\n\nexport default function getSortingRules(sorting) {\n    return new SortingRules(sorting);\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getSortByLookup(sortBy, primaryKey, secondaryKey) {\n    const sortByLookup = new Map();\n    for (const cell of sortBy) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!sortByLookup.has(primary))\n            sortByLookup.set(primary, new Map());\n\n        sortByLookup.get(primary).set(secondary, cell.direction);\n    }\n    return sortByLookup;\n}\n\nfunction flush(temp, result) {\n    temp.sort((lhs, rhs) => {\n        const result = lhs.comparator(lhs.cell, rhs.cell);\n        if (typeof result === 'number')\n            return result;\n        return result ? -1 : 1;\n    });\n    result.push(...temp.map(entry => entry.entity));\n    temp.length = 0;\n}\n\nexport function getSortedRows(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return rows;\n\n    const sortByLookup = getSortByLookup(sortBy, 'columnId', 'rowId');\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const sortedColumns = sortBy\n        .map(cell => stringifyId(cell.columnId))\n        .filter(key => columnLookup.has(key))\n        .map(key => columnLookup.get(key))\n        .reverse();\n\n    if (sortedColumns.length === 0)\n        return rows;\n\n    for (const column of sortedColumns) {\n        const result = [];\n        const temp = [];\n\n        for (const row of rows) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(column.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(row);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: row, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        rows = result;\n    }\n\n    return rows;\n}\n\nexport function getSortedColumns(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return columns;\n\n    const sortByLookup = getSortByLookup(sortBy, 'rowId', 'columnId');\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const sortedRows = sortBy\n        .map(cell => stringifyId(cell.rowId))\n        .filter(key => rowLookup.has(key))\n        .map(key => rowLookup.get(key))\n        .reverse();\n\n    if (sortedRows.length === 0)\n        return columns;\n\n    for (const row of sortedRows) {\n        const result = [];\n        const temp = [];\n\n        for (const column of columns) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(row.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(column);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: column, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        columns = result;\n    }\n\n    return columns;\n}",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const x = internalPosition.x;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const y = internalPosition.y;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, element, mousePosition, isReordering, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n    if (isReordering)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const x = internalPosition.x;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, element, mousePosition, isReordering, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n    if (isReordering)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const y = internalPosition.y;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
         "export default function getResolvedSortBy(sortBy) {\n    return sortBy.map(sort => ({\n        columnId: 'columnId' in sort ? sort.columnId : 'HEADER',\n        rowId: 'rowId' in sort ? sort.rowId : 'HEADER',\n        direction: sort.direction\n    }));\n}",
         "export default function getResolvedFilters(filters) {\n    return filters.map(filter => ({\n        columnId: 'columnId' in filter ? filter.columnId : 'FILTER',\n        rowId: 'rowId' in filter ? filter.rowId : 'FILTER',\n        expression: filter.expression\n    }));\n}",
         "function getActive(entries, callback) {\n    const ids = entries\n        .filter(entry => entry.type === 'DATA')\n        .map(entry => entry.id);\n\n    callback(ids);\n\n    return ids;\n}\n\nexport function getActiveColumns(columns, callback) {\n    return getActive(columns, callback);\n}\n\nexport function getActiveRows(rows, callback) {\n    return getActive(rows, callback);\n}",
         "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getContextFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'tooltip']);\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getTooltip(hoveredCell, formatResolver, columnLookup, rowLookup) {\n    if (!hoveredCell)\n        return null;\n\n    const columnKey = stringifyId(hoveredCell.columnId);\n    const rowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(columnKey))\n        return null;\n    if (!rowLookup.has(rowKey))\n        return null;\n\n    const row = rowLookup.get(rowKey);\n    const column = columnLookup.get(columnKey);\n\n    return formatResolver.resolve(row, column).tooltip;\n}",
         "import getCellPlacement from \"./getCellPlacement.js\";\n\nexport default function getTooltipPlacement(tooltip, focusedCell, columnLookup, rowLookup, sections) {\n    if (!tooltip)\n        return null;\n\n    const cellPlacement = getCellPlacement(focusedCell, columnLookup, rowLookup, sections);\n\n    if (!cellPlacement)\n        return null;\n\n    return {\n        top: cellPlacement.top,\n        left: cellPlacement.left\n    };\n}",
-        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\nimport getContextFormatting from \"../state-utils/getContextFormatting.js\";\nimport getTooltip from \"../state-utils/getTooltip.js\";\nimport getTooltipPlacement from \"../state-utils/getTooltipPlacement.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    // console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n    const element = context.element;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, options.borderWidth]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n    const contextFormatting = cache('contextFormatting', getContextFormatting, [dataFormatting]);\n    const contextFormattingRules = cache('contextFormattingRules', getFormattingRules, [contextFormatting]);\n    const contextFormatResolver = cache('contextFormatResolver', getFormatResolver, [contextFormattingRules, data, rows, columns, edition]);\n    const tooltip = cache('tooltip', getTooltip, [hoveredCell, contextFormatResolver, columnLookup, rowLookup]);\n    const tooltipPlacement = cache('tooltipPlacement', getTooltipPlacement, [tooltip, hoveredCell, columnLookup, rowLookup, sections]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n        tooltip,\n        tooltipPlacement,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getOrder(order) {\n    return order.map(id => stringifyId(id));\n}",
+        "export default function getOrdered(entries, order) {\n    if (!order) {\n        return entries;\n    }\n\n    const map = new Map();\n\n    for (const entry of entries) {\n        map.set(entry.key, entry);\n    }\n\n    const mixedResult = [];\n\n    for (const key of order) {\n        if (map.has(key)) {\n            mixedResult.push(map.get(key));\n            map.delete(key);\n        }\n    }\n\n    for (const entry of entries) {\n        if (map.has(entry.key)) {\n            mixedResult.push(map.get(entry.key));\n        }\n    }\n\n    return [\n        ...mixedResult.filter(entry => entry.pinned === \"BEGIN\"),\n        ...mixedResult.filter(entry => !entry.pinned),\n        ...mixedResult.filter(entry => entry.pinned === \"END\")\n    ]\n}",
+        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\nimport getContextFormatting from \"../state-utils/getContextFormatting.js\";\nimport getTooltip from \"../state-utils/getTooltip.js\";\nimport getTooltipPlacement from \"../state-utils/getTooltipPlacement.js\";\nimport getOrder from \"../state-utils/getOrder.js\";\nimport getOrdered from \"../state-utils/getOrdered.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    // console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n    const element = context.element;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n\n    // Resolving\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Ordering\n    const columnsOrder = cache('columnsOrder', getOrder, [options.columnsOrder]);\n    const rowsOrder = cache('rowsOrder', getOrder, [options.rowsOrder]);\n    const orderedColumns = cache('orderedColumns', getOrdered, [unfilteredColumns, columnsOrder]);\n    const orderedRows = cache('orderedRows', getOrdered, [unfilteredRows, rowsOrder]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, orderedRows, orderedColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, orderedRows, orderedColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const isReordering = context.isReordering;\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, isReordering, fixedSize, totalSize]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, isReordering, fixedSize, totalSize]);\n    const isMouseDown = context.isMouseDown;\n    const canHighlight = !resizableColumn && !resizableRow && !context.didReorder;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, canHighlight, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, options.borderWidth, isReordering, context.reorderedColumn, context.reorderedRow]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n    const contextFormatting = cache('contextFormatting', getContextFormatting, [dataFormatting]);\n    const contextFormattingRules = cache('contextFormattingRules', getFormattingRules, [contextFormatting]);\n    const contextFormatResolver = cache('contextFormatResolver', getFormatResolver, [contextFormattingRules, data, rows, columns, edition]);\n    const tooltip = cache('tooltip', getTooltip, [hoveredCell, contextFormatResolver, columnLookup, rowLookup]);\n    const tooltipPlacement = cache('tooltipPlacement', getTooltipPlacement, [tooltip, hoveredCell, columnLookup, rowLookup, sections]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n        tooltip,\n        tooltipPlacement,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
         "import getColumnIndex from \"./getColumnIndex.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\nimport getRowIndex from \"./getRowIndex.js\";\n\nexport default function getHoveredCell(element, mousePosition, rows, columns, fixedSize, totalSize) {\n    if (!mousePosition)\n        return null;\n    if (mousePosition.x < 0 || mousePosition.y < 0 || mousePosition.x > totalSize.width || mousePosition.y > totalSize.height)\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    const hoverRowIndex = getRowIndex(rows, internalPosition.y);\n    const hoverColumnIndex = getColumnIndex(columns, internalPosition.x);\n\n    if (hoverRowIndex === -1 || hoverColumnIndex === -1)\n        return null;\n\n    return {\n        rowId: rows[hoverRowIndex].id,\n        columnId: columns[hoverColumnIndex].id\n    };\n}\n",
         "export default function getRowIndex(rows, y) {\n    if (rows.length === 0)\n        return -1;\n    if (y < rows[0].topWithBorder)\n        return -1;\n    if (y > rows[rows.length - 1].bottomWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = rows.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (y < rows[iterB].topWithBorder)\n            iterC = iterB - 1;\n        else if (y > rows[iterB].bottomWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "export default function getColumnIndex(columns, x) {\n    if (columns.length === 0)\n        return -1;\n    if (x < columns[0].leftWithBorder)\n        return -1;\n    if (x > columns[columns.length - 1].rightWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = columns.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (x < columns[iterB].leftWithBorder)\n            iterC = iterB - 1;\n        else if (x > columns[iterB].rightWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getCombinedCells(previousCells, newCells) {\n    const selection = new Selection(newCells);\n    return [...newCells, ...previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId))];\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getReducedCells(previousCells, cellsToRemove) {\n    const selection = new Selection(cellsToRemove);\n    return previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId));\n}\n",
         "export default function getMousePosition(event) {\n    const element = event.currentTarget;\n    const rect = element.getBoundingClientRect();\n    return {\n        x: event.clientX - rect.left,\n        y: event.clientY - rect.top\n    };\n}",
         "export function getWithAssumedId(cells, defaultId) {\n    return cells.map(cell => ({\n        ...cell,\n        columnId: 'id' in cell ? cell.id : defaultId,\n        rowId: 'id' in cell ? cell.id : defaultId\n    }));\n}",
-        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellEditType from \"./state-utils/getCellEditType.js\";\nimport getInternalPosition from \"./state-utils/getInternalPosition.js\";\nimport { getWithAssumedId } from \"./state-utils/getWithAssumedId.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    // console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n    const tooltip = document.createElement('div');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n    tooltip.setAttribute('style', 'pointer-events: none; background-color: white; color: black; border: 1px solid black; padding: 5px;');\n    tooltip.setAttribute('popover', '');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        tooltip: tooltip,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data?.[row.id]?.[column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newColumnWidth = Math.max(10, internalPosition.x - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newRowHeight = Math.max(10, internalPosition.y - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n        const eventProperties = {\n            ctrlKey: event.ctrlKey,\n            shiftKey: event.shiftKey,\n            button: event.button,\n            buttons: event.buttons\n        };\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellEditType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    // console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction findMove(entries, focusedId, hoveredId) {\n    const focusedKey = stringifyId(focusedId);\n    const hoveredKey = stringifyId(hoveredId);\n\n    if (focusedKey === hoveredKey)\n        return null;\n\n    const focusedIndex = entries.findIndex(entry => entry.key === focusedKey);\n    const hoveredIndex = entries.findIndex(entry => entry.key === hoveredKey);\n\n    if (focusedIndex === -1)\n        return null;\n    if (hoveredIndex === -1)\n        return null;\n    if (focusedIndex === hoveredIndex)\n        return null;\n\n    return [focusedIndex, hoveredIndex];\n}\n\nexport function getReorderedColumns(columns, columnId, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const move = findMove(columns, columnId, hoveredCell.columnId);\n\n    if (!move)\n        return null;\n\n    const [from, to] = move;\n    const adjustedTo = to <= from\n        ? (mousePosition.x < columns[to].leftWithBorder + columns[from].width ? to : to + 1)\n        : (mousePosition.x > columns[to].rightWithBorder - columns[from].width ? to : to - 1);\n\n    if (adjustedTo === from)\n        return null;\n\n    const reordered = columns.map(entry => entry.id);\n    reordered.splice(from, 1);\n    reordered.splice(adjustedTo, 0, columnId);\n\n    return reordered;\n}\n\nexport function getReorderedRows(rows, rowId, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const move = findMove(rows, rowId, hoveredCell.rowId);\n\n    if (!move)\n        return null;\n\n    const [from, to] = move;\n    const adjustedTo = to <= from\n        ? (mousePosition.y < rows[to].topWithBorder + rows[from].height ? to : to + 1)\n        : (mousePosition.y > rows[to].bottomWithBorder - rows[from].height ? to : to - 1);\n\n    if (adjustedTo === from)\n        return null;\n\n    const reordered = rows.map(entry => entry.id);\n    reordered.splice(from, 1);\n    reordered.splice(adjustedTo, 0, rowId);\n\n    return reordered;\n}",
+        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellEditType from \"./state-utils/getCellEditType.js\";\nimport getInternalPosition from \"./state-utils/getInternalPosition.js\";\nimport { getWithAssumedId } from \"./state-utils/getWithAssumedId.js\";\nimport { getReorderedColumns, getReorderedRows } from \"./state-utils/getReordered.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    // console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n    const tooltip = document.createElement('div');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n    tooltip.setAttribute('style', 'pointer-events: none; background-color: white; color: black; border: 1px solid black; padding: 5px;');\n    tooltip.setAttribute('popover', '');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        tooltip: tooltip,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data?.[row.id]?.[column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        columnsOrder: [],\n        onColumnsOrderChange: (columnsOrder) => {\n            context.localOptions.columnsOrder = columnsOrder;\n            context.requestNewRender();\n        },\n        rowsOrder: [],\n        onRowsOrderChange: (rowsOrder) => {\n            context.localOptions.rowsOrder = rowsOrder;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newColumnWidth = Math.max(10, internalPosition.x - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newRowHeight = Math.max(10, internalPosition.y - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n        if (context.reorderedColumn) {\n            const columns = context.state.columns;\n            const hoveredCell = context.state.hoveredCell;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const reorderedColumns = getReorderedColumns(columns, context.reorderedColumn, hoveredCell, internalPosition);\n            if (reorderedColumns) {\n                context.didReorder = true;\n                context.isReordering = true;\n                context.state.options.onColumnsOrderChange(reorderedColumns);\n            }\n        }\n        if (context.reorderedRow) {\n            const rows = context.state.rows;\n            const hoveredCell = context.state.hoveredCell;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const reorderedRows = getReorderedRows(rows, context.reorderedRow, hoveredCell, internalPosition);\n            if (reorderedRows) {\n                context.didReorder = true;\n                context.isReordering = true;\n                context.state.options.onRowsOrderChange(reorderedRows);\n            }\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        const hoveredCell = context.state.hoveredCell;\n\n        context.isMouseDown = true;\n        context.didReorder = false;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.resizingColumn && hoveredCell) {\n            const row = context.state.rowLookup.get(stringifyId(hoveredCell.rowId));\n            context.reorderedColumn = row.type === 'HEADER' ? hoveredCell.columnId : null;\n        }\n        if (!context.resizingRow && hoveredCell) {\n            const column = context.state.columnLookup.get(stringifyId(hoveredCell.columnId));\n            context.reorderedRow = column.type === 'HEADER' ? hoveredCell.rowId : null;\n        }\n\n        if (!context.resizingColumn && !context.resizingRow) {\n            context.state.options.onFocusedCellChange(hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.isReordering = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n        context.reorderedColumn = null;\n        context.reorderedRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (context.didReorder)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n        const eventProperties = {\n            ctrlKey: event.ctrlKey,\n            shiftKey: event.shiftKey,\n            button: event.button,\n            buttons: event.buttons\n        };\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellEditType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick({ ...context.state.hoveredCell, ...eventProperties });\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    // console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
         "export default function getToggledValue(cell, column, row, edition) {\n    const value = edition.hasValueByKey(row.key, column.key)\n        ? edition.getValueByKey(row.key, column.key)\n        : cell.value;\n    const toggle = cell.edit.toggle;\n\n    if (typeof toggle === 'function')\n        return toggle({value}); // TODO: expand by context\n\n    return toggle[(toggle.indexOf(value) + 1) % toggle.length];\n}",
         "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.key === stringifyId(columnId) && row.key === stringifyId(rowId);\n    }\n\n    function isConflictingWithCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.type === 'HEADER' && column.key === stringifyId(columnId)\n            || row.type === 'HEADER' && row.key === stringifyId(rowId);\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld\n        ? sortBy.filter(rule => !isCurrentRule(rule))\n        : sortBy.filter(rule => !isConflictingWithCurrentRule(rule));\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport Selection from \"../types/Selection.js\";\n\nexport default function getClipboardData(selectedCells, columns, rows, formatResolver) {\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const selectedCellKeys = selectedCells.map(cell => ({\n        columnKey: stringifyId(cell.columnId),\n        rowKey: stringifyId(cell.rowId)\n    })).filter(cell => columnLookup.has(cell.columnKey) && rowLookup.has(cell.rowKey));\n    const selectedColumns = new Set(selectedCellKeys.map(cell => cell.columnKey));\n    const selectedRows = new Set(selectedCellKeys.map(cell => cell.rowKey));\n\n    if (selectedCellKeys.length === 0)\n        return '';\n\n    const selection = new Selection(selectedCells);\n    const minColumnIndex = Math.min(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const maxColumnIndex = Math.max(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const minRowIndex = Math.min(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n    const maxRowIndex = Math.max(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n\n    const stringBuilder = [];\n\n    for (let rowIndex = minRowIndex; rowIndex <= maxRowIndex; rowIndex++) {\n        const row = rows[rowIndex];\n        const rowKey = row.key;\n\n        if (!selectedRows.has(rowKey))\n            continue;\n\n        for (let columnIndex = minColumnIndex; columnIndex <= maxColumnIndex; columnIndex++) {\n            const column = columns[columnIndex];\n            const columnKey = column.key;\n\n            if (!selectedColumns.has(columnKey))\n                continue;\n\n            if (selection.isKeySelected(rowKey, columnKey)) {\n                const cellData = formatResolver.resolve(row, column).text;\n                stringBuilder.push(cellData);\n            }\n\n            if (columnIndex < maxColumnIndex)\n                stringBuilder.push('\\t');\n        }\n\n        if (rowIndex < maxRowIndex)\n            stringBuilder.push('\\n');\n    }\n\n    return stringBuilder.join('');\n}",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_3m1716794736\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_4m1717004035\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
     ],
     "version": 3
 }
```

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/metadata.json` & `dash_spread_grid-0.1.4/dash_spread_grid/metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'src/lib/components/DashSpreadGrid.jsx'": "{'props': {'column_widths': OrderedDict([('type', "*

 * *                                            "OrderedDict([('name', 'array')])), ('required', "*

 * *                                            "False), ('description', ''), ('defaultValue', "*

 * *                                            "OrderedDict([('value', '[]'), ('computed', "*

 * *                                            "False)]))]), 'row_heights': OrderedDict([('type', "*

 * *                                         […]*

```diff
@@ -55,15 +55,15 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
-            "columnWidths": {
+            "column_widths": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
                 "type": {
@@ -77,14 +77,25 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
+            "columns_order": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "[]"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "array"
+                }
+            },
             "data": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
@@ -216,15 +227,15 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
-            "rowHeights": {
+            "row_heights": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
                 "type": {
@@ -238,14 +249,25 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
+            "rows_order": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "[]"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "array"
+                }
+            },
             "selected_cells": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
```

### Comparing `dash_spread_grid-0.1.3/dash_spread_grid/package-info.json` & `dash_spread_grid-0.1.4/dash_spread_grid/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.3",
+    "version": "0.1.4",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

### Comparing `dash_spread_grid-0.1.3/package.json` & `dash_spread_grid-0.1.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.3",
+    "version": "0.1.4",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

