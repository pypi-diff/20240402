# Comparing `tmp/botl-104.tar.gz` & `tmp/botl-105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botl-104.tar", last modified: Sun Feb 25 14:16:44 2024, max compression
+gzip compressed data, was "botl-105.tar", last modified: Tue Apr  2 03:06:51 2024, max compression
```

## Comparing `botl-104.tar` & `botl-105.tar`

### file list

```diff
@@ -1,21 +1,40 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-25 14:16:44.405084 botl-104/
--rw-r--r--   0 bart      (1000) bart      (1000)     1288 2024-02-25 14:16:44.405084 botl-104/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      764 2024-02-25 14:15:20.000000 botl-104/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-25 14:16:44.405084 botl-104/botl/
--rw-r--r--   0 bart      (1000) bart      (1000)      735 2024-02-25 14:07:16.000000 botl-104/botl/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-02-25 14:07:16.000000 botl-104/botl/brokers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1535 2024-02-25 14:07:16.000000 botl-104/botl/excepts.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6303 2024-02-25 14:07:16.000000 botl-104/botl/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6003 2024-02-25 14:07:16.000000 botl-104/botl/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1234 2024-02-25 14:07:16.000000 botl-104/botl/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1845 2024-02-25 14:07:16.000000 botl-104/botl/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-02-25 14:16:44.405084 botl-104/botl.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     1288 2024-02-25 14:16:44.000000 botl-104/botl.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      309 2024-02-25 14:16:44.000000 botl-104/botl.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-25 14:16:44.000000 botl-104/botl.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-02-25 14:16:44.000000 botl-104/botl.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-02-25 14:16:44.000000 botl-104/botl.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-02-25 14:15:27.000000 botl-104/botl.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      729 2024-02-25 14:16:24.000000 botl-104/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-02-25 14:16:44.405084 botl-104/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-02-24 07:27:58.000000 botl-104/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.256918 botl-105/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3964 2024-04-02 03:06:51.252917 botl-105/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3445 2024-04-02 02:53:55.000000 botl-105/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl/
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-04-01 19:52:46.000000 botl-105/botl/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3930 2024-04-02 02:56:38.000000 botl-105/botl/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-04-01 19:52:46.000000 botl-105/botl/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-04-01 19:52:46.000000 botl-105/botl/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-04-01 19:52:46.000000 botl-105/botl/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-04-01 20:34:46.000000 botl-105/botl/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-04-01 19:52:51.000000 botl-105/botl/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-04-01 19:52:51.000000 botl-105/botl/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-04-01 19:52:51.000000 botl-105/botl/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2024-04-01 19:52:51.000000 botl-105/botl/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17673 2024-04-01 19:52:51.000000 botl-105/botl/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-04-01 19:52:51.000000 botl-105/botl/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3485 2024-04-01 19:52:51.000000 botl-105/botl/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16976 2024-04-01 19:55:33.000000 botl-105/botl/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-04-01 19:52:51.000000 botl-105/botl/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2398 2024-04-01 19:52:51.000000 botl-105/botl/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-04-01 19:52:51.000000 botl-105/botl/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2737 2024-04-01 19:52:51.000000 botl-105/botl/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1118 2024-04-01 19:52:51.000000 botl-105/botl/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-04-01 19:52:51.000000 botl-105/botl/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5020 2024-04-01 19:52:51.000000 botl-105/botl/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2913 2024-04-01 19:52:51.000000 botl-105/botl/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-04-01 19:52:46.000000 botl-105/botl/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-04-01 19:52:46.000000 botl-105/botl/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-04-01 19:52:46.000000 botl-105/botl/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-02 03:06:51.252917 botl-105/botl.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3964 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      671 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       47 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-02 03:06:51.000000 botl-105/botl.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      836 2024-04-02 02:59:24.000000 botl-105/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-02 03:06:51.256918 botl-105/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-01 19:43:21.000000 botl-105/setup.py
```

### Comparing `botl-104/botl/brokers.py` & `botl-105/botl/broker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,E0402
+# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402,E1102
 
 
-"object cache"
+"""object broker
 
+This Broker class stores objects on their repr name and can thus be
+retrieved by a client presenting a repr of an object.
 
-from objx import Object, keys, values
+Client can carry a string (the repr) around instead of a memory
+reference to the object.
 
+Adding an object takes the repr and stores it in a dict, the rest are
+methods to retrieve an object from the broker.
 
-def __dir__():
-    return (
-        'Broker',
-    )
+Broker is operating at an class level where the class level attributes
+are manipulated instead of an object inherited from that class.
 
+"""
 
-__all__ = __dir__()
+
+from .object import Object, keys, values
 
 
 rpr = object.__repr__
 
 
