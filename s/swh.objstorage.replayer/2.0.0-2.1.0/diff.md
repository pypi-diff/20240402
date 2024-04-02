# Comparing `tmp/swh.objstorage.replayer-2.0.0.tar.gz` & `tmp/swh.objstorage.replayer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.objstorage.replayer-2.0.0.tar", last modified: Thu Jan  4 14:33:20 2024, max compression
+gzip compressed data, was "swh.objstorage.replayer-2.1.0.tar", last modified: Tue Apr  2 09:37:09 2024, max compression
```

## Comparing `swh.objstorage.replayer-2.0.0.tar` & `swh.objstorage.replayer-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.239245 swh.objstorage.replayer-2.0.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      389 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      943 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1700 2024-01-04 14:33:20.239245 swh.objstorage.replayer-2.0.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.231245 swh.objstorage.replayer-2.0.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.231245 swh.objstorage.replayer-2.0.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.231245 swh.objstorage.replayer-2.0.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      182 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2692 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      543 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2139 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       97 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      249 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-01-04 14:33:20.239245 swh.objstorage.replayer-2.0.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.223245 swh.objstorage.replayer-2.0.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.223245 swh.objstorage.replayer-2.0.0/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.235245 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7423 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15653 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/replay.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.239245 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25021 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3313 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_replay.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11025 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_replay_errors.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4099 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_statsd.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-01-04 14:33:20.239245 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1700 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1028 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-01-04 14:33:20.000000 swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1454 2024-01-04 14:33:13.000000 swh.objstorage.replayer-2.0.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.193183 swh.objstorage.replayer-2.1.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      389 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1705 2024-04-02 09:37:09.193183 swh.objstorage.replayer-2.1.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.185183 swh.objstorage.replayer-2.1.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.185183 swh.objstorage.replayer-2.1.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.185183 swh.objstorage.replayer-2.1.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      182 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2692 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      543 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2139 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       70 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      249 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-02 09:37:09.193183 swh.objstorage.replayer-2.1.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.177183 swh.objstorage.replayer-2.1.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.181183 swh.objstorage.replayer-2.1.0/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.189183 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7760 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18686 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/replay.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.189183 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28045 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3371 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_replay.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11536 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_replay_errors.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4099 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_statsd.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 09:37:09.189183 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1705 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1028 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       76 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      164 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-02 09:37:09.000000 swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1184 2024-04-02 09:37:03.000000 swh.objstorage.replayer-2.1.0/tox.ini
```

### Comparing `swh.objstorage.replayer-2.0.0/CODE_OF_CONDUCT.md` & `swh.objstorage.replayer-2.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/LICENSE` & `swh.objstorage.replayer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/PKG-INFO` & `swh.objstorage.replayer-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage.replayer
-Version: 2.0.0
+Version: 2.1.0
 Summary: Software Heritage content replayer
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage-replayer/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer.git
@@ -20,15 +20,15 @@
 Requires-Dist: humanize
 Requires-Dist: redis
 Requires-Dist: tenacity
 Requires-Dist: swh.core[http]>=0.3
 Requires-Dist: swh.objstorage>=2.3.1
 Requires-Dist: swh.journal>=0.4.2
 Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: swh.core[testing]; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
 
 Software Heritage - Object storage replayer
 ===========================================
