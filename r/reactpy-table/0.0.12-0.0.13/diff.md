# Comparing `tmp/reactpy_table-0.0.12.tar.gz` & `tmp/reactpy_table-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_table-0.0.12.tar", max compression
+gzip compressed data, was "reactpy_table-0.0.13.tar", max compression
```

## Comparing `reactpy_table-0.0.12.tar` & `reactpy_table-0.0.13.tar`

### file list

```diff
@@ -1,24 +1,29 @@
--rw-r--r--   0        0        0     1428 2024-03-16 16:19:05.956859 reactpy_table-0.0.12/pyproject.toml
--rw-r--r--   0        0        0      229 2024-03-16 16:19:14.115386 reactpy_table-0.0.12/reactpy_table/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 09:34:43.413923 reactpy_table-0.0.12/reactpy_table/core/__init__.py
--rw-r--r--   0        0        0      434 2024-03-13 09:05:43.214911 reactpy_table-0.0.12/reactpy_table/core/feature_factories.py
--rw-r--r--   0        0        0     1460 2024-03-16 16:11:47.085749 reactpy_table-0.0.12/reactpy_table/core/options.py
--rw-r--r--   0        0        0     1721 2024-03-16 08:48:31.562098 reactpy_table-0.0.12/reactpy_table/core/reactpy_table.py
--rw-r--r--   0        0        0     1534 2024-03-16 16:14:23.177437 reactpy_table-0.0.12/reactpy_table/core/reactpy_table_init.py
--rw-r--r--   0        0        0      421 2024-03-15 13:11:25.099806 reactpy_table-0.0.12/reactpy_table/core/table.py
--rw-r--r--   0        0        0      316 2024-03-12 11:40:24.094486 reactpy_table-0.0.12/reactpy_table/features/__init__.py
--rw-r--r--   0        0        0     2987 2024-03-16 08:54:21.919465 reactpy_table-0.0.12/reactpy_table/features/column_sort.py
--rw-r--r--   0        0        0     3856 2024-03-16 16:10:11.817910 reactpy_table-0.0.12/reactpy_table/features/paginator.py
--rw-r--r--   0        0        0     2649 2024-03-16 15:41:04.146517 reactpy_table-0.0.12/reactpy_table/features/row_model.py
--rw-r--r--   0        0        0     2113 2024-03-16 08:45:14.054479 reactpy_table-0.0.12/reactpy_table/features/table_search.py
--rw-r--r--   0        0        0      526 2024-03-15 14:48:58.398996 reactpy_table-0.0.12/reactpy_table/types/__init__.py
--rw-r--r--   0        0        0      405 2024-03-11 14:25:32.365298 reactpy_table-0.0.12/reactpy_table/types/abstract_column_sort.py
--rw-r--r--   0        0        0     1462 2024-03-15 16:25:05.507221 reactpy_table-0.0.12/reactpy_table/types/abstract_paginator.py
--rw-r--r--   0        0        0      405 2024-03-12 08:54:26.176120 reactpy_table-0.0.12/reactpy_table/types/abstract_row_model.py
--rw-r--r--   0        0        0      810 2024-03-15 13:15:17.944873 reactpy_table-0.0.12/reactpy_table/types/abstract_table.py
--rw-r--r--   0        0        0      327 2024-02-25 10:45:23.629577 reactpy_table-0.0.12/reactpy_table/types/abstract_table_search.py
--rw-r--r--   0        0        0     1730 2024-03-16 08:16:05.752178 reactpy_table-0.0.12/reactpy_table/types/feature.py
--rw-r--r--   0        0        0     1111 2024-03-16 06:58:24.501828 reactpy_table-0.0.12/reactpy_table/types/table_data.py
--rw-r--r--   0        0        0      197 2024-03-15 14:48:58.396075 reactpy_table-0.0.12/reactpy_table/types/updater.py
--rw-r--r--   0        0        0     2969 2024-03-15 14:48:10.122180 reactpy_table-0.0.12/README.md
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 reactpy_table-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1469 2024-04-02 12:33:22.477220 reactpy_table-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0      287 2024-04-02 12:33:13.538920 reactpy_table-0.0.13/reactpy_table/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:34:43.413923 reactpy_table-0.0.13/reactpy_table/core/__init__.py
+-rw-r--r--   0        0        0      434 2024-03-16 16:20:49.561713 reactpy_table-0.0.13/reactpy_table/core/feature_factories.py
+-rw-r--r--   0        0        0     3276 2024-04-02 07:18:15.118079 reactpy_table-0.0.13/reactpy_table/core/options.py
+-rw-r--r--   0        0        0     3294 2024-04-02 07:48:29.950742 reactpy_table-0.0.13/reactpy_table/core/reactpy_table.py
+-rw-r--r--   0        0        0     1890 2024-04-02 10:29:24.687616 reactpy_table-0.0.13/reactpy_table/core/reactpy_table_init.py
+-rw-r--r--   0        0        0      316 2024-04-02 07:14:51.990561 reactpy_table-0.0.13/reactpy_table/features/__init__.py
+-rw-r--r--   0        0        0     3567 2024-04-02 07:21:37.484748 reactpy_table-0.0.13/reactpy_table/features/column_sort.py
+-rw-r--r--   0        0        0      471 2024-04-01 11:39:24.234353 reactpy_table-0.0.13/reactpy_table/features/null_updater.py
+-rw-r--r--   0        0        0     4594 2024-04-02 07:31:18.811981 reactpy_table-0.0.13/reactpy_table/features/paginator.py
+-rw-r--r--   0        0        0     2649 2024-03-31 06:22:03.596864 reactpy_table-0.0.13/reactpy_table/features/row_model.py
+-rw-r--r--   0        0        0     2304 2024-04-01 10:32:16.291727 reactpy_table-0.0.13/reactpy_table/features/table_search.py
+-rw-r--r--   0        0        0      787 2024-04-02 10:29:16.464273 reactpy_table-0.0.13/reactpy_table/types/__init__.py
+-rw-r--r--   0        0        0      405 2024-03-31 06:24:13.605740 reactpy_table-0.0.13/reactpy_table/types/abstract_column_sort.py
+-rw-r--r--   0        0        0     1460 2024-03-27 08:30:11.088878 reactpy_table-0.0.13/reactpy_table/types/abstract_paginator.py
+-rw-r--r--   0        0        0      405 2024-03-12 08:54:26.176120 reactpy_table-0.0.13/reactpy_table/types/abstract_row_model.py
+-rw-r--r--   0        0        0     1179 2024-04-02 07:02:00.776177 reactpy_table-0.0.13/reactpy_table/types/abstract_table.py
+-rw-r--r--   0        0        0      327 2024-04-01 16:08:43.301863 reactpy_table-0.0.13/reactpy_table/types/abstract_table_search.py
+-rw-r--r--   0        0        0     1756 2024-04-02 10:20:19.175628 reactpy_table-0.0.13/reactpy_table/types/feature.py
+-rw-r--r--   0        0        0      105 2024-04-01 09:21:02.103481 reactpy_table-0.0.13/reactpy_table/types/feature_control.py
+-rw-r--r--   0        0        0      451 2024-04-02 10:39:06.135382 reactpy_table-0.0.13/reactpy_table/types/paginator_state.py
+-rw-r--r--   0        0        0      303 2024-04-01 16:08:43.302835 reactpy_table-0.0.13/reactpy_table/types/search_state.py
+-rw-r--r--   0        0        0      356 2024-03-31 06:24:13.608661 reactpy_table-0.0.13/reactpy_table/types/sort_state.py
+-rw-r--r--   0        0        0      806 2024-04-02 10:25:58.585141 reactpy_table-0.0.13/reactpy_table/types/table.py
+-rw-r--r--   0        0        0     1164 2024-04-02 10:24:22.290194 reactpy_table-0.0.13/reactpy_table/types/table_data.py
+-rw-r--r--   0        0        0     2058 2024-04-02 06:59:10.101228 reactpy_table-0.0.13/reactpy_table/types/table_state.py
+-rw-r--r--   0        0        0     3782 2024-04-02 12:14:38.146196 reactpy_table-0.0.13/README.md
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 reactpy_table-0.0.13/PKG-INFO
```

### Comparing `reactpy_table-0.0.12/pyproject.toml` & `reactpy_table-0.0.13/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reactpy-table"
-version = "0.0.12"
+version = "0.0.13"
 description = "Headless UI for building powerful tables"
 authors = ["Steve Jones <jonesst2608@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/stevej2608/reactpy-table/blob/master/README.md"
 repository = "https://github.com/stevej2608/reactpy-table"
 include = ["reactpy-tablet/*.py"]
@@ -20,14 +20,16 @@
 playwright = "1.41.1"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 starlette = ">=0.13.6"
 trio = "^0.24.0"
 twine = "^4.0.2"
 uvicorn = {extras = ["standard"], version = ">=0.19.0"}
+faker = "^24.3.0"
+sqlmodel = "^0.0.16"
 
 
 [tool.ruff]
 # https://docs.astral.sh/ruff/configuration/
 # https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff
 
 line-length = 120
```

### Comparing `reactpy_table-0.0.12/reactpy_table/core/reactpy_table.py` & `reactpy_table-0.0.13/reactpy_table/types/feature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,71 @@
-from typing import Generic, Self, Callable
+from typing import Any, Callable, Generic, Protocol, TypeVar, cast
+from enum import Enum
+from .abstract_table import ITable
+from .table_data import TableData, TData, UpstreamData
+
+class FeatureControl(Enum):
+    DISABLED = 1
+    DEFAULT = 2
+    MANUAL = 3
 
-from utils import log
 
-from ..types import TableData, TData
-from .feature_factories import FeatureFactories
-from .table import Table
+class IFeature(Protocol, Generic[TData]):
 
+    @property
+    def data(self) -> TableData[TData]:
+        ...
+
+    pipeline: Callable[[], TableData[TData]]
 
-class ReactpyTable(Table[TData], Generic[TData]):
+
+class FeatureBase(IFeature[TData], Generic[TData]):
 
     @property
     def data(self) -> TableData[TData]:
-        return self._data
+        return self._table.data
+
+    @property
+    def table(self) -> ITable[TData]:
+        return self._table
+
+    def __init__(self, table: ITable[TData]):
+        self._table = table
+
+
+    def refresh(self):
+        self.table.refresh()
 
-    def refresh(self) -> Self:
 
-        # The following call triggers an update of
-        # the entire feature pipeline
 
-        self._data = self.row_model.pipeline()
-        self.model_update(self)
+TFeature= TypeVar("TFeature")
 
-        return self
+TFeatureFactory = Callable[[ITable[TData], UpstreamData[TData]], TFeature]
+"""Generic signature of a Callable that returns a Feature instance
 
+Returns:
+    TFeature: When called returns an instantiated feature
 
-    def __init__(self, data: TableData[TData],
-                 updater: Callable[['ReactpyTable[TData]'], None],
-                 features: FeatureFactories[TData]):
+Example Usage:
+```
+def getMyRowModel(<custom parameters>) -> TFeatureFactory[TData, RowModel[TData]]:
 
-        # Daisy chain the feature pipeline. Each of
-        # these functions is passed into it's respective
-        # feature. Each function returns the table data
-        # from the next feature up the pipeline.
+    # < Any persistent data/refs here>
 
-        def search_update() -> TableData[TData]:
-            return self._initial_data
+    def wrapper(table: ITable[TData], updater: Updater[TData]) -> RowModel[TData]:
+    
+        # <Any pre-initialization code here>
 
-        def sort_update() -> TableData[TData]:
-            return self.search.pipeline()
+        return MyRowModel(table=table, updater=updater, <Any Additional Args>)
 
-        def paginator_update() -> TableData[TData]:
-            return self.sort.pipeline()
+    return wrapper
+```
+"""
 
-        def row_model_update() -> TableData[TData]:
-            return self.paginator.pipeline()
+Func = TypeVar("Func", bound=Callable[..., Any])
+def update_state(func: Func) -> Func:
+    def wrapper(self: FeatureBase[TData], *args: Any, **kwargs: Any) -> Any:
+        result = func(self, *args, **kwargs)
+        self.table.refresh()
+        return result
 
-        self._initial_data: TableData[TData] = data
-        self._data: TableData[TData] = data
-        self.model_update = updater
-        self.search = features.search(self, search_update)
-        self.sort = features.sort(self, sort_update)
-        self.paginator = features.paginator(self, paginator_update)
-        self.row_model = features.row_model(self, row_model_update)
+    return cast(Func, wrapper)
```

### Comparing `reactpy_table-0.0.12/reactpy_table/features/column_sort.py` & `reactpy_table-0.0.13/reactpy_table/features/column_sort.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,25 @@
-from typing import Dict, Tuple, Any
+from typing import Any, Dict, Tuple
 
 from pydantic import BaseModel
-from utils.memo import memo, MemoOpts
 
-from ..types import ColumnDef, ColumnSort, ITable, TData, TableData, TFeatureFactory, UpstreamData, update_state
+from utils.memo import MemoOpts, memo
+
+from ..types import (
+    ColumnDef,
+    ColumnSort,
+    FeatureControl,
+    ITable,
+    SortState,
+    TableData,
+    TData,
+    TFeatureFactory,
+    UpstreamData,
+)
+from .null_updater import null_updater
 
 
 class ColumnState(BaseModel):
     column_name: str
     reverse: bool = False
 
     def __str__(self):
@@ -16,15 +28,15 @@
     def __repr__(self):
         return f"ColumnState[{id(self)}](column_name={self.column_name}, reverse={self.reverse})"
 
 
 class DefaultColumnSort(ColumnSort[TData]):
 
     def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData], state: Dict[str, ColumnState]):
