# Comparing `tmp/fabsync-1.1.0.tar.gz` & `tmp/fabsync-1.2.0.tar.gz`

## Comparing `fabsync-1.1.0.tar` & `fabsync-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,71 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fabsync-1.1.0/.coveragerc
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fabsync-1.1.0/.flake8
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fabsync-1.1.0/.hgtags
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/make.bat
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/source/conf.py
--rw-r--r--   0        0        0    20355 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/source/index.rst
--rw-r--r--   0        0        0    12526 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/__init__.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/config.py
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/files.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/fs.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/functools.py
--rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/md5.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_config.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_files.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_functools.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/absent/.keepme
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/complete/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/empty/_sync.toml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/schema_error/_sync.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/tags/_sync.toml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/tags2/_sync.toml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/toml_error/_sync.toml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/vars/_sync.toml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/_sync.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-profile
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/file1.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/file2.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/_sync.toml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/ignore-me.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-config/_sync.toml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-config/sync.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/ignore-me/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/ignore-me/file.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/etc/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/etc/pf.conf
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/usr/local/bin/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/usr/local/bin/myapp.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/var/myapp/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/empty/tmp/_sync.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/group/home/hg/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/mode/var
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/mode/etc/_sync.toml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/render/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/render/file.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/user/home/hg/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/etc/pf.conf
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/_sync.toml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/dot-hgrc
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/_sync.toml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/blob
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/hook.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fabsync-1.1.0/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fabsync-1.1.0/.hgignore
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 fabsync-1.1.0/README.md
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fabsync-1.1.0/UNLICENSE
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 fabsync-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 fabsync-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fabsync-1.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fabsync-1.2.0/.coveragerc
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fabsync-1.2.0/.flake8
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fabsync-1.2.0/.hgtags
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 fabsync-1.2.0/CHANGES.rst
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fabsync-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fabsync-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.2.0/docs/source/changes.rst
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fabsync-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0    22149 2020-02-02 00:00:00.000000 fabsync-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/__init__.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/config.py
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/files.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/fs.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/functools.py
+-rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/md5.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/src/fabsync/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/test_files.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/test_functools.py
+-rw-r--r--   0        0        0    12540 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/test_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/absent/.keepme
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/complete/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/empty/_sync.toml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/schema_error/_sync.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/tags/_sync.toml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/tags2/_sync.toml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/toml_error/_sync.toml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/config/vars/_sync.toml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/_sync.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dot-profile
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/file1.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/file2.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dir1/_sync.toml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dir1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dir1/ignore-me.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dot-config/_sync.toml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/dot-config/sync.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/ignore-me/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/loading/ignore-me/file.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/selection/etc/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/selection/etc/pf.conf
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/selection/usr/local/bin/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/selection/usr/local/bin/myapp.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/files/selection/var/myapp/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/empty/tmp/_sync.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/group/home/hg/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/mode/var
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/mode/etc/_sync.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/_sync.toml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/bad_module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/builtin.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/missing.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/render/no_render.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/errors/user/home/hg/_sync.toml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/etc/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/etc/pf.conf
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/etc/rc.conf.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/home/hg/_sync.toml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/home/hg/dot-hgrc
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/home/hg/bin/_sync.toml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/home/hg/bin/blob
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fabsync-1.2.0/tests/sync/general/home/hg/bin/hook.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fabsync-1.2.0/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fabsync-1.2.0/.hgignore
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 fabsync-1.2.0/README.md
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fabsync-1.2.0/UNLICENSE
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 fabsync-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 fabsync-1.2.0/PKG-INFO
```

### Comparing `fabsync-1.1.0/docs/Makefile` & `fabsync-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/docs/make.bat` & `fabsync-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/docs/source/conf.py` & `fabsync-1.2.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'fabsync'
 project_copyright = "2022, Peter Sagerson"
 author = "Peter Sagerson"
 
 # The full version, including alpha/beta/rc tags