```

### Comparing `swh.objstorage.replayer-2.0.0/docs/index.rst` & `swh.objstorage.replayer-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/mypy.ini` & `swh.objstorage.replayer-2.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/pyproject.toml` & `swh.objstorage.replayer-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/cli.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,41 @@
     "--size-limit",
     default=0,
     type=int,
     help="Exclude files which size is over this limit. 0 (default) means no size limit.",
 )
 @click.option(
     "--check-dst/--no-check-dst",
+    is_flag=True,
     default=True,
     help="Check whether the destination contains the object before copying.",
 )
 @click.option(
+    "--check-src-hashes",
+    is_flag=True,
+    default=False,
+    help="Check objects in flight.",
+)
+@click.option(
     "--concurrency",
     default=4,
     help=(
         "Number of concurrent threads doing the actual copy of blobs between "
         "the source and destination objstorages."
     ),
 )
 @click.pass_context
 def content_replay(
-    ctx, stop_after_objects, exclude_sha1_file, size_limit, check_dst, concurrency
+    ctx,
+    stop_after_objects,
+    exclude_sha1_file,
+    size_limit,
+    check_dst,
+    check_src_hashes,
+    concurrency,
 ) -> None:
     """Fill a destination Object Storage using a journal stream.
 
     This is typically used for a mirror configuration, by reading a Journal
     and retrieving objects from an existing source ObjStorage.
 
     There can be several 'replayers' filling a given ObjStorage as long as they
@@ -78,14 +91,17 @@
     ``--size-limit`` exclude file content which size is (strictly) above
     the given size limit. If 0, then there is no size limit.
 
     ``--check-dst`` sets whether the replayer should check in the destination
     ObjStorage before copying an object. You can turn that off if you know
     you're copying to an empty ObjStorage.
 
+    ``--check-src-hashes`` computes the hashes of the fetched object before
+    sending it to the destination.
+
     ``--concurrency N`` sets the number of threads in charge of copy blob objects
     from the source objstorage to the destination one. Using a large concurrency
     value make sense if both the source and destination objstorages support highly
     parallel workloads. Make not to set the ``batch_size`` configuration option too
     low for the concurrency to be actually useful (each batch of kafka messages is
     dispatched among the threads).
 
@@ -191,14 +207,15 @@
     )
     try:
         with ContentReplayer(
             src=objstorage_src_cfg,
             dst=objstorage_dst_cfg,
             exclude_fn=exclude_fn,
             check_dst=check_dst,
+            check_src_hashes=check_src_hashes,
             concurrency=concurrency,
         ) as replayer:
             if notify:
                 notify("READY=1")
             client.process(replayer.replay)
     except KeyboardInterrupt:
         ctx.exit(0)
```

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/replay.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/replay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright (C) 2019-2023 The Software Heritage developers
+# Copyright (C) 2019-2024 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import logging
 from queue import Empty, Queue
 import sys
 from threading import Event, Thread
 from time import time
 from traceback import format_tb
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from humanize import naturaldelta, naturalsize
 import msgpack
-from sentry_sdk import capture_exception, push_scope
+import sentry_sdk
 
 from swh.objstorage.interface import (
     CompositeObjId,
     ObjStorageInterface,
     objid_from_dict,
 )
 
@@ -32,15 +32,15 @@
     retry_if_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 from tenacity.retry import retry_base
 
 from swh.core.statsd import statsd
-from swh.model.hashutil import hash_to_hex
+from swh.model.hashutil import MultiHash, hash_to_hex
 from swh.model.model import SHA1_SIZE
 from swh.objstorage.exc import Error, ObjNotFoundError
 
 # import the factory module is needed to make tests work (get_objstorage is patched)
 import swh.objstorage.factory as factory
 
 logger = logging.getLogger(__name__)
@@ -48,24 +48,64 @@
 
 CONTENT_OPERATIONS_METRIC = "swh_content_replayer_operations_total"
 CONTENT_RETRY_METRIC = "swh_content_replayer_retries_total"
 CONTENT_BYTES_METRIC = "swh_content_replayer_bytes"
 CONTENT_DURATION_METRIC = "swh_content_replayer_duration_seconds"
 
 
+class LengthMismatch(Exception):
+    def __init__(self, expected, received):
+        self.expected = expected
+        self.received = received
+
+    def __str__(self):
+        return f"Length mismatch: received {self.received} != expected {self.expected}"
+
+
+class HashMismatch(Exception):
+    def __init__(self, expected, received):
+        self.mismatched = {}
+        self.matched = {}
+        for algo, value in expected.items():
+            received_value = received.get(algo)
+            if received_value != value:
+                self.mismatched[algo] = (received_value, value)
+            else:
+                self.matched[algo] = value
+
+    def __str__(self):
+        return "\n".join(
+            ["Hash Mismatch:"]
+            + [
+                f"  {algo}: {v[0].hex()} != expected {v[1].hex()}"
+                for algo, v in self.mismatched.items()
+            ]
+            + (
+                ["Matched hashes:"]
+                + [f" {algo}: {v.hex()}" for algo, v in self.matched]
+            )
+            if self.matched
+            else []
+        )
+
+
 def format_obj_id(obj_id: CompositeObjId) -> str:
     return ";".join(
         (
             "%s:%s" % (algo, hash_to_hex(hash))
             for algo, hash in sorted(obj_id.items())
             if hash
         )
     )
 
 
+def hex_obj_id(obj_id: CompositeObjId) -> Dict[str, str]:
+    return {algo: hash_to_hex(hash) for algo, hash in obj_id.items() if hash}
+
+
 def logger_debug_obj_id(msg, args, **kwargs):
     if logger.isEnabledFor(logging.DEBUG):
         if sys.version_info >= (3, 8):
             # Ignore this helper in line/function calculation
             kwargs = {**kwargs, "stacklevel": kwargs.get("stacklevel", 1) + 1}
         logger.debug(msg, {**args, "obj_id": format_obj_id(args["obj_id"])}, **kwargs)
 
@@ -148,46 +188,59 @@
             "operation": operation,
             "obj_id": exc.obj_id,
             "exc": str(exc.exc),
         },
     )
 
 
-def log_replay_error(retry_state: RetryCallState) -> None:
-    """Log a replay error to sentry"""
-    assert retry_state.outcome
-    exc = retry_state.outcome.exception()
-
-    assert isinstance(exc, ReplayError)
-    assert retry_state.fn
-
-    with push_scope() as scope:
-        scope.set_tag("operation", retry_state.fn.__name__)
-        scope.set_extra("obj_id", exc.obj_id)
-        capture_exception(exc.exc)
+def log_replay_error(
+    obj_id: CompositeObjId, exc: Exception, operation: str, retries: int
+) -> None:
+    with sentry_sdk.push_scope() as scope:
+        scope.set_tag("operation", operation)
+        scope.set_extra("obj_id", hex_obj_id(obj_id))
+        sentry_sdk.capture_exception(exc)
 
     error_context = {
-        "obj_id": format_obj_id(exc.obj_id),
-        "operation": retry_state.fn.__name__,
+        "obj_id": format_obj_id(obj_id),
+        "operation": operation,
         "exc": str(exc),
-        "retries": retry_state.attempt_number,
+        "retries": retries,
     }
 
     logger.error(
         "Failed operation %(operation)s on %(obj_id)s after %(retries)s"
         " retries; last exception: %(exc)s",
         error_context,
     )
 
     # if we have a global error (redis) reporter
     if REPORTER is not None:
-        oid = f"blob:{format_obj_id(exc.obj_id)}"
+        oid = f"blob:{format_obj_id(obj_id)}"
         msg = msgpack.dumps(error_context)
         REPORTER(oid, msg)
 
+
+def retry_error_callback(retry_state: RetryCallState) -> None:
+    """Log a replay error to sentry"""
+    assert retry_state.outcome
+    exc = retry_state.outcome.exception()
+
+    assert isinstance(exc, ReplayError)
+    assert retry_state.fn
+
+    operation = retry_state.fn.__name__
+
+    log_replay_error(
+        obj_id=exc.obj_id,
+        exc=exc.exc,
+        operation=operation,
+        retries=retry_state.attempt_number,
+    )
+
     raise exc
 
 
 CONTENT_REPLAY_RETRIES = 3
 
 
 class retry_log_if_success(retry_base):
@@ -208,15 +261,15 @@
 
 
 content_replay_retry = retry(
     retry=retry_if_exception_type(ReplayError) | retry_log_if_success(),
     stop=stop_after_attempt(CONTENT_REPLAY_RETRIES),
     wait=wait_random_exponential(multiplier=1, max=60),
     before_sleep=log_replay_retry,
-    retry_error_callback=log_replay_error,
+    retry_error_callback=retry_error_callback,
 )
 
 
 @content_replay_retry
 def get_object(objstorage: ObjStorageInterface, obj_id: CompositeObjId) -> bytes:
     try:
         with statsd.timed(CONTENT_DURATION_METRIC, tags={"request": "get"}):
@@ -229,14 +282,24 @@
             {"obj_id": format_obj_id(obj_id)},
         )
         raise
     except Exception as exc:
         raise ReplayError(obj_id=obj_id, exc=exc) from None
 
 
+def check_hashes(obj: bytes, obj_id: CompositeObjId):
+    h = MultiHash.from_data(obj, hash_names=obj_id.keys())
+    computed = h.digest()
+
+    if computed != obj_id:
+        exc = HashMismatch(obj_id, computed)
+        log_replay_error(obj_id=obj_id, exc=exc, operation="check_hashes", retries=1)
+        raise exc
+
+
 @content_replay_retry
 def put_object(objstorage: ObjStorageInterface, obj_id: CompositeObjId, obj: bytes):
     try:
         logger_debug_obj_id("putting %(obj_id)s", {"obj_id": obj_id})
         with statsd.timed(CONTENT_DURATION_METRIC, tags={"request": "put"}):
             logger_debug_obj_id("storing %(obj_id)s", {"obj_id": obj_id})
             objstorage.add(obj, obj_id, check_presence=False)
@@ -246,18 +309,26 @@
             "putting %(obj_id)s failed: %(exc)r",
             {"obj_id": format_obj_id(obj_id), "exc": exc},
         )
         raise ReplayError(obj_id=obj_id, exc=exc) from None
 
 
 def copy_object(
-    obj_id: CompositeObjId, src: ObjStorageInterface, dst: ObjStorageInterface
+    obj_id: CompositeObjId,
+    obj_len: int,
+    src: ObjStorageInterface,
+    dst: ObjStorageInterface,
+    check_src_hashes: bool = False,
 ) -> int:
     obj = get_object(src, obj_id)
     if obj is not None:
+        if len(obj) != obj_len:
+            raise LengthMismatch(obj_len, len(obj))
+        if check_src_hashes:
+            check_hashes(obj, obj_id)
         put_object(dst, obj_id, obj)
         statsd.increment(CONTENT_BYTES_METRIC, len(obj))
         return len(obj)
     return 0
 
 
 @content_replay_retry
@@ -273,14 +344,15 @@
     def __init__(
         self,
         src: Dict[str, Any],
         dst: Dict[str, Any],
         exclude_fn: Optional[Callable[[Dict[str, Any]], bool]] = None,
         check_dst: bool = True,
         check_obj: bool = False,
+        check_src_hashes: bool = False,
         concurrency: int = 16,
     ):
         """Helper class that takes a list of records from Kafka (see
         :py:func:`swh.journal.client.JournalClient.process`) and copies them
         from the `src` objstorage to the `dst` objstorage, if:
 
         * `obj['status']` is `'visible'`