-        super().__init__(table, upstream_data)
+        super().__init__(table)
         self._all_columns_state = state
         self._active_column_state: ColumnState | None = None
 
 
         def deps() -> Tuple[TableData[TData], ColumnState | None]:
             return (
                 upstream_data(),
@@ -47,21 +59,34 @@
                 col = active_column_state
                 rows = table_data.rows.copy()
                 rows.sort(key=lambda element: _sort(col, element), reverse=True)
                 return TableData(rows=rows, cols=table_data.cols)
             else:
                 return table_data
 
-        self.pipeline = memo(deps, updater, MemoOpts(name='2. DefaultColumnSort'))
+
+        if self.table.table_state.sort_control is FeatureControl.DEFAULT:
+            self.pipeline = memo(deps, updater, MemoOpts(name='      3. DefaultColumnSort', debug=False))
+        else:
+            self.pipeline = null_updater(upstream_data=upstream_data)
 
 
-    @update_state
-    def toggle_sort(self, col: ColumnDef) -> bool:
+    # @update_state
+    def toggle_sort(self, col: ColumnDef) -> None:
         self._active_column_state = self.get_state(col, toggle=True)
-        return self._active_column_state.reverse
+        if self.table.table_state.on_sort_change:
+
+            new_state= SortState(
+                id=self._active_column_state.column_name,
+                desc= 'DESC' if self._active_column_state.reverse else 'ASC'
+                )
+
+            self.table.table_state.on_sort_change(new_state)
+        else:
+            self.refresh()
 
 
     def is_sort_reverse(self, col: ColumnDef) -> bool:
         state = self.get_state(col)
         return state.reverse
```

### Comparing `reactpy_table-0.0.12/reactpy_table/features/paginator.py` & `reactpy_table-0.0.13/reactpy_table/features/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,79 @@
-from typing import Tuple
-from ctypes import ArgumentError
+import logging
 import math
+from ctypes import ArgumentError
+from typing import Tuple
 
-from utils.logger import log
-from utils.memo import memo, MemoOpts
 
-from ..types import ITable, Paginator, TableData, TData, TFeatureFactory, UpstreamData, update_state
+from utils.memo import MemoOpts, memo
 
+from ..types import FeatureControl, ITable, Paginator, PaginatorState, TableData, TData, TFeatureFactory, UpstreamData
+from .null_updater import null_updater
 
-DEFAULT_PAGE_SIZE = 10
+log = logging.getLogger(__name__)
 
+DEFAULT_PAGE_SIZE = 10
 
 class DefaultPaginator(Paginator[TData]):
 
-    def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData], page_size: int, enabled:bool=False):
-        super().__init__(table, upstream_data)
+    def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData], page_size: int):
+        super().__init__(table)
         self.upstream_data = upstream_data