-class Broker(Object):
+class Broker:
 
     objs = Object()
 
     @staticmethod
     def add(obj):
+        "add an object to the broker."
         setattr(Broker.objs, rpr(obj), obj)
 
     @staticmethod
     def all():
+        "return all objects."
         return values(Broker.objs)
 
     @staticmethod
     def first():
+        "return first object."
         for key in keys(Broker.objs):
             return getattr(Broker.objs, key)
 
     @staticmethod
     def get(orig):
+        "return object by origin (repr)"
         return getattr(Broker.objs, orig, None)
 
     @staticmethod
     def remove(obj):
+        "remove object from broker"
         delattr(Broker.objs, rpr(obj))
+
+
+"interfacce"
+
+
+def __dir__():
+    return (
+        'Broker',
+    )
+
+
+__all__ = __dir__()
```

### Comparing `botl-104/botl/handler.py` & `botl-105/botl/object.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,276 +1,311 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402
+# pylint: disable=C,R,W0105,W0613,E0101
 
 
-"handler"
+"""a clean namespace
 
+This module allows for easy json save//load to/from disk of objects. It
+provides an "clean namespace" Object class that only has dunder
+methods, so the namespace is not cluttered with method names. This makes
+storing and reading to/from json possible.
 
-import inspect
-import queue
-import threading
-import time
+"""
+
+
+import json
+import os
+import pathlib
 import _thread
 
 
-from objx import Default, Object, Persist, spl
+disklock = _thread.allocate_lock()
 
 
-from .brokers import Broker
-from .excepts import Error
-from .threads import launch
+class Object:
 
+    "Base class."
 
-class Command(Object):
+    def __contains__(self, key):
+        return key in dir(self)
 
-    cmds = Object()
+    def __iter__(self):
+        return iter(self.__dict__)
 
-    @staticmethod
-    def add(func):
-        setattr(Command.cmds, func.__name__, func)
+    def __len__(self):
+        return len(self.__dict__)
 
+    def __str__(self):
+        return str(self.__dict__)
 
-class Message(Default):
 
-    def __init__(self):
-        Default.__init__(self)
-        self._ready  = threading.Event()
-        self._thr    = None
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-        self.type    = "event"
-
-    def ready(self):
-        self._ready.set()
-
-    def reply(self, txt):
-        self.result.append(txt)
-
-    def show(self):
-        bot = Broker.get(self.orig)
-        for txt in self.result:
-            bot.say(self.channel, txt)
-
-    def wait(self):
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
+def construct(obj, *args, **kwargs):
+    "construct an object from provided arguments."
+    if args:
+        val = args[0]
+        if isinstance(val, zip):
+            update(obj, dict(val))
+        elif isinstance(val, dict):
+            update(obj, val)
+        elif isinstance(val, Object):
+            update(obj, vars(val))
+    if kwargs:
+        update(obj, kwargs)
 
 
-class Handler(Object):
+def edit(obj, setter, skip=False):
+    "edit an object from provided dict/dict-like."
+    for key, val in items(setter):
+        if skip and val == "":
+            continue
+        try:
+            setattr(obj, key, int(val))
+            continue
+        except ValueError:
+            pass
+        try:
+            setattr(obj, key, float(val))
+            continue
+        except ValueError:
+            pass
+        if val in ["True", "true"]:
+            setattr(obj, key, True)
+        elif val in ["False", "false"]:
+            setattr(obj, key, False)
+        else:
+            setattr(obj, key, val)
 
-    def __init__(self):
-        Object.__init__(self)
-        self.cbs      = Object()
-        self.queue    = queue.Queue()
-        self.stopped  = threading.Event()
-        self.threaded = True
-        Broker.add(self)
-
-    def callback(self, evt):
-        func = getattr(self.cbs, evt.type, None)
-        if not func:
-            evt.ready()
-            return
-        if self.threaded:
-            evt._thr = launch(func, evt)
+
+def fmt(obj, args=None, skip=None, plain=False):
+    "format an object to a printable string."
+    if args is None:
+        args = keys(obj)
+    if skip is None:
+        skip = []
+    txt = ""
+    for key in args:
+        if key.startswith("__"):
+            continue
+        if key in skip:
+            continue
+        value = getattr(obj, key, None)
+        if value is None:
+            continue
+        if plain:
+            txt += f"{value} "
+        elif isinstance(value, str) and len(value.split()) >= 2:
+            txt += f'{key}="{value}" '
         else:
-            func(evt)
-            evt.ready()
+            txt += f"{key}={value} "
+    return txt.strip()
 
-    def loop(self):
-        while not self.stopped.is_set():
-            try:
-                evt = self.poll()
-                self.callback(evt)
-            except (KeyboardInterrupt, EOFError):
-                _thread.interrupt_main()
 