@@ -294,24 +366,26 @@
                 :py:func:`swh.objstorage.get_objstorage`)
             exclude_fn: Determines whether an object should be copied.
             check_dst: Determines whether we should check the destination
                 objstorage before copying.
             check_obj: If check_dst is true, determines whether we should check
                 the existing object in the destination objstorage is valid; if not,
                 put the replayed object.
+            check_src_hashes: Checks the object before sending it to the dst objstorage.
             concurrency: Number of worker threads doing the replication process
                 (retrieve, check, store).
 
         See swh/objstorage/replayer/tests/test_replay.py for usage examples.
         """
         self.src_cfg = src
         self.dst_cfg = dst
         self.exclude_fn = exclude_fn
         self.check_dst = check_dst
         self.check_obj = check_obj
+        self.check_src_hashes = check_src_hashes
         self.concurrency = concurrency
         self.obj_queue: Queue = Queue()
         self.return_queue: Queue = Queue()
         self.stop_event = Event()
         self.workers = [Thread(target=self._worker) for i in range(self.concurrency)]
         for w in self.workers:
             w.start()
@@ -362,20 +436,34 @@
                     dst.check(obj_id)
                 except Error:
                     logger.info("invalid object found in dst %s", format_obj_id(obj_id))
                     decision = None
                     tags["status"] = "invalid_in_dst"
         if decision is None:
             try:
-                copied_bytes = copy_object(obj_id, src, dst)
+                copied_bytes = copy_object(
+                    obj_id,
+                    obj_len=obj["length"],
+                    src=src,
+                    dst=dst,
+                    check_src_hashes=self.check_src_hashes,
+                )
             except ObjNotFoundError:
                 logger_debug_obj_id("not found %(obj_id)s", {"obj_id": obj_id})
                 decision = "not_found"
                 if not self.check_dst and obj_in_objstorage(obj_id, dst):
                     tags["status"] = "found_in_dst"
+            except LengthMismatch as exc:
+                logger.info("length mismatch %s", format_obj_id(obj_id), exc_info=exc)
+                decision = "length_mismatch"
+                if not self.check_dst and obj_in_objstorage(obj_id, dst):
+                    tags["status"] = "found_in_dst"
+            except HashMismatch as exc:
+                logger.info("hash mismatch %s", format_obj_id(obj_id), exc_info=exc)
+                decision = "hash_mismatch"
             except Exception as exc:
                 logger.info("failed %s", format_obj_id(obj_id), exc_info=exc)
                 decision = "failed"
             else:
                 if copied_bytes is None:
                     logger_debug_obj_id("failed %(obj_id)s (None)", {"obj_id": obj_id})
                     decision = "failed"
@@ -394,27 +482,37 @@
         dst = factory.get_objstorage(**self.dst_cfg)
         while not self.stop_event.is_set():
             try:
                 obj = self.obj_queue.get(timeout=1)
             except Empty:
                 continue
             try:
-                decision, nbytes = self._copy_object(obj, src, dst)
+                decision, nbytes = self._copy_object(obj, src=src, dst=dst)
             except Exception as exc:
                 self.return_queue.put(("error", 0, exc))
             else:
                 self.return_queue.put((decision, nbytes, None))
 
     def replay(
         self,
         all_objects: Dict[str, List[dict]],
     ):
         vol = 0
         stats = dict.fromkeys(
-            ["skipped", "excluded", "not_found", "failed", "copied", "in_dst"], 0
+            [
+                "skipped",
+                "excluded",
+                "not_found",
+                "failed",
+                "copied",
+                "in_dst",
+                "hash_mismatch",
+                "length_mismatch",
+            ],
+            0,
         )
         t0 = time()
         nobjs = 0
         for object_type, objects in all_objects.items():
             if object_type != "content":
                 logger.warning(
                     "Received a series of %s, this should not happen", object_type
```

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_cli.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from click.testing import CliRunner
 from confluent_kafka import Producer
 import msgpack
 import pytest
 import yaml
 
-from swh.journal.serializers import key_to_kafka
+from swh.journal.serializers import key_to_kafka, value_to_kafka
 from swh.model.hashutil import MultiHash
 from swh.objstorage.backends.in_memory import InMemoryObjStorage
 from swh.objstorage.replayer.cli import objstorage_cli_group
 from swh.objstorage.replayer.replay import CONTENT_REPLAY_RETRIES, format_obj_id
 
 logger = logging.getLogger(__name__)
 
@@ -97,15 +97,17 @@
     assert result.exit_code == 0, result.output
     assert re.match(expected, result.output, re.MULTILINE), result.output
 
 
 NUM_CONTENTS = 10
 
 
-def _fill_objstorage_and_kafka(kafka_server, kafka_prefix, objstorage):
+def _fill_objstorage_and_kafka(
+    kafka_server, kafka_prefix, objstorage, mangle_value=None
+):
     producer = Producer(
         {
             "bootstrap.servers": kafka_server,
             "client.id": "test-producer",
             "acks": "all",
         }
     )
@@ -116,24 +118,25 @@
         obj_id = (
             MultiHash(["sha1", "sha1_git", "sha256", "blake2s256"], length=len(content))
             .from_data(content)
             .digest()
         )
         objstorage.add(content=content, obj_id=obj_id)
         contents.append((obj_id, content))
+        value = {
+            **obj_id,
+            "length": len(content),
+            "status": "visible",
+        }
+        if mangle_value:
+            value = mangle_value(value)
         producer.produce(
             topic=kafka_prefix + ".content",
             key=key_to_kafka(obj_id),
-            value=key_to_kafka(
-                {
-                    **obj_id,
-                    "length": len(content),
-                    "status": "visible",
-                }
-            ),
+            value=value_to_kafka(value),
         )
 
     producer.flush()
 
     return contents
 
 
@@ -318,14 +321,121 @@
             assert obj_id not in objstorages["dst"], format_obj_id(obj_id)
         else:
             assert obj_id in objstorages["dst"], obj_id
             assert objstorages["dst"].get(obj_id) == content
 
 
 @_patch_objstorages(["src", "dst"])
+def test_replay_content_hash_mismatch(
+    objstorages,
+    kafka_prefix: str,
+    kafka_consumer_group: str,
+    kafka_server: Tuple[Popen, int],
+):
+    """Check the content replayer in normal conditions
+
+    with hash mismatches
+    """
+
+    mangled = set()
+    unmangled = set()
+
+    def mangle_value(value):
+        if value["sha256"][0] > 128:
+            mangled.add(value["sha256"])
+            return {**value, "sha256": bytes(32)}
+        else:
+            unmangled.add(value["sha256"])
+            return value
+
+    contents = _fill_objstorage_and_kafka(
+        kafka_server, kafka_prefix, objstorages["src"], mangle_value=mangle_value
+    )
+
+    assert mangled
+    assert unmangled
+
+    result = invoke(
+        "replay",
+        "--stop-after-objects",
+        str(NUM_CONTENTS),
+        "--check-src-hashes",
+        journal_client={
+            "cls": "kafka",
+            "brokers": kafka_server,
+            "group_id": kafka_consumer_group,
+            "prefix": kafka_prefix,
+        },
+    )
+    expected = r"Done.\n"
+    assert result.exit_code == 0, result.output
+    assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
+
+    for obj_id, content in contents:
+        if obj_id["sha256"] in mangled:
+            assert obj_id not in objstorages["dst"], format_obj_id(obj_id)
+        else:
+            assert obj_id in objstorages["dst"], obj_id
+            assert objstorages["dst"].get(obj_id) == content
+
+
+@_patch_objstorages(["src", "dst"])
+def test_replay_content_length_mismatch(
+    objstorages,
+    kafka_prefix: str,
+    kafka_consumer_group: str,
+    kafka_server: Tuple[Popen, int],
+):
+    """Check the content replayer in normal conditions
+
+    with hash mismatches
+    """
+
+    mangled = set()
+    unmangled = set()
+
+    def mangle_value(value):
+        if value["sha256"][0] > 128:
+            mangled.add(value["sha256"])
+            return {**value, "length": value["length"] + 1}
+        else:
+            unmangled.add(value["sha256"])
+            return value
+
+    contents = _fill_objstorage_and_kafka(
+        kafka_server, kafka_prefix, objstorages["src"], mangle_value=mangle_value
+    )
+
+    assert mangled
+    assert unmangled
+
+    result = invoke(
+        "replay",
+        "--stop-after-objects",
+        str(NUM_CONTENTS),
+        journal_client={
+            "cls": "kafka",
+            "brokers": kafka_server,
+            "group_id": kafka_consumer_group,
+            "prefix": kafka_prefix,
+        },
+    )
+    expected = r"Done.\n"
+    assert result.exit_code == 0, result.output
+    assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
+
+    for obj_id, content in contents:
+        if obj_id["sha256"] in mangled:
+            assert obj_id not in objstorages["dst"], format_obj_id(obj_id)
+        else:
+            assert obj_id in objstorages["dst"], obj_id
+            assert objstorages["dst"].get(obj_id) == content
+
+
+@_patch_objstorages(["src", "dst"])
 def test_replay_content_exclude_by_size(
     objstorages,
     kafka_prefix: str,
     kafka_consumer_group: str,
     kafka_server: Tuple[Popen, int],
 ):
     """Check the content replayer in normal conditions
