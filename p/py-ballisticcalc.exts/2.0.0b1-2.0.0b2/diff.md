# Comparing `tmp/py_ballisticcalc.exts-2.0.0b1.tar.gz` & `tmp/py_ballisticcalc.exts-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc.exts-2.0.0b1.tar", last modified: Tue Mar 26 09:01:41 2024, max compression
+gzip compressed data, was "py_ballisticcalc.exts-2.0.0b2.tar", last modified: Tue Apr  2 04:25:34 2024, max compression
```

## Comparing `py_ballisticcalc.exts-2.0.0b1.tar` & `py_ballisticcalc.exts-2.0.0b2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:41.518371 py_ballisticcalc.exts-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-03-26 09:01:41.518371 py_ballisticcalc.exts-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:41.518371 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-03-26 09:01:41.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-26 09:01:41.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 09:01:41.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 09:01:41.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 09:01:41.514371 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   574585 2024-03-26 09:01:40.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/drag_model.c
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/drag_model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   893254 2024-03-26 09:01:41.000000 py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/trajectory_calc.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 09:01:41.518371 py_ballisticcalc.exts-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-26 09:01:24.000000 py_ballisticcalc.exts-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   575422 2024-04-02 04:25:33.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   894073 2024-04-02 04:25:33.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/trajectory_calc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/setup.py
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/LICENSE` & `py_ballisticcalc.exts-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b1/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/README.md` & `py_ballisticcalc.exts-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc.exts.egg-info/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/drag_model.c` & `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "py_ballisticcalc_exts.drag_model",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -6720,24 +6750,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__ *__pyx_freelist_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__)))) {
     o = (PyObject*)__pyx_freelist_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__[--__pyx_freecount_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__];
     memset(o, 0, sizeof(struct __pyx_obj_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -6756,15 +6788,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__)))) {
     __pyx_freelist_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__[__pyx_freecount_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__++] = ((struct __pyx_obj_21py_ballisticcalc_exts_10drag_model___pyx_scope_struct____iter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/drag_model.pyi` & `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.pyi`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b1/py_ballisticcalc_exts/trajectory_calc.c` & `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/trajectory_calc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "py_ballisticcalc_exts.trajectory_calc",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/pyproject.toml` & `py_ballisticcalc.exts-2.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel", 'cython']
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc.exts"
-version = "2.0.0b1"
+version = "2.0.0b2"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
```

### Comparing `py_ballisticcalc.exts-2.0.0b1/setup.py` & `py_ballisticcalc.exts-2.0.0b2/setup.py`

 * *Files identical despite different names*