-    def poll(self):
-        return self.queue.get()
+def fqn(obj):
+    "return full qualified name of an object."
+    kin = str(type(obj)).split()[-1][1:-2]
+    if kin == "type":
+        kin = obj.__name__
+    return kin
+
+
+def items(obj):
+    "return the items of an object."
+    if isinstance(obj, type({})):
+        return obj.items()
+    return obj.__dict__.items()
+
+
+def keys(obj):
+    "return keys of an object."
+    if isinstance(obj, type({})):
+        return obj.keys()
+    return list(obj.__dict__.keys())
+
+
+def read(obj, pth):
+    "read an object from file path."
+    with disklock:
+        with open(pth, 'r', encoding='utf-8') as ofile:
+            update(obj, load(ofile))
+
+
+def search(obj, selector):
+    "check if object matches provided values."
+    res = False
+    if not selector:
+        return True
+    for key, value in items(selector):
+        val = getattr(obj, key, None)
+        if str(value).lower() in str(val).lower():
+            res = True
+        else:
+            res = False
+            break
+    return res
 
-    def put(self, evt):
-        self.queue.put_nowait(evt)
 
-    def register(self, typ, cbs):
-        setattr(self.cbs, typ, cbs)
+def update(obj, data, empty=True):
+    "update an object."
+    for key, value in items(data):
+        if empty and not value:
+            continue
+        setattr(obj, key, value)
 
-    def start(self):
-        launch(self.loop)
 
-    def stop(self):
-        self.stopped.set()
+def values(obj):
+    "return values of an object."
+    return obj.__dict__.values()
 
 
-class Client(Handler):
+def write(obj, pth):
+    "write an object to disk."
+    with disklock:
+        cdir(os.path.dirname(pth))
+        with open(pth, 'w', encoding='utf-8') as ofile:
+            dump(obj, ofile, indent=4)
 
-    def __init__(self):
-        Handler.__init__(self)
-        self.register("command", command)
 
-    def announce(self, txt):
-        self.raw(txt)
+class ObjectDecoder(json.JSONDecoder):
 
-    def say(self, channel, txt):
-        self.raw(txt)
+    "Object decoded"
 
-    def show(self, evt):
-        for txt in evt.result:
-            self.say(evt.channel, txt)
+    def __init__(self, *args, **kwargs):
+        return json.JSONDecoder.__init__(self, *args)
 
-    def raw(self, txt):
-        pass
+    def decode(self, s, _w=None):
+        "decoding string to object."
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
 
+    def raw_decode(self, s, idx=0):
+        "decode partial string to object."
+        return json.JSONDecoder.raw_decode(self, s, idx)
 
-"utility"
 
+def hook(objdict, typ=None):
+    "construct object from dict."
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw):
+    "load object from file."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw):
+    "load object from string."
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    "Object encoder."
+
+    def __init__(self, *args, **kwargs):
+        return json.JSONEncoder.__init__(self, *args, **kwargs)
+
+    def default(self, o):
+        "return stringable value."
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return o.__dict__
 
-def cmnd(txt, out):
-    clt = Client()
-    clt.raw = out
-    evn = Message()
-    evn.orig = object.__repr__(clt)
-    evn.txt = txt
-    command(evn)
-    evn.wait()
-    return evn
+    def encode(self, o) -> str:
+        "encode object to string."
+        return json.JSONEncoder.encode(self, o)
 
+    def iterencode(self, o, _one_shot=False):
+        "loop over object to encode to string."
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
 
-def command(evt):
-    parse_cmd(evt)
-    func = getattr(Command.cmds, evt.cmd, None)
-    if func:
-        try:
-            func(evt)
-            evt.show()
-        except Exception as exc:
-            Error.add(exc)
-    evt.ready()
 
+def dump(*args, **kw):
+    "dump object to file."
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
 
-def forever():
-    while 1:
-        try:
-            time.sleep(1.0)
-        except (KeyboardInterrupt, EOFError):
-            _thread.interrupt_main()
 
+def dumps(*args, **kw):
+    "dump object to string."
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
 