```

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_replay.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_replay.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,18 +83,20 @@
     id2 = Content.from_data(cnt2).hashes()
     src.add(b"foo bar", obj_id=id1)
     src.add(b"baz qux", obj_id=id2)
     kafka_partitions = {
         "content": [
             {
                 **id1,
+                "length": 7,
                 "status": "visible",
             },
             {
                 **id2,
+                "length": 7,
                 "status": "visible",
             },
         ]
     }
     with ContentReplayer(
         src={"cls": "mocked", "name": "src"},
         dst={"cls": "mocked", "name": "dst"},
```

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_replay_errors.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_replay_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022-2023  The Software Heritage developers
+# Copyright (C) 2022-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
 from queue import Queue
 from typing import Tuple, cast
@@ -84,17 +84,17 @@
     return replayer, src_objstorage
 
 
 def copy_object_q(q):
     """Wrap the original copy_object function to capture (thread-local) tenacity
     stats and puch them in a queue suitable for checking in a test session"""
 
-    def wrap(obj_id, src, dst):
+    def wrap(obj_id, *args, **kwargs):
         try:
-            ret = copy_object(obj_id, src, dst)
+            ret = copy_object(obj_id, *args, **kwargs)
             return ret
         finally:
             q.put(("get", obj_id, replay.get_object.retry.statistics.copy()))
             q.put(("put", obj_id, replay.put_object.retry.statistics.copy()))
 
     return wrap
 