-release = '1.1.0'
+release = '1.2.0'
 version = '.'.join(release.split('.')[:2])
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `fabsync-1.1.0/docs/source/index.rst` & `fabsync-1.2.0/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -279,27 +279,32 @@
 file can be configured with a renderer, which is simply a function that takes
 the :class:`~pathlib.Path` of the source file plus any configured render vars
 and returns a new :class:`str` or :class:`bytes` with the final contents. The
 default (trivial) renderer looks like this:
 
 .. code-block:: python
 
-   def renderer(path: Path, _vars: Mapping[str, Any]) -> bytes:
+   def renderer(path: Path, _vars: Mapping[str, Any], **kwargs) -> bytes:
        with path.open('rb') as f:
            return f.read()
 
 Custom renderers can be hooked up to a template engine, Python string
 formatting, or any other transformation that you want. If a string is returned,
 it will be encoded as utf-8 for uploading.
 
+Note that all renderers should include ``**kwargs`` in their argument list for
+forward compatibility. As of version 1.2, legacy renderers with just the two
+positional arguments are supported with a deprecation warning.
+
 In :ref:`sync-toml`, the renderer is specified as an arbitrary string. At sync
 time, you need to provide a mapping from these strings to the functions that
-implement them. The ``renderer`` key is valid for individual files and also in
-the ``[defaults]`` section. You can also supply a mapping of arbitrary values
-for the render function.
+implement them. (Renderer names beginning with ``'fabsync/'`` are reserved and
+can not be registered). The ``renderer`` key is valid for individual files and
+also in the ``[defaults]`` section. You can also supply a mapping of arbitrary
+values to parameterize the render function.
 
 .. code-block:: text
 
    .
    ├── files
    │   └── etc
    │       ├── _sync.toml
@@ -309,14 +314,17 @@
 .. code-block:: toml
    :caption: files/etc/_sync.toml
 
    [files.'aliases']
    renderer = 'mako'
    vars = {'postmaster': 'alice@example.com'}
 
+Individual vars can be overidden at each configuration level. Values are not
+merged recursively.
+
 It's likely that you'll want to load a render context once at the beginning of
 the sync operation and reuse it for each file. Here's an example of what this
 might look like:
 
 .. code-block:: python
    :caption: fabfile.py
 
@@ -325,33 +333,70 @@
    import tomli
    from typing import Mapping, Any
    from fabric import task
    from mako.template import Template
    import fabsync
 
    def mako_renderer(conn):
+       # Load some host-specific template context.
        result = conn.get('/usr/local/etc/fabsync.toml', io.BytesIO())
        host = tomli.loads(result.local.getvalue().decode())
 
-       def render(path: Path, vars: Mapping[str, Any]) -> str:
+       def render(path: Path, vars: Mapping[str, Any], **kwargs) -> str:
            return Template(filename=str(path)).render(host | vars)
 
        return render
 
    @task(iterable=['tag'])
    def sync(conn, subpath=None, tag=(), dry_run=False):
        root = fabsync.load('files', '/')
        selector = fabsync.ItemSelector.new(subpath, tag)
        renderers = {'mako': mako_renderer(conn)}
 
        for result in fabsync.isync(conn, root, selector, renderers, dry_run=dry_run):
            print(f"{result.path}{' [modified]' if result.modified else ''}")
 
-To-level vars can be overidden at each level. The dicts are not merged recursively.
 
+Advanced Rendering
+~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 1.2
+
+Render functions are given one additional keyword argument: ``get_content``.
+This is a thunk (a zero-argument function) that will return the current (remote)
+content of the file as a ``bytes`` object. This can be used by renderers that
+wish to inspect and modify an existing file rather than simply create/overwrite
+it. In this case, the source file could contain information you wish to merge
+into the target or it might simply be an empty placeholder file to trigger the
+renderer.
+
+As a convenience, there is a special builtin renderer called ``fabsync/py`` that
+will load a source file as a Python module, look for a function named
+``render``, and call it as the render function. For example:
+
+.. code-block:: toml
+   :caption: _sync.toml
+
+   [files.'rc.conf.py']
+   name = 'rc.conf'
+   renderer = 'fabsync/py'
+
+.. code-block:: python
+   :caption: rc.conf.py
+
+   import re
+
+   def render(_src, _vars, get_content, **kwargs) -> bytes:
+       content = get_content()
+
+       content = re.sub(rb'^pf_enable=.*$', b'pf_enable="YES"', content, flags=re.M)
+       content = re.sub(rb'^jail_enable=.*$', b'jail_enable="YES"', content, flags=re.M)
+       content = re.sub(rb'^sendmail_enable=.*$', b'sendmail_enable="NO"', content, flags=re.M)
+
+       return content
 
 Diffs
 -----
 
 By default, any time we decide to upload a file, we generate a diff of the
 original and uploaded content. This is included in the
 :class:`~fabsync.SyncResult` objected returned by :func:`~fabsync.isync`. This
@@ -698,7 +743,16 @@
    group = -1
    dir_perms = -1
    file_perms = -1
    tags = ['tag2']
    renderer = ''
    vars = {}
    diff = true
+
+
+Change log
+----------
+
+.. toctree::
+   :maxdepth: 1
+
+   changes
```