-def laps(seconds, short=True):
-    txt = ""
-    nsec = float(seconds)
-    if nsec < 1:
-        return f"{nsec:.2f}s"
-    yea = 365*24*60*60
-    week = 7*24*60*60
-    nday = 24*60*60
-    hour = 60*60
-    minute = 60
-    yeas = int(nsec/yea)
-    nsec -= yeas*yea
-    weeks = int(nsec/week)
-    nsec -= weeks*week
-    nrdays = int(nsec/nday)
-    nsec -= nrdays*nday
-    hours = int(nsec/hour)
-    nsec -= hours*hour
-    minutes = int(nsec/minute)
-    nsec -= int(minute*minutes)
-    sec = int(nsec)
-    if yeas:
-        txt += f"{yeas}y"
-    if weeks:
-        nrdays += weeks * 7
-    if nrdays:
-        txt += f"{nrdays}d"
-    if short and txt:
-        return txt.strip()
-    if hours:
-        txt += f"{hours}h"
-    if minutes:
-        txt += f"{minutes}m"
-    if sec:
-        txt += f"{sec}s"
-    txt = txt.strip()
-    return txt
-
-
-def parse_cmd(obj, txt=None):
-    args = []
-    obj.args    = obj.args or []
-    obj.cmd     = obj.cmd or ""
-    obj.gets    = obj.gets or Default()
-    obj.hasmods = obj.hasmod or False
-    obj.index   = None
-    obj.mod     = obj.mod or ""
-    obj.opts    = obj.opts or ""
-    obj.result  = obj.reult or []
-    obj.sets    = obj.sets or Default()
-    obj.txt     = txt or obj.txt or ""
-    obj.otxt    = obj.txt
-    _nr = -1
-    for spli in obj.otxt.split():
-        if spli.startswith("-"):
-            try:
-                obj.index = int(spli[1:])
-            except ValueError:
-                obj.opts += spli[1:]
-            continue
-        if "==" in spli:
-            key, value = spli.split("==", maxsplit=1)
-            if key in obj.gets:
-                val = getattr(obj.gets, key)
-                value = val + "," + value
-            setattr(obj.gets, key, value)
-            continue
-        if "=" in spli:
-            key, value = spli.split("=", maxsplit=1)
-            if key == "mod":
-                obj.hasmods = True
-                if obj.mod:
-                    obj.mod += f",{value}"
-                else:
-                    obj.mod = value
-                continue
-            setattr(obj.sets, key, value)
-            continue
-        _nr += 1
-        if _nr == 0:
-            obj.cmd = spli
-            continue
-        args.append(spli)
-    if args:
-        obj.args = args
-        obj.txt  = obj.cmd or ""
-        obj.rest = " ".join(obj.args)
-        obj.txt  = obj.cmd + " " + obj.rest
-    else:
-        obj.txt = obj.cmd or ""
 
+class Default(Object):
 
+    "Object that return a default value if key does not exist."
 
-def scan(pkg, modstr, initer=False, disable="", wait=True):
-    mds = []
-    for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        for _key, cmd in inspect.getmembers(module, inspect.isfunction):
-            if 'event' in cmd.__code__.co_varnames:
-                Command.add(cmd)
-        for _key, clz in inspect.getmembers(module, inspect.isclass):
-            if not issubclass(clz, Object):
-                continue
-            Persist.add(clz)
-        if initer and "init" in dir(module):
-            module._thr = launch(module.init, name=f"init {modname}")
-            mds.append(module)
-    if wait and initer:
-        for mod in mds:
-            mod._thr.join()
-    return mds
+    __slots__ = ("__default__",)
+
+    def __init__(self):
+        Object.__init__(self)
+        self.__default__ = ""
+
+    def __getattr__(self, key):
+        return self.__dict__.get(key, self.__default__)
+
+
+def cdir(pth):
+    "create directory."
+    if os.path.exists(pth):
+        return
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
+def spl(txt):
+    "split comma separated string into a list."
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
+
+
+"interface"
+
+
+def __dir__():
+    return (
+        'Default',
+        'Object',
+        'construct',
+        'dump',
+        'dumps',
+        'edit',
+        'fmt',
+        'fqn',
+        'hook',
+        'items',
+        'keys',
+        'load',
+        'loads',
+        'read',
+        'search',
+        'update',
+        'values',
+        'write'
+    )
+
+
+__all__ = __dir__()
```

### Comparing `botl-104/pyproject.toml` & `botl-105/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -3,36 +3,44 @@
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "botl"
-description = "cli library"
-version = "104"
+description = "cli bot"
+version = "105"
 authors = [
-    {name = "Bart Thate",email = "objx@proton.me"},
+    {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
-dependencies = [
-    "objx",
-]
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
+[project.scripts]
+"botl" = "botl.__main__:wrapped"
+
+
 [project.urls]
 "home" = "https://pypi.org/project/botl"
 "bugs" = "https://github.com/xobjectz/botl/issues"
 "source" = "https://github.com/xobjectz/botl"
 
-[tool.setuptools]
 
+[tool.setuptools]
 packages = [
     "botl",
+    "botl.modules"
 ]
 zip-safe=true
+
+
+[tool.setuptools.data-files]
+"share/doc/botl" = [
+    "README.rst"
+]
```