@@ -146,16 +146,26 @@
         assert get.get("start_time") > 0
         assert get.get("idle_for") > 0
         assert get.get("delay_since_first_attempt") > 0
 
 
 @patch_objstorages(["src", "dst"])
 def test_replay_content_with_errors(
-    objstorages, kafka_server, kafka_prefix, kafka_consumer_group, monkeypatch
+    objstorages,
+    kafka_server,
+    kafka_prefix,
+    kafka_consumer_group,
+    monkeypatch,
+    mocker,
 ):
+    import sentry_sdk
+
+    sentry_sdk.init()
+    capture_event = mocker.spy(sentry_sdk.Hub.current.client, "capture_event")
+
     client, src_objstorage = prepare_test(
         kafka_server, kafka_prefix, kafka_consumer_group
     )
     dst_objstorage = objstorages["dst"]
     objstorages["src"] = FailingObjstorage(src_objstorage)
 
     q = Queue()
@@ -166,14 +176,15 @@
         src={"cls": "mocked", "name": "src"},
         dst={"cls": "mocked", "name": "dst"},
     ) as replayer:
         client.process(replayer.replay)
 
     # no object could be replicated
     assert dst_objstorage.state == {}
+    assert capture_event.mock_calls
 
     stats = [q.get_nowait() for i in range(q.qsize())]
     for obj in CONTENTS:
         if obj.status != "visible":
             continue
 
         obj_id = obj.hashes()