### Comparing `fabsync-1.1.0/src/fabsync/__init__.py` & `fabsync-1.2.0/src/fabsync/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 import difflib
 from functools import cached_property, singledispatchmethod
 import hashlib
+import importlib.util
+import inspect
 import io
 import os
 from pathlib import Path, PurePath
 import stat
 from typing import Callable, Generator, Mapping, Optional, Union
+import warnings
 
-from .config import RenderVars
 from .files import (
     ItemSelector,
     load,
     select,
     SyncedDir,
     SyncedFile,
     SyncedItem,
     SyncedRoot,
 )
 from .fs import FS, new_fs, SysInfo
 
 
-Renderer = Callable[[Path, RenderVars], Union[str, bytes]]
+Renderer = Callable[..., Union[str, bytes]]
 Renderers = Mapping[str, Renderer]
 
 
 __all__ = ['ItemSelector', 'load', 'isync', 'sync', 'SyncError']
 
 
 class SyncError(Exception):
@@ -208,36 +210,90 @@
             pass
 
         return content.getvalue()
 
     @cached_property
     def content(self) -> bytes:
         """The expected content of the file (after rendering)."""
+        renderer: Renderer
+
         file = self.file
 
-        if key := file.opts.renderer:
-            try:
-                renderer = self.renderers[key]
-            except KeyError as e:
-                raise SyncError(f"Renderer {key} is not configured.") from e
-        else:
+        key = file.opts.renderer
+        if not key:
             renderer = self._read_file
+        elif key == 'fabsync/py':
+            renderer = self._render_py
+        elif key.startswith('fabsync/'):
+            raise SyncError(f"Renderer {key} is not defined.")
+        elif key in self.renderers:
+            renderer = self.renderers[key]
+        else:
+            raise SyncError(f"Renderer {key} is not configured.")
+
+        if self._is_legacy_renderer(renderer):
+            warnings.warn(
+                f"Two-argument render functions are deprecated ({renderer.__module__}.{renderer.__qualname__}). Hint: add **kwargs.",
+                DeprecationWarning,
+                stacklevel=1,
+            )
+            content = renderer(file.src, file.opts.vars)
+        else:
+            content = renderer(
+                file.src, file.opts.vars, get_content=lambda: self.remote_content
+            )
 
-        content = renderer(file.src, file.opts.vars)
         if isinstance(content, str):
             content = content.encode()
 
         return content
 
-    def _read_file(self, src: Path, _vars: RenderVars) -> bytes:
+    @staticmethod
+    def _read_file(src: Path, _vars, **kwargs) -> bytes:
         with src.open('rb') as f:
             content = f.read()
 
         return content
 
+    @staticmethod
+    def _render_py(
+        src: Path, vars, get_content: Callable[[], bytes], **kwargs
+    ) -> bytes:
+        content: bytes
+
+        if (
+            spec := importlib.util.spec_from_file_location('renderer', src)
+        ) and spec.loader:
+            mod = importlib.util.module_from_spec(spec)
+            try:
+                spec.loader.exec_module(mod)
+            except SyntaxError as e:
+                raise SyncError(f"Failed to load {src} as a python module.") from e
+
+            if hasattr(mod, 'render'):
+                content = mod.render(src, vars, get_content=get_content)
+            else:
+                raise SyncError(f"{src} has no 'render' function.")
+        else:  # pragma: no cover
+            # This should be unreachable.
+            raise SyncError(f"Failed to load {src} as a python module.")
+
+        return content
+
+    @staticmethod
+    def _is_legacy_renderer(func: Callable) -> bool:
+        param_kinds = tuple(
+            param.kind for param in inspect.signature(func).parameters.values()
+        )
+
+        return param_kinds == (
+            inspect.Parameter.POSITIONAL_OR_KEYWORD,
+            inspect.Parameter.POSITIONAL_OR_KEYWORD,
+        )
+
     def reset(self) -> None:
         super().reset()
 
         if 'md5' in self.__dict__:
             del self.md5
 
         if 'remote_content' in self.__dict__:
```

### Comparing `fabsync-1.1.0/src/fabsync/config.py` & `fabsync-1.2.0/src/fabsync/config.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/src/fabsync/files.py` & `fabsync-1.2.0/src/fabsync/files.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/src/fabsync/fs.py` & `fabsync-1.2.0/src/fabsync/fs.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/src/fabsync/functools.py` & `fabsync-1.2.0/src/fabsync/functools.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/tests/test_config.py` & `fabsync-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/tests/test_files.py` & `fabsync-1.2.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/tests/test_functools.py` & `fabsync-1.2.0/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/tests/test_sync.py` & `fabsync-1.2.0/tests/test_sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
-from functools import cached_property, partial
+from functools import cached_property
 import io
 import os
 from pathlib import Path, PurePath
 import shlex
 import shutil
 import subprocess
 from tempfile import TemporaryDirectory
 from typing import Mapping, Tuple, Union
 from unittest import TestCase
 from unittest.mock import patch
+import warnings
 
 import invoke
 
 import fabsync
 from fabsync import ItemSelector, Syncer, SyncError
 from fabsync.fs import SysInfo
 
@@ -33,16 +34,16 @@
     pass
 
 
 class TestRemoteFS(TestFSMixin, fabsync.fs.RemoteFS):
     pass
 
 