-        self._page_size = page_size
-        self._page_index = 0
-        self.enabled = enabled
+        self._paginator_state = PaginatorState(page_index=0, page_size=page_size)
+
 
         def deps() -> Tuple[TableData[TData], int, int, bool]:
             return (
                 upstream_data(),
-                self._page_size,
-                self._page_index,
-                self.enabled
+                self.page_size,
+                self.page_index,
+                self.table.table_state.pagination_control == FeatureControl.DISABLED
             )
 
         def updater(upstream_data: TableData[TData],
-                   page_size: int, 
+                   page_size: int,
                    page_index:int,
-                   enabled: bool
+                   disabled: bool
                    ) -> TableData[TData]:
-            
-            if not enabled:
+
+            if disabled:
                 return upstream_data
-            
+
             low = page_size * page_index
             high = min(low + page_size, len(upstream_data.rows))
 
             rows = upstream_data.rows[low:high]
             table_data = TableData(rows=rows, cols=upstream_data.cols)
             return table_data
 
-        self.pipeline = memo(deps, updater, MemoOpts(name='3. DefaultPaginator'))
+
+        if self.table.table_state.pagination_control is FeatureControl.DEFAULT:
+            self.pipeline = memo(deps, updater, MemoOpts(name='    2. DefaultPaginator', debug=False))
+        else:
+            self.pipeline = null_updater(upstream_data=upstream_data)
 
 
     @property
     def page_index(self) -> int:
-        return self._page_index
+        return self._paginator_state.page_index
 
     @property
     def page_size(self) -> int:
-        return self._page_size
+        return self._paginator_state.page_size
 
     @property
     def page_base(self) -> int:
         return self.page_size * self.page_index + 1
 
     @property
     def page_count(self) -> int:
-        row_count = self.row_count
-        return math.ceil(row_count / self.page_size)
+        pages = self.table.table_state.page_count
+        if pages is None:
+            pages = math.ceil(self.row_count / self.page_size)
+        return pages
 
     @property
     def row_count(self) -> int:
         return len(self.upstream_data().rows)
 
     def first_page(self):
         self.set_page_index(0)
@@ -79,43 +86,57 @@
         if self.page_index < self.page_count - 1:
             self.set_page_index(self.page_index + 1)
 
     def last_page(self):
         last_page = self.page_count - 1
         self.set_page_index(last_page)
 
-    @update_state
+
     def set_page_size(self, page_size: int):
         log.info("set_page_size")
+        self.set_pagination(self.page_index, page_size)
 
-        self._page_index = int((self.page_index * self.page_size) / page_size)
-        self._page_size = page_size
 
-    @update_state
     def set_page_index(self, page_index: int):
         if page_index < 0 or page_index > self.page_count-1:
             raise ArgumentError(f'Requested page {page_index} is not in range [0..{self.page_count-1}]')
