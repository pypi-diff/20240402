# Comparing `tmp/ndbioimage-2024.3.7.tar.gz` & `tmp/ndbioimage-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.3.7.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.0.tar", max compression
```

## Comparing `ndbioimage-2024.3.7.tar` & `ndbioimage-2024.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.3.7/LICENSE
--rw-r--r--   0        0        0     2608 2023-11-21 15:08:51.110664 ndbioimage-2024.3.7/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.3.7/ndbioimage/.DS_Store
--rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2024.3.7/ndbioimage/AiryScan.xml
--rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2024.3.7/ndbioimage/Elyra_test.xml
--rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2024.3.7/ndbioimage/Elyra_test2.xml
--rwxr-xr-x   0        0        0    50023 2024-03-26 13:18:37.527233 ndbioimage-2024.3.7/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.3.7/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.3.7/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.3.7/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    29477 2024-03-26 13:24:25.131240 ndbioimage-2024.3.7/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2596 2024-03-26 13:15:53.427049 ndbioimage-2024.3.7/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2076 2024-03-26 13:14:17.966942 ndbioimage-2024.3.7/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6436 2024-03-26 13:13:06.574862 ndbioimage-2024.3.7/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3007 2024-03-26 13:15:53.467049 ndbioimage-2024.3.7/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.3.7/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17829 2024-03-26 13:15:53.507049 ndbioimage-2024.3.7/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1010 2024-03-26 13:18:27.611222 ndbioimage-2024.3.7/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     2608 2023-11-21 15:08:51.110664 ndbioimage-2024.4.0/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.0/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2024.4.0/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2024.4.0/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2024.4.0/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    51234 2024-04-02 16:23:58.720136 ndbioimage-2024.4.0/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.0/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.0/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.0/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.0/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.0/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.0/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.0/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.0/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.0/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.0/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1010 2024-04-02 16:19:40.692305 ndbioimage-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.0/PKG-INFO
```

### Comparing `ndbioimage-2024.3.7/LICENSE` & `ndbioimage-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/README.md` & `ndbioimage-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/.DS_Store` & `ndbioimage-2024.4.0/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/AiryScan.xml` & `ndbioimage-2024.4.0/ndbioimage/AiryScan.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/Elyra_test.xml` & `ndbioimage-2024.4.0/ndbioimage/Elyra_test.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/Elyra_test2.xml` & `ndbioimage-2024.4.0/ndbioimage/Elyra_test2.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/__init__.py` & `ndbioimage-2024.4.0/ndbioimage/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1167 +1,1225 @@
-import multiprocessing
-import re
-import warnings
-from abc import ABC, ABCMeta, abstractmethod
-from argparse import ArgumentParser
-from collections import OrderedDict
-from datetime import datetime
-from functools import cached_property, wraps
-from importlib.metadata import version
-from itertools import product
-from numbers import Number
-from operator import truediv
-from pathlib import Path
-from traceback import print_exc
-
-import numpy as np
-import ome_types
-import yaml
-from ome_types import OME, model, ureg
-from pint import set_application_registry
-from tiffwrite import IJTiffFile
-from tqdm.auto import tqdm
-
-from .jvm import JVM
-from .transforms import Transform, Transforms
-
-try:
-    __version__ = version(Path(__file__).parent.name)
-except Exception:  # noqa
-    __version__ = 'unknown'
-
-try:
-    with open(Path(__file__).parent.parent / '.git' / 'HEAD') as g:
-        head = g.read().split(':')[1].strip()
-    with open(Path(__file__).parent.parent / '.git' / head) as h:
-        __git_commit_hash__ = h.read().rstrip('\n')
-except Exception:  # noqa
-    __git_commit_hash__ = 'unknown'
-
-ureg.default_format = '~P'
-set_application_registry(ureg)
-warnings.filterwarnings('ignore', 'Reference to unknown ID')
-
-
-class ReaderNotFoundError(Exception):
-    pass
-
-
-class TransformTiff(IJTiffFile):
-    """ transform frames in a parallel process to speed up saving """
-    def __init__(self, image, *args, **kwargs):
-        self.image = image
-        super().__init__(*args, **kwargs)
-
-    def compress_frame(self, frame):
-        return super().compress_frame(np.asarray(self.image(*frame)).astype(self.dtype))
-
-
-class DequeDict(OrderedDict):
-    def __init__(self, maxlen=None, *args, **kwargs):
-        self.maxlen = maxlen
-        super().__init__(*args, **kwargs)
-
-    def __truncate__(self):
-        if self.maxlen is not None:
-            while len(self) > self.maxlen:
-                self.popitem(False)
-
-    def __setitem__(self, *args, **kwargs):
-        super().__setitem__(*args, **kwargs)
-        self.__truncate__()
-
-    def update(self, *args, **kwargs):
-        super().update(*args, **kwargs)
-        self.__truncate__()
-
-
-def find(obj, **kwargs):
-    for item in obj:
-        try:
-            if all([getattr(item, key) == value for key, value in kwargs.items()]):
-                return item
-        except AttributeError:
-            pass
-
-
-def try_default(fun, default, *args, **kwargs):
-    try:
-        return fun(*args, **kwargs)
-    except Exception:  # noqa
-        return default
-
-
-def get_ome(path):
-    from .readers.bfread import jars
-    try:
-        jvm = JVM(jars)  # noqa
-        ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
-        reader = jvm.image_reader()
-        reader.setMetadataStore(ome_meta)
-        reader.setId(str(path))
-        ome = ome_types.from_xml(str(ome_meta.dumpXML()), parser='lxml')
-    except Exception:  # noqa
-        print_exc()
-        ome = model.OME()
-    finally:
-        jvm.kill_vm()  # noqa
-    return ome
-
-
-class Shape(tuple):
-    def __new__(cls, shape, axes='yxczt'):
-        if isinstance(shape, Shape):
-            axes = shape.axes
-        instance = super().__new__(cls, shape)
-        instance.axes = axes.lower()
-        return instance
-
-    def __getitem__(self, n):
-        if isinstance(n, str):
-            if len(n) == 1:
-                return self[self.axes.find(n.lower())] if n.lower() in self.axes else 1
-            else:
-                return tuple(self[i] for i in n)
-        return super().__getitem__(n)
-
-    @cached_property
-    def yxczt(self):
-        return tuple(self[i] for i in 'yxczt')
-
-
-class OmeCache(DequeDict):
-    def __new__(cls, *args, **kwargs):
-        if not hasattr(cls, 'instance'):
-            cls.instance = super().__new__(cls)
-        return cls.instance
-
-    def __init__(self):
-        super().__init__(64)
-
-
-class Imread(np.lib.mixins.NDArrayOperatorsMixin, ABC):
-    """ class to read image files, while taking good care of important metadata,
-        currently optimized for .czi files, but can open anything that bioformats can handle
-            path: path to the image file
-            optional:
-            series: in case multiple experiments are saved in one file, like in .lif files
-            dtype: datatype to be used when returning frames
-            meta: define metadata, used for pickle-ing
-
-            NOTE: run imread.kill_vm() at the end of your script/program, otherwise python might not terminate
-
-            modify images on the fly with a decorator function:
-                define a function which takes an instance of this object, one image frame,
-                and the coordinates c, z, t as arguments, and one image frame as return
-                >> imread.frame_decorator = fun
-                then use imread as usually
-
-            Examples:
-                >> im = imread('/DATA/lenstra_lab/w.pomp/data/20190913/01_YTL639_JF646_DefiniteFocus.czi')
-                >> im
-                 << shows summary
-                >> im.shape
-                 << (256, 256, 2, 1, 600)
-                >> plt.imshow(im(1, 0, 100))
-                 << plots frame at position c=1, z=0, t=100 (python type indexing), note: round brackets; always 2d array
-                    with 1 frame
-                >> data = im[:,:,0,0,:25]
-                 << retrieves 5d numpy array containing first 25 frames at c=0, z=0, note: square brackets; always 5d array
-                >> plt.imshow(im.max(0, None, 0))
-                 << plots max-z projection at c=0, t=0
-                >> len(im)
-                 << total number of frames
-                >> im.pxsize
-                 << 0.09708737864077668 image-plane pixel size in um
-                >> im.laserwavelengths
-                 << [642, 488]
-                >> im.laserpowers
-                 << [0.02, 0.0005] in %
-
-                See __init__ and other functions for more ideas.
-
-            Subclassing:
-                Subclass AbstractReader to add more file types. A subclass should always have at least the following
-                methods:
-                    staticmethod _can_open(path): returns True when the subclass can open the image in path
-                    __metadata__(self): pulls some metadata from the file and do other format specific things,
-                                        it needs to define a few properties, like shape, etc.
-                    __frame__(self, c, z, t): this should return a single frame at channel c, slice z and time t
-                    optional close(self): close the file in a proper way
-                    optional field priority: subclasses with lower priority will be tried first, default = 99
-                    Any other method can be overridden as needed
-            wp@tl2019-2023 """
-
-    def __new__(cls, path=None, *args, **kwargs):
-        if cls is not Imread:
-            return super().__new__(cls)
-        if len(AbstractReader.__subclasses__()) == 0:
-            raise Exception('Restart python kernel please!')
-        if isinstance(path, Imread):
-            return path
-        path, _ = AbstractReader.split_path_series(path)
-        for subclass in sorted(AbstractReader.__subclasses__(), key=lambda subclass_: subclass_.priority):
-            if subclass._can_open(path):
-                do_not_pickle = (AbstractReader.do_not_pickle,) if isinstance(AbstractReader.do_not_pickle, str) \
-                    else AbstractReader.do_not_pickle
-                subclass_do_not_pickle = (subclass.do_not_pickle,) if isinstance(subclass.do_not_pickle, str) \
-                    else subclass.do_not_pickle if hasattr(subclass, 'do_not_pickle') else ()
-                subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
-
-                return super().__new__(subclass)
-        raise ReaderNotFoundError(f'No reader found for {path}.')
-
-    def __init__(self, base=None, slice=None, shape=(0, 0, 0, 0, 0), dtype=None, frame_decorator=None):
-        self.base = base or self
-        self.slice = slice
-        self._shape = Shape(shape)
-        self.dtype = dtype
-        self.frame_decorator = frame_decorator
-        self.transform = Transforms()
-        self.flags = dict(C_CONTIGUOUS=False, F_CONTIGUOUS=False, OWNDATA=False, WRITEABLE=False,
-                          ALIGNED=False, WRITEBACKIFCOPY=False, UPDATEIFCOPY=False)
-
-    def __call__(self, c=None, z=None, t=None, x=None, y=None):
-        """ same as im[] but allowing keyword axes, but slices need to made with slice() or np.s_ """
-        return self[{k: slice(v) if v is None else v for k, v in dict(c=c, z=z, t=t, x=x, y=y).items()}]
-
-    def __copy__(self):
-        return self.copy()
-
-    def __contains__(self, item):
-        def unique_yield(a, b):
-            for k in a:
-                yield k
-            for k in b:
-                if k not in a:
-                    yield k
-
-        for idx in unique_yield([key[:3] for key in self.cache.keys()],
-                                product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t']))):
-            yxczt = (slice(None), slice(None)) + idx
-            in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-            if item in np.asarray(self[in_idx]):
-                return True
-        return False
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *args, **kwargs):
-        if not self.isclosed:
-            self.isclosed = True
-            if hasattr(self, 'close'):
-                self.close()
-
-    def __getitem__(self, n):
-        """ slice like a numpy array but return an Imread instance """
-        if self.isclosed:
-            raise OSError('file is closed')
-        if isinstance(n, (slice, Number)):  # None = :
-            n = (n,)
-        elif isinstance(n, type(Ellipsis)):
-            n = (None,) * len(self.axes)
-        elif isinstance(n, dict):  # allow im[dict(z=0)] etc.
-            n = [n.get(i, slice(None)) for i in self.axes]
-        n = list(n)
-
-        # deal with ...
-        ell = [i for i, e in enumerate(n) if isinstance(e, type(Ellipsis))]
-        if len(ell) > 1:
-            raise IndexError('an index can only have a single ellipsis (...)')
-        if len(ell):
-            if len(n) > self.ndim:
-                n.remove(Ellipsis)
-            else:
-                n[ell[0]] = None
-                while len(n) < self.ndim:
-                    n.insert(ell[0], None)
-        while len(n) < self.ndim:
-            n.append(None)
-
-        axes_idx = [self.shape.axes.find(i) for i in 'yxczt']
-        n = [n[j] if 0 <= j < len(n) else None for j in axes_idx]  # reorder n
-
-        new_slice = []
-        for s, e in zip(self.slice, n):
-            if e is None:
-                new_slice.append(s)
-            else:
-                new_slice.append(s[e])
-
-        # TODO: check output dimensionality when requested shape in some dimension is 1
-        if all([isinstance(s, Number) or a < 0 and s.size == 1 for s, a in zip(new_slice, axes_idx)]):
-            return self.block(*new_slice).item()
-        else:
-            new = View(self)
-            new.slice = new_slice
-            new._shape = Shape([1 if isinstance(s, Number) else len(s) for s in new_slice])
-            new.axes = ''.join(j for j in self.axes if j in [i for i, s in zip('yxczt', new_slice)
-                                                             if not isinstance(s, Number)])
-            return new
-
-    def __getstate__(self):
-        return {key: value for key, value in self.__dict__.items() if key not in self.do_not_pickle}
-
-    def __len__(self):
-        return self.shape[0]
-
-    def __repr__(self):
-        return self.summary
-
-    def __setstate__(self, state):
-        """ What happens during unpickling """
-        self.__dict__.update(state)
-        if isinstance(self, AbstractReader):
-            self.open()
-        self.cache = DequeDict(16)
-
-    def __str__(self):
-        return str(self.path)
-
-    def __array__(self, dtype=None):
-        block = self.block(*self.slice)
-        axes_idx = [self.shape.axes.find(i) for i in 'yxczt']
-        axes_squeeze = tuple({i for i, j in enumerate(axes_idx) if j == -1}.union(
-            {i for i, j in enumerate(self.slice) if isinstance(j, Number)}))
-        block = block.squeeze(axes_squeeze)
-        if dtype is not None:
-            block = block.astype(dtype)
-        if block.ndim == 0:
-            return block.item()
-        axes = ''.join(j for i, j in enumerate('yxczt') if i not in axes_squeeze)
-        return block.transpose([axes.find(i) for i in self.shape.axes if i in axes])
-
-    def __array_arg_fun__(self, fun, axis=None, out=None):
-        """ frame-wise application of np.argmin and np.argmax """
-        if axis is None:
-            value = arg = None
-            for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                yxczt = (slice(None), slice(None)) + idx
-                in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-                new = np.asarray(self[in_idx])
-                new_arg = np.unravel_index(fun(new), new.shape)
-                new_value = new[new_arg]
-                if value is None:
-                    arg = new_arg + idx
-                    value = new_value
-                else:
-                    i = fun((value, new_value))
-                    arg = (arg, new_arg + idx)[i]
-                    value = (value, new_value)[i]
-            axes = ''.join(i for i in self.axes if i in 'yx') + 'czt'
-            arg = np.ravel_multi_index([arg[axes.find(i)] for i in self.axes], self.shape)
-            if out is None:
-                return arg
-            else:
-                out.itemset(arg)
-                return out
-        else:
-            if isinstance(axis, str):
-                axis_str, axis_idx = axis, self.axes.index(axis)
-            else:
-                axis_str, axis_idx = self.axes[axis], axis
-            if axis_str not in self.axes:
-                raise IndexError(f'Axis {axis_str} not in {self.axes}.')
-            out_shape = list(self.shape)
-            out_axes = list(self.axes)
-            out_shape.pop(axis_idx)
-            out_axes.pop(axis_idx)
-            if out is None:
-                out = np.zeros(out_shape, int)
-            if axis_str in 'yx':
-                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                    yxczt = (slice(None), slice(None)) + idx
-                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
-                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-                    new = self[in_idx]
-                    out[out_idx] = fun(np.asarray(new), new.axes.find(axis_str))
-            else:
-                value = np.zeros(out.shape, self.dtype)
-                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                    yxczt = (slice(None), slice(None)) + idx
-                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
-                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-                    new_value = self[in_idx]
-                    new_arg = np.full_like(new_value, idx['czt'.find(axis_str)])
-                    if idx['czt'.find(axis_str)] == 0:
-                        value[out_idx] = new_value
-                        out[out_idx] = new_arg
-                    else:
-                        old_value = value[out_idx]
-                        i = fun((old_value, new_value), 0)
-                        value[out_idx] = np.where(i, new_value, old_value)
-                        out[out_idx] = np.where(i, new_arg, out[out_idx])
-            return out
-
-    def __array_fun__(self, funs, axis=None, dtype=None, out=None, keepdims=False, initials=None, where=True,
-                      ffuns=None, cfun=None):
-        """ frame-wise application of np.min, np.max, np.sum, np.mean and their nan equivalents """
-        p = re.compile(r'\d')
-        dtype = self.dtype if dtype is None else np.dtype(dtype)
-        if initials is None:
-            initials = [None for _ in funs]
-        if ffuns is None:
-            ffuns = [None for _ in funs]
-
-        def ffun_(frame):
-            return np.asarray(frame)
-        ffuns = [ffun_ if ffun is None else ffun for ffun in ffuns]
-        if cfun is None:
-            def cfun(*res):
-                return res[0]
-
-        # TODO: smarter transforms
-        if axis is None:
-            for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                yxczt = (slice(None), slice(None)) + idx
-                in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-                w = where if where is None or isinstance(where, bool) else where[in_idx]
-                initials = [fun(np.asarray(ffun(self[in_idx])), initial=initial, where=w)
-                            for fun, ffun, initial in zip(funs, ffuns, initials)]
-            res = cfun(*initials)
-            res = (np.round(res) if dtype.kind in 'ui' else res).astype(p.sub('', dtype.name))
-            if keepdims:
-                res = np.array(res, dtype, ndmin=self.ndim)
-            if out is None:
-                return res
-            else:
-                out.itemset(res)
-                return out
-        else:
-            if isinstance(axis, str):
-                axis_str, axis_idx = axis, self.axes.index(axis)
-            else:
-                axis_idx = axis % self.ndim
-                axis_str = self.axes[axis_idx]
-            if axis_str not in self.axes:
-                raise IndexError(f'Axis {axis_str} not in {self.axes}.')
-            out_shape = list(self.shape)
-            out_axes = list(self.axes)
-            if not keepdims:
-                out_shape.pop(axis_idx)
-                out_axes.pop(axis_idx)
-            if out is None:
-                out = np.zeros(out_shape, dtype)
-            if axis_str in 'yx':
-                yx = 'yx' if self.axes.find('x') > self.axes.find('y') else 'yx'
-                frame_ax = yx.find(axis_str)
-                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                    yxczt = (slice(None), slice(None)) + idx
-                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
-                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-                    w = where if where is None or isinstance(where, bool) else where[in_idx]
-                    res = cfun(*[fun(ffun(self[in_idx]), frame_ax, initial=initial, where=w)
-                                 for fun, ffun, initial in zip(funs, ffuns, initials)])
-                    out[out_idx] = (np.round(res) if out.dtype.kind in 'ui' else res).astype(p.sub('', dtype.name))
-            else:
-                tmps = [np.zeros(out_shape) for _ in ffuns]
-                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
-                    yxczt = (slice(None), slice(None)) + idx
-                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
-                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
-
-                    if idx['czt'.find(axis_str)] == 0:
-                        w = where if where is None or isinstance(where, bool) else (where[in_idx],)
-                        for tmp, fun, ffun, initial in zip(tmps, funs, ffuns, initials):
-                            tmp[out_idx] = fun((ffun(self[in_idx]),), 0, initial=initial, where=w)
-                    else:
-                        w = where if where is None or isinstance(where, bool) else \
-                            (np.ones_like(where[in_idx]), where[in_idx])
-                        for tmp, fun, ffun in zip(tmps, funs, ffuns):
-                            tmp[out_idx] = fun((tmp[out_idx], ffun(self[in_idx])), 0, where=w)
-                out[...] = (np.round(cfun(*tmps)) if out.dtype.kind in 'ui' else
-                            cfun(*tmps)).astype(p.sub('', dtype.name))
-            return out
-
-    @property
-    def axes(self):
-        return self.shape.axes
-
-    @axes.setter
-    def axes(self, value):
-        shape = self.shape[value]
-        if isinstance(shape, Number):
-            shape = (shape,)
-        self._shape = Shape(shape, value)
-
-    @property
-    def dtype(self):
-        return self._dtype
-
-    @dtype.setter
-    def dtype(self, value):
-        self._dtype = np.dtype(value)
-
-    @cached_property
-    def extrametadata(self):
-        if isinstance(self.path, Path):
-            if self.path.with_suffix('.pzl2').exists():
-                pname = self.path.with_suffix('.pzl2')
-            elif self.path.with_suffix('.pzl').exists():
-                pname = self.path.with_suffix('.pzl')
-            else:
-                return
-            try:
-                return self.get_config(pname)
-            except Exception:  # noqa
-                return
-        return
-
-    @property
-    def ndim(self):
-        return len(self.shape)
-
-    @property
-    def size(self):
-        return np.prod(self.shape)
-
-    @property
-    def shape(self):
-        return self._shape
-
-    @shape.setter
-    def shape(self, value):
-        if isinstance(value, Shape):
-            self._shape = value
-        else:
-            self._shape = Shape((value['yxczt'.find(i.lower())] for i in self.axes), self.axes)
-
-    @property
-    def summary(self):
-        """ gives a helpful summary of the recorded experiment """
-        s = [f'path/filename: {self.path}',
-             f'series/pos:    {self.series}',
-             f"reader:        {self.base.__class__.__module__.split('.')[-1]}"]
-        s.extend((f'dtype:         {self.dtype}',
-                  f'shape ({self.axes}):'.ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"))
-        if self.pxsize_um:
-            s.append(f'pixel size:    {1000 * self.pxsize_um:.2f} nm')
-        if self.zstack and self.deltaz_um:
-            s.append(f'z-interval:    {1000 * self.deltaz_um:.2f} nm')
-        if self.exposuretime_s and not all(e is None for e in self.exposuretime_s):
-            s.append(f'exposuretime:  {self.exposuretime_s[0]:.2f} s')
-        if self.timeseries and self.timeinterval:
-            s.append(f'time interval: {self.timeinterval:.3f} s')
-        if self.binning:
-            s.append('binning:       {}x{}'.format(*self.binning))
-        if self.laserwavelengths:
-            s.append('laser colors:  ' + ' | '.join([' & '.join(len(w) * ('{:.0f}',)).format(*w)
-                                                     for w in self.laserwavelengths]) + ' nm')
-        if self.laserpowers:
-            s.append('laser powers:  ' + ' | '.join([' & '.join(len(p) * ('{:.3g}',)).format(*[100 * i for i in p])
-                                                     for p in self.laserpowers]) + ' %')
-        if self.objective and self.objective.model:
-            s.append(f'objective:     {self.objective.model}')
-        if self.magnification:
-            s.append(f'magnification: {self.magnification}x')
-        if self.tubelens and self.tubelens.model:
-            s.append(f'tubelens:      {self.tubelens.model}')
-        if self.filter:
-            s.append(f'filterset:     {self.filter}')
-        if self.powermode:
-            s.append(f'powermode:     {self.powermode}')
-        if self.collimator:
-            s.append('collimator:   ' + (' {}' * len(self.collimator)).format(*self.collimator))
-        if self.tirfangle:
-            s.append('TIRF angle:   ' + (' {:.2f}°' * len(self.tirfangle)).format(*self.tirfangle))
-        if self.gain:
-            s.append('gain:         ' + (' {:.0f}' * len(self.gain)).format(*self.gain))
-        if self.pcf:
-            s.append('pcf:          ' + (' {:.2f}' * len(self.pcf)).format(*self.pcf))
-        return '\n'.join(s)
-
-    @property
-    def T(self):
-        return self.transpose()
-
-    @cached_property
-    def timeseries(self):
-        return self.shape['t'] > 1
-
-    @cached_property
-    def zstack(self):
-        return self.shape['z'] > 1
-
-    @wraps(np.argmax)
-    def argmax(self, *args, **kwargs):
-        return self.__array_arg_fun__(np.argmax, *args, **kwargs)
-
-    @wraps(np.argmin)
-    def argmin(self, *args, **kwargs):
-        return self.__array_arg_fun__(np.argmin, *args, **kwargs)
-
-    @wraps(np.max)
-    def max(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.max], axis, None, out, keepdims, [initial], where)
-
-    @wraps(np.mean)
-    def mean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
-        dtype = dtype or float
-        n = np.prod(self.shape) if axis is None else self.shape[axis]
-
-        def sfun(frame):
-            return np.asarray(frame).astype(float)
-
-        def cfun(res):
-            return res / n
-
-        return self.__array_fun__([np.sum], axis, dtype, out, keepdims, None, where, [sfun], cfun)
-
-    @wraps(np.min)
-    def min(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.min], axis, None, out, keepdims, [initial], where)
-
-    @wraps(np.moveaxis)
-    def moveaxis(self, source, destination):
-        raise NotImplementedError('moveaxis is not implemented')
-
-    @wraps(np.nanmax)
-    def nanmax(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.nanmax], axis, None, out, keepdims, [initial], where)
-
-    @wraps(np.nanmean)
-    def nanmean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
-        dtype = dtype or float
-
-        def sfun(frame):
-            return np.asarray(frame).astype(float)
-
-        def nfun(frame):
-            return np.invert(np.isnan(frame))
-
-        return self.__array_fun__([np.nansum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, nfun), truediv)
-
-    @wraps(np.nanmin)
-    def nanmin(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.nanmin], axis, None, out, keepdims, [initial], where)
-
-    @wraps(np.nansum)
-    def nansum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.nansum], axis, dtype, out, keepdims, [initial], where)
-
-    @wraps(np.nanstd)
-    def nanstd(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=None):
-        return self.nanvar(axis, dtype, out, ddof, keepdims, where=where, std=True)
-
-    @wraps(np.nanvar)
-    def nanvar(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True, std=False):
-        dtype = dtype or float
-
-        def sfun(frame):
-            return np.asarray(frame).astype(float)
-
-        def s2fun(frame):
-            return np.asarray(frame).astype(float) ** 2
-
-        def nfun(frame):
-            return np.invert(np.isnan(frame))
-
-        if std:
-            def cfun(s, s2, n):
-                return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
-        else:
-            def cfun(s, s2, n):
-                return (s2 - s ** 2 / n) / (n - ddof)
-        return self.__array_fun__([np.nansum, np.nansum, np.sum], axis, dtype, out, keepdims, None, where,
-                                  (sfun, s2fun, nfun), cfun)
-
-    def flatten(self, *args, **kwargs):
-        return np.asarray(self).flatten(*args, **kwargs)
-
-    @wraps(np.reshape)
-    def reshape(self, *args, **kwargs):
-        return np.asarray(self).reshape(*args, **kwargs)
-
-    @wraps(np.squeeze)
-    def squeeze(self, axes=None):
-        new = self.copy()
-        if axes is None:
-            axes = tuple(i for i, j in enumerate(new.shape) if j == 1)
-        elif isinstance(axes, Number):
-            axes = (axes,)
-        else:
-            axes = tuple(new.axes.find(ax) if isinstance(ax, str) else ax for ax in axes)
-        if any([new.shape[ax] != 1 for ax in axes]):
-            raise ValueError('cannot select an axis to squeeze out which has size not equal to one')
-        new.axes = ''.join(j for i, j in enumerate(new.axes) if i not in axes)
-        return new
-
-    @wraps(np.std)
-    def std(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True):
-        return self.var(axis, dtype, out, ddof, keepdims, where=where, std=True)
-
-    @wraps(np.sum)
-    def sum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
-        return self.__array_fun__([np.sum], axis, dtype, out, keepdims, [initial], where)
-
-    @wraps(np.swapaxes)
-    def swapaxes(self, axis1, axis2):
-        new = self.copy()
-        axes = new.axes
-        if isinstance(axis1, str):
-            axis1 = axes.find(axis1)
-        if isinstance(axis2, str):
-            axis2 = axes.find(axis2)
-        axes[axis1], axes[axis2] = axes[axis2], axes[axis1]
-        new.axes = axes
-        return new
-
-    @wraps(np.transpose)
-    def transpose(self, *axes):
-        new = self.copy()
-        if not axes:
-            new.axes = new.axes[::-1]
-        else:
-            new.axes = ''.join(ax if isinstance(ax, str) else new.axes[ax] for ax in axes)
-        return new
-
-    @wraps(np.var)
-    def var(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True, std=False):
-        dtype = dtype or float
-        n = np.prod(self.shape) if axis is None else self.shape[axis]
-
-        def sfun(frame):
-            return np.asarray(frame).astype(float)
-
-        def s2fun(frame):
-            return np.asarray(frame).astype(float) ** 2
-
-        if std:
-            def cfun(s, s2):
-                return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
-        else:
-            def cfun(s, s2):
-                return (s2 - s ** 2 / n) / (n - ddof)
-        return self.__array_fun__([np.sum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, s2fun), cfun)
-
-    def asarray(self):
-        return self.__array__()
-
-    def astype(self, dtype, *args, **kwargs):
-        new = self.copy()
-        new.dtype = dtype
-        return new
-
-    def block(self, y=None, x=None, c=None, z=None, t=None):
-        """ returns 5D block of frames """
-        y, x, c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1)
-                         for i, e in zip('yxczt', (y, x, c, z, t)))
-        d = np.empty((len(y), len(x), len(c), len(z), len(t)), self.dtype)
-        for (ci, cj), (zi, zj), (ti, tj) in product(enumerate(c), enumerate(z), enumerate(t)):
-            d[:, :, ci, zi, ti] = self.frame(cj, zj, tj)[y][:, x]
-        return d
-
-    def copy(self):
-        return View(self)
-
-    def data(self, c=0, z=0, t=0):
-        """ returns 3D stack of frames """
-        c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1) for i, e in zip('czt', (c, z, t)))
-        return np.dstack([self.frame(ci, zi, ti) for ci, zi, ti in product(c, z, t)])
-
-    def frame(self, c=0, z=0, t=0):
-        """ returns single 2D frame """
-        c = self.get_channel(c)
-        c %= self.base.shape['c']
-        z %= self.base.shape['z']
-        t %= self.base.shape['t']
-
-        # cache last n (default 16) frames in memory for speed (~250x faster)
-        key = (c, z, t, self.transform, self.frame_decorator)
-        if key in self.cache:
-            self.cache.move_to_end(key)
-            f = self.cache[key]
-        else:
-            f = self.transform[self.channel_names[c], t].frame(self.__frame__(c, z, t))
-            if self.frame_decorator is not None:
-                f = self.frame_decorator(self, f, c, z, t)
-            self.cache[key] = f
-        if self.dtype is not None:
-            return f.copy().astype(self.dtype)
-        else:
-            return f.copy()
-
-    def get_channel(self, channel_name):
-        if not isinstance(channel_name, str):
-            return channel_name
-        else:
-            c = [i for i, c in enumerate(self.channel_names) if c.lower().startswith(channel_name.lower())]
-            assert len(c) > 0, f'Channel {c} not found in {self.channel_names}'
-            assert len(c) < 2, f'Channel {c} not unique in {self.channel_names}'
-            return c[0]
-
-    @staticmethod
-    def get_config(file):
-        """ Open a yml config file """
-        loader = yaml.SafeLoader
-        loader.add_implicit_resolver(
-            r'tag:yaml.org,2002:float',
-            re.compile(r'''^(?:
-                     [-+]?(?:[0-9][0-9_]*)\.[0-9_]*(?:[eE][-+]?[0-9]+)?
-                    |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
-                    |\.[0-9_]+(?:[eE][-+][0-9]+)?
-                    |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\.[0-9_]*
-                    |[-+]?\\.(?:inf|Inf|INF)
-                    |\.(?:nan|NaN|NAN))$''', re.X),
-            list(r'-+0123456789.'))
-        with open(file) as f:
-            return yaml.load(f, loader)
-
-    def get_czt(self, c, z, t):
-        czt = []
-        for i, n in zip('czt', (c, z, t)):
-            if n is None:
-                czt.append(list(range(self.shape[i])))
-            elif isinstance(n, range):
-                if n.stop < 0:
-                    stop = n.stop % self.shape[i]
-                elif n.stop > self.shape[i]:
-                    stop = self.shape[i]
-                else:
-                    stop = n.stop
-                czt.append(list(range(n.start % self.shape[i], stop, n.step)))
-            elif isinstance(n, Number):
-                czt.append([n % self.shape[i]])  # noqa
-            else:
-                czt.append([k % self.shape[i] for k in n])
-        return [self.get_channel(c) for c in czt[0]], *czt[1:]
-
-    @staticmethod
-    def get_ome(path: [str, Path]) -> OME:
-        """ Use java BioFormats to make an ome metadata structure. """
-        with multiprocessing.get_context('spawn').Pool(1) as pool:
-            ome = pool.map(get_ome, (path,))[0]
-
-        # fix ome if necessary
-        for image in ome.images:
-            try:
-                if image.pixels.physical_size_z is None and len(set([plane.the_z
-                                                                     for plane in image.pixels.planes])) > 1:
-                    z = np.array([(plane.position_z * ureg.Quantity(plane.position_z_unit.value).to(ureg.m).magnitude,
-                                   plane.the_z)
-                                  for plane in image.pixels.planes if plane.the_c == 0 and plane.the_t == 0])
-                    i = np.argsort(z[:, 1])
-                    image.pixels.physical_size_z = np.nanmean(np.true_divide(*np.diff(z[i], axis=0).T)) * 1e6
-                    image.pixels.physical_size_z_unit = 'µm'
-            except Exception:
-                pass
-        return ome
-
-    @cached_property
-    def ome(self) -> OME:
-        cache = OmeCache()
-        if self.path not in cache:
-            cache[self.path] = self.get_ome(self.path)
-        return cache[self.path]
-
-    def is_noise(self, volume=None):
-        """ True if volume only has noise """
-        if volume is None:
-            volume = self
-        fft = np.fft.fftn(volume)
-        corr = np.fft.fftshift(np.fft.ifftn(fft * fft.conj()).real / np.sum(volume ** 2))
-        return 1 - corr[tuple([0] * corr.ndim)] < 0.0067
-
-    @staticmethod
-    def kill_vm():
-        JVM().kill_vm()
-
-    def new(self, *args, **kwargs):
-        warnings.warn('Imread.new has been deprecated, use Imread.view instead.', DeprecationWarning, 2)
-        return self.view(*args, **kwargs)
-
-    def save_as_tiff(self, fname=None, c=None, z=None, t=None, split=False, bar=True, pixel_type='uint16', **kwargs):
-        """ saves the image as a tif file
-            split: split channels into different files """
-        if fname is None:
-            fname = self.path.with_suffix('.tif')
-            if fname == self.path:
-                raise FileExistsError(f'File {fname} exists already.')
-        if not isinstance(fname, Path):
-            fname = Path(fname)
-        if split:
-            for i in range(self.shape['c']):
-                if self.timeseries:
-                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, 0, None, False,
-                                      bar, pixel_type)
-                else:
-                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, None, 0, False,
-                                      bar, pixel_type)
-        else:
-            n = [c, z, t]
-            for i, ax in enumerate('czt'):
-                if n[i] is None:
-                    n[i] = range(self.shape[ax])
-                elif not isinstance(n[i], (tuple, list)):
-                    n[i] = (n[i],)
-
-            shape = [len(i) for i in n]
-            with TransformTiff(self, fname.with_suffix('.tif'), shape, pixel_type,
-                            pxsize=self.pxsize_um, deltaz=self.deltaz_um, **kwargs) as tif:
-                for i, m in tqdm(zip(product(*[range(s) for s in shape]), product(*n)),  # noqa
-                                 total=np.prod(shape), desc='Saving tiff', disable=not bar):
-                    tif.save(m, *i)
-
-    def with_transform(self, channels=True, drift=False, file=None, bead_files=()):
-        """ returns a view where channels and/or frames are registered with an affine transformation
-            channels: True/False register channels using bead_files
-            drift: True/False register frames to correct drift
-            file: load registration from file with name file, default: transform.yml in self.path.parent
-            bead_files: files used to register channels, default: files in self.path.parent,
-                with names starting with 'beads'
-            """
-        view = self.view()
-        if file is None:
-            file = Path(view.path.parent) / 'transform.yml'
-        if not bead_files:
-            try:
-                bead_files = Transforms.get_bead_files(view.path.parent)
-            except Exception:
-                if not file.exists():
-                    raise Exception('No transform file and no bead file found.')
-                bead_files = ()
-
-        if channels:
-            try:
-                view.transform = Transforms.from_file(file, T=drift)
-            except Exception:  # noqa
-                view.transform = Transforms().with_beads(view.cyllens, bead_files)
-                if drift:
-                    view.transform = view.transform.with_drift(view)
-                view.transform.save(file.with_suffix('.yml'))
-                view.transform.save_channel_transform_tiff(bead_files, file.with_suffix('.tif'))
-        elif drift:
-            try:
-                view.transform = Transforms.from_file(file, C=False)
-            except Exception:  # noqa
-                view.transform = Transforms().with_drift(self)
-        view.transform.adapt(view.frameoffset, view.shape.yxczt, view.channel_names)
-        return view
-
-    @staticmethod
-    def split_path_series(path):
-        if isinstance(path, str):
-            path = Path(path)
-        if isinstance(path, Path) and path.name.startswith('Pos') and path.name.lstrip('Pos').isdigit():
-            return path.parent, int(path.name.lstrip('Pos'))
-        return path, 0
-
-    def view(self, *args, **kwargs):
-        return View(self, *args, **kwargs)
-
-
-class View(Imread, ABC):
-    def __init__(self, base, dtype=None):
-        super().__init__(base.base, base.slice, base.shape, dtype or base.dtype, base.frame_decorator)
-        self.transform = base.transform
-
-    def __getattr__(self, item):
-        if not hasattr(self.base, item):
-            raise AttributeError(f'{self.__class__} object has no attribute {item}')
-        return self.base.__getattribute__(item)
-
-
-class AbstractReader(Imread, metaclass=ABCMeta):
-    priority = 99
-    do_not_pickle = 'cache'
-    ureg = ureg
-
-    @staticmethod
-    @abstractmethod
-    def _can_open(path):  # Override this method, and return true when the subclass can open the file
-        return False
-
-    @abstractmethod
-    def __frame__(self, c, z, t):  # Override this, return the frame at c, z, t
-        return np.random.randint(0, 255, self.shape['yx'])
-
-    def open(self):  # Optionally override this, open file handles etc.
-        """ filehandles cannot be pickled and should be marked such by setting do_not_pickle = 'file_handle_name' """
-        return
-
-    def close(self):  # Optionally override this, close file handles etc.
-        return
-
-    def __init__(self, path, dtype=None, axes=None):
-        if isinstance(path, Imread):
-            return
-        super().__init__()
-        self.isclosed = False
-        if isinstance(path, str):
-            path = Path(path)
-        self.path, self.series = self.split_path_series(path)
-        if isinstance(path, Path) and path.exists():
-            self.title = self.path.name
-            self.acquisitiondate = datetime.fromtimestamp(self.path.stat().st_mtime).strftime('%y-%m-%dT%H:%M:%S')
-        else:  # ndarray
-            self.title = self.__class__.__name__
-            self.acquisitiondate = 'now'
-
-        self.reader = None
-        self.pcf = None
-        self.powermode = None
-        self.collimator = None
-        self.tirfangle = None
-        self.cyllens = ['None', 'None']
-        self.duolink = 'None'
-        self.detector = [0, 1]
-        self.track = [0]
-        self.cache = DequeDict(16)
-        self.frameoffset = 0, 0  # how far apart the centers of frame and sensor are
-
-        self.open()
-        # extract some metadata from ome
-        instrument = self.ome.instruments[0] if self.ome.instruments else None
-        image = self.ome.images[self.series if len(self.ome.images) > 1 else 0]
-        pixels = image.pixels
-        self.shape = pixels.size_y, pixels.size_x, pixels.size_c, pixels.size_z, pixels.size_t
-        self.dtype = pixels.type.value if dtype is None else dtype
-        self.pxsize = pixels.physical_size_x_quantity
-        try:
-            self.exposuretime = tuple(find(image.pixels.planes, the_c=c).exposure_time_quantity
-                                      for c in range(self.shape['c']))
-        except AttributeError:
-            self.exposuretime = ()
-
-        if self.zstack:
-            self.deltaz = image.pixels.physical_size_z_quantity
-            self.deltaz_um = None if self.deltaz is None else self.deltaz.to(self.ureg.um).m
-        else:
-            self.deltaz = self.deltaz_um = None
-        if image.objective_settings:
-            self.objective = find(instrument.objectives, id=image.objective_settings.id)
-        else:
-            self.objective = None
-        try:
-            t0 = find(image.pixels.planes, the_c=0, the_t=0, the_z=0).delta_t
-            t1 = find(image.pixels.planes, the_c=0, the_t=self.shape['t'] - 1, the_z=0).delta_t
-            self.timeinterval = (t1 - t0) / (self.shape['t'] - 1) if self.shape['t'] > 1 else None
-        except AttributeError:
-            self.timeinterval = None
-        try:
-            self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
-            self.pxsize *= self.binning[0]
-        except (AttributeError, IndexError, ValueError):
-            self.binning = None
-        self.channel_names = [channel.name for channel in image.pixels.channels]
-        self.channel_names += [chr(97 + i) for i in range(len(self.channel_names), self.shape['c'])]
-        self.cnamelist = self.channel_names
-        try:
-            optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
-        except AttributeError:
-            optovars = []
-        if len(optovars) == 0:
-            self.tubelens = None
-        else:
-            self.tubelens = optovars[0]
-        if self.objective:
-            if self.tubelens:
-                self.magnification = self.objective.nominal_magnification * self.tubelens.nominal_magnification
-            else:
-                self.magnification = self.objective.nominal_magnification
-            self.NA = self.objective.lens_na
-        else:
-            self.magnification = None
-            self.NA = None
-
-        self.gain = [find(instrument.detectors, id=channel.detector_settings.id).amplification_gain
-                     for channel in image.pixels.channels
-                     if channel.detector_settings
-                     and find(instrument.detectors, id=channel.detector_settings.id).amplification_gain]
-        self.laserwavelengths = [(channel.excitation_wavelength_quantity.to(self.ureg.nm).m,)
-                                 for channel in pixels.channels if channel.excitation_wavelength_quantity]
-        self.laserpowers = try_default(lambda: [(1 - channel.light_source_settings.attenuation,)
-                                                for channel in pixels.channels], [])
-        self.filter = try_default(lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
-                                           for channel in image.pixels.channels], None)
-        self.pxsize_um = None if self.pxsize is None else self.pxsize.to(self.ureg.um).m
-        self.exposuretime_s = [None if i is None else i.to(self.ureg.s).m for i in self.exposuretime]
-
-        if axes is None:
-            self.axes = ''.join(i for i in 'cztyx' if self.shape[i] > 1)
-        elif axes.lower() == 'full':
-            self.axes = 'cztyx'
-        else:
-            self.axes = axes
-        self.slice = [np.arange(s, dtype=int) for s in self.shape.yxczt]
-
-        m = self.extrametadata
-        if m is not None:
-            try:
-                self.cyllens = m['CylLens']
-                self.duolink = m['DLFilterSet'].split(' & ')[m['DLFilterChannel']]
-                if 'FeedbackChannels' in m:
-                    self.feedback = m['FeedbackChannels']
-                else:
-                    self.feedback = m['FeedbackChannel']
-            except Exception:  # noqa
-                self.cyllens = ['None', 'None']
-                self.duolink = 'None'
-                self.feedback = []
-        try:
-            self.cyllenschannels = np.where([self.cyllens[self.detector[c]].lower() != 'none'
-                                             for c in range(self.shape['c'])])[0].tolist()
-        except Exception:  # noqa
-            pass
-        try:
-            s = int(re.findall(r'_(\d{3})_', self.duolink)[0]) * ureg.nm
-        except Exception:  # noqa
-            s = 561 * ureg.nm
-        try:
-            sigma = []
-            for c, d in enumerate(self.detector):
-                emission = (np.hstack(self.laserwavelengths[c]) + 22) * ureg.nm
-                sigma.append([emission[emission > s].max(initial=0), emission[emission < s].max(initial=0)][d])
-            sigma = np.hstack(sigma)
-            sigma[sigma == 0] = 600 * ureg.nm
-            sigma /= 2 * self.NA * self.pxsize
-            self.sigma = sigma.magnitude.tolist()
-        except Exception:  # noqa
-            self.sigma = [2] * self.shape['c']
-        if not self.NA:
-            self.immersionN = 1
-        elif 1.5 < self.NA:
-            self.immersionN = 1.661
-        elif 1.3 < self.NA < 1.5:
-            self.immersionN = 1.518
-        elif 1 < self.NA < 1.3:
-            self.immersionN = 1.33
-        else:
-            self.immersionN = 1
-
-        p = re.compile(r'(\d+):(\d+)$')
-        try:
-            self.track, self.detector = zip(*[[int(i) for i in p.findall(find(
-                self.ome.images[self.series].pixels.channels, id=f'Channel:{c}').detector_settings.id)[0]]
-                                              for c in range(self.shape['c'])])
-        except Exception:
-            pass
-
-
-def main():
-    parser = ArgumentParser(description='Display info and save as tif')
-    parser.add_argument('file', help='image_file')
-    parser.add_argument('out', help='path to tif out', type=str, default=None, nargs='?')
-    parser.add_argument('-r', '--register', help='register channels', action='store_true')
-    parser.add_argument('-c', '--channel', help='channel', type=int, default=None)
-    parser.add_argument('-z', '--zslice', help='z-slice', type=int, default=None)
-    parser.add_argument('-t', '--time', help='time', type=int, default=None)
-    parser.add_argument('-s', '--split', help='split channels', action='store_true')
-    parser.add_argument('-f', '--force', help='force overwrite', action='store_true')
-    args = parser.parse_args()
-
-    with Imread(args.file) as im:
-        if args.register:
-            im = im.with_transform()
-        print(im.summary)
-        if args.out:
-            out = Path(args.out).absolute()
-            out.parent.mkdir(parents=True, exist_ok=True)
-            if out.exists() and not args.force:
-                print(f'File {args.out} exists already, add the -f flag if you want to overwrite it.')
-            else:
-                im.save_as_tiff(out, args.channel, args.zslice, args.time, args.split)
-
-
-from .readers import *
+from __future__ import annotations
+
+import multiprocessing
+import re
+import warnings
+from abc import ABC, ABCMeta, abstractmethod
+from argparse import ArgumentParser
+from collections import OrderedDict
+from datetime import datetime
+from functools import cached_property, wraps
+from importlib.metadata import version
+from itertools import product
+from numbers import Number
+from operator import truediv
+from pathlib import Path
+from traceback import print_exc
+from typing import Any, Callable, Mapping, Optional
+
+import numpy as np
+import ome_types
+import yaml
+from ome_types import OME, model, ureg
+from pint import set_application_registry
+from tiffwrite import IFD, IJTiffFile
+from tqdm.auto import tqdm
+
+from .jvm import JVM
+from .transforms import Transform, Transforms
+
+try:
+    __version__ = version(Path(__file__).parent.name)
+except Exception:  # noqa
+    __version__ = 'unknown'
+
+try:
+    with open(Path(__file__).parent.parent / '.git' / 'HEAD') as g:
+        head = g.read().split(':')[1].strip()
+    with open(Path(__file__).parent.parent / '.git' / head) as h:
+        __git_commit_hash__ = h.read().rstrip('\n')
+except Exception:  # noqa
+    __git_commit_hash__ = 'unknown'
+
+ureg.default_format = '~P'
+set_application_registry(ureg)
+warnings.filterwarnings('ignore', 'Reference to unknown ID')
+
+
+class ReaderNotFoundError(Exception):
+    pass
+
+
+class TransformTiff(IJTiffFile):
+    """ transform frames in a parallel process to speed up saving """
+    def __init__(self, image: Imread, *args: Any, **kwargs: Any) -> None:
+        self.image = image
+        super().__init__(*args, **kwargs)
+
+    def compress_frame(self, frame: tuple[int, int, int]) -> tuple[IFD, tuple[list[int], list[int]]]:
+        return super().compress_frame(np.asarray(self.image(*frame)).astype(self.dtype))
+
+
+class DequeDict(OrderedDict):
+    def __init__(self, maxlen: int = None, *args: Any, **kwargs: Any) -> None:
+        self.maxlen = maxlen
+        super().__init__(*args, **kwargs)
+
+    def __truncate__(self) -> None:
+        if self.maxlen is not None:
+            while len(self) > self.maxlen:
+                self.popitem(False)
+
+    def __setitem__(self, *args: Any, **kwargs: Any) -> None:
+        super().__setitem__(*args, **kwargs)
+        self.__truncate__()
+
+    def update(self, *args: Any, **kwargs: Any) -> None:
+        super().update(*args, **kwargs)
+        self.__truncate__()
+
+
+def find(obj: Mapping, **kwargs: Any) -> Any:
+    for item in obj:
+        try:
+            if all([getattr(item, key) == value for key, value in kwargs.items()]):
+                return item
+        except AttributeError:
+            pass
+
+
+def try_default(fun: Callable, default: Any, *args: Any, **kwargs: Any) -> Any:
+    try:
+        return fun(*args, **kwargs)
+    except Exception:  # noqa
+        return default
+
+
+def bioformats_ome(path: str | Path) -> OME:
+    from .readers.bfread import jars
+    try:
+        jvm = JVM(jars)  # noqa
+        ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
+        reader = jvm.image_reader()
+        reader.setMetadataStore(ome_meta)
+        reader.setId(str(path))
+        ome = ome_types.from_xml(str(ome_meta.dumpXML()), parser='lxml')
+    except Exception:  # noqa
+        print_exc()
+        ome = model.OME()
+    finally:
+        jvm.kill_vm()  # noqa
+    return ome
+
+
+class Shape(tuple):
+    def __new__(cls, shape: tuple[int] | Shape[int], axes: str = 'yxczt') -> Shape[int]:
+        if isinstance(shape, Shape):
+            axes = shape.axes  # type: ignore
+        instance = super().__new__(cls, shape)
+        instance.axes = axes.lower()
+        return instance  # type: ignore
+
+    def __getitem__(self, n: int | str) -> int | tuple[int]:
+        if isinstance(n, str):
+            if len(n) == 1:
+                return self[self.axes.find(n.lower())] if n.lower() in self.axes else 1
+            else:
+                return tuple(self[i] for i in n)  # type: ignore
+        return super().__getitem__(n)
+
+    @cached_property
+    def yxczt(self) -> tuple[int, int, int, int, int]:
+        return tuple(self[i] for i in 'yxczt')  # type: ignore
+
+
+class CachedPath(Path):
+    """ helper class for checking whether a file has changed, used by OmeCache """
+
+    def __init__(self, path: Path | str) -> None:
+        super().__init__(path)
+        if self.exists():
+            self._lstat = super().lstat()  # save file metadata like creation time etc.
+        else:
+            self._lstat = None
+
+    def __eq__(self, other: Path | CachedPath) -> bool:
+        return super().__eq__(other) and self.lstat() == other.lstat()
+
+    def __hash__(self) -> int:
+        return hash((super().__hash__(), self.lstat()))
+
+    def lstat(self):
+        return self._lstat
+
+
+class OmeCache(DequeDict):
+    """ prevent (potentially expensive) rereading of ome data by caching """
+
+    instance = None
+
+    def __new__(cls) -> OmeCache:
+        if cls.instance is None:
+            cls.instance = super().__new__(cls)
+        return cls.instance
+
+    def __init__(self) -> None:
+        super().__init__(64)
+
+    def __reduce__(self) -> tuple[type, tuple]:
+        return self.__class__, ()
+
+    def __getitem__(self, item: Path | CachedPath) -> OME:
+        return super().__getitem__(CachedPath(item))
+
+    def __setitem__(self, key: Path | CachedPath, value: OME) -> None:
+        super().__setitem__(CachedPath(key), value)
+
+    def __contains__(self, item: Path | CachedPath) -> bool:
+        return super().__contains__(CachedPath(item))
+
+
+class Imread(np.lib.mixins.NDArrayOperatorsMixin, ABC):
+    """ class to read image files, while taking good care of important metadata,
+        currently optimized for .czi files, but can open anything that bioformats can handle
+            path: path to the image file
+            optional:
+            series: in case multiple experiments are saved in one file, like in .lif files
+            dtype: datatype to be used when returning frames
+            meta: define metadata, used for pickle-ing
+
+            NOTE: run imread.kill_vm() at the end of your script/program, otherwise python might not terminate
+
+            modify images on the fly with a decorator function:
+                define a function which takes an instance of this object, one image frame,
+                and the coordinates c, z, t as arguments, and one image frame as return
+                >> imread.frame_decorator = fun
+                then use imread as usually
+
+            Examples:
+                >> im = imread('/DATA/lenstra_lab/w.pomp/data/20190913/01_YTL639_JF646_DefiniteFocus.czi')
+                >> im
+                 << shows summary
+                >> im.shape
+                 << (256, 256, 2, 1, 600)
+                >> plt.imshow(im(1, 0, 100))
+                 << plots frame at position c=1, z=0, t=100 (python type indexing), note: round brackets; always 2d array
+                    with 1 frame
+                >> data = im[:,:,0,0,:25]
+                 << retrieves 5d numpy array containing first 25 frames at c=0, z=0, note: square brackets; always 5d array
+                >> plt.imshow(im.max(0, None, 0))
+                 << plots max-z projection at c=0, t=0
+                >> len(im)
+                 << total number of frames
+                >> im.pxsize
+                 << 0.09708737864077668 image-plane pixel size in um
+                >> im.laserwavelengths
+                 << [642, 488]
+                >> im.laserpowers
+                 << [0.02, 0.0005] in %
+
+                See __init__ and other functions for more ideas.
+
+            Subclassing:
+                Subclass AbstractReader to add more file types. A subclass should always have at least the following
+                methods:
+                    staticmethod _can_open(path): returns True when the subclass can open the image in path
+                    __metadata__(self): pulls some metadata from the file and do other format specific things,
+                                        it needs to define a few properties, like shape, etc.
+                    __frame__(self, c, z, t): this should return a single frame at channel c, slice z and time t
+                    optional close(self): close the file in a proper way
+                    optional field priority: subclasses with lower priority will be tried first, default = 99
+                    Any other method can be overridden as needed
+            wp@tl2019-2023 """
+
+    def __new__(cls, path=None, *args, **kwargs):
+        if cls is not Imread:
+            return super().__new__(cls)
+        if len(AbstractReader.__subclasses__()) == 0:
+            raise Exception('Restart python kernel please!')
+        if isinstance(path, Imread):
+            return path
+        path, _ = AbstractReader.split_path_series(path)
+        for subclass in sorted(AbstractReader.__subclasses__(), key=lambda subclass_: subclass_.priority):
+            if subclass._can_open(path):
+                do_not_pickle = (AbstractReader.do_not_pickle,) if isinstance(AbstractReader.do_not_pickle, str) \
+                    else AbstractReader.do_not_pickle
+                subclass_do_not_pickle = (subclass.do_not_pickle,) if isinstance(subclass.do_not_pickle, str) \
+                    else subclass.do_not_pickle if hasattr(subclass, 'do_not_pickle') else ()
+                subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
+
+                return super().__new__(subclass)
+        raise ReaderNotFoundError(f'No reader found for {path}.')
+
+    def __init__(self, base=None, slice=None, shape=(0, 0, 0, 0, 0), dtype=None, frame_decorator=None):
+        self.base = base or self
+        self.slice = slice
+        self._shape = Shape(shape)
+        self.dtype = dtype
+        self.frame_decorator = frame_decorator
+        self.transform = Transforms()
+        self.flags = dict(C_CONTIGUOUS=False, F_CONTIGUOUS=False, OWNDATA=False, WRITEABLE=False,
+                          ALIGNED=False, WRITEBACKIFCOPY=False, UPDATEIFCOPY=False)
+
+    def __call__(self, c=None, z=None, t=None, x=None, y=None):
+        """ same as im[] but allowing keyword axes, but slices need to made with slice() or np.s_ """
+        return self[{k: slice(v) if v is None else v for k, v in dict(c=c, z=z, t=t, x=x, y=y).items()}]
+
+    def __copy__(self):
+        return self.copy()
+
+    def __contains__(self, item):
+        def unique_yield(a, b):
+            for k in a:
+                yield k
+            for k in b:
+                if k not in a:
+                    yield k
+
+        for idx in unique_yield([key[:3] for key in self.cache.keys()],
+                                product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t']))):
+            yxczt = (slice(None), slice(None)) + idx
+            in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+            if item in np.asarray(self[in_idx]):
+                return True
+        return False
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        if not self.isclosed:
+            self.isclosed = True
+            if hasattr(self, 'close'):
+                self.close()
+
+    def __getitem__(self, n):
+        """ slice like a numpy array but return an Imread instance """
+        if self.isclosed:
+            raise OSError('file is closed')
+        if isinstance(n, (slice, Number)):  # None = :
+            n = (n,)
+        elif isinstance(n, type(Ellipsis)):
+            n = (None,) * len(self.axes)
+        elif isinstance(n, dict):  # allow im[dict(z=0)] etc.
+            n = [n.get(i, slice(None)) for i in self.axes]
+        n = list(n)
+
+        # deal with ...
+        ell = [i for i, e in enumerate(n) if isinstance(e, type(Ellipsis))]
+        if len(ell) > 1:
+            raise IndexError('an index can only have a single ellipsis (...)')
+        if len(ell):
+            if len(n) > self.ndim:
+                n.remove(Ellipsis)
+            else:
+                n[ell[0]] = None
+                while len(n) < self.ndim:
+                    n.insert(ell[0], None)
+        while len(n) < self.ndim:
+            n.append(None)
+
+        axes_idx = [self.shape.axes.find(i) for i in 'yxczt']
+        n = [n[j] if 0 <= j < len(n) else None for j in axes_idx]  # reorder n
+
+        new_slice = []
+        for s, e in zip(self.slice, n):
+            if e is None:
+                new_slice.append(s)
+            else:
+                new_slice.append(s[e])
+
+        # TODO: check output dimensionality when requested shape in some dimension is 1
+        if all([isinstance(s, Number) or a < 0 and s.size == 1 for s, a in zip(new_slice, axes_idx)]):
+            return self.block(*new_slice).item()
+        else:
+            new = View(self)
+            new.slice = new_slice
+            new._shape = Shape([1 if isinstance(s, Number) else len(s) for s in new_slice])
+            new.axes = ''.join(j for j in self.axes if j in [i for i, s in zip('yxczt', new_slice)
+                                                             if not isinstance(s, Number)])
+            return new
+
+    def __getstate__(self):
+        return {key: value for key, value in self.__dict__.items() if key not in self.do_not_pickle}
+
+    def __len__(self):
+        return self.shape[0]
+
+    def __repr__(self):
+        return self.summary
+
+    def __setstate__(self, state):
+        """ What happens during unpickling """
+        self.__dict__.update(state)
+        if isinstance(self, AbstractReader):
+            self.open()
+        self.cache = DequeDict(16)
+
+    def __str__(self):
+        return str(self.path)
+
+    def __array__(self, dtype=None):
+        block = self.block(*self.slice)
+        axes_idx = [self.shape.axes.find(i) for i in 'yxczt']
+        axes_squeeze = tuple({i for i, j in enumerate(axes_idx) if j == -1}.union(
+            {i for i, j in enumerate(self.slice) if isinstance(j, Number)}))
+        block = block.squeeze(axes_squeeze)
+        if dtype is not None:
+            block = block.astype(dtype)
+        if block.ndim == 0:
+            return block.item()
+        axes = ''.join(j for i, j in enumerate('yxczt') if i not in axes_squeeze)
+        return block.transpose([axes.find(i) for i in self.shape.axes if i in axes])
+
+    def __array_arg_fun__(self, fun, axis=None, out=None):
+        """ frame-wise application of np.argmin and np.argmax """
+        if axis is None:
+            value = arg = None
+            for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                yxczt = (slice(None), slice(None)) + idx
+                in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+                new = np.asarray(self[in_idx])
+                new_arg = np.unravel_index(fun(new), new.shape)
+                new_value = new[new_arg]
+                if value is None:
+                    arg = new_arg + idx
+                    value = new_value
+                else:
+                    i = fun((value, new_value))
+                    arg = (arg, new_arg + idx)[i]
+                    value = (value, new_value)[i]
+            axes = ''.join(i for i in self.axes if i in 'yx') + 'czt'
+            arg = np.ravel_multi_index([arg[axes.find(i)] for i in self.axes], self.shape)
+            if out is None:
+                return arg
+            else:
+                out.itemset(arg)
+                return out
+        else:
+            if isinstance(axis, str):
+                axis_str, axis_idx = axis, self.axes.index(axis)
+            else:
+                axis_str, axis_idx = self.axes[axis], axis
+            if axis_str not in self.axes:
+                raise IndexError(f'Axis {axis_str} not in {self.axes}.')
+            out_shape = list(self.shape)
+            out_axes = list(self.axes)
+            out_shape.pop(axis_idx)
+            out_axes.pop(axis_idx)
+            if out is None:
+                out = np.zeros(out_shape, int)
+            if axis_str in 'yx':
+                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                    yxczt = (slice(None), slice(None)) + idx
+                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
+                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+                    new = self[in_idx]
+                    out[out_idx] = fun(np.asarray(new), new.axes.find(axis_str))
+            else:
+                value = np.zeros(out.shape, self.dtype)
+                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                    yxczt = (slice(None), slice(None)) + idx
+                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
+                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+                    new_value = self[in_idx]
+                    new_arg = np.full_like(new_value, idx['czt'.find(axis_str)])
+                    if idx['czt'.find(axis_str)] == 0:
+                        value[out_idx] = new_value
+                        out[out_idx] = new_arg
+                    else:
+                        old_value = value[out_idx]
+                        i = fun((old_value, new_value), 0)
+                        value[out_idx] = np.where(i, new_value, old_value)
+                        out[out_idx] = np.where(i, new_arg, out[out_idx])
+            return out
+
+    def __array_fun__(self, funs, axis=None, dtype=None, out=None, keepdims=False, initials=None, where=True,
+                      ffuns=None, cfun=None):
+        """ frame-wise application of np.min, np.max, np.sum, np.mean and their nan equivalents """
+        p = re.compile(r'\d')
+        dtype = self.dtype if dtype is None else np.dtype(dtype)
+        if initials is None:
+            initials = [None for _ in funs]
+        if ffuns is None:
+            ffuns = [None for _ in funs]
+
+        def ffun_(frame):
+            return np.asarray(frame)
+        ffuns = [ffun_ if ffun is None else ffun for ffun in ffuns]
+        if cfun is None:
+            def cfun(*res):
+                return res[0]
+
+        # TODO: smarter transforms
+        if axis is None:
+            for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                yxczt = (slice(None), slice(None)) + idx
+                in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+                w = where if where is None or isinstance(where, bool) else where[in_idx]
+                initials = [fun(np.asarray(ffun(self[in_idx])), initial=initial, where=w)
+                            for fun, ffun, initial in zip(funs, ffuns, initials)]
+            res = cfun(*initials)
+            res = (np.round(res) if dtype.kind in 'ui' else res).astype(p.sub('', dtype.name))
+            if keepdims:
+                res = np.array(res, dtype, ndmin=self.ndim)
+            if out is None:
+                return res
+            else:
+                out.itemset(res)
+                return out
+        else:
+            if isinstance(axis, str):
+                axis_str, axis_idx = axis, self.axes.index(axis)
+            else:
+                axis_idx = axis % self.ndim
+                axis_str = self.axes[axis_idx]
+            if axis_str not in self.axes:
+                raise IndexError(f'Axis {axis_str} not in {self.axes}.')
+            out_shape = list(self.shape)
+            out_axes = list(self.axes)
+            if not keepdims:
+                out_shape.pop(axis_idx)
+                out_axes.pop(axis_idx)
+            if out is None:
+                out = np.zeros(out_shape, dtype)
+            if axis_str in 'yx':
+                yx = 'yx' if self.axes.find('x') > self.axes.find('y') else 'yx'
+                frame_ax = yx.find(axis_str)
+                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                    yxczt = (slice(None), slice(None)) + idx
+                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
+                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+                    w = where if where is None or isinstance(where, bool) else where[in_idx]
+                    res = cfun(*[fun(ffun(self[in_idx]), frame_ax, initial=initial, where=w)
+                                 for fun, ffun, initial in zip(funs, ffuns, initials)])
+                    out[out_idx] = (np.round(res) if out.dtype.kind in 'ui' else res).astype(p.sub('', dtype.name))
+            else:
+                tmps = [np.zeros(out_shape) for _ in ffuns]
+                for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
+                    yxczt = (slice(None), slice(None)) + idx
+                    out_idx = tuple(yxczt['yxczt'.find(i)] for i in out_axes)
+                    in_idx = tuple(yxczt['yxczt'.find(i)] for i in self.axes)
+
+                    if idx['czt'.find(axis_str)] == 0:
+                        w = where if where is None or isinstance(where, bool) else (where[in_idx],)
+                        for tmp, fun, ffun, initial in zip(tmps, funs, ffuns, initials):
+                            tmp[out_idx] = fun((ffun(self[in_idx]),), 0, initial=initial, where=w)
+                    else:
+                        w = where if where is None or isinstance(where, bool) else \
+                            (np.ones_like(where[in_idx]), where[in_idx])
+                        for tmp, fun, ffun in zip(tmps, funs, ffuns):
+                            tmp[out_idx] = fun((tmp[out_idx], ffun(self[in_idx])), 0, where=w)
+                out[...] = (np.round(cfun(*tmps)) if out.dtype.kind in 'ui' else
+                            cfun(*tmps)).astype(p.sub('', dtype.name))
+            return out
+
+    @property
+    def axes(self):
+        return self.shape.axes
+
+    @axes.setter
+    def axes(self, value):
+        shape = self.shape[value]
+        if isinstance(shape, Number):
+            shape = (shape,)
+        self._shape = Shape(shape, value)
+
+    @property
+    def dtype(self):
+        return self._dtype
+
+    @dtype.setter
+    def dtype(self, value):
+        self._dtype = np.dtype(value)
+
+    @cached_property
+    def extrametadata(self):
+        if isinstance(self.path, Path):
+            if self.path.with_suffix('.pzl2').exists():
+                pname = self.path.with_suffix('.pzl2')
+            elif self.path.with_suffix('.pzl').exists():
+                pname = self.path.with_suffix('.pzl')
+            else:
+                return
+            try:
+                return self.get_config(pname)
+            except Exception:  # noqa
+                return
+        return
+
+    @property
+    def ndim(self):
+        return len(self.shape)
+
+    @property
+    def size(self):
+        return np.prod(self.shape)
+
+    @property
+    def shape(self):
+        return self._shape
+
+    @shape.setter
+    def shape(self, value):
+        if isinstance(value, Shape):
+            self._shape = value
+        else:
+            self._shape = Shape((value['yxczt'.find(i.lower())] for i in self.axes), self.axes)
+
+    @property
+    def summary(self):
+        """ gives a helpful summary of the recorded experiment """
+        s = [f'path/filename: {self.path}',
+             f'series/pos:    {self.series}',
+             f"reader:        {self.base.__class__.__module__.split('.')[-1]}"]
+        s.extend((f'dtype:         {self.dtype}',
+                  f'shape ({self.axes}):'.ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"))
+        if self.pxsize_um:
+            s.append(f'pixel size:    {1000 * self.pxsize_um:.2f} nm')
+        if self.zstack and self.deltaz_um:
+            s.append(f'z-interval:    {1000 * self.deltaz_um:.2f} nm')
+        if self.exposuretime_s and not all(e is None for e in self.exposuretime_s):
+            s.append(f'exposuretime:  {self.exposuretime_s[0]:.2f} s')
+        if self.timeseries and self.timeinterval:
+            s.append(f'time interval: {self.timeinterval:.3f} s')
+        if self.binning:
+            s.append('binning:       {}x{}'.format(*self.binning))
+        if self.laserwavelengths:
+            s.append('laser colors:  ' + ' | '.join([' & '.join(len(w) * ('{:.0f}',)).format(*w)
+                                                     for w in self.laserwavelengths]) + ' nm')
+        if self.laserpowers:
+            s.append('laser powers:  ' + ' | '.join([' & '.join(len(p) * ('{:.3g}',)).format(*[100 * i for i in p])
+                                                     for p in self.laserpowers]) + ' %')
+        if self.objective and self.objective.model:
+            s.append(f'objective:     {self.objective.model}')
+        if self.magnification:
+            s.append(f'magnification: {self.magnification}x')
+        if self.tubelens and self.tubelens.model:
+            s.append(f'tubelens:      {self.tubelens.model}')
+        if self.filter:
+            s.append(f'filterset:     {self.filter}')
+        if self.powermode:
+            s.append(f'powermode:     {self.powermode}')
+        if self.collimator:
+            s.append('collimator:   ' + (' {}' * len(self.collimator)).format(*self.collimator))
+        if self.tirfangle:
+            s.append('TIRF angle:   ' + (' {:.2f}°' * len(self.tirfangle)).format(*self.tirfangle))
+        if self.gain:
+            s.append('gain:         ' + (' {:.0f}' * len(self.gain)).format(*self.gain))
+        if self.pcf:
+            s.append('pcf:          ' + (' {:.2f}' * len(self.pcf)).format(*self.pcf))
+        return '\n'.join(s)
+
+    @property
+    def T(self):
+        return self.transpose()
+
+    @cached_property
+    def timeseries(self):
+        return self.shape['t'] > 1
+
+    @cached_property
+    def zstack(self):
+        return self.shape['z'] > 1
+
+    @wraps(np.argmax)
+    def argmax(self, *args, **kwargs):
+        return self.__array_arg_fun__(np.argmax, *args, **kwargs)
+
+    @wraps(np.argmin)
+    def argmin(self, *args, **kwargs):
+        return self.__array_arg_fun__(np.argmin, *args, **kwargs)
+
+    @wraps(np.max)
+    def max(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.max], axis, None, out, keepdims, [initial], where)
+
+    @wraps(np.mean)
+    def mean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
+        dtype = dtype or float
+        n = np.prod(self.shape) if axis is None else self.shape[axis]
+
+        def sfun(frame):
+            return np.asarray(frame).astype(float)
+
+        def cfun(res):
+            return res / n
+
+        return self.__array_fun__([np.sum], axis, dtype, out, keepdims, None, where, [sfun], cfun)
+
+    @wraps(np.min)
+    def min(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.min], axis, None, out, keepdims, [initial], where)
+
+    @wraps(np.moveaxis)
+    def moveaxis(self, source, destination):
+        raise NotImplementedError('moveaxis is not implemented')
+
+    @wraps(np.nanmax)
+    def nanmax(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.nanmax], axis, None, out, keepdims, [initial], where)
+
+    @wraps(np.nanmean)
+    def nanmean(self, axis=None, dtype=None, out=None, keepdims=False, *, where=True, **kwargs):
+        dtype = dtype or float
+
+        def sfun(frame):
+            return np.asarray(frame).astype(float)
+
+        def nfun(frame):
+            return np.invert(np.isnan(frame))
+
+        return self.__array_fun__([np.nansum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, nfun), truediv)
+
+    @wraps(np.nanmin)
+    def nanmin(self, axis=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.nanmin], axis, None, out, keepdims, [initial], where)
+
+    @wraps(np.nansum)
+    def nansum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.nansum], axis, dtype, out, keepdims, [initial], where)
+
+    @wraps(np.nanstd)
+    def nanstd(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=None):
+        return self.nanvar(axis, dtype, out, ddof, keepdims, where=where, std=True)
+
+    @wraps(np.nanvar)
+    def nanvar(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True, std=False):
+        dtype = dtype or float
+
+        def sfun(frame):
+            return np.asarray(frame).astype(float)
+
+        def s2fun(frame):
+            return np.asarray(frame).astype(float) ** 2
+
+        def nfun(frame):
+            return np.invert(np.isnan(frame))
+
+        if std:
+            def cfun(s, s2, n):
+                return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
+        else:
+            def cfun(s, s2, n):
+                return (s2 - s ** 2 / n) / (n - ddof)
+        return self.__array_fun__([np.nansum, np.nansum, np.sum], axis, dtype, out, keepdims, None, where,
+                                  (sfun, s2fun, nfun), cfun)
+
+    def flatten(self, *args, **kwargs):
+        return np.asarray(self).flatten(*args, **kwargs)
+
+    @wraps(np.reshape)
+    def reshape(self, *args, **kwargs):
+        return np.asarray(self).reshape(*args, **kwargs)
+
+    @wraps(np.squeeze)
+    def squeeze(self, axes=None):
+        new = self.copy()
+        if axes is None:
+            axes = tuple(i for i, j in enumerate(new.shape) if j == 1)
+        elif isinstance(axes, Number):
+            axes = (axes,)
+        else:
+            axes = tuple(new.axes.find(ax) if isinstance(ax, str) else ax for ax in axes)
+        if any([new.shape[ax] != 1 for ax in axes]):
+            raise ValueError('cannot select an axis to squeeze out which has size not equal to one')
+        new.axes = ''.join(j for i, j in enumerate(new.axes) if i not in axes)
+        return new
+
+    @wraps(np.std)
+    def std(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True):
+        return self.var(axis, dtype, out, ddof, keepdims, where=where, std=True)
+
+    @wraps(np.sum)
+    def sum(self, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, **kwargs):
+        return self.__array_fun__([np.sum], axis, dtype, out, keepdims, [initial], where)
+
+    @wraps(np.swapaxes)
+    def swapaxes(self, axis1, axis2):
+        new = self.copy()
+        axes = new.axes
+        if isinstance(axis1, str):
+            axis1 = axes.find(axis1)
+        if isinstance(axis2, str):
+            axis2 = axes.find(axis2)
+        axes[axis1], axes[axis2] = axes[axis2], axes[axis1]
+        new.axes = axes
+        return new
+
+    @wraps(np.transpose)
+    def transpose(self, *axes):
+        new = self.copy()
+        if not axes:
+            new.axes = new.axes[::-1]
+        else:
+            new.axes = ''.join(ax if isinstance(ax, str) else new.axes[ax] for ax in axes)
+        return new
+
+    @wraps(np.var)
+    def var(self, axis=None, dtype=None, out=None, ddof=0, keepdims=None, *, where=True, std=False):
+        dtype = dtype or float
+        n = np.prod(self.shape) if axis is None else self.shape[axis]
+
+        def sfun(frame):
+            return np.asarray(frame).astype(float)
+
+        def s2fun(frame):
+            return np.asarray(frame).astype(float) ** 2
+
+        if std:
+            def cfun(s, s2):
+                return np.sqrt((s2 - s ** 2 / n) / (n - ddof))
+        else:
+            def cfun(s, s2):
+                return (s2 - s ** 2 / n) / (n - ddof)
+        return self.__array_fun__([np.sum, np.sum], axis, dtype, out, keepdims, None, where, (sfun, s2fun), cfun)
+
+    def asarray(self):
+        return self.__array__()
+
+    def astype(self, dtype, *args, **kwargs):
+        new = self.copy()
+        new.dtype = dtype
+        return new
+
+    def block(self, y=None, x=None, c=None, z=None, t=None):
+        """ returns 5D block of frames """
+        y, x, c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1)
+                         for i, e in zip('yxczt', (y, x, c, z, t)))
+        d = np.empty((len(y), len(x), len(c), len(z), len(t)), self.dtype)
+        for (ci, cj), (zi, zj), (ti, tj) in product(enumerate(c), enumerate(z), enumerate(t)):
+            d[:, :, ci, zi, ti] = self.frame(cj, zj, tj)[y][:, x]
+        return d
+
+    def copy(self):
+        return View(self)
+
+    def data(self, c=0, z=0, t=0):
+        """ returns 3D stack of frames """
+        c, z, t = (np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1) for i, e in zip('czt', (c, z, t)))
+        return np.dstack([self.frame(ci, zi, ti) for ci, zi, ti in product(c, z, t)])
+
+    def frame(self, c=0, z=0, t=0):
+        """ returns single 2D frame """
+        c = self.get_channel(c)
+        c %= self.base.shape['c']
+        z %= self.base.shape['z']
+        t %= self.base.shape['t']
+
+        # cache last n (default 16) frames in memory for speed (~250x faster)
+        key = (c, z, t, self.transform, self.frame_decorator)
+        if key in self.cache:
+            self.cache.move_to_end(key)
+            f = self.cache[key]
+        else:
+            f = self.transform[self.channel_names[c], t].frame(self.__frame__(c, z, t))
+            if self.frame_decorator is not None:
+                f = self.frame_decorator(self, f, c, z, t)
+            self.cache[key] = f
+        if self.dtype is not None:
+            return f.copy().astype(self.dtype)
+        else:
+            return f.copy()
+
+    def get_channel(self, channel_name):
+        if not isinstance(channel_name, str):
+            return channel_name
+        else:
+            c = [i for i, c in enumerate(self.channel_names) if c.lower().startswith(channel_name.lower())]
+            assert len(c) > 0, f'Channel {c} not found in {self.channel_names}'
+            assert len(c) < 2, f'Channel {c} not unique in {self.channel_names}'
+            return c[0]
+
+    @staticmethod
+    def get_config(file):
+        """ Open a yml config file """
+        loader = yaml.SafeLoader
+        loader.add_implicit_resolver(
+            r'tag:yaml.org,2002:float',
+            re.compile(r'''^(?:
+                     [-+]?(?:[0-9][0-9_]*)\.[0-9_]*(?:[eE][-+]?[0-9]+)?
+                    |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
+                    |\.[0-9_]+(?:[eE][-+][0-9]+)?
+                    |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\.[0-9_]*
+                    |[-+]?\\.(?:inf|Inf|INF)
+                    |\.(?:nan|NaN|NAN))$''', re.X),
+            list(r'-+0123456789.'))
+        with open(file) as f:
+            return yaml.load(f, loader)
+
+    def get_czt(self, c, z, t):
+        czt = []
+        for i, n in zip('czt', (c, z, t)):
+            if n is None:
+                czt.append(list(range(self.shape[i])))
+            elif isinstance(n, range):
+                if n.stop < 0:
+                    stop = n.stop % self.shape[i]
+                elif n.stop > self.shape[i]:
+                    stop = self.shape[i]
+                else:
+                    stop = n.stop
+                czt.append(list(range(n.start % self.shape[i], stop, n.step)))
+            elif isinstance(n, Number):
+                czt.append([n % self.shape[i]])  # noqa
+            else:
+                czt.append([k % self.shape[i] for k in n])
+        return [self.get_channel(c) for c in czt[0]], *czt[1:]
+
+    @staticmethod
+    def bioformats_ome(path: [str, Path]) -> OME:
+        """ Use java BioFormats to make an ome metadata structure. """
+        with multiprocessing.get_context('spawn').Pool(1) as pool:
+            return pool.map(bioformats_ome, (path,))[0]
+
+    @staticmethod
+    def fix_ome(ome: OME) -> OME:
+        # fix ome if necessary
+        for image in ome.images:
+            try:
+                if image.pixels.physical_size_z is None and len(set([plane.the_z
+                                                                     for plane in image.pixels.planes])) > 1:
+                    z = np.array([(plane.position_z * ureg.Quantity(plane.position_z_unit.value).to(ureg.m).magnitude,
+                                   plane.the_z)
+                                  for plane in image.pixels.planes if plane.the_c == 0 and plane.the_t == 0])
+                    i = np.argsort(z[:, 1])
+                    image.pixels.physical_size_z = np.nanmean(np.true_divide(*np.diff(z[i], axis=0).T)) * 1e6
+                    image.pixels.physical_size_z_unit = 'µm'
+            except Exception:
+                pass
+        return ome
+
+    @staticmethod
+    def read_ome(path: [str, Path]) -> Optional[OME]:
+        path = Path(path)
+        if path.with_suffix('.ome.xml').exists():
+            return OME.from_xml(path.with_suffix('.ome.xml'))
+
+    def get_ome(self) -> OME:
+        """ overload this """
+        return self.bioformats_ome(self.path)
+
+    @cached_property
+    def ome(self) -> OME:
+        cache = OmeCache()
+        if self.path not in cache:
+            ome = self.read_ome(self.path)
+            if ome is None:
+                ome = self.get_ome()
+            cache[self.path] = self.fix_ome(ome)
+        return cache[self.path]
+
+    def is_noise(self, volume=None):
+        """ True if volume only has noise """
+        if volume is None:
+            volume = self
+        fft = np.fft.fftn(volume)
+        corr = np.fft.fftshift(np.fft.ifftn(fft * fft.conj()).real / np.sum(volume ** 2))
+        return 1 - corr[tuple([0] * corr.ndim)] < 0.0067
+
+    @staticmethod
+    def kill_vm():
+        JVM().kill_vm()
+
+    def new(self, *args, **kwargs):
+        warnings.warn('Imread.new has been deprecated, use Imread.view instead.', DeprecationWarning, 2)
+        return self.view(*args, **kwargs)
+
+    def save_as_tiff(self, fname=None, c=None, z=None, t=None, split=False, bar=True, pixel_type='uint16', **kwargs):
+        """ saves the image as a tif file
+            split: split channels into different files """
+        if fname is None:
+            fname = self.path.with_suffix('.tif')
+            if fname == self.path:
+                raise FileExistsError(f'File {fname} exists already.')
+        if not isinstance(fname, Path):
+            fname = Path(fname)
+        if split:
+            for i in range(self.shape['c']):
+                if self.timeseries:
+                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, 0, None, False,
+                                      bar, pixel_type)
+                else:
+                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, None, 0, False,
+                                      bar, pixel_type)
+        else:
+            n = [c, z, t]
+            for i, ax in enumerate('czt'):
+                if n[i] is None:
+                    n[i] = range(self.shape[ax])
+                elif not isinstance(n[i], (tuple, list)):
+                    n[i] = (n[i],)
+
+            shape = [len(i) for i in n]
+            with TransformTiff(self, fname.with_suffix('.tif'), shape, pixel_type,
+                               pxsize=self.pxsize_um, deltaz=self.deltaz_um, **kwargs) as tif:
+                for i, m in tqdm(zip(product(*[range(s) for s in shape]), product(*n)),  # noqa
+                                 total=np.prod(shape), desc='Saving tiff', disable=not bar):
+                    tif.save(m, *i)
+
+    def with_transform(self, channels=True, drift=False, file=None, bead_files=()):
+        """ returns a view where channels and/or frames are registered with an affine transformation
+            channels: True/False register channels using bead_files
+            drift: True/False register frames to correct drift
+            file: load registration from file with name file, default: transform.yml in self.path.parent
+            bead_files: files used to register channels, default: files in self.path.parent,
+                with names starting with 'beads'
+            """
+        view = self.view()
+        if file is None:
+            file = Path(view.path.parent) / 'transform.yml'
+        if not bead_files:
+            try:
+                bead_files = Transforms.get_bead_files(view.path.parent)
+            except Exception:
+                if not file.exists():
+                    raise Exception('No transform file and no bead file found.')
+                bead_files = ()
+
+        if channels:
+            try:
+                view.transform = Transforms.from_file(file, T=drift)
+            except Exception:  # noqa
+                view.transform = Transforms().with_beads(view.cyllens, bead_files)
+                if drift:
+                    view.transform = view.transform.with_drift(view)
+                view.transform.save(file.with_suffix('.yml'))
+                view.transform.save_channel_transform_tiff(bead_files, file.with_suffix('.tif'))
+        elif drift:
+            try:
+                view.transform = Transforms.from_file(file, C=False)
+            except Exception:  # noqa
+                view.transform = Transforms().with_drift(self)
+        view.transform.adapt(view.frameoffset, view.shape.yxczt, view.channel_names)
+        return view
+
+    @staticmethod
+    def split_path_series(path):
+        if isinstance(path, str):
+            path = Path(path)
+        if isinstance(path, Path) and path.name.startswith('Pos') and path.name.lstrip('Pos').isdigit():
+            return path.parent, int(path.name.lstrip('Pos'))
+        return path, 0
+
+    def view(self, *args, **kwargs):
+        return View(self, *args, **kwargs)
+
+
+class View(Imread, ABC):
+    def __init__(self, base, dtype=None):
+        super().__init__(base.base, base.slice, base.shape, dtype or base.dtype, base.frame_decorator)
+        self.transform = base.transform
+
+    def __getattr__(self, item):
+        if not hasattr(self.base, item):
+            raise AttributeError(f'{self.__class__} object has no attribute {item}')
+        return self.base.__getattribute__(item)
+
+
+class AbstractReader(Imread, metaclass=ABCMeta):
+    priority = 99
+    do_not_pickle = 'cache'
+    ureg = ureg
+
+    @staticmethod
+    @abstractmethod
+    def _can_open(path):  # Override this method, and return true when the subclass can open the file
+        return False
+
+    @abstractmethod
+    def __frame__(self, c, z, t):  # Override this, return the frame at c, z, t
+        return np.random.randint(0, 255, self.shape['yx'])
+
+    def open(self):  # Optionally override this, open file handles etc.
+        """ filehandles cannot be pickled and should be marked such by setting do_not_pickle = 'file_handle_name' """
+        return
+
+    def close(self):  # Optionally override this, close file handles etc.
+        return
+
+    def __init__(self, path, dtype=None, axes=None):
+        if isinstance(path, Imread):
+            return
+        super().__init__()
+        self.isclosed = False
+        if isinstance(path, str):
+            path = Path(path)
+        self.path, self.series = self.split_path_series(path)
+        if isinstance(path, Path) and path.exists():
+            self.title = self.path.name
+            self.acquisitiondate = datetime.fromtimestamp(self.path.stat().st_mtime).strftime('%y-%m-%dT%H:%M:%S')
+        else:  # ndarray
+            self.title = self.__class__.__name__
+            self.acquisitiondate = 'now'
+
+        self.reader = None
+        self.pcf = None
+        self.powermode = None
+        self.collimator = None
+        self.tirfangle = None
+        self.cyllens = ['None', 'None']
+        self.duolink = 'None'
+        self.detector = [0, 1]
+        self.track = [0]
+        self.cache = DequeDict(16)
+        self.frameoffset = 0, 0  # how far apart the centers of frame and sensor are
+
+        self.open()
+        # extract some metadata from ome
+        instrument = self.ome.instruments[0] if self.ome.instruments else None
+        image = self.ome.images[self.series if len(self.ome.images) > 1 else 0]
+        pixels = image.pixels
+        self.shape = pixels.size_y, pixels.size_x, pixels.size_c, pixels.size_z, pixels.size_t
+        self.dtype = pixels.type.value if dtype is None else dtype
+        self.pxsize = pixels.physical_size_x_quantity
+        try:
+            self.exposuretime = tuple(find(image.pixels.planes, the_c=c).exposure_time_quantity
+                                      for c in range(self.shape['c']))
+        except AttributeError:
+            self.exposuretime = ()
+
+        if self.zstack:
+            self.deltaz = image.pixels.physical_size_z_quantity
+            self.deltaz_um = None if self.deltaz is None else self.deltaz.to(self.ureg.um).m
+        else:
+            self.deltaz = self.deltaz_um = None
+        if image.objective_settings:
+            self.objective = find(instrument.objectives, id=image.objective_settings.id)
+        else:
+            self.objective = None
+        try:
+            t0 = find(image.pixels.planes, the_c=0, the_t=0, the_z=0).delta_t
+            t1 = find(image.pixels.planes, the_c=0, the_t=self.shape['t'] - 1, the_z=0).delta_t
+            self.timeinterval = (t1 - t0) / (self.shape['t'] - 1) if self.shape['t'] > 1 else None
+        except AttributeError:
+            self.timeinterval = None
+        try:
+            self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
+            self.pxsize *= self.binning[0]
+        except (AttributeError, IndexError, ValueError):
+            self.binning = None
+        self.channel_names = [channel.name for channel in image.pixels.channels]
+        self.channel_names += [chr(97 + i) for i in range(len(self.channel_names), self.shape['c'])]
+        self.cnamelist = self.channel_names
+        try:
+            optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
+        except AttributeError:
+            optovars = []
+        if len(optovars) == 0:
+            self.tubelens = None
+        else:
+            self.tubelens = optovars[0]
+        if self.objective:
+            if self.tubelens:
+                self.magnification = self.objective.nominal_magnification * self.tubelens.nominal_magnification
+            else:
+                self.magnification = self.objective.nominal_magnification
+            self.NA = self.objective.lens_na
+        else:
+            self.magnification = None
+            self.NA = None
+
+        self.gain = [find(instrument.detectors, id=channel.detector_settings.id).amplification_gain
+                     for channel in image.pixels.channels
+                     if channel.detector_settings
+                     and find(instrument.detectors, id=channel.detector_settings.id).amplification_gain]
+        self.laserwavelengths = [(channel.excitation_wavelength_quantity.to(self.ureg.nm).m,)
+                                 for channel in pixels.channels if channel.excitation_wavelength_quantity]
+        self.laserpowers = try_default(lambda: [(1 - channel.light_source_settings.attenuation,)
+                                                for channel in pixels.channels], [])
+        self.filter = try_default(lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
+                                           for channel in image.pixels.channels], None)
+        self.pxsize_um = None if self.pxsize is None else self.pxsize.to(self.ureg.um).m
+        self.exposuretime_s = [None if i is None else i.to(self.ureg.s).m for i in self.exposuretime]
+
+        if axes is None:
+            self.axes = ''.join(i for i in 'cztyx' if self.shape[i] > 1)
+        elif axes.lower() == 'full':
+            self.axes = 'cztyx'
+        else:
+            self.axes = axes
+        self.slice = [np.arange(s, dtype=int) for s in self.shape.yxczt]
+
+        m = self.extrametadata
+        if m is not None:
+            try:
+                self.cyllens = m['CylLens']
+                self.duolink = m['DLFilterSet'].split(' & ')[m['DLFilterChannel']]
+                if 'FeedbackChannels' in m:
+                    self.feedback = m['FeedbackChannels']
+                else:
+                    self.feedback = m['FeedbackChannel']
+            except Exception:  # noqa
+                self.cyllens = ['None', 'None']
+                self.duolink = 'None'
+                self.feedback = []
+        try:
+            self.cyllenschannels = np.where([self.cyllens[self.detector[c]].lower() != 'none'
+                                             for c in range(self.shape['c'])])[0].tolist()
+        except Exception:  # noqa
+            pass
+        try:
+            s = int(re.findall(r'_(\d{3})_', self.duolink)[0]) * ureg.nm
+        except Exception:  # noqa
+            s = 561 * ureg.nm
+        try:
+            sigma = []
+            for c, d in enumerate(self.detector):
+                emission = (np.hstack(self.laserwavelengths[c]) + 22) * ureg.nm
+                sigma.append([emission[emission > s].max(initial=0), emission[emission < s].max(initial=0)][d])
+            sigma = np.hstack(sigma)
+            sigma[sigma == 0] = 600 * ureg.nm
+            sigma /= 2 * self.NA * self.pxsize
+            self.sigma = sigma.magnitude.tolist()
+        except Exception:  # noqa
+            self.sigma = [2] * self.shape['c']
+        if not self.NA:
+            self.immersionN = 1
+        elif 1.5 < self.NA:
+            self.immersionN = 1.661
+        elif 1.3 < self.NA < 1.5:
+            self.immersionN = 1.518
+        elif 1 < self.NA < 1.3:
+            self.immersionN = 1.33
+        else:
+            self.immersionN = 1
+
+        p = re.compile(r'(\d+):(\d+)$')
+        try:
+            self.track, self.detector = zip(*[[int(i) for i in p.findall(find(
+                self.ome.images[self.series].pixels.channels, id=f'Channel:{c}').detector_settings.id)[0]]
+                                              for c in range(self.shape['c'])])
+        except Exception:
+            pass
+
+
+def main():
+    parser = ArgumentParser(description='Display info and save as tif')
+    parser.add_argument('file', help='image_file')
+    parser.add_argument('out', help='path to tif out', type=str, default=None, nargs='?')
+    parser.add_argument('-o', '--extract_ome', help='extract ome to xml file', action='store_true')
+    parser.add_argument('-r', '--register', help='register channels', action='store_true')
+    parser.add_argument('-c', '--channel', help='channel', type=int, default=None)
+    parser.add_argument('-z', '--zslice', help='z-slice', type=int, default=None)
+    parser.add_argument('-t', '--time', help='time', type=int, default=None)
+    parser.add_argument('-s', '--split', help='split channels', action='store_true')
+    parser.add_argument('-f', '--force', help='force overwrite', action='store_true')
+    args = parser.parse_args()
+
+    with Imread(args.file) as im:
+        if args.register:
+            im = im.with_transform()
+        print(im.summary)
+        if args.out:
+            out = Path(args.out).absolute()
+            out.parent.mkdir(parents=True, exist_ok=True)
+            if out.exists() and not args.force:
+                print(f'File {args.out} exists already, add the -f flag if you want to overwrite it.')
+            else:
+                im.save_as_tiff(out, args.channel, args.zslice, args.time, args.split)
+        if args.extract_ome:
+            with open(im.path.with_suffix('.ome.xml'), 'w') as f:
+                f.write(im.ome.to_xml())
+
+
+from .readers import *
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/jvm.py` & `ndbioimage-2024.4.0/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/cziread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,608 +1,602 @@
-import re
-import warnings
-from abc import ABC
-from functools import cached_property
-from io import BytesIO
-from itertools import product
-from pathlib import Path
-
-import czifile
-import imagecodecs
-import numpy as np
-from lxml import etree
-from ome_types import model
-from tifffile import repeat_nd
-
-from .. import AbstractReader, OmeCache
-
-try:
-    # TODO: use zoom from imagecodecs implementation when available
-    from scipy.ndimage.interpolation import zoom
-except ImportError:
-    try:
-        from ndimage.interpolation import zoom
-    except ImportError:
-        zoom = None
-
-
-def zstd_decode(data: bytes) -> bytes:
-    """ decode zstd bytes, copied from BioFormats ZeissCZIReader """
-    def read_var_int(stream: BytesIO) -> int:
-        a = stream.read(1)[0]
-        if a & 128:
-            b = stream.read(1)[0]
-            if b & 128:
-                c = stream.read(1)[0]
-                return (c << 14) | ((b & 127) << 7) | (a & 127)
-            return (b << 7) | (a & 127)
-        return a & 255
-
-    try:
-        with BytesIO(data) as stream:
-            size_of_header = read_var_int(stream)
-            high_low_unpacking = False
-            while stream.tell() < size_of_header:
-                chunk_id = read_var_int(stream)
-                # only one chunk ID defined so far
-                if chunk_id == 1:
-                    high_low_unpacking = (stream.read(1)[0] & 1) == 1
-                else:
-                    raise ValueError(f'Invalid chunk id: {chunk_id}')
-            pointer = stream.tell()
-    except Exception:
-        high_low_unpacking = False
-        pointer = 0
-
-    decoded = imagecodecs.zstd_decode(data[pointer:])
-    if high_low_unpacking:
-        second_half = len(decoded) // 2
-        return bytes([decoded[second_half + i // 2] if i % 2 else decoded[i // 2] for i in range(len(decoded))])
-    else:
-        return decoded
-
-
-def data(self, raw=False, resize=True, order=0):
-    """Read image data from file and return as numpy array."""
-    DECOMPRESS = czifile.czifile.DECOMPRESS
-    DECOMPRESS[5] = imagecodecs.zstd_decode
-    DECOMPRESS[6] = zstd_decode
-
-    de = self.directory_entry
-    fh = self._fh
-    if raw:
-        with fh.lock:
-            fh.seek(self.data_offset)
-            data = fh.read(self.data_size)
-        return data
-    if de.compression:
-        # if de.compression not in DECOMPRESS:
-        #     raise ValueError('compression unknown or not supported')
-        with fh.lock:
-            fh.seek(self.data_offset)
-            data = fh.read(self.data_size)
-        data = DECOMPRESS[de.compression](data)
-        if de.compression == 2:
-            # LZW
-            data = np.fromstring(data, de.dtype)  # noqa
-        elif de.compression in (5, 6):
-            # ZSTD
-            data = np.frombuffer(data, de.dtype)
-    else:
-        dtype = np.dtype(de.dtype)
-        with fh.lock:
-            fh.seek(self.data_offset)
-            data = fh.read_array(dtype, self.data_size // dtype.itemsize)
-
-    data = data.reshape(de.stored_shape)
-    if de.compression != 4 and de.stored_shape[-1] in (3, 4):
-        if de.stored_shape[-1] == 3:
-            # BGR -> RGB
-            data = data[..., ::-1]
-        else:
-            # BGRA -> RGBA
-            tmp = data[..., 0].copy()
-            data[..., 0] = data[..., 2]
-            data[..., 2] = tmp
-    if de.stored_shape == de.shape or not resize:
-        return data
-
-    # sub / supersampling
-    factors = [j / i for i, j in zip(de.stored_shape, de.shape)]
-    factors = [(int(round(f)) if abs(f - round(f)) < 0.0001 else f)
-               for f in factors]
-
-    # use repeat if possible
-    if order == 0 and all(isinstance(f, int) for f in factors):
-        data = repeat_nd(data, factors).copy()
-        data.shape = de.shape
-        return data
-
-    # remove leading dimensions with size 1 for speed
-    shape = list(de.stored_shape)
-    i = 0
-    for s in shape:
-        if s != 1:
-            break
-        i += 1
-    shape = shape[i:]
-    factors = factors[i:]
-    data.shape = shape
-
-    # resize RGB components separately for speed
-    if zoom is None:
-        raise ImportError("cannot import 'zoom' from scipy or ndimage")
-    if shape[-1] in (3, 4) and factors[-1] == 1.0:
-        factors = factors[:-1]
-        old = data
-        data = np.empty(de.shape, de.dtype[-2:])
-        for i in range(shape[-1]):
-            data[..., i] = zoom(old[..., i], zoom=factors, order=order)
-    else:
-        data = zoom(data, zoom=factors, order=order)
-
-    data.shape = de.shape
-    return data
-
-
-# monkeypatch zstd into czifile
-czifile.czifile.SubBlockSegment.data = data
-
-
-class Reader(AbstractReader, ABC):
-    priority = 0
-    do_not_pickle = 'reader', 'filedict'
-
-    @staticmethod
-    def _can_open(path):
-        return isinstance(path, Path) and path.suffix == '.czi'
-
-    def open(self):
-        self.reader = czifile.CziFile(self.path)
-        filedict = {}
-        for directory_entry in self.reader.filtered_subblock_directory:
-            idx = self.get_index(directory_entry, self.reader.start)
-            if 'S' not in self.reader.axes or self.series in range(*idx[self.reader.axes.index('S')]):
-                for c in range(*idx[self.reader.axes.index('C')]):
-                    for z in range(*idx[self.reader.axes.index('Z')]):
-                        for t in range(*idx[self.reader.axes.index('T')]):
-                            if (c, z, t) in filedict:
-                                filedict[c, z, t].append(directory_entry)
-                            else:
-                                filedict[c, z, t] = [directory_entry]
-        self.filedict = filedict  # noqa
-
-    def close(self):
-        self.reader.close()
-
-    @cached_property
-    def ome(self):
-        cache = OmeCache()
-        if self.path not in cache:
-            xml = self.reader.metadata()
-            attachments = {i.attachment_entry.name: i.attachment_entry.data_segment()
-                           for i in self.reader.attachments()}
-            tree = etree.fromstring(xml)
-            metadata = tree.find('Metadata')
-            version = metadata.find('Version')
-            if version is not None:
-                version = version.text
-            else:
-                version = metadata.find('Experiment').attrib['Version']
-
-            if version == '1.0':
-                cache[self.path] = self.ome_10(tree, attachments)
-            elif version == '1.2':
-                cache[self.path] = self.ome_12(tree, attachments)
-
-        return cache[self.path]
-
-    def ome_12(self, tree, attachments):
-        def text(item, default=""):
-            return default if item is None else item.text
-
-        def def_list(item):
-            return [] if item is None else item
-
-        ome = model.OME()
-
-        metadata = tree.find('Metadata')
-
-        information = metadata.find('Information')
-        display_setting = metadata.find('DisplaySetting')
-        ome.experimenters = [model.Experimenter(id='Experimenter:0',
-                                                user_name=information.find('Document').find('UserName').text)]
-
-        instrument = information.find('Instrument')
-        for _ in instrument.find('Microscopes'):
-            ome.instruments.append(model.Instrument(id='Instrument:0'))
-
-        for detector in instrument.find('Detectors'):
-            try:
-                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
-            except ValueError:
-                detector_type = model.Detector_Type.OTHER
-
-            ome.instruments[0].detectors.append(
-                model.Detector(
-                    id=detector.attrib['Id'].replace(' ', ''), model=text(detector.find('Manufacturer').find('Model')),
-                    type=detector_type
-                ))
-
-        for objective in instrument.find('Objectives'):
-            ome.instruments[0].objectives.append(
-                model.Objective(
-                    id=objective.attrib['Id'],
-                    model=text(objective.find('Manufacturer').find('Model')),
-                    immersion=text(objective.find('Immersion')),
-                    lens_na=float(text(objective.find('LensNA'))),
-                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
-
-        for tubelens in instrument.find('TubeLenses'):
-            try:
-                nominal_magnification = float(re.findall(r'\d+(?:[,.]\d*)?',
-                                                         tubelens.attrib['Name'])[0].replace(',', '.'))
-            except Exception:
-                nominal_magnification = 1.0
-
-            ome.instruments[0].objectives.append(
-                model.Objective(
-                    id=f"Objective:{tubelens.attrib['Id']}",
-                    model=tubelens.attrib['Name'],
-                    nominal_magnification=nominal_magnification))
-
-        for light_source in def_list(instrument.find('LightSources')):
-            if light_source.find('LightSourceType').find('Laser') is not None:
-                ome.instruments[0].lasers.append(
-                    model.Laser(
-                        id=f"LightSource:{light_source.attrib['Id']}",
-                        power=float(text(light_source.find('Power'))),
-                        wavelength=float(light_source.attrib['Id'][-3:])))
-
-        x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        size_x = x_max - x_min
-        size_y = y_max - y_min
-        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
-                                  for directory_entry in 'CZT')
-
-        image = information.find('Image')
-        pixel_type = text(image.find('PixelType'), 'Gray16')
-        if pixel_type.startswith('Gray'):
-            pixel_type = 'uint' + pixel_type[4:]
-        objective_settings = image.find('ObjectiveSettings')
-        try:  # TODO
-            scenes = image.find('Dimensions').find('S').find('Scenes')
-            center_position = [float(pos) for pos in text(scenes[0].find('CenterPosition')).split(',')]
-        except AttributeError:
-            center_position = [0, 0]
-        um = model.UnitsLength.MICROMETER
-        nm = model.UnitsLength.NANOMETER
-
-        ome.images.append(
-            model.Image(
-                id='Image:0',
-                name=f"{text(information.find('Document').find('Name'))} #1",
-                pixels=model.Pixels(
-                    id='Pixels:0', size_x=size_x, size_y=size_y,
-                    size_c=size_c, size_z=size_z, size_t=size_t,
-                    dimension_order='XYCZT', type=pixel_type,
-                    significant_bits=int(text(image.find('ComponentBitCount'))),
-                    big_endian=False, interleaved=False, metadata_only=True),
-                experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
-                instrument_ref=model.InstrumentRef(id='Instrument:0'),
-                objective_settings=model.ObjectiveSettings(
-                    id=objective_settings.find('ObjectiveRef').attrib['Id'],
-                    medium=text(objective_settings.find('Medium')),
-                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
-                stage_label=model.StageLabel(
-                    name=f'Scene position #0',
-                    x=center_position[0], x_unit=um,
-                    y=center_position[1], y_unit=um)))
-
-        for distance in metadata.find('Scaling').find('Items'):
-            if distance.attrib['Id'] == 'X':
-                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
-            elif distance.attrib['Id'] == 'Y':
-                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
-            elif size_z > 1 and distance.attrib['Id'] == 'Z':
-                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
-
-        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
-        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
-
-        for idx, (key, channel) in enumerate(channels_im.items()):
-            detector_settings = channel.find('DetectorSettings')
-            laser_scan_info = channel.find('LaserScanInfo')
-            detector = detector_settings.find('Detector')
-            try:
-                binning = model.Binning(text(detector_settings.find('Binning')))
-            except ValueError:
-                binning = model.Binning.OTHER
-
-            light_sources_settings = channel.find('LightSourcesSettings')
-            # no space in ome for multiple lightsources simultaneously
-            if light_sources_settings is not None:
-                light_source_settings = light_sources_settings[0]
-                light_source_settings = model.LightSourceSettings(
-                    id='LightSource:' + '_'.join([light_source_settings.find('LightSource').attrib['Id']
-                                                  for light_source_settings in light_sources_settings]),
-                    attenuation=float(text(light_source_settings.find('Attenuation'))),
-                    wavelength=float(text(light_source_settings.find('Wavelength'))),
-                    wavelength_unit=nm)
-            else:
-                light_source_settings = None
-
-            ome.images[0].pixels.channels.append(
-                model.Channel(
-                    id=f'Channel:{idx}',
-                    name=channel.attrib['Name'],
-                    acquisition_mode=text(channel.find('AcquisitionMode')).replace('SingleMoleculeLocalisation',
-                                                                                   'SingleMoleculeImaging'),
-                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
-                    detector_settings=model.DetectorSettings(
-                        id=detector.attrib['Id'].replace(' ', ""),
-                        binning=binning),
-                    emission_wavelength=i if (i := text(channel.find('EmissionWavelength'))) != '0' else '100',
-                    excitation_wavelength=text(channel.find('ExcitationWavelength')),
-                    # filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
-                    illumination_type=text(channel.find('IlluminationType')),
-                    light_source_settings=light_source_settings,
-                    samples_per_pixel=int(text(laser_scan_info.find('Averaging'), '1'))))
-
-        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'), '100')) for channel in
-                          channels_im.values()]
-        delta_ts = attachments['TimeStamps'].data()
-        dt = np.diff(delta_ts)
-        if np.std(dt) / np.mean(dt) > 0.02:
-            dt = np.median(dt[dt > 0])
-            delta_ts = dt * np.arange(len(delta_ts))
-            warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
-
-        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
-            ome.images[0].pixels.planes.append(
-                model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t], exposure_time=exposure_times[c]))
-
-        idx = 0
-        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
-            rectangle = layer.find('Elements').find('Rectangle')
-            if rectangle is not None:
-                geometry = rectangle.find('Geometry')
-                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
-                roi.union.append(
-                    model.Rectangle(
-                        id='Shape:0:0',
-                        height=float(text(geometry.find('Height'))),
-                        width=float(text(geometry.find('Width'))),
-                        x=float(text(geometry.find('Left'))),
-                        y=float(text(geometry.find('Top')))))
-                ome.rois.append(roi)
-                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
-                idx += 1
-        return ome
-
-    def ome_10(self, tree, attachments):
-        def text(item, default=""):
-            return default if item is None else item.text
-
-        def def_list(item):
-            return [] if item is None else item
-
-        ome = model.OME()
-
-        metadata = tree.find('Metadata')
-
-        information = metadata.find('Information')
-        display_setting = metadata.find('DisplaySetting')
-        experiment = metadata.find('Experiment')
-        acquisition_block = experiment.find('ExperimentBlocks').find('AcquisitionBlock')
-
-        ome.experimenters = [model.Experimenter(id='Experimenter:0',
-                                                user_name=information.find('User').find('DisplayName').text)]
-
-        instrument = information.find('Instrument')
-        ome.instruments.append(model.Instrument(id=instrument.attrib['Id']))
-
-        for detector in instrument.find('Detectors'):
-            try:
-                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
-            except ValueError:
-                detector_type = model.Detector_Type.OTHER
-
-            ome.instruments[0].detectors.append(
-                model.Detector(
-                    id=detector.attrib['Id'], model=text(detector.find('Manufacturer').find('Model')),
-                    amplification_gain=float(text(detector.find('AmplificationGain'))),
-                    gain=float(text(detector.find('Gain'))), zoom=float(text(detector.find('Zoom'))),
-                    type=detector_type
-                ))
-
-        for objective in instrument.find('Objectives'):
-            ome.instruments[0].objectives.append(
-                model.Objective(
-                    id=objective.attrib['Id'],
-                    model=text(objective.find('Manufacturer').find('Model')),
-                    immersion=text(objective.find('Immersion')),
-                    lens_na=float(text(objective.find('LensNA'))),
-                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
-
-        for light_source in def_list(instrument.find('LightSources')):
-            if light_source.find('LightSourceType').find('Laser') is not None:
-                ome.instruments[0].lasers.append(
-                    model.Laser(
-                        id=light_source.attrib['Id'],
-                        model=text(light_source.find('Manufacturer').find('Model')),
-                        power=float(text(light_source.find('Power'))),
-                        wavelength=float(
-                            text(light_source.find('LightSourceType').find('Laser').find('Wavelength')))))
-
-        multi_track_setup = acquisition_block.find('MultiTrackSetup')
-        for idx, tube_lens in enumerate({text(track_setup.find('TubeLensPosition'))
-                                         for track_setup in multi_track_setup}):
-            ome.instruments[0].objectives.append(
-                model.Objective(id=f'Objective:Tubelens:{idx}', model=tube_lens,
-                                nominal_magnification=float(
-                                    re.findall(r'\d+[,.]\d*', tube_lens)[0].replace(',', '.'))
-                                ))
-
-        for idx, filter_ in enumerate({text(beam_splitter.find('Filter'))
-                                       for track_setup in multi_track_setup
-                                       for beam_splitter in track_setup.find('BeamSplitters')}):
-            ome.instruments[0].filter_sets.append(
-                model.FilterSet(id=f'FilterSet:{idx}', model=filter_)
-            )
-
-        for idx, collimator in enumerate({text(track_setup.find('FWFOVPosition'))
-                                          for track_setup in multi_track_setup}):
-            ome.instruments[0].filters.append(model.Filter(id=f'Filter:Collimator:{idx}', model=collimator))
-
-        x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        size_x = x_max - x_min
-        size_y = y_max - y_min
-        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
-                                  for directory_entry in 'CZT')
-
-        image = information.find('Image')
-        pixel_type = text(image.find('PixelType'), 'Gray16')
-        if pixel_type.startswith('Gray'):
-            pixel_type = 'uint' + pixel_type[4:]
-        objective_settings = image.find('ObjectiveSettings')
-        scenes = image.find('Dimensions').find('S').find('Scenes')
-        positions = scenes[0].find('Positions')[0]
-        um = model.UnitsLength.MICROMETER
-        nm = model.UnitsLength.NANOMETER
-
-        ome.images.append(
-            model.Image(
-                id='Image:0',
-                name=f"{text(information.find('Document').find('Name'))} #1",
-                pixels=model.Pixels(
-                    id='Pixels:0', size_x=size_x, size_y=size_y,
-                    size_c=size_c, size_z=size_z, size_t=size_t,
-                    dimension_order='XYCZT', type=pixel_type,
-                    significant_bits=int(text(image.find('ComponentBitCount'))),
-                    big_endian=False, interleaved=False, metadata_only=True),
-                experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
-                instrument_ref=model.InstrumentRef(id='Instrument:0'),
-                objective_settings=model.ObjectiveSettings(
-                    id=objective_settings.find('ObjectiveRef').attrib['Id'],
-                    medium=text(objective_settings.find('Medium')),
-                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
-                stage_label=model.StageLabel(
-                    name=f'Scene position #0',
-                    x=float(positions.attrib['X']), x_unit=um,
-                    y=float(positions.attrib['Y']), y_unit=um,
-                    z=float(positions.attrib['Z']), z_unit=um)))
-
-        for distance in metadata.find('Scaling').find('Items'):
-            if distance.attrib['Id'] == 'X':
-                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
-            elif distance.attrib['Id'] == 'Y':
-                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
-            elif size_z > 1 and distance.attrib['Id'] == 'Z':
-                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
-
-        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
-        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
-        channels_ts = {detector.attrib['Id']: track_setup
-                       for track_setup in
-                       experiment.find('ExperimentBlocks').find('AcquisitionBlock').find('MultiTrackSetup')
-                       for detector in track_setup.find('Detectors')}
-
-        for idx, (key, channel) in enumerate(channels_im.items()):
-            detector_settings = channel.find('DetectorSettings')
-            laser_scan_info = channel.find('LaserScanInfo')
-            detector = detector_settings.find('Detector')
-            try:
-                binning = model.Binning(text(detector_settings.find('Binning')))
-            except ValueError:
-                binning = model.Binning.OTHER
-
-            filterset = text(channels_ts[key].find('BeamSplitters')[0].find('Filter'))
-            filterset_idx = [filterset.model for filterset in ome.instruments[0].filter_sets].index(filterset)
-
-            light_sources_settings = channel.find('LightSourcesSettings')
-            # no space in ome for multiple lightsources simultaneously
-            if len(light_sources_settings) > idx:
-                light_source_settings = light_sources_settings[idx]
-            else:
-                light_source_settings = light_sources_settings[0]
-            light_source_settings = model.LightSourceSettings(
-                id=light_source_settings.find('LightSource').attrib['Id'],
-                attenuation=float(text(light_source_settings.find('Attenuation'))),
-                wavelength=float(text(light_source_settings.find('Wavelength'))),
-                wavelength_unit=nm)
-
-            ome.images[0].pixels.channels.append(
-                model.Channel(
-                    id=f'Channel:{idx}',
-                    name=channel.attrib['Name'],
-                    acquisition_mode=text(channel.find('AcquisitionMode')),
-                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
-                    detector_settings=model.DetectorSettings(id=detector.attrib['Id'], binning=binning),
-                    # emission_wavelength=text(channel.find('EmissionWavelength')),  # TODO: fix
-                    excitation_wavelength=light_source_settings.wavelength,
-                    filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
-                    illumination_type=text(channel.find('IlluminationType')),
-                    light_source_settings=light_source_settings,
-                    samples_per_pixel=int(text(laser_scan_info.find('Averaging')))))
-
-        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'))) for channel in
-                          channels_im.values()]
-        delta_ts = attachments['TimeStamps'].data()
-        dt = np.diff(delta_ts)
-        if np.std(dt) / np.mean(dt) > 0.02:
-            dt = np.median(dt[dt > 0])
-            delta_ts = dt * np.arange(len(delta_ts))
-            warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
-
-        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
-            ome.images[0].pixels.planes.append(
-                model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t],
-                            exposure_time=exposure_times[c],
-                            position_x=float(positions.attrib['X']), position_x_unit=um,
-                            position_y=float(positions.attrib['Y']), position_y_unit=um,
-                            position_z=float(positions.attrib['Z']), position_z_unit=um))
-
-        idx = 0
-        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
-            rectangle = layer.find('Elements').find('Rectangle')
-            if rectangle is not None:
-                geometry = rectangle.find('Geometry')
-                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
-                roi.union.append(
-                    model.Rectangle(
-                        id='Shape:0:0',
-                        height=float(text(geometry.find('Height'))),
-                        width=float(text(geometry.find('Width'))),
-                        x=float(text(geometry.find('Left'))),
-                        y=float(text(geometry.find('Top')))))
-                ome.rois.append(roi)
-                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
-                idx += 1
-        return ome
-
-    def __frame__(self, c=0, z=0, t=0):
-        f = np.zeros(self.base.shape['yx'], self.dtype)
-        if (c, z, t) in self.filedict:
-            directory_entries = self.filedict[c, z, t]
-            x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
-            y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
-            xy_min = {'X': x_min, 'Y': y_min}
-            for directory_entry in directory_entries:
-                subblock = directory_entry.data_segment()
-                tile = subblock.data(resize=True, order=0)
-                axes_min = [xy_min.get(ax, 0) for ax in directory_entry.axes]
-                index = [slice(i - j - m, i - j + k)
-                         for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
-                index = tuple(index[self.reader.axes.index(i)] for i in 'YX')
-                f[index] = tile.squeeze()
-        return f
-
-    @staticmethod
-    def get_index(directory_entry, start):
-        return [(i - j, i - j + k) for i, j, k in zip(directory_entry.start, start, directory_entry.shape)]
+import re
+import warnings
+from abc import ABC
+from io import BytesIO
+from itertools import product
+from pathlib import Path
+
+import czifile
+import imagecodecs
+import numpy as np
+from lxml import etree
+from ome_types import model
+from tifffile import repeat_nd
+
+from .. import AbstractReader
+
+try:
+    # TODO: use zoom from imagecodecs implementation when available
+    from scipy.ndimage.interpolation import zoom
+except ImportError:
+    try:
+        from ndimage.interpolation import zoom
+    except ImportError:
+        zoom = None
+
+
+def zstd_decode(data: bytes) -> bytes:
+    """ decode zstd bytes, copied from BioFormats ZeissCZIReader """
+    def read_var_int(stream: BytesIO) -> int:
+        a = stream.read(1)[0]
+        if a & 128:
+            b = stream.read(1)[0]
+            if b & 128:
+                c = stream.read(1)[0]
+                return (c << 14) | ((b & 127) << 7) | (a & 127)
+            return (b << 7) | (a & 127)
+        return a & 255
+
+    try:
+        with BytesIO(data) as stream:
+            size_of_header = read_var_int(stream)
+            high_low_unpacking = False
+            while stream.tell() < size_of_header:
+                chunk_id = read_var_int(stream)
+                # only one chunk ID defined so far
+                if chunk_id == 1:
+                    high_low_unpacking = (stream.read(1)[0] & 1) == 1
+                else:
+                    raise ValueError(f'Invalid chunk id: {chunk_id}')
+            pointer = stream.tell()
+    except Exception:
+        high_low_unpacking = False
+        pointer = 0
+
+    decoded = imagecodecs.zstd_decode(data[pointer:])
+    if high_low_unpacking:
+        second_half = len(decoded) // 2
+        return bytes([decoded[second_half + i // 2] if i % 2 else decoded[i // 2] for i in range(len(decoded))])
+    else:
+        return decoded
+
+
+def data(self, raw=False, resize=True, order=0):
+    """Read image data from file and return as numpy array."""
+    DECOMPRESS = czifile.czifile.DECOMPRESS
+    DECOMPRESS[5] = imagecodecs.zstd_decode
+    DECOMPRESS[6] = zstd_decode
+
+    de = self.directory_entry
+    fh = self._fh
+    if raw:
+        with fh.lock:
+            fh.seek(self.data_offset)
+            data = fh.read(self.data_size)
+        return data
+    if de.compression:
+        # if de.compression not in DECOMPRESS:
+        #     raise ValueError('compression unknown or not supported')
+        with fh.lock:
+            fh.seek(self.data_offset)
+            data = fh.read(self.data_size)
+        data = DECOMPRESS[de.compression](data)
+        if de.compression == 2:
+            # LZW
+            data = np.fromstring(data, de.dtype)  # noqa
+        elif de.compression in (5, 6):
+            # ZSTD
+            data = np.frombuffer(data, de.dtype)
+    else:
+        dtype = np.dtype(de.dtype)
+        with fh.lock:
+            fh.seek(self.data_offset)
+            data = fh.read_array(dtype, self.data_size // dtype.itemsize)
+
+    data = data.reshape(de.stored_shape)
+    if de.compression != 4 and de.stored_shape[-1] in (3, 4):
+        if de.stored_shape[-1] == 3:
+            # BGR -> RGB
+            data = data[..., ::-1]
+        else:
+            # BGRA -> RGBA
+            tmp = data[..., 0].copy()
+            data[..., 0] = data[..., 2]
+            data[..., 2] = tmp
+    if de.stored_shape == de.shape or not resize:
+        return data
+
+    # sub / supersampling
+    factors = [j / i for i, j in zip(de.stored_shape, de.shape)]
+    factors = [(int(round(f)) if abs(f - round(f)) < 0.0001 else f)
+               for f in factors]
+
+    # use repeat if possible
+    if order == 0 and all(isinstance(f, int) for f in factors):
+        data = repeat_nd(data, factors).copy()
+        data.shape = de.shape
+        return data
+
+    # remove leading dimensions with size 1 for speed
+    shape = list(de.stored_shape)
+    i = 0
+    for s in shape:
+        if s != 1:
+            break
+        i += 1
+    shape = shape[i:]
+    factors = factors[i:]
+    data.shape = shape
+
+    # resize RGB components separately for speed
+    if zoom is None:
+        raise ImportError("cannot import 'zoom' from scipy or ndimage")
+    if shape[-1] in (3, 4) and factors[-1] == 1.0:
+        factors = factors[:-1]
+        old = data
+        data = np.empty(de.shape, de.dtype[-2:])
+        for i in range(shape[-1]):
+            data[..., i] = zoom(old[..., i], zoom=factors, order=order)
+    else:
+        data = zoom(data, zoom=factors, order=order)
+
+    data.shape = de.shape
+    return data
+
+
+# monkeypatch zstd into czifile
+czifile.czifile.SubBlockSegment.data = data
+
+
+class Reader(AbstractReader, ABC):
+    priority = 0
+    do_not_pickle = 'reader', 'filedict'
+
+    @staticmethod
+    def _can_open(path):
+        return isinstance(path, Path) and path.suffix == '.czi'
+
+    def open(self):
+        self.reader = czifile.CziFile(self.path)
+        filedict = {}
+        for directory_entry in self.reader.filtered_subblock_directory:
+            idx = self.get_index(directory_entry, self.reader.start)
+            if 'S' not in self.reader.axes or self.series in range(*idx[self.reader.axes.index('S')]):
+                for c in range(*idx[self.reader.axes.index('C')]):
+                    for z in range(*idx[self.reader.axes.index('Z')]):
+                        for t in range(*idx[self.reader.axes.index('T')]):
+                            if (c, z, t) in filedict:
+                                filedict[c, z, t].append(directory_entry)
+                            else:
+                                filedict[c, z, t] = [directory_entry]
+        self.filedict = filedict  # noqa
+
+    def close(self):
+        self.reader.close()
+
+    def get_ome(self):
+        xml = self.reader.metadata()
+        attachments = {i.attachment_entry.name: i.attachment_entry.data_segment()
+                       for i in self.reader.attachments()}
+        tree = etree.fromstring(xml)
+        metadata = tree.find('Metadata')
+        version = metadata.find('Version')
+        if version is not None:
+            version = version.text
+        else:
+            version = metadata.find('Experiment').attrib['Version']
+
+        if version == '1.0':
+            return self.ome_10(tree, attachments)
+        elif version == '1.2':
+            return self.ome_12(tree, attachments)
+
+    def ome_12(self, tree, attachments):
+        def text(item, default=""):
+            return default if item is None else item.text
+
+        def def_list(item):
+            return [] if item is None else item
+
+        ome = model.OME()
+
+        metadata = tree.find('Metadata')
+
+        information = metadata.find('Information')
+        display_setting = metadata.find('DisplaySetting')
+        ome.experimenters = [model.Experimenter(id='Experimenter:0',
+                                                user_name=information.find('Document').find('UserName').text)]
+
+        instrument = information.find('Instrument')
+        for _ in instrument.find('Microscopes'):
+            ome.instruments.append(model.Instrument(id='Instrument:0'))
+
+        for detector in instrument.find('Detectors'):
+            try:
+                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
+            except ValueError:
+                detector_type = model.Detector_Type.OTHER
+
+            ome.instruments[0].detectors.append(
+                model.Detector(
+                    id=detector.attrib['Id'].replace(' ', ''), model=text(detector.find('Manufacturer').find('Model')),
+                    type=detector_type
+                ))
+
+        for objective in instrument.find('Objectives'):
+            ome.instruments[0].objectives.append(
+                model.Objective(
+                    id=objective.attrib['Id'],
+                    model=text(objective.find('Manufacturer').find('Model')),
+                    immersion=text(objective.find('Immersion')),
+                    lens_na=float(text(objective.find('LensNA'))),
+                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
+
+        for tubelens in instrument.find('TubeLenses'):
+            try:
+                nominal_magnification = float(re.findall(r'\d+(?:[,.]\d*)?',
+                                                         tubelens.attrib['Name'])[0].replace(',', '.'))
+            except Exception:
+                nominal_magnification = 1.0
+
+            ome.instruments[0].objectives.append(
+                model.Objective(
+                    id=f"Objective:{tubelens.attrib['Id']}",
+                    model=tubelens.attrib['Name'],
+                    nominal_magnification=nominal_magnification))
+
+        for light_source in def_list(instrument.find('LightSources')):
+            if light_source.find('LightSourceType').find('Laser') is not None:
+                ome.instruments[0].lasers.append(
+                    model.Laser(
+                        id=f"LightSource:{light_source.attrib['Id']}",
+                        power=float(text(light_source.find('Power'))),
+                        wavelength=float(light_source.attrib['Id'][-3:])))
+
+        x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
+        y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
+        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
+        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
+        size_x = x_max - x_min
+        size_y = y_max - y_min
+        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
+                                  for directory_entry in 'CZT')
+
+        image = information.find('Image')
+        pixel_type = text(image.find('PixelType'), 'Gray16')
+        if pixel_type.startswith('Gray'):
+            pixel_type = 'uint' + pixel_type[4:]
+        objective_settings = image.find('ObjectiveSettings')
+        try:  # TODO
+            scenes = image.find('Dimensions').find('S').find('Scenes')
+            center_position = [float(pos) for pos in text(scenes[0].find('CenterPosition')).split(',')]
+        except AttributeError:
+            center_position = [0, 0]
+        um = model.UnitsLength.MICROMETER
+        nm = model.UnitsLength.NANOMETER
+
+        ome.images.append(
+            model.Image(
+                id='Image:0',
+                name=f"{text(information.find('Document').find('Name'))} #1",
+                pixels=model.Pixels(
+                    id='Pixels:0', size_x=size_x, size_y=size_y,
+                    size_c=size_c, size_z=size_z, size_t=size_t,
+                    dimension_order='XYCZT', type=pixel_type,
+                    significant_bits=int(text(image.find('ComponentBitCount'))),
+                    big_endian=False, interleaved=False, metadata_only=True),
+                experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
+                instrument_ref=model.InstrumentRef(id='Instrument:0'),
+                objective_settings=model.ObjectiveSettings(
+                    id=objective_settings.find('ObjectiveRef').attrib['Id'],
+                    medium=text(objective_settings.find('Medium')),
+                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
+                stage_label=model.StageLabel(
+                    name=f'Scene position #0',
+                    x=center_position[0], x_unit=um,
+                    y=center_position[1], y_unit=um)))
+
+        for distance in metadata.find('Scaling').find('Items'):
+            if distance.attrib['Id'] == 'X':
+                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
+            elif distance.attrib['Id'] == 'Y':
+                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
+            elif size_z > 1 and distance.attrib['Id'] == 'Z':
+                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
+
+        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
+        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
+
+        for idx, (key, channel) in enumerate(channels_im.items()):
+            detector_settings = channel.find('DetectorSettings')
+            laser_scan_info = channel.find('LaserScanInfo')
+            detector = detector_settings.find('Detector')
+            try:
+                binning = model.Binning(text(detector_settings.find('Binning')))
+            except ValueError:
+                binning = model.Binning.OTHER
+
+            light_sources_settings = channel.find('LightSourcesSettings')
+            # no space in ome for multiple lightsources simultaneously
+            if light_sources_settings is not None:
+                light_source_settings = light_sources_settings[0]
+                light_source_settings = model.LightSourceSettings(
+                    id='LightSource:' + '_'.join([light_source_settings.find('LightSource').attrib['Id']
+                                                  for light_source_settings in light_sources_settings]),
+                    attenuation=float(text(light_source_settings.find('Attenuation'))),
+                    wavelength=float(text(light_source_settings.find('Wavelength'))),
+                    wavelength_unit=nm)
+            else:
+                light_source_settings = None
+
+            ome.images[0].pixels.channels.append(
+                model.Channel(
+                    id=f'Channel:{idx}',
+                    name=channel.attrib['Name'],
+                    acquisition_mode=text(channel.find('AcquisitionMode')).replace('SingleMoleculeLocalisation',
+                                                                                   'SingleMoleculeImaging'),
+                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
+                    detector_settings=model.DetectorSettings(
+                        id=detector.attrib['Id'].replace(' ', ""),
+                        binning=binning),
+                    emission_wavelength=i if (i := text(channel.find('EmissionWavelength'))) != '0' else '100',
+                    excitation_wavelength=text(channel.find('ExcitationWavelength')),
+                    # filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
+                    illumination_type=text(channel.find('IlluminationType')),
+                    light_source_settings=light_source_settings,
+                    samples_per_pixel=int(text(laser_scan_info.find('Averaging'), '1'))))
+
+        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'), '100')) for channel in
+                          channels_im.values()]
+        delta_ts = attachments['TimeStamps'].data()
+        dt = np.diff(delta_ts)
+        if np.std(dt) / np.mean(dt) > 0.02:
+            dt = np.median(dt[dt > 0])
+            delta_ts = dt * np.arange(len(delta_ts))
+            warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
+
+        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
+            ome.images[0].pixels.planes.append(
+                model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t], exposure_time=exposure_times[c]))
+
+        idx = 0
+        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
+            rectangle = layer.find('Elements').find('Rectangle')
+            if rectangle is not None:
+                geometry = rectangle.find('Geometry')
+                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
+                roi.union.append(
+                    model.Rectangle(
+                        id='Shape:0:0',
+                        height=float(text(geometry.find('Height'))),
+                        width=float(text(geometry.find('Width'))),
+                        x=float(text(geometry.find('Left'))),
+                        y=float(text(geometry.find('Top')))))
+                ome.rois.append(roi)
+                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
+                idx += 1
+        return ome
+
+    def ome_10(self, tree, attachments):
+        def text(item, default=""):
+            return default if item is None else item.text
+
+        def def_list(item):
+            return [] if item is None else item
+
+        ome = model.OME()
+
+        metadata = tree.find('Metadata')
+
+        information = metadata.find('Information')
+        display_setting = metadata.find('DisplaySetting')
+        experiment = metadata.find('Experiment')
+        acquisition_block = experiment.find('ExperimentBlocks').find('AcquisitionBlock')
+
+        ome.experimenters = [model.Experimenter(id='Experimenter:0',
+                                                user_name=information.find('User').find('DisplayName').text)]
+
+        instrument = information.find('Instrument')
+        ome.instruments.append(model.Instrument(id=instrument.attrib['Id']))
+
+        for detector in instrument.find('Detectors'):
+            try:
+                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
+            except ValueError:
+                detector_type = model.Detector_Type.OTHER
+
+            ome.instruments[0].detectors.append(
+                model.Detector(
+                    id=detector.attrib['Id'], model=text(detector.find('Manufacturer').find('Model')),
+                    amplification_gain=float(text(detector.find('AmplificationGain'))),
+                    gain=float(text(detector.find('Gain'))), zoom=float(text(detector.find('Zoom'))),
+                    type=detector_type
+                ))
+
+        for objective in instrument.find('Objectives'):
+            ome.instruments[0].objectives.append(
+                model.Objective(
+                    id=objective.attrib['Id'],
+                    model=text(objective.find('Manufacturer').find('Model')),
+                    immersion=text(objective.find('Immersion')),
+                    lens_na=float(text(objective.find('LensNA'))),
+                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
+
+        for light_source in def_list(instrument.find('LightSources')):
+            if light_source.find('LightSourceType').find('Laser') is not None:
+                ome.instruments[0].lasers.append(
+                    model.Laser(
+                        id=light_source.attrib['Id'],
+                        model=text(light_source.find('Manufacturer').find('Model')),
+                        power=float(text(light_source.find('Power'))),
+                        wavelength=float(
+                            text(light_source.find('LightSourceType').find('Laser').find('Wavelength')))))
+
+        multi_track_setup = acquisition_block.find('MultiTrackSetup')
+        for idx, tube_lens in enumerate({text(track_setup.find('TubeLensPosition'))
+                                         for track_setup in multi_track_setup}):
+            ome.instruments[0].objectives.append(
+                model.Objective(id=f'Objective:Tubelens:{idx}', model=tube_lens,
+                                nominal_magnification=float(
+                                    re.findall(r'\d+[,.]\d*', tube_lens)[0].replace(',', '.'))
+                                ))
+
+        for idx, filter_ in enumerate({text(beam_splitter.find('Filter'))
+                                       for track_setup in multi_track_setup
+                                       for beam_splitter in track_setup.find('BeamSplitters')}):
+            ome.instruments[0].filter_sets.append(
+                model.FilterSet(id=f'FilterSet:{idx}', model=filter_)
+            )
+
+        for idx, collimator in enumerate({text(track_setup.find('FWFOVPosition'))
+                                          for track_setup in multi_track_setup}):
+            ome.instruments[0].filters.append(model.Filter(id=f'Filter:Collimator:{idx}', model=collimator))
+
+        x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
+        y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
+        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
+        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
+        size_x = x_max - x_min
+        size_y = y_max - y_min
+        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
+                                  for directory_entry in 'CZT')
+
+        image = information.find('Image')
+        pixel_type = text(image.find('PixelType'), 'Gray16')
+        if pixel_type.startswith('Gray'):
+            pixel_type = 'uint' + pixel_type[4:]
+        objective_settings = image.find('ObjectiveSettings')
+        scenes = image.find('Dimensions').find('S').find('Scenes')
+        positions = scenes[0].find('Positions')[0]
+        um = model.UnitsLength.MICROMETER
+        nm = model.UnitsLength.NANOMETER
+
+        ome.images.append(
+            model.Image(
+                id='Image:0',
+                name=f"{text(information.find('Document').find('Name'))} #1",
+                pixels=model.Pixels(
+                    id='Pixels:0', size_x=size_x, size_y=size_y,
+                    size_c=size_c, size_z=size_z, size_t=size_t,
+                    dimension_order='XYCZT', type=pixel_type,
+                    significant_bits=int(text(image.find('ComponentBitCount'))),
+                    big_endian=False, interleaved=False, metadata_only=True),
+                experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
+                instrument_ref=model.InstrumentRef(id='Instrument:0'),
+                objective_settings=model.ObjectiveSettings(
+                    id=objective_settings.find('ObjectiveRef').attrib['Id'],
+                    medium=text(objective_settings.find('Medium')),
+                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
+                stage_label=model.StageLabel(
+                    name=f'Scene position #0',
+                    x=float(positions.attrib['X']), x_unit=um,
+                    y=float(positions.attrib['Y']), y_unit=um,
+                    z=float(positions.attrib['Z']), z_unit=um)))
+
+        for distance in metadata.find('Scaling').find('Items'):
+            if distance.attrib['Id'] == 'X':
+                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
+            elif distance.attrib['Id'] == 'Y':
+                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
+            elif size_z > 1 and distance.attrib['Id'] == 'Z':
+                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
+
+        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
+        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
+        channels_ts = {detector.attrib['Id']: track_setup
+                       for track_setup in
+                       experiment.find('ExperimentBlocks').find('AcquisitionBlock').find('MultiTrackSetup')
+                       for detector in track_setup.find('Detectors')}
+
+        for idx, (key, channel) in enumerate(channels_im.items()):
+            detector_settings = channel.find('DetectorSettings')
+            laser_scan_info = channel.find('LaserScanInfo')
+            detector = detector_settings.find('Detector')
+            try:
+                binning = model.Binning(text(detector_settings.find('Binning')))
+            except ValueError:
+                binning = model.Binning.OTHER
+
+            filterset = text(channels_ts[key].find('BeamSplitters')[0].find('Filter'))
+            filterset_idx = [filterset.model for filterset in ome.instruments[0].filter_sets].index(filterset)
+
+            light_sources_settings = channel.find('LightSourcesSettings')
+            # no space in ome for multiple lightsources simultaneously
+            if len(light_sources_settings) > idx:
+                light_source_settings = light_sources_settings[idx]
+            else:
+                light_source_settings = light_sources_settings[0]
+            light_source_settings = model.LightSourceSettings(
+                id=light_source_settings.find('LightSource').attrib['Id'],
+                attenuation=float(text(light_source_settings.find('Attenuation'))),
+                wavelength=float(text(light_source_settings.find('Wavelength'))),
+                wavelength_unit=nm)
+
+            ome.images[0].pixels.channels.append(
+                model.Channel(
+                    id=f'Channel:{idx}',
+                    name=channel.attrib['Name'],
+                    acquisition_mode=text(channel.find('AcquisitionMode')),
+                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
+                    detector_settings=model.DetectorSettings(id=detector.attrib['Id'], binning=binning),
+                    # emission_wavelength=text(channel.find('EmissionWavelength')),  # TODO: fix
+                    excitation_wavelength=light_source_settings.wavelength,
+                    filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
+                    illumination_type=text(channel.find('IlluminationType')),
+                    light_source_settings=light_source_settings,
+                    samples_per_pixel=int(text(laser_scan_info.find('Averaging')))))
+
+        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'))) for channel in
+                          channels_im.values()]
+        delta_ts = attachments['TimeStamps'].data()
+        dt = np.diff(delta_ts)
+        if np.std(dt) / np.mean(dt) > 0.02:
+            dt = np.median(dt[dt > 0])
+            delta_ts = dt * np.arange(len(delta_ts))
+            warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
+
+        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
+            ome.images[0].pixels.planes.append(
+                model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t],
+                            exposure_time=exposure_times[c],
+                            position_x=float(positions.attrib['X']), position_x_unit=um,
+                            position_y=float(positions.attrib['Y']), position_y_unit=um,
+                            position_z=float(positions.attrib['Z']), position_z_unit=um))
+
+        idx = 0
+        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
+            rectangle = layer.find('Elements').find('Rectangle')
+            if rectangle is not None:
+                geometry = rectangle.find('Geometry')
+                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
+                roi.union.append(
+                    model.Rectangle(
+                        id='Shape:0:0',
+                        height=float(text(geometry.find('Height'))),
+                        width=float(text(geometry.find('Width'))),
+                        x=float(text(geometry.find('Left'))),
+                        y=float(text(geometry.find('Top')))))
+                ome.rois.append(roi)
+                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
+                idx += 1
+        return ome
+
+    def __frame__(self, c=0, z=0, t=0):
+        f = np.zeros(self.base.shape['yx'], self.dtype)
+        if (c, z, t) in self.filedict:
+            directory_entries = self.filedict[c, z, t]
+            x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
+            y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
+            xy_min = {'X': x_min, 'Y': y_min}
+            for directory_entry in directory_entries:
+                subblock = directory_entry.data_segment()
+                tile = subblock.data(resize=True, order=0)
+                axes_min = [xy_min.get(ax, 0) for ax in directory_entry.axes]
+                index = [slice(i - j - m, i - j + k)
+                         for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
+                index = tuple(index[self.reader.axes.index(i)] for i in 'YX')
+                f[index] = tile.squeeze()
+        return f
+
+    @staticmethod
+    def get_index(directory_entry, start):
+        return [(i - j, i - j + k) for i, j, k in zip(directory_entry.start, start, directory_entry.shape)]
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/fijiread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC
-from functools import cached_property
 from itertools import product
 from pathlib import Path
 from struct import unpack
 from warnings import warn
 
 import numpy as np
 from ome_types import model
@@ -38,16 +37,15 @@
         self.count = self.reader.pages[0].databytecounts[0]  # noqa
         self.bytes_per_sample = self.reader.pages[0].bitspersample // 8  # noqa
         self.fmt = self.reader.byteorder + self.count // self.bytes_per_sample * 'BHILQ'[self.bytes_per_sample - 1]  # noqa
 
     def close(self):
         self.reader.close()
 
-    @cached_property
-    def ome(self):
+    def get_ome(self):
         size_y, size_x = self.reader.pages[0].shape
         size_c, size_z = 1, 1
         size_t = int(np.floor((self.reader.filehandle.size - self.reader.pages[0].dataoffsets[0]) / self.count))
         pixel_type = model.PixelType(self.reader.pages[0].dtype.name)
         ome = model.OME()
         ome.instruments.append(model.Instrument())
         ome.images.append(
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/ndread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC
-from functools import cached_property
 from itertools import product
 
 import numpy as np
 from ome_types import model
 
 from .. import AbstractReader
 
@@ -11,16 +10,15 @@
 class Reader(AbstractReader, ABC):
     priority = 20
 
     @staticmethod
     def _can_open(path):
         return isinstance(path, np.ndarray) and 1 <= path.ndim <= 5
 
-    @cached_property
-    def ome(self):
+    def get_ome(self):
         def shape(size_x=1, size_y=1, size_c=1, size_z=1, size_t=1):  # noqa
             return size_x, size_y, size_c, size_z, size_t
         size_x, size_y, size_c, size_z, size_t = shape(*self.array.shape)
         try:
             pixel_type = model.PixelType(self.array.dtype.name)
         except ValueError:
             if self.array.dtype.name.startswith('int'):
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/seqread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from abc import ABC
 from datetime import datetime
-from functools import cached_property
 from itertools import product
 from pathlib import Path
 
 import tifffile
 import yaml
 from ome_types import model
 from ome_types.units import _quantity_property  # noqa
@@ -45,16 +44,15 @@
 class Reader(AbstractReader, ABC):
     priority = 10
 
     @staticmethod
     def _can_open(path):
         return isinstance(path, Path) and path.is_dir()
 
-    @cached_property
-    def ome(self):
+    def get_ome(self):
         ome = model.OME()
         with tifffile.TiffFile(self.filedict[0, 0, 0]) as tif:
             metadata = {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
         ome.experimenters.append(
             model.Experimenter(id='Experimenter:0', user_name=metadata['Info']['Summary']['UserName']))
         objective_str = metadata['Info']['ZeissObjectiveTurret-Label']
         ome.instruments.append(model.Instrument())
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.0/ndbioimage/readers/tifread.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,41 @@
         if isinstance(path, Path) and path.suffix in ('.tif', '.tiff'):
             with tifffile.TiffFile(path) as tif:
                 return tif.is_imagej and tif.pages[-1]._nextifd() == 0  # noqa
         else:
             return False
 
     @cached_property
-    def ome(self):
-        metadata = {key: yaml.safe_load(value) if isinstance(value, str) else value
-                    for key, value in self.reader.imagej_metadata.items()}
+    def metadata(self):
+        return {key: yaml.safe_load(value) if isinstance(value, str) else value
+                for key, value in self.reader.imagej_metadata.items()}
 
+    def get_ome(self):
         page = self.reader.pages[0]
-        self.p_ndim = page.ndim  # noqa
         size_y = page.imagelength
         size_x = page.imagewidth
         if self.p_ndim == 3:
             size_c = page.samplesperpixel
-            self.p_transpose = [i for i in [page.axes.find(j) for j in 'SYX'] if i >= 0]  # noqa
-            size_t = metadata.get('frames', 1)  # // C
+            size_t = self.metadata.get('frames', 1)  # // C
         else:
-            size_c = metadata.get('channels', 1)
-            size_t = metadata.get('frames', 1)
-        size_z = metadata.get('slices', 1)
+            size_c = self.metadata.get('channels', 1)
+            size_t = self.metadata.get('frames', 1)
+        size_z = self.metadata.get('slices', 1)
         if 282 in page.tags and 296 in page.tags and page.tags[296].value == 1:
             f = page.tags[282].value
             pxsize = f[1] / f[0]
         else:
             pxsize = None
 
         dtype = page.dtype.name
         if dtype not in ('int8', 'int16', 'int32', 'uint8', 'uint16', 'uint32',
                          'float', 'double', 'complex', 'double-complex', 'bit'):
             dtype = 'float'
 
-        interval_t = metadata.get('interval', 0)
+        interval_t = self.metadata.get('interval', 0)
 
         ome = model.OME()
         ome.instruments.append(model.Instrument(id='Instrument:0'))
         ome.instruments[0].objectives.append(model.Objective(id='Objective:0'))
         ome.images.append(
             model.Image(
                 id='Image:0',
@@ -66,14 +65,18 @@
                 objective_settings=model.ObjectiveSettings(id='Objective:0')))
         for c, z, t in product(range(size_c), range(size_z), range(size_t)):
             ome.images[0].pixels.planes.append(model.Plane(the_c=c, the_z=z, the_t=t, delta_t=interval_t * t))
         return ome
 
     def open(self):
         self.reader = tifffile.TiffFile(self.path)
+        page = self.reader.pages[0]
+        self.p_ndim = page.ndim  # noqa
+        if self.p_ndim == 3:
+            self.p_transpose = [i for i in [page.axes.find(j) for j in 'SYX'] if i >= 0]  # noqa
 
     def close(self):
         self.reader.close()
 
     def __frame__(self, c, z, t):
         if self.p_ndim == 3:
             return np.transpose(self.reader.asarray(z + t * self.base.shape['z']), self.p_transpose)[c]
```

### Comparing `ndbioimage-2024.3.7/ndbioimage/transforms.py` & `ndbioimage-2024.4.0/ndbioimage/transforms.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,458 +1,458 @@
-import warnings
-from copy import deepcopy
-from pathlib import Path
-
-import numpy as np
-import yaml
-from parfor import Chunks, pmap
-from skimage import filters
-from tiffwrite import IJTiffFile
-from tqdm.auto import tqdm
-
-try:
-    # best if SimpleElastix is installed: https://simpleelastix.readthedocs.io/GettingStarted.html
-    import SimpleITK as sitk  # noqa
-except ImportError:
-    sitk = None
-
-try:
-    from pandas import DataFrame, Series, concat
-except ImportError:
-    DataFrame, Series, concat = None, None, None
-
-
-if hasattr(yaml, 'full_load'):
-    yamlload = yaml.full_load
-else:
-    yamlload = yaml.load
-
-
-class Transforms(dict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.default = Transform()
-
-    @classmethod
-    def from_file(cls, file, C=True, T=True):
-        with open(Path(file).with_suffix('.yml')) as f:
-            return cls.from_dict(yamlload(f), C, T)
-
-    @classmethod
-    def from_dict(cls, d, C=True, T=True):
-        new = cls()
-        for key, value in d.items():
-            if isinstance(key, str) and C:
-                new[key.replace(r'\:', ':').replace('\\\\', '\\')] = Transform.from_dict(value)
-            elif T:
-                new[key] = Transform.from_dict(value)
-        return new
-
-    @classmethod
-    def from_shifts(cls, shifts):
-        new = cls()
-        for key, shift in shifts.items():
-            new[key] = Transform.from_shift(shift)
-        return new
-
-    def __mul__(self, other):
-        new = Transforms()
-        if isinstance(other, Transforms):
-            for key0, value0 in self.items():
-                for key1, value1 in other.items():
-                    new[key0 + key1] = value0 * value1
-            return new
-        elif other is None:
-            return self
-        else:
-            for key in self.keys():
-                new[key] = self[key] * other
-            return new
-
-    def asdict(self):
-        return {key.replace('\\', '\\\\').replace(':', r'\:') if isinstance(key, str) else key: value.asdict()
-                for key, value in self.items()}
-
-    def __getitem__(self, item):
-        return np.prod([self[i] for i in item[::-1]]) if isinstance(item, tuple) else super().__getitem__(item)
-
-    def __missing__(self, key):
-        return self.default
-
-    def __getstate__(self):
-        return self.__dict__
-
-    def __setstate__(self, state):
-        self.__dict__.update(state)
-
-    def __hash__(self):
-        return hash(frozenset((*self.__dict__.items(), *self.items())))
-
-    def save(self, file):
-        with open(Path(file).with_suffix('.yml'), 'w') as f:
-            yaml.safe_dump(self.asdict(), f, default_flow_style=None)
-
-    def copy(self):
-        return deepcopy(self)
-
-    def adapt(self, origin, shape, channel_names):
-        def key_map(a, b):
-            def fun(b, key_a):
-                for key_b in b:
-                    if key_b in key_a or key_a in key_b:
-                        return key_a, key_b
-
-            return {n[0]: n[1] for key_a in a if (n := fun(b, key_a))}
-
-        for value in self.values():
-            value.adapt(origin, shape)
-        self.default.adapt(origin, shape)
-        transform_channels = {key for key in self.keys() if isinstance(key, str)}
-        if set(channel_names) - transform_channels:
-            mapping = key_map(channel_names, transform_channels)
-            warnings.warn(f'The image file and the transform do not have the same channels,'
-                          f' creating a mapping: {mapping}')
-            for key_im, key_t in mapping.items():
-                self[key_im] = self[key_t]
-
-    @property
-    def inverse(self):
-        # TODO: check for C@T
-        inverse = self.copy()
-        for key, value in self.items():
-            inverse[key] = value.inverse
-        return inverse
-
-    def coords_pandas(self, array, channel_names, columns=None):
-        if isinstance(array, DataFrame):
-            return concat([self.coords_pandas(row, channel_names, columns) for _, row in array.iterrows()], axis=1).T
-        elif isinstance(array, Series):
-            key = []
-            if 'C' in array:
-                key.append(channel_names[int(array['C'])])
-            if 'T' in array:
-                key.append(int(array['T']))
-            return self[tuple(key)].coords(array, columns)
-        else:
-            raise TypeError('Not a pandas DataFrame or Series.')
-
-    def with_beads(self, cyllens, bead_files):
-        assert len(bead_files) > 0, 'At least one file is needed to calculate the registration.'
-        transforms = [self.calculate_channel_transforms(file, cyllens) for file in bead_files]
-        for key in {key for transform in transforms for key in transform.keys()}:
-            new_transforms = [transform[key] for transform in transforms if key in transform]
-            if len(new_transforms) == 1:
-                self[key] = new_transforms[0]
-            else:
-                self[key] = Transform()
-                self[key].parameters = np.mean([t.parameters for t in new_transforms], 0)
-                self[key].dparameters = (np.std([t.parameters for t in new_transforms], 0) /
-                                        np.sqrt(len(new_transforms))).tolist()
-        return self
-
-    @staticmethod
-    def get_bead_files(path):
-        from . import Imread
-        files = []
-        for file in path.iterdir():
-            if file.name.lower().startswith('beads'):
-                try:
-                    with Imread(file):
-                        files.append(file)
-                except Exception:
-                    pass
-        files = sorted(files)
-        if not files:
-            raise Exception('No bead file found!')
-        checked_files = []
-        for file in files:
-            try:
-                if file.is_dir():
-                    file /= 'Pos0'
-                with Imread(file):  # check for errors opening the file
-                    checked_files.append(file)
-            except (Exception,):
-                continue
-        if not checked_files:
-            raise Exception('No bead file found!')
-        return checked_files
-
-    @staticmethod
-    def calculate_channel_transforms(bead_file, cyllens):
-        """ When no channel is not transformed by a cylindrical lens, assume that the image is scaled by a factor 1.162
-            in the horizontal direction """
-        from . import Imread
-
-        with Imread(bead_file, axes='zcxy') as im:  # noqa
-            max_ims = im.max('z')
-            goodch = [c for c, max_im in enumerate(max_ims) if not im.is_noise(max_im)]
-            if not goodch:
-                goodch = list(range(len(max_ims)))
-            untransformed = [c for c in range(im.shape['c']) if cyllens[im.detector[c]].lower() == 'none']
-
-            good_and_untrans = sorted(set(goodch) & set(untransformed))
-            if good_and_untrans:
-                masterch = good_and_untrans[0]
-            else:
-                masterch = goodch[0]
-            transform = Transform()
-            if not good_and_untrans:
-                matrix = transform.matrix
-                matrix[0, 0] = 0.86
-                transform.matrix = matrix
-            transforms = Transforms()
-            for c in tqdm(goodch, desc='Calculating channel transforms'):  # noqa
-                if c == masterch:
-                    transforms[im.channel_names[c]] = transform
-                else:
-                    transforms[im.channel_names[c]] = Transform.register(max_ims[masterch], max_ims[c]) * transform
-        return transforms
-
-    @staticmethod
-    def save_channel_transform_tiff(bead_files, tiffile):
-        from . import Imread
-        n_channels = 0
-        for file in bead_files:
-            with Imread(file) as im:
-                n_channels = max(n_channels, im.shape['c'])
-        with IJTiffFile(tiffile, (n_channels, 1, len(bead_files))) as tif:
-            for t, file in enumerate(bead_files):
-                with Imread(file) as im:
-                    with Imread(file).with_transform() as jm:
-                        for c in range(im.shape['c']):
-                            tif.save(np.hstack((im(c=c, t=0).max('z'), jm(c=c, t=0).max('z'))), c, 0, t)
-
-    def with_drift(self, im):
-        """ Calculate shifts relative to the first frame
-            divide the sequence into groups,
-            compare each frame to the frame in the middle of the group and compare these middle frames to each other
-        """
-        im = im.transpose('tzycx')
-        t_groups = [list(chunk) for chunk in Chunks(range(im.shape['t']), size=round(np.sqrt(im.shape['t'])))]
-        t_keys = [int(np.round(np.mean(t_group))) for t_group in t_groups]
-        t_pairs = [(int(np.round(np.mean(t_group))), frame) for t_group in t_groups for frame in t_group]
-        t_pairs.extend(zip(t_keys, t_keys[1:]))
-        fmaxz_keys = {t_key: filters.gaussian(im[t_key].max('z'), 5) for t_key in t_keys}
-
-        def fun(t_key_t, im, fmaxz_keys):
-            t_key, t = t_key_t
-            if t_key == t:
-                return 0, 0
-            else:
-                fmaxz = filters.gaussian(im[t].max('z'), 5)
-                return Transform.register(fmaxz_keys[t_key], fmaxz, 'translation').parameters[4:]
-
-        shifts = np.array(pmap(fun, t_pairs, (im, fmaxz_keys), desc='Calculating image shifts.'))
-        shift_keys_cum = np.zeros(2)
-        for shift_keys, t_group in zip(np.vstack((-shifts[0], shifts[im.shape['t']:])), t_groups):
-            shift_keys_cum += shift_keys
-            shifts[t_group] += shift_keys_cum
-
-        for i, shift in enumerate(shifts[:im.shape['t']]):
-            self[i] = Transform.from_shift(shift)
-        return self
-
-
-class Transform:
-    def __init__(self):
-        if sitk is None:
-            self.transform = None
-        else:
-            self.transform = sitk.ReadTransform(str(Path(__file__).parent / 'transform.txt'))
-        self.dparameters = [0., 0., 0., 0., 0., 0.]
-        self.shape = [512., 512.]
-        self.origin = [255.5, 255.5]
-        self._last, self._inverse = None, None
-
-    def __reduce__(self):
-        return self.from_dict, (self.asdict(),)
-
-    def __repr__(self):
-        return self.asdict().__repr__()
-
-    def __str__(self):
-        return self.asdict().__str__()
-
-    @classmethod
-    def register(cls, fix, mov, kind=None):
-        """ kind: 'affine', 'translation', 'rigid' """
-        if sitk is None:
-            raise ImportError('SimpleElastix is not installed: '
-                              'https://simpleelastix.readthedocs.io/GettingStarted.html')
-        new = cls()
-        kind = kind or 'affine'
-        new.shape = fix.shape
-        fix, mov = new.cast_image(fix), new.cast_image(mov)
-        # TODO: implement RigidTransform
-        tfilter = sitk.ElastixImageFilter()
-        tfilter.LogToConsoleOff()
-        tfilter.SetFixedImage(fix)
-        tfilter.SetMovingImage(mov)
-        tfilter.SetParameterMap(sitk.GetDefaultParameterMap(kind))
-        tfilter.Execute()
-        transform = tfilter.GetTransformParameterMap()[0]
-        if kind == 'affine':
-            new.parameters = [float(t) for t in transform['TransformParameters']]
-            new.shape = [float(t) for t in transform['Size']]
-            new.origin = [float(t) for t in transform['CenterOfRotationPoint']]
-        elif kind == 'translation':
-            new.parameters = [1.0, 0.0, 0.0, 1.0] + [float(t) for t in transform['TransformParameters']]
-            new.shape = [float(t) for t in transform['Size']]
-            new.origin = [(t - 1) / 2 for t in new.shape]
-        else:
-            raise NotImplementedError(f'{kind} tranforms not implemented (yet)')
-        new.dparameters = 6 * [np.nan]
-        return new
-
-    @classmethod
-    def from_shift(cls, shift):
-        return cls.from_array(np.array(((1, 0, shift[0]), (0, 1, shift[1]), (0, 0, 1))))
-
-    @classmethod
-    def from_array(cls, array):
-        new = cls()
-        new.matrix = array
-        return new
-
-    @classmethod
-    def from_file(cls, file):
-        with open(Path(file).with_suffix('.yml')) as f:
-            return cls.from_dict(yamlload(f))
-
-    @classmethod
-    def from_dict(cls, d):
-        new = cls()
-        new.origin = [float(i) for i in d['CenterOfRotationPoint']]
-        new.parameters = [float(i) for i in d['TransformParameters']]
-        new.dparameters = [float(i) for i in d['dTransformParameters']] if 'dTransformParameters' in d else 6 * [np.nan]
-        new.shape = [float(i) for i in d['Size']]
-        return new
-
-    def __mul__(self, other):  # TODO: take care of dmatrix
-        result = self.copy()
-        if isinstance(other, Transform):
-            result.matrix = self.matrix @ other.matrix
-            result.dmatrix = self.dmatrix @ other.matrix + self.matrix @ other.dmatrix
-        else:
-            result.matrix = self.matrix @ other
-            result.dmatrix = self.dmatrix @ other
-        return result
-
-    def is_unity(self):
-        return self.parameters == [1, 0, 0, 1, 0, 0]
-
-    def copy(self):
-        return deepcopy(self)
-
-    @staticmethod
-    def cast_image(im):
-        if not isinstance(im, sitk.Image):
-            im = sitk.GetImageFromArray(np.asarray(im))
-        return im
-
-    @staticmethod
-    def cast_array(im):
-        if isinstance(im, sitk.Image):
-            im = sitk.GetArrayFromImage(im)
-        return im
-
-    @property
-    def matrix(self):
-        return np.array(((*self.parameters[:2], self.parameters[4]),
-                         (*self.parameters[2:4], self.parameters[5]),
-                         (0, 0, 1)))
-
-    @matrix.setter
-    def matrix(self, value):
-        value = np.asarray(value)
-        self.parameters = [*value[0, :2], *value[1, :2], *value[:2, 2]]
-
-    @property
-    def dmatrix(self):
-        return np.array(((*self.dparameters[:2], self.dparameters[4]),
-                         (*self.dparameters[2:4], self.dparameters[5]),
-                         (0, 0, 0)))
-
-    @dmatrix.setter
-    def dmatrix(self, value):
-        value = np.asarray(value)
-        self.dparameters = [*value[0, :2], *value[1, :2], *value[:2, 2]]
-
-    @property
-    def parameters(self):
-        if self.transform is not None:
-            return list(self.transform.GetParameters())
-
-    @parameters.setter
-    def parameters(self, value):
-        if self.transform is not None:
-            value = np.asarray(value)
-            self.transform.SetParameters(value.tolist())
-
-    @property
-    def origin(self):
-        if self.transform is not None:
-            return self.transform.GetFixedParameters()
-
-    @origin.setter
-    def origin(self, value):
-        if self.transform is not None:
-            value = np.asarray(value)
-            self.transform.SetFixedParameters(value.tolist())
-
-    @property
-    def inverse(self):
-        if self.is_unity():
-            return self
-        if self._last is None or self._last != self.asdict():
-            self._last = self.asdict()
-            self._inverse = Transform.from_dict(self.asdict())
-            self._inverse.transform = self._inverse.transform.GetInverse()
-            self._inverse._last = self._inverse.asdict()
-            self._inverse._inverse = self
-        return self._inverse
-
-    def adapt(self, origin, shape):
-        self.origin -= np.array(origin) + (self.shape - np.array(shape)[:2]) / 2
-        self.shape = shape[:2]
-
-    def asdict(self):
-        return {'CenterOfRotationPoint': self.origin, 'Size': self.shape, 'TransformParameters': self.parameters,
-                'dTransformParameters': np.nan_to_num(self.dparameters, nan=1e99).tolist()}
-
-    def frame(self, im, default=0):
-        if self.is_unity():
-            return im
-        else:
-            if sitk is None:
-                raise ImportError('SimpleElastix is not installed: '
-                                  'https://simpleelastix.readthedocs.io/GettingStarted.html')
-            dtype = im.dtype
-            im = im.astype('float')
-            intp = sitk.sitkBSpline if np.issubdtype(dtype, np.floating) else sitk.sitkNearestNeighbor
-            return self.cast_array(sitk.Resample(self.cast_image(im), self.transform, intp, default)).astype(dtype)
-
-    def coords(self, array, columns=None):
-        """ Transform coordinates in 2 column numpy array,
-            or in pandas DataFrame or Series objects in columns ['x', 'y']
-        """
-        if self.is_unity():
-            return array.copy()
-        elif DataFrame is not None and isinstance(array, (DataFrame, Series)):
-            columns = columns or ['x', 'y']
-            array = array.copy()
-            if isinstance(array, DataFrame):
-                array[columns] = self.coords(np.atleast_2d(array[columns].to_numpy()))
-            elif isinstance(array, Series):
-                array[columns] = self.coords(np.atleast_2d(array[columns].to_numpy()))[0]
-            return array
-        else:  # somehow we need to use the inverse here to get the same effect as when using self.frame
-            return np.array([self.inverse.transform.TransformPoint(i.tolist()) for i in np.asarray(array)])
-
-    def save(self, file):
-        """ save the parameters of the transform calculated
-            with affine_registration to a yaml file
-        """
-        if not file[-3:] == 'yml':
-            file += '.yml'
-        with open(file, 'w') as f:
-            yaml.safe_dump(self.asdict(), f, default_flow_style=None)
+import warnings
+from copy import deepcopy
+from pathlib import Path
+
+import numpy as np
+import yaml
+from parfor import Chunks, pmap
+from skimage import filters
+from tiffwrite import IJTiffFile
+from tqdm.auto import tqdm
+
+try:
+    # best if SimpleElastix is installed: https://simpleelastix.readthedocs.io/GettingStarted.html
+    import SimpleITK as sitk  # noqa
+except ImportError:
+    sitk = None
+
+try:
+    from pandas import DataFrame, Series, concat
+except ImportError:
+    DataFrame, Series, concat = None, None, None
+
+
+if hasattr(yaml, 'full_load'):
+    yamlload = yaml.full_load
+else:
+    yamlload = yaml.load
+
+
+class Transforms(dict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.default = Transform()
+
+    @classmethod
+    def from_file(cls, file, C=True, T=True):
+        with open(Path(file).with_suffix('.yml')) as f:
+            return cls.from_dict(yamlload(f), C, T)
+
+    @classmethod
+    def from_dict(cls, d, C=True, T=True):
+        new = cls()
+        for key, value in d.items():
+            if isinstance(key, str) and C:
+                new[key.replace(r'\:', ':').replace('\\\\', '\\')] = Transform.from_dict(value)
+            elif T:
+                new[key] = Transform.from_dict(value)
+        return new
+
+    @classmethod
+    def from_shifts(cls, shifts):
+        new = cls()
+        for key, shift in shifts.items():
+            new[key] = Transform.from_shift(shift)
+        return new
+
+    def __mul__(self, other):
+        new = Transforms()
+        if isinstance(other, Transforms):
+            for key0, value0 in self.items():
+                for key1, value1 in other.items():
+                    new[key0 + key1] = value0 * value1
+            return new
+        elif other is None:
+            return self
+        else:
+            for key in self.keys():
+                new[key] = self[key] * other
+            return new
+
+    def asdict(self):
+        return {key.replace('\\', '\\\\').replace(':', r'\:') if isinstance(key, str) else key: value.asdict()
+                for key, value in self.items()}
+
+    def __getitem__(self, item):
+        return np.prod([self[i] for i in item[::-1]]) if isinstance(item, tuple) else super().__getitem__(item)
+
+    def __missing__(self, key):
+        return self.default
+
+    def __getstate__(self):
+        return self.__dict__
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+
+    def __hash__(self):
+        return hash(frozenset((*self.__dict__.items(), *self.items())))
+
+    def save(self, file):
+        with open(Path(file).with_suffix('.yml'), 'w') as f:
+            yaml.safe_dump(self.asdict(), f, default_flow_style=None)
+
+    def copy(self):
+        return deepcopy(self)
+
+    def adapt(self, origin, shape, channel_names):
+        def key_map(a, b):
+            def fun(b, key_a):
+                for key_b in b:
+                    if key_b in key_a or key_a in key_b:
+                        return key_a, key_b
+
+            return {n[0]: n[1] for key_a in a if (n := fun(b, key_a))}
+
+        for value in self.values():
+            value.adapt(origin, shape)
+        self.default.adapt(origin, shape)
+        transform_channels = {key for key in self.keys() if isinstance(key, str)}
+        if set(channel_names) - transform_channels:
+            mapping = key_map(channel_names, transform_channels)
+            warnings.warn(f'The image file and the transform do not have the same channels,'
+                          f' creating a mapping: {mapping}')
+            for key_im, key_t in mapping.items():
+                self[key_im] = self[key_t]
+
+    @property
+    def inverse(self):
+        # TODO: check for C@T
+        inverse = self.copy()
+        for key, value in self.items():
+            inverse[key] = value.inverse
+        return inverse
+
+    def coords_pandas(self, array, channel_names, columns=None):
+        if isinstance(array, DataFrame):
+            return concat([self.coords_pandas(row, channel_names, columns) for _, row in array.iterrows()], axis=1).T
+        elif isinstance(array, Series):
+            key = []
+            if 'C' in array:
+                key.append(channel_names[int(array['C'])])
+            if 'T' in array:
+                key.append(int(array['T']))
+            return self[tuple(key)].coords(array, columns)
+        else:
+            raise TypeError('Not a pandas DataFrame or Series.')
+
+    def with_beads(self, cyllens, bead_files):
+        assert len(bead_files) > 0, 'At least one file is needed to calculate the registration.'
+        transforms = [self.calculate_channel_transforms(file, cyllens) for file in bead_files]
+        for key in {key for transform in transforms for key in transform.keys()}:
+            new_transforms = [transform[key] for transform in transforms if key in transform]
+            if len(new_transforms) == 1:
+                self[key] = new_transforms[0]
+            else:
+                self[key] = Transform()
+                self[key].parameters = np.mean([t.parameters for t in new_transforms], 0)
+                self[key].dparameters = (np.std([t.parameters for t in new_transforms], 0) /
+                                        np.sqrt(len(new_transforms))).tolist()
+        return self
+
+    @staticmethod
+    def get_bead_files(path):
+        from . import Imread
+        files = []
+        for file in path.iterdir():
+            if file.name.lower().startswith('beads'):
+                try:
+                    with Imread(file):
+                        files.append(file)
+                except Exception:
+                    pass
+        files = sorted(files)
+        if not files:
+            raise Exception('No bead file found!')
+        checked_files = []
+        for file in files:
+            try:
+                if file.is_dir():
+                    file /= 'Pos0'
+                with Imread(file):  # check for errors opening the file
+                    checked_files.append(file)
+            except (Exception,):
+                continue
+        if not checked_files:
+            raise Exception('No bead file found!')
+        return checked_files
+
+    @staticmethod
+    def calculate_channel_transforms(bead_file, cyllens):
+        """ When no channel is not transformed by a cylindrical lens, assume that the image is scaled by a factor 1.162
+            in the horizontal direction """
+        from . import Imread
+
+        with Imread(bead_file, axes='zcxy') as im:  # noqa
+            max_ims = im.max('z')
+            goodch = [c for c, max_im in enumerate(max_ims) if not im.is_noise(max_im)]
+            if not goodch:
+                goodch = list(range(len(max_ims)))
+            untransformed = [c for c in range(im.shape['c']) if cyllens[im.detector[c]].lower() == 'none']
+
+            good_and_untrans = sorted(set(goodch) & set(untransformed))
+            if good_and_untrans:
+                masterch = good_and_untrans[0]
+            else:
+                masterch = goodch[0]
+            transform = Transform()
+            if not good_and_untrans:
+                matrix = transform.matrix
+                matrix[0, 0] = 0.86
+                transform.matrix = matrix
+            transforms = Transforms()
+            for c in tqdm(goodch, desc='Calculating channel transforms'):  # noqa
+                if c == masterch:
+                    transforms[im.channel_names[c]] = transform
+                else:
+                    transforms[im.channel_names[c]] = Transform.register(max_ims[masterch], max_ims[c]) * transform
+        return transforms
+
+    @staticmethod
+    def save_channel_transform_tiff(bead_files, tiffile):
+        from . import Imread
+        n_channels = 0
+        for file in bead_files:
+            with Imread(file) as im:
+                n_channels = max(n_channels, im.shape['c'])
+        with IJTiffFile(tiffile, (n_channels, 1, len(bead_files))) as tif:
+            for t, file in enumerate(bead_files):
+                with Imread(file) as im:
+                    with Imread(file).with_transform() as jm:
+                        for c in range(im.shape['c']):
+                            tif.save(np.hstack((im(c=c, t=0).max('z'), jm(c=c, t=0).max('z'))), c, 0, t)
+
+    def with_drift(self, im):
+        """ Calculate shifts relative to the first frame
+            divide the sequence into groups,
+            compare each frame to the frame in the middle of the group and compare these middle frames to each other
+        """
+        im = im.transpose('tzycx')
+        t_groups = [list(chunk) for chunk in Chunks(range(im.shape['t']), size=round(np.sqrt(im.shape['t'])))]
+        t_keys = [int(np.round(np.mean(t_group))) for t_group in t_groups]
+        t_pairs = [(int(np.round(np.mean(t_group))), frame) for t_group in t_groups for frame in t_group]
+        t_pairs.extend(zip(t_keys, t_keys[1:]))
+        fmaxz_keys = {t_key: filters.gaussian(im[t_key].max('z'), 5) for t_key in t_keys}
+
+        def fun(t_key_t, im, fmaxz_keys):
+            t_key, t = t_key_t
+            if t_key == t:
+                return 0, 0
+            else:
+                fmaxz = filters.gaussian(im[t].max('z'), 5)
+                return Transform.register(fmaxz_keys[t_key], fmaxz, 'translation').parameters[4:]
+
+        shifts = np.array(pmap(fun, t_pairs, (im, fmaxz_keys), desc='Calculating image shifts.'))
+        shift_keys_cum = np.zeros(2)
+        for shift_keys, t_group in zip(np.vstack((-shifts[0], shifts[im.shape['t']:])), t_groups):
+            shift_keys_cum += shift_keys
+            shifts[t_group] += shift_keys_cum
+
+        for i, shift in enumerate(shifts[:im.shape['t']]):
+            self[i] = Transform.from_shift(shift)
+        return self
+
+
+class Transform:
+    def __init__(self):
+        if sitk is None:
+            self.transform = None
+        else:
+            self.transform = sitk.ReadTransform(str(Path(__file__).parent / 'transform.txt'))
+        self.dparameters = [0., 0., 0., 0., 0., 0.]
+        self.shape = [512., 512.]
+        self.origin = [255.5, 255.5]
+        self._last, self._inverse = None, None
+
+    def __reduce__(self):
+        return self.from_dict, (self.asdict(),)
+
+    def __repr__(self):
+        return self.asdict().__repr__()
+
+    def __str__(self):
+        return self.asdict().__str__()
+
+    @classmethod
+    def register(cls, fix, mov, kind=None):
+        """ kind: 'affine', 'translation', 'rigid' """
+        if sitk is None:
+            raise ImportError('SimpleElastix is not installed: '
+                              'https://simpleelastix.readthedocs.io/GettingStarted.html')
+        new = cls()
+        kind = kind or 'affine'
+        new.shape = fix.shape
+        fix, mov = new.cast_image(fix), new.cast_image(mov)
+        # TODO: implement RigidTransform
+        tfilter = sitk.ElastixImageFilter()
+        tfilter.LogToConsoleOff()
+        tfilter.SetFixedImage(fix)
+        tfilter.SetMovingImage(mov)
+        tfilter.SetParameterMap(sitk.GetDefaultParameterMap(kind))
+        tfilter.Execute()
+        transform = tfilter.GetTransformParameterMap()[0]
+        if kind == 'affine':
+            new.parameters = [float(t) for t in transform['TransformParameters']]
+            new.shape = [float(t) for t in transform['Size']]
+            new.origin = [float(t) for t in transform['CenterOfRotationPoint']]
+        elif kind == 'translation':
+            new.parameters = [1.0, 0.0, 0.0, 1.0] + [float(t) for t in transform['TransformParameters']]
+            new.shape = [float(t) for t in transform['Size']]
+            new.origin = [(t - 1) / 2 for t in new.shape]
+        else:
+            raise NotImplementedError(f'{kind} tranforms not implemented (yet)')
+        new.dparameters = 6 * [np.nan]
+        return new
+
+    @classmethod
+    def from_shift(cls, shift):
+        return cls.from_array(np.array(((1, 0, shift[0]), (0, 1, shift[1]), (0, 0, 1))))
+
+    @classmethod
+    def from_array(cls, array):
+        new = cls()
+        new.matrix = array
+        return new
+
+    @classmethod
+    def from_file(cls, file):
+        with open(Path(file).with_suffix('.yml')) as f:
+            return cls.from_dict(yamlload(f))
+
+    @classmethod
+    def from_dict(cls, d):
+        new = cls()
+        new.origin = [float(i) for i in d['CenterOfRotationPoint']]
+        new.parameters = [float(i) for i in d['TransformParameters']]
+        new.dparameters = [float(i) for i in d['dTransformParameters']] if 'dTransformParameters' in d else 6 * [np.nan]
+        new.shape = [float(i) for i in d['Size']]
+        return new
+
+    def __mul__(self, other):  # TODO: take care of dmatrix
+        result = self.copy()
+        if isinstance(other, Transform):
+            result.matrix = self.matrix @ other.matrix
+            result.dmatrix = self.dmatrix @ other.matrix + self.matrix @ other.dmatrix
+        else:
+            result.matrix = self.matrix @ other
+            result.dmatrix = self.dmatrix @ other
+        return result
+
+    def is_unity(self):
+        return self.parameters == [1, 0, 0, 1, 0, 0]
+
+    def copy(self):
+        return deepcopy(self)
+
+    @staticmethod
+    def cast_image(im):
+        if not isinstance(im, sitk.Image):
+            im = sitk.GetImageFromArray(np.asarray(im))
+        return im
+
+    @staticmethod
+    def cast_array(im):
+        if isinstance(im, sitk.Image):
+            im = sitk.GetArrayFromImage(im)
+        return im
+
+    @property
+    def matrix(self):
+        return np.array(((*self.parameters[:2], self.parameters[4]),
+                         (*self.parameters[2:4], self.parameters[5]),
+                         (0, 0, 1)))
+
+    @matrix.setter
+    def matrix(self, value):
+        value = np.asarray(value)
+        self.parameters = [*value[0, :2], *value[1, :2], *value[:2, 2]]
+
+    @property
+    def dmatrix(self):
+        return np.array(((*self.dparameters[:2], self.dparameters[4]),
+                         (*self.dparameters[2:4], self.dparameters[5]),
+                         (0, 0, 0)))
+
+    @dmatrix.setter
+    def dmatrix(self, value):
+        value = np.asarray(value)
+        self.dparameters = [*value[0, :2], *value[1, :2], *value[:2, 2]]
+
+    @property
+    def parameters(self):
+        if self.transform is not None:
+            return list(self.transform.GetParameters())
+
+    @parameters.setter
+    def parameters(self, value):
+        if self.transform is not None:
+            value = np.asarray(value)
+            self.transform.SetParameters(value.tolist())
+
+    @property
+    def origin(self):
+        if self.transform is not None:
+            return self.transform.GetFixedParameters()
+
+    @origin.setter
+    def origin(self, value):
+        if self.transform is not None:
+            value = np.asarray(value)
+            self.transform.SetFixedParameters(value.tolist())
+
+    @property
+    def inverse(self):
+        if self.is_unity():
+            return self
+        if self._last is None or self._last != self.asdict():
+            self._last = self.asdict()
+            self._inverse = Transform.from_dict(self.asdict())
+            self._inverse.transform = self._inverse.transform.GetInverse()
+            self._inverse._last = self._inverse.asdict()
+            self._inverse._inverse = self
+        return self._inverse
+
+    def adapt(self, origin, shape):
+        self.origin -= np.array(origin) + (self.shape - np.array(shape)[:2]) / 2
+        self.shape = shape[:2]
+
+    def asdict(self):
+        return {'CenterOfRotationPoint': self.origin, 'Size': self.shape, 'TransformParameters': self.parameters,
+                'dTransformParameters': np.nan_to_num(self.dparameters, nan=1e99).tolist()}
+
+    def frame(self, im, default=0):
+        if self.is_unity():
+            return im
+        else:
+            if sitk is None:
+                raise ImportError('SimpleElastix is not installed: '
+                                  'https://simpleelastix.readthedocs.io/GettingStarted.html')
+            dtype = im.dtype
+            im = im.astype('float')
+            intp = sitk.sitkBSpline if np.issubdtype(dtype, np.floating) else sitk.sitkNearestNeighbor
+            return self.cast_array(sitk.Resample(self.cast_image(im), self.transform, intp, default)).astype(dtype)
+
+    def coords(self, array, columns=None):
+        """ Transform coordinates in 2 column numpy array,
+            or in pandas DataFrame or Series objects in columns ['x', 'y']
+        """
+        if self.is_unity():
+            return array.copy()
+        elif DataFrame is not None and isinstance(array, (DataFrame, Series)):
+            columns = columns or ['x', 'y']
+            array = array.copy()
+            if isinstance(array, DataFrame):
+                array[columns] = self.coords(np.atleast_2d(array[columns].to_numpy()))
+            elif isinstance(array, Series):
+                array[columns] = self.coords(np.atleast_2d(array[columns].to_numpy()))[0]
+            return array
+        else:  # somehow we need to use the inverse here to get the same effect as when using self.frame
+            return np.array([self.inverse.transform.TransformPoint(i.tolist()) for i in np.asarray(array)])
+
+    def save(self, file):
+        """ save the parameters of the transform calculated
+            with affine_registration to a yaml file
+        """
+        if not file[-3:] == 'yml':
+            file += '.yml'
+        with open(file, 'w') as f:
+            yaml.safe_dump(self.asdict(), f, default_flow_style=None)
```

### Comparing `ndbioimage-2024.3.7/pyproject.toml` & `ndbioimage-2024.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.3.7"
+version = "2024.4.0"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.3.7/PKG-INFO` & `ndbioimage-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.3.7
+Version: 2024.4.0
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
```