-def slurp(file, vars, **kwargs):
-    with open(file, **kwargs) as f:
+def slurp(path, vars, **kwargs):
+    with path.open(mode='rb') as f:
         return f.read()
 
 
 class SyncTestCase(TestCase):
     """
     Base class for sync tests.
 
@@ -78,15 +79,15 @@
         return self.local_path
 
     def _new_connection(self):
         return invoke.Context()
 
     def sync(self, selector=None, renderers=None, dry_run=False):
         if renderers is None:
-            renderers = {'test': partial(slurp, mode='rb')}
+            renderers = {'test': slurp}
 
         return fabsync.sync(
             self.conn,
             self.root,
             selector,
             renderers,
             dry_run=dry_run,
@@ -108,15 +109,34 @@
 
 
 class MissingRenderer(SyncTestCase):
     root_name = 'errors/render'
 
     def test_renderer_missing(self):
         with self.assertRaises(SyncError):
-            self.sync()
+            self.sync(selector=ItemSelector.new(subpath='missing.txt'))
+
+    def test_builtin_renderer_missing(self):
+        """
+        Renderers with the 'fabsync/' prefix are reserved and may not be
+        defined.
+        """
+        with self.assertRaises(SyncError):
+            self.sync(
+                selector=ItemSelector.new(subpath='builtin.txt'),
+                renderers={'fabsync/custom': lambda p, v: b''},
+            )
+
+    def test_bad_module(self):
+        with self.assertRaises(SyncError):
+            self.sync(selector=ItemSelector.new(subpath='bad_module.py'))
+
+    def test_no_render_function(self):
+        with self.assertRaises(SyncError):
+            self.sync(selector=ItemSelector.new(subpath='no_render.py'))
 
 
 class ModeMismatch(SyncTestCase):
     root_name = 'errors/mode'
 
     def test_dir_over_file(self):
         (self.local_path / 'etc').touch()
@@ -199,26 +219,43 @@
         self.assertNotEqual(result.diff, b'')
         self.assertEqual(
             (self.local_path / 'home/hg/bin/hook.sh').read_text(),
             (self.root.src / 'home/hg/bin/hook.sh').read_text(),
         )
 
     def test_sync_noop(self):
-        selector = ItemSelector(subpath=PurePath('etc'))
+        selector = ItemSelector.new(subpath=PurePath('etc'))
         results = self.sync(selector=selector)
         results = self.sync(selector=selector)
 
         for result in results.values():
             with self.subTest(result.path):
                 self.assertFalse(result.created)
                 self.assertFalse(result.modified)
                 self.assertEqual(result.diff, b'')
 
+    def test_sync_py(self):
+        dest_path = self.local_path / 'etc/rc.conf'
+        dest_path.parent.mkdir(parents=True, exist_ok=True)
+        with open(dest_path, 'wt') as f:
+            f.write('hostname="test"\npf_enable="NO"\njail_enable="YES"\n')
+
+        results = self.sync()
+
+        result = results[self.dest / 'etc/rc.conf']
+        self.assertFalse(result.created)
+        self.assertTrue(result.modified)
+        self.assertNotEqual(result.diff, b'')
+        self.assertEqual(
+            dest_path.read_text(),
+            'hostname="test"\npf_enable="YES"\njail_enable="YES"\n',
+        )
+
     def test_content_check(self):
-        def upper(path: Path, vars: Mapping) -> str:
+        def upper(path: Path, _vars: Mapping, **kwargs) -> str:
             with path.open('rt') as f:
                 return f.read().upper()
 
         self.sync()
         results = self.sync(renderers={'test': upper})
 
         result = results[self.dest / 'home/hg/.hgrc']
@@ -234,14 +271,24 @@
         with Syncer(self.conn, {}) as syncer:
             file = next(item for item in fabsync.files.walk(self.root) if item.is_file)
             item_syncer = syncer._item_syncer(file)
             content = item_syncer.remote_content
 
         self.assertEqual(content, b'')
 
+    def test_deprecated_render_function(self):
+        def renderer(path: Path, _vars: Mapping) -> bytes:
+            with path.open('rb') as f:
+                return f.read()
+
+        with warnings.catch_warnings(record=True) as warns:
+            self.sync(renderers={'test': renderer})
+            self.assertEqual(len(warns), 1)
+            self.assertEqual(warns[0].category, DeprecationWarning)
+
 
 @patch('fabsync.fs.LocalFS', TestLocalFS)
 class Local(GeneralTests, SyncTestCase):
     """
     General tests using fabsync.fs.LocalFS.
     """
```

### Comparing `fabsync-1.1.0/README.md` & `fabsync-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/UNLICENSE` & `fabsync-1.2.0/UNLICENSE`

 * *Files identical despite different names*

### Comparing `fabsync-1.1.0/pyproject.toml` & `fabsync-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'fabsync'
-version = '1.1.0'
+version = '1.2.0'
 description = "File syncing via Fabric."
 keywords = ['fabric']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: The Unlicense (Unlicense)',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
@@ -34,14 +34,15 @@
 packages = ['src/fabsync']
 
 # The default environment is for general development.
 [tool.hatch.envs.default]
 python = '3.8'
 dependencies = [
     'black',
+    'bumpversion',
     'coverage~=6.3',
     'flake8-bugbear',
     'flake8~=5.0',
     'isort~=5.0',
     'mypy',
     'types-invoke',
     'types-jsonschema',
@@ -80,16 +81,16 @@
 dependencies = [
     # TEMP: Work around https://github.com/fabric/fabric/issues/2263
     'invoke<2.1',
     'sphinx~=4.5',
 ]
 
 [tool.hatch.envs.docs.scripts]
-make = 'make -C docs html'
-gmake = 'gmake -C docs html'
+make = 'command make -C docs html'
+gmake = 'command gmake -C docs html'
 open = 'xdg-open docs/build/html/index.html'
 
 
 # The test environment just defines a test matrix. The test scripts are all
 # inherited from default.
 [tool.hatch.envs.test]
 dependencies = [
```

### Comparing `fabsync-1.1.0/PKG-INFO` & `fabsync-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabsync
-Version: 1.1.0
+Version: 1.2.0
 Summary: File syncing via Fabric.
 Project-URL: Homepage, https://sr.ht/~psagers/fabsync/
 Project-URL: Source code, https://hg.sr.ht/~psagers/fabsync
 Project-URL: Documentation, https://fabsync.ignorare.net/
 Author-email: Peter Sagerson <psagers@ignorare.net>
 License-Expression: Unlicense
 License-File: UNLICENSE
```