-        self._page_index = page_index
+        self.set_pagination(page_index, self.page_size)
+
+
+    # @update_state
+    def set_pagination(self, page_index: int, page_size: int):
+
+        page_index = int((page_index * page_size) / page_size)
+        new_state = PaginatorState(page_index=page_index, page_size=page_size)
+
+        if new_state != self._paginator_state:
+
+            self._paginator_state = new_state
+
+            if self.table.table_state.on_pagination_change:
+                self.table.table_state.on_pagination_change(new_state)
+            else:
+                self.refresh()
 
 
     def can_get_previous_page(self) -> bool:
         return self.page_index > 0
 
     def can_get_next_page(self) -> bool:
         page_count = self.page_count
         return self.page_index < page_count - 1
 
 
-def getDefaultPaginator(page_size: int=DEFAULT_PAGE_SIZE, enabled:bool=False) -> TFeatureFactory[TData, Paginator[TData]]:
+def getDefaultPaginator(page_size: int=DEFAULT_PAGE_SIZE) -> TFeatureFactory[TData, Paginator[TData]]:
     """Return a wrapped function that when called creates a DefaultPaginator instance
 
     Args:
         page_size (int, optional): The default page size. Defaults to DEFAULT_PAGE_SIZE.
 
     Returns:
         Callable[[ITable[TData], Updater[TData]], Paginator[TData]]: A function that creates the default paginator
     """
 
     def wrapper(table: ITable[TData], upstream_data: UpstreamData[TData]) -> Paginator[TData]:
-        return DefaultPaginator(table=table, upstream_data=upstream_data, page_size=page_size, enabled=enabled)
+        return DefaultPaginator(table, upstream_data, page_size=page_size)
 
     return wrapper
```

### Comparing `reactpy_table-0.0.12/reactpy_table/features/row_model.py` & `reactpy_table-0.0.13/reactpy_table/features/row_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NO_ACTION = RowAction()
 
 
 class DefaultRowModel(RowModel[TData]):
 
     def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData]):
-        super().__init__(table, upstream_data)
+        super().__init__(table)
 
         self.row_actions: List[RowAction[TData]] = []
 
         def deps() -> Tuple[TableData[TData], List[RowAction]]:
             return (
                 upstream_data(),
                 self.row_actions.copy()
@@ -44,15 +44,15 @@
 
                 if action.action == Action.UPDATE and action.row:
                     rows[action.index] = action.row
 
             return TableData(rows=rows, cols=upstream_data.cols)
 
 
-        self.pipeline = memo(deps, updater, MemoOpts(name='4. DefaultRowModel'))
+        self.pipeline = memo(deps, updater, MemoOpts(name='  1. DefaultRowModel', debug=False))
 
 
     def table_index(self, index:int) -> int:
         """Check range and return index as range[0..n]
 
         Args:
             index (int): user index [1...n]
```

### Comparing `reactpy_table-0.0.12/reactpy_table/features/table_search.py` & `reactpy_table-0.0.13/reactpy_table/features/table_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from typing import Tuple
 
 from utils.memo import MemoOpts, memo
 
-from ..types import ITable, TableData, TableSearch, TData, TFeatureFactory, UpstreamData, update_state
+from ..types import ITable, TableData, TableSearch, SearchState, TData, TFeatureFactory, UpstreamData
 
 
 class DefaultTableSearch(TableSearch[TData]):
 
     def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData]):
-        super().__init__(table, upstream_data)
-        self.search_term: str = ''
-        self.case_sensitive: bool = False
+        super().__init__(table)
+        self._search_state = SearchState()
 
-        def deps() -> Tuple[TableData[TData], str, bool]:
+
+        def deps() -> Tuple[TableData[TData], SearchState]:
             return (
                 upstream_data(),
-                self.search_term,
-                self.case_sensitive
+                self._search_state,
             )
 
         def updater(upstream_data: TableData[TData],
-                   search_term: str, case_sensitive:bool
+                   state: SearchState
                    ) -> TableData[TData]:
 
+            case_sensitive = state.case_sensitive
+            search_term = state.search_term
+
             def _filter(row: TData) -> bool:
                 nonlocal search_term
 
                 row_text = " ".join([str(val) for val in row.model_dump().values()])
 
                 if not case_sensitive:
                     row_text = row_text.lower()
@@ -42,26 +44,29 @@
 
                 rows = list(filter(_filter, table_data.rows))
                 return TableData(rows=rows, cols=table_data.cols)
             else:
                 return table_data
 
 
-        self.pipeline = memo(deps, updater, MemoOpts(name='1. DefaultTableSearch'))
+        self.pipeline = memo(deps, updater, MemoOpts(name='        4. DefaultTableSearch', debug=False))
 
 
-    @update_state
+    # @update_state
     def table_search(self, search_term: str, case_sensitive: bool = False):
 
-        self.case_sensitive = case_sensitive
+        new_state = SearchState(search_term=search_term, case_sensitive=case_sensitive)
 
-        if case_sensitive:
-            self.search_term = search_term.lower()
-        else:
-            self.search_term = search_term
+        if new_state != self._search_state:
+            self._search_state = new_state
+
+            if self.table.table_state.on_search_change:
+                self.table.table_state.on_search_change(new_state)
+            else:
+                self.refresh()
 
 
 def getDefaultTableSearch() -> TFeatureFactory[TData, TableSearch[TData]]:
 
     def wrapper(table: ITable[TData], updater: UpstreamData[TData]) -> TableSearch[TData]:
         return DefaultTableSearch(table=table, upstream_data=updater)
```

### Comparing `reactpy_table-0.0.12/reactpy_table/types/abstract_paginator.py` & `reactpy_table-0.0.13/reactpy_table/types/abstract_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Protocol
-
 from .feature import FeatureBase, IFeature
 from .table_data import TData
 
 # pyright: reportReturnType=false
 
 
 class IPaginator(IFeature[TData], Protocol):
```

### Comparing `reactpy_table-0.0.12/reactpy_table/types/abstract_table.py` & `reactpy_table-0.0.13/reactpy_table/types/abstract_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from typing import Generic, Protocol, Callable, Self
 from utils.memo import TMemoResult
 from .table_data import TableData, TData
-
-
+from .table_state import TableState
 
 
 class ITable(Generic[TData], Protocol):
 
     @property
     def data(self) -> TableData[TData]:
         """Return data for presentation by the user"""
         ... # pylint: disable=unnecessary-ellipsis
 
+    @property
+    def initial_data(self) -> TableData[TData]:
+        """Return data for presentation by the user"""
+        ... # pylint: disable=unnecessary-ellipsis
+
+    @property
+    def table_state(self) -> TableState[TData]:
+        """Return the table options"""
+        ... # pylint: disable=unnecessary-ellipsis
+
+
     def refresh(self) -> Self:
         """Force refresh of the table"""
         ... # pylint: disable=unnecessary-ellipsis
 
+
 class IPipeline(Protocol, Generic[TMemoResult]):
     pipeline: Callable[[], TMemoResult]
 
 
 class ITablePipeline(ITable[TData], Protocol, Generic[TData]):
 
     paginator : IPipeline[TableData[TData]]
```

### Comparing `reactpy_table-0.0.12/reactpy_table/types/table_data.py` & `reactpy_table-0.0.13/reactpy_table/types/table_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable, Dict, Generic, List, Optional, Protocol, TypeVar
 
 from pydantic import BaseModel
 
+
 # https://tanstack.com/table/v8/docs/api/core/column-def
 
 class ColumnDef(BaseModel):
     """Column definitions"""
 
     name: str
     label: str
@@ -38,7 +39,10 @@
         self.rows = rows
         self.cols = cols
 
     def __repr__(self):
         return f"TableData(rows({len(self.rows)}), cols({len(self.cols)})"
 
 EMPTY_TABLE = TableData[Any](rows=[], cols=[])
+
+
+UpstreamData = Callable[[], TableData[TData]]
```

### Comparing `reactpy_table-0.0.12/README.md` & `reactpy_table-0.0.13/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 
 The initial release supports the following features:
 
 - [X] Headless UI, CSS agnostic
 - [X] Freeform text search
 - [X] Forward/Reverse column based sort
 - [X] Pagination
+- [X] Integration with SQLAlchemy (full text search, sort and pagination)
 - [ ] Integration with Pandas and SQLAlchemy (in progress)
 - [ ] Remote large dataset support
 
 ## Usage
 
 	pip install reactpy-table
 
 *[basic_example.py](examples/basic_example.py)*
-```
+```python
+from reactpy import component, html, use_memo
+from reactpy_table import Options, Table, use_reactpy_table
+
+from .data.sp500 import COLS, CompanyModel, get_sp500
+
 @component
-def THead(table: Table):
+def THead(table: Table[CompanyModel]):
     cols = table.data.cols
     return html.thead(
         html.th(cols[0].label),
         html.th(cols[1].label),
         html.th(cols[2].label),
         html.th(cols[3].label)
     )
 
-@component
+
 def TRow(index: int, row: CompanyModel):
     return  html.tr(
         html.td(str(row.index)),
         html.td(row.symbol),
         html.td(row.name),
         html.td(row.sector),
     )
@@ -47,27 +53,41 @@
     )
 
 @component
 def AppMain():
     table_data = use_memo(lambda:get_sp500(rows=50))
     table = use_reactpy_table(Options(
         rows=table_data,
-        cols = COLS
+        cols = COLS,
     ))
 
     return html.div(
         html.br(),
         html.h2('ReactPy Table Example'),
         html.table({"role": "grid"},
             THead(table),
             TBody(table)
         ),
     )
+
 ```
 
+### More complex examples
+
+**examples/table_example.py** demonstrates search, sort and pagination on SP500 
+companies table. The built-in feature data pipeline is used.
+
+**examples/books/books_example.py** demonstrates search, sort and pagination on
+a SQLite book database containing 100k books. Search, sort and 
+pagination is handled by SQL queries.
+
+* Full text search on database < 20ms
+* Page traversal < 2ms
+
+
 ## Feature Set
 
 The row data presented to the user for display is pre-processed by a
 data-pipeline of table features:
 
     1. Search, filters the initial usr data
     2. Sort, the search result by column (up/down)
@@ -77,14 +97,19 @@
 Each feature presents an API to the user that directs its
 operation. Any change will, if required, recalculate the table data.
 
 A default set of features is applied by default. One or more custom
 features that will replace the default can be supplied as options 
 when the table is created.
 
+A callback mechanism is available for each feature that provides
+support for accessing external data sources (databases, 
+pandas data-frames etc).
+
+
 ### Custom Features
 
 All features are instantiated using a strict pattern. As
 an example a custom paginator that accepts *page _size* and
 *start_page* would be created as follows:
 
 ```
```

### Comparing `reactpy_table-0.0.12/PKG-INFO` & `reactpy_table-0.0.13/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-table
-Version: 0.0.12
+Version: 0.0.13
 Summary: Headless UI for building powerful tables
 Home-page: https://github.com/stevej2608/reactpy-table/blob/master/README.md
 License: MIT
 Author: Steve Jones
 Author-email: jonesst2608@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,34 +24,40 @@
 
 The initial release supports the following features:
 
 - [X] Headless UI, CSS agnostic
 - [X] Freeform text search
 - [X] Forward/Reverse column based sort
 - [X] Pagination
+- [X] Integration with SQLAlchemy (full text search, sort and pagination)
 - [ ] Integration with Pandas and SQLAlchemy (in progress)
 - [ ] Remote large dataset support
 
 ## Usage
 
 	pip install reactpy-table
 
 *[basic_example.py](examples/basic_example.py)*
-```
+```python
+from reactpy import component, html, use_memo
+from reactpy_table import Options, Table, use_reactpy_table
+
+from .data.sp500 import COLS, CompanyModel, get_sp500
+
 @component
-def THead(table: Table):
+def THead(table: Table[CompanyModel]):
     cols = table.data.cols
     return html.thead(
         html.th(cols[0].label),
         html.th(cols[1].label),
         html.th(cols[2].label),
         html.th(cols[3].label)
     )
 
-@component
+
 def TRow(index: int, row: CompanyModel):
     return  html.tr(
         html.td(str(row.index)),
         html.td(row.symbol),
         html.td(row.name),
         html.td(row.sector),
     )
@@ -64,27 +70,41 @@
     )
 
 @component
 def AppMain():
     table_data = use_memo(lambda:get_sp500(rows=50))
     table = use_reactpy_table(Options(
         rows=table_data,
-        cols = COLS
+        cols = COLS,
     ))
 
     return html.div(
         html.br(),
         html.h2('ReactPy Table Example'),
         html.table({"role": "grid"},
             THead(table),
             TBody(table)
         ),
     )
+
 ```
 
+### More complex examples
+
+**examples/table_example.py** demonstrates search, sort and pagination on SP500 
+companies table. The built-in feature data pipeline is used.
+
+**examples/books/books_example.py** demonstrates search, sort and pagination on
+a SQLite book database containing 100k books. Search, sort and 
+pagination is handled by SQL queries.
+
+* Full text search on database < 20ms
+* Page traversal < 2ms
+
+
 ## Feature Set
 
 The row data presented to the user for display is pre-processed by a
 data-pipeline of table features:
 
     1. Search, filters the initial usr data
     2. Sort, the search result by column (up/down)
@@ -94,14 +114,19 @@
 Each feature presents an API to the user that directs its
 operation. Any change will, if required, recalculate the table data.
 
 A default set of features is applied by default. One or more custom
 features that will replace the default can be supplied as options 
 when the table is created.
 
+A callback mechanism is available for each feature that provides
+support for accessing external data sources (databases, 
+pandas data-frames etc).
+
+
 ### Custom Features
 
 All features are instantiated using a strict pattern. As
 an example a custom paginator that accepts *page _size* and
 *start_page* would be created as follows:
 
 ```
```