@@ -186,14 +197,21 @@
             stat for (meth, oid, stat) in stats if oid == obj_id and meth == "get"
         )
         assert get.get("attempt_number") == 2
         assert get.get("start_time") > 0
         assert get.get("idle_for") > 0
         assert get.get("delay_since_first_attempt") > 0
 
+        # check hexadecimal hashes are available in sentry event extra data
+        hex_objid = {algo: hash.hex() for algo, hash in obj_id.items()}
+        assert any(
+            mock_call.kwargs["event"]["extra"].get("obj_id") == hex_objid
+            for mock_call in capture_event.mock_calls
+        )
+
 
 @patch_objstorages(["src", "dst"])
 def test_replay_content_not_found(
     objstorages, kafka_server, kafka_prefix, kafka_consumer_group, monkeypatch
 ):
     client, src_objstorage = prepare_test(
         kafka_server, kafka_prefix, kafka_consumer_group
```

### Comparing `swh.objstorage.replayer-2.0.0/swh/objstorage/replayer/tests/test_statsd.py` & `swh.objstorage.replayer-2.1.0/swh/objstorage/replayer/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/PKG-INFO` & `swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage.replayer
-Version: 2.0.0
+Version: 2.1.0
 Summary: Software Heritage content replayer
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage-replayer/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage-replayer.git
@@ -20,15 +20,15 @@
 Requires-Dist: humanize
 Requires-Dist: redis
 Requires-Dist: tenacity
 Requires-Dist: swh.core[http]>=0.3
 Requires-Dist: swh.objstorage>=2.3.1
 Requires-Dist: swh.journal>=0.4.2
 Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: swh.core[testing]; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
 
 Software Heritage - Object storage replayer
 ===========================================
```

### Comparing `swh.objstorage.replayer-2.0.0/swh.objstorage.replayer.egg-info/SOURCES.txt` & `swh.objstorage.replayer-2.1.0/swh.objstorage.replayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

