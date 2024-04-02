# Comparing `tmp/ode-style-0.0.1.tar.gz` & `tmp/ode-style-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ode-style-0.0.1.tar", last modified: Fri Mar 22 00:43:00 2024, max compression
+gzip compressed data, was "ode-style-0.0.2.tar", last modified: Tue Apr  2 16:34:01 2024, max compression
```

## Comparing `ode-style-0.0.1.tar` & `ode-style-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:43:00.372424 ode-style-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-22 00:43:00.372424 ode-style-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 00:42:50.000000 ode-style-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:43:00.372424 ode-style-0.0.1/ode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/authentication_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/callback_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/chained_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/composite_job_disposable.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/error_output.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/guard_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/internet_connection_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/sequence_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/use_case_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/use_case_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/use_case_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-22 00:42:50.000000 ode-style-0.0.1/ode/value_out_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 00:43:00.372424 ode-style-0.0.1/ode_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-22 00:43:00.000000 ode-style-0.0.1/ode_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-22 00:43:00.000000 ode-style-0.0.1/ode_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 00:43:00.000000 ode-style-0.0.1/ode_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-22 00:43:00.000000 ode-style-0.0.1/ode_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 00:43:00.372424 ode-style-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-22 00:42:50.000000 ode-style-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 16:34:01.880241 ode-style-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:33:49.000000 ode-style-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/ode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/authentication_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/callback_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/chained_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/composite_job_disposable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/error_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/guard_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/internet_connection_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/sequence_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/use_case_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 16:33:49.000000 ode-style-0.0.2/ode/value_out_put.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:34:01.880241 ode-style-0.0.2/ode_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 16:34:01.000000 ode-style-0.0.2/ode_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:34:01.880241 ode-style-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-02 16:33:49.000000 ode-style-0.0.2/setup.py
```

### Comparing `ode-style-0.0.1/ode/base_controller.py` & `ode-style-0.0.2/ode/base_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, Optional, TypeVar
 
-from BabelFish.use_case import UseCase
-from BabelFish.callback_decorator import CallbackDecorator
+from ode.use_case import UseCase
+from ode.callback_decorator import CallbackDecorator
 
-from BabelFish.composite_job_disposable import CompositeJobDisposable
-from BabelFish.output import Output
-from BabelFish.use_case_decorator import UseCaseDispatcher
-from BabelFish.use_case_unit import UseCaseUnit
+from ode.composite_job_disposable import CompositeJobDisposable
+from ode.output import Output
+from ode.use_case_decorator import UseCaseDispatcher
+from ode.use_case_unit import UseCaseUnit
 
 P = TypeVar('P', bound=object)
 R = TypeVar('R', bound=object)
 
 class BaseController(object):
     composite_job_disposable: Optional[CompositeJobDisposable] = None
```

### Comparing `ode-style-0.0.1/ode/chained_use_case.py` & `ode-style-0.0.2/ode/chained_use_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar
-from BabelFish.use_case import UseCase
+from ode.use_case import UseCase
 from output import Output
 from error_output import ErrorOutput
 
 P = TypeVar('P')
 R = TypeVar('R')
 T = TypeVar('T')
```

### Comparing `ode-style-0.0.1/ode/composite_job_disposable.py` & `ode-style-0.0.2/ode/composite_job_disposable.py`

 * *Files identical despite different names*

### Comparing `ode-style-0.0.1/ode/sequence_use_case.py` & `ode-style-0.0.2/ode/sequence_use_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar, List, Optional
-from BabelFish.use_case import UseCase
+from ode.use_case import UseCase
 from output import Output
 from value_out_put import ValueOutput
 from use_case_unit import UseCaseUnit
 
 P = TypeVar('P')
 R = TypeVar('R')
 T = TypeVar('T')
```

### Comparing `ode-style-0.0.1/ode/use_case.py` & `ode-style-0.0.2/ode/use_case.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import TypeVar, Generic
-from BabelFish.output import Output
-from BabelFish.error_output import ErrorOutput
+from ode.output import Output
+from ode.error_output import ErrorOutput
 
 P = TypeVar('P')
 R = TypeVar('R')
 
 class UseCase(ABC, Generic[P, R]):
 
     def execute(self, param: P = None) -> Output[R]:
```

### Comparing `ode-style-0.0.1/ode/use_case_decorator.py` & `ode-style-0.0.2/ode/use_case_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import TypeVar, Optional
-from BabelFish.use_case import UseCase
-from BabelFish.output import Output
+from ode.use_case import UseCase
+from ode.output import Output
 import asyncio
 
 P = TypeVar('P')
 R = TypeVar('R')
 
 
 class UseCaseDecorator(UseCase[P, R]):
```

### Comparing `ode-style-0.0.1/ode/use_case_dispatcher.py` & `ode-style-0.0.2/ode/use_case_dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from BabelFish.use_case_decorator import UseCaseDecorator
+from ode.use_case_decorator import UseCaseDecorator
 import threading
 
 class UseCaseDispatcher:
     def __init__(self, use_case, execute_on=None, result_on=None):
         self.decorator = DispatcherDecorator(use_case, execute_on, result_on)
 
     def dispatch(self, param=None):
```

### Comparing `ode-style-0.0.1/ode/use_case_unit.py` & `ode-style-0.0.2/ode/use_case_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TypeVar, Generic, Optional
-from BabelFish.callback_decorator import CallbackDecorator
-from BabelFish.output import Output
-from BabelFish.value_out_put import ValueOutput
+from ode.callback_decorator import CallbackDecorator
+from ode.output import Output
+from ode.value_out_put import ValueOutput
 
-from BabelFish.use_case import UseCase
+from ode.use_case import UseCase
 
 P = TypeVar('P')
 R = TypeVar('R')
 
 class UseCaseUnit(Generic[P, R]):
     def __init__(self, use_case: UseCase[P, R], param: Optional[P] = None):
         self.use_case = use_case
```

### Comparing `ode-style-0.0.1/ode_style.egg-info/SOURCES.txt` & `ode-style-0.0.2/ode_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

