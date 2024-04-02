# Comparing `tmp/bdownload-0.1.7.tar.gz` & `tmp/bdownload-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bdownload-0.1.7.tar", last modified: Mon Mar 11 09:07:49 2024, max compression
+gzip compressed data, was "dist\bdownload-0.1.8.tar", last modified: Tue Apr  2 15:20:41 2024, max compression
```

## Comparing `bdownload-0.1.7.tar` & `bdownload-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/
--rw-rw-rw-   0        0        0      616 2022-05-30 12:25:29.000000 bdownload-0.1.7/.travis.yml
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/docs/
--rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.1.7/docs/make.bat
--rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.1.7/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/docs/source/
--rw-rw-rw-   0        0        0      313 2022-02-22 14:19:45.000000 bdownload-0.1.7/docs/source/bdownload.rst
--rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.1.7/docs/source/cli.rst
--rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.1.7/docs/source/conf.py
--rw-rw-rw-   0        0        0     7281 2024-03-11 08:48:51.000000 bdownload-0.1.7/docs/source/index.rst
--rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.1.7/docs/source/requirements.txt
--rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.1.7/docs/source/test_bdownloader.rst
--rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.1.7/docs/source/test_multisource_download.rst
--rw-rw-rw-   0        0        0      152 2021-11-15 14:26:13.000000 bdownload-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    20606 2024-03-11 09:07:49.000000 bdownload-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    19016 2024-03-11 08:46:28.000000 bdownload-0.1.7/README.md
--rw-rw-rw-   0        0        0      464 2024-03-08 08:14:53.000000 bdownload-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       58 2024-03-11 09:07:49.000000 bdownload-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2610 2024-03-06 15:56:18.000000 bdownload-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/src/bdownload/
--rw-rw-rw-   0        0        0    18170 2022-02-22 08:53:43.000000 bdownload-0.1.7/src/bdownload/cli.py
--rw-rw-rw-   0        0        0    93286 2024-03-11 07:56:20.000000 bdownload-0.1.7/src/bdownload/download.py
--rw-rw-rw-   0        0        0     5518 2022-05-30 15:36:27.000000 bdownload-0.1.7/src/bdownload/utils.py
--rw-rw-rw-   0        0        0        5 2024-03-11 08:53:43.000000 bdownload-0.1.7/src/bdownload/VERSION
--rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.1.7/src/bdownload/__init__.py
--rw-rw-rw-   0        0        0      352 2022-05-29 11:33:53.000000 bdownload-0.1.7/src/bdownload/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/tests/
--rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.1.7/tests/test_bdownloader.py
--rw-rw-rw-   0        0        0     1527 2021-11-10 14:24:48.000000 bdownload-0.1.7/tests/test_cli.py
--rw-rw-rw-   0        0        0     3303 2021-11-10 14:24:48.000000 bdownload-0.1.7/tests/test_multisource_download.py
--rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.1.7/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/third_parties/
-drwxrwxrwx   0        0        0        0 2024-03-11 09:07:49.000000 bdownload-0.1.7/third_parties/setupext_janitor/
--rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.1.7/third_parties/setupext_janitor/janitor.py
--rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.1.7/third_parties/setupext_janitor/README.rst
--rw-rw-rw-   0        0        0      159 2021-11-16 03:28:13.000000 bdownload-0.1.7/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/
+-rw-rw-rw-   0        0        0     1035 2024-03-08 08:14:53.000000 bdownload-0.1.8/.readthedocs.yaml
+-rw-rw-rw-   0        0        0      702 2024-03-16 15:16:23.000000 bdownload-0.1.8/.travis.yml
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/docs/
+-rwxrwxrwx   0        0        0      756 2021-11-10 14:24:48.000000 bdownload-0.1.8/docs/make.bat
+-rw-rw-rw-   0        0        0      584 2021-11-10 14:24:48.000000 bdownload-0.1.8/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/docs/source/
+-rw-rw-rw-   0        0        0      449 2024-03-15 02:56:16.000000 bdownload-0.1.8/docs/source/bdownload.rst
+-rw-rw-rw-   0        0        0      231 2022-02-23 10:08:54.000000 bdownload-0.1.8/docs/source/cli.rst
+-rw-rw-rw-   0        0        0     6494 2024-03-08 06:08:09.000000 bdownload-0.1.8/docs/source/conf.py
+-rw-rw-rw-   0        0        0     7283 2024-03-15 02:56:16.000000 bdownload-0.1.8/docs/source/index.rst
+-rw-rw-rw-   0        0        0      314 2024-03-08 08:14:53.000000 bdownload-0.1.8/docs/source/requirements.txt
+-rw-rw-rw-   0        0        0      267 2022-02-23 10:23:42.000000 bdownload-0.1.8/docs/source/test_bdownloader.rst
+-rw-rw-rw-   0        0        0      359 2022-02-23 10:23:42.000000 bdownload-0.1.8/docs/source/test_multisource_download.rst
+-rw-rw-rw-   0        0        0      178 2024-03-15 02:56:16.000000 bdownload-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    20720 2024-04-02 15:20:41.000000 bdownload-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    19026 2024-04-02 10:26:45.000000 bdownload-0.1.8/README.md
+-rw-rw-rw-   0        0        0      464 2024-03-08 08:14:53.000000 bdownload-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       58 2024-04-02 15:20:41.000000 bdownload-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2710 2024-03-16 15:18:02.000000 bdownload-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/src/bdownload/
+-rw-rw-rw-   0        0        0    18170 2024-03-31 08:11:00.000000 bdownload-0.1.8/src/bdownload/cli.py
+-rw-rw-rw-   0        0        0    96037 2024-04-02 10:26:45.000000 bdownload-0.1.8/src/bdownload/download.py
+-rw-rw-rw-   0        0        0     6157 2024-03-15 02:56:16.000000 bdownload-0.1.8/src/bdownload/utils.py
+-rw-rw-rw-   0        0        0        5 2024-04-02 15:10:01.000000 bdownload-0.1.8/src/bdownload/VERSION
+-rw-rw-rw-   0        0        0      364 2022-03-05 07:28:46.000000 bdownload-0.1.8/src/bdownload/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-03-15 02:56:16.000000 bdownload-0.1.8/src/bdownload/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/tests/
+-rw-rw-rw-   0        0        0     4248 2021-11-19 11:24:44.000000 bdownload-0.1.8/tests/test_bdownloader.py
+-rw-rw-rw-   0        0        0     1521 2024-03-17 06:34:08.000000 bdownload-0.1.8/tests/test_cli.py
+-rw-rw-rw-   0        0        0     3331 2024-03-17 10:05:27.000000 bdownload-0.1.8/tests/test_multisource_download.py
+-rw-rw-rw-   0        0        0        0 2021-11-10 14:24:48.000000 bdownload-0.1.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/third_parties/
+drwxrwxrwx   0        0        0        0 2024-04-02 15:20:41.000000 bdownload-0.1.8/third_parties/setupext_janitor/
+-rw-rw-rw-   0        0        0     7272 2021-11-10 14:24:48.000000 bdownload-0.1.8/third_parties/setupext_janitor/janitor.py
+-rw-rw-rw-   0        0        0     5228 2021-11-10 14:24:48.000000 bdownload-0.1.8/third_parties/setupext_janitor/README.rst
+-rw-rw-rw-   0        0        0      167 2024-03-16 15:11:35.000000 bdownload-0.1.8/tox.ini
```

### Comparing `bdownload-0.1.7/.travis.yml` & `bdownload-0.1.8/.travis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 #      if: tag IS present
 #  - deploy
 
 
 jobs:
   include:
     - stage: test
-      python: 3.9
+      python: 3.11
+      env: TOXENV=py311
+    - python: 3.10
+      env: TOXENV=py310
+    - python: 3.9
       env: TOXENV=py39
     - python: 3.8
       env: TOXENV=py38
     - python: 3.7
       env: TOXENV=py37
     - python: 3.6
       env: TOXENV=py36
```

### Comparing `bdownload-0.1.7/docs/make.bat` & `bdownload-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/docs/Makefile` & `bdownload-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/docs/source/conf.py` & `bdownload-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/docs/source/index.rst` & `bdownload-0.1.8/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     ``$ pip install .``
 
     Note that you should ``git clone`` or download the source tarball (and unpack it of course) from the repository first
 
 .. admonition:: Notes
 
-    **For Python2.7**:  Since the version of 2022.5.18, `certifi` has dropped the support for Python2.x. To upgrade to
+    **For Python2.7**:  Since the version of 2022.5.18, ``certifi`` has dropped the support for Python2.x. To upgrade to
     the latest CA certificates bundle after installation, simply run:
 
         ``$ bdownload-upd-cacert-py2``
 
 Usage: as a Python package
 --------------------------
 Importing
```

### Comparing `bdownload-0.1.7/PKG-INFO` & `bdownload-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdownload
-Version: 0.1.7
+Version: 0.1.8
 Summary: A multi-threaded and multi-source aria2-like batch file downloading library for Python
 Home-page: https://github.com/Jesseatgao/bdownload
 Author: Jesse Gao
 Author-email: changxigao@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 
@@ -458,14 +460,14 @@
     show help message and exit
 
 #### Examples
 
     bdownload https://www.afilelink.com/afile.tar.gz
     bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz
     bdownload -O /abspath/to/a/dir/ https://www.afilelink.com/afile.tar.gz
-    bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz
+    bdownload -O /abspath/to/afile.tar.gz "https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"
     bdownload -D path/to/working_dir/ -O relpath/to/working_dir/alias_afile.tar.gz https://www.afilelink.com/afile.tar.gz
     bdownload -D path/to/working/dir https://www.afilelink.com/afile.tar.gz
-    bdownload -o /abspath/to/file1.zip ~/file2.tgz -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz
-    bdownload -D path/to/working/dir -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz
+    bdownload -o /abspath/to/file1.zip ~/file2.tgz -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
+    bdownload -D path/to/working/dir -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
```

### Comparing `bdownload-0.1.7/README.md` & `bdownload-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -432,12 +432,12 @@
     show help message and exit
 
 #### Examples
 
     bdownload https://www.afilelink.com/afile.tar.gz
     bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz
     bdownload -O /abspath/to/a/dir/ https://www.afilelink.com/afile.tar.gz
-    bdownload -O /abspath/to/afile.tar.gz https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz
+    bdownload -O /abspath/to/afile.tar.gz "https://www.afilelink.com/afile.tar.gz\thttps://nianpei.bpfatran.com/afile.tar.gz"
     bdownload -D path/to/working_dir/ -O relpath/to/working_dir/alias_afile.tar.gz https://www.afilelink.com/afile.tar.gz
     bdownload -D path/to/working/dir https://www.afilelink.com/afile.tar.gz
-    bdownload -o /abspath/to/file1.zip ~/file2.tgz -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz
-    bdownload -D path/to/working/dir -L http://foo.cc/file1.zip http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz
+    bdownload -o /abspath/to/file1.zip ~/file2.tgz -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
+    bdownload -D path/to/working/dir -L "http://foo.cc/file1.zip" "http://bar.cc/file2.tgz\thttp://bar2.cc/file2.tgz"
```

### Comparing `bdownload-0.1.7/setup.py` & `bdownload-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,13 +66,15 @@
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ]
 )
```

### Comparing `bdownload-0.1.7/src/bdownload/cli.py` & `bdownload-0.1.8/src/bdownload/cli.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/src/bdownload/download.py` & `bdownload-0.1.8/src/bdownload/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
     _os_exit_force = partial(os._exit, -1)
 
 
 # Default retry configuration
 
 #: int: Default number of retries factor for :data:`_requests_extended_retries_factor`.
-REQUESTS_EXTENDED_RETRIES_FACTOR = 3
+REQUESTS_EXTENDED_RETRIES_FACTOR = 1
 
 #: int: Default number of retries on exception set through ``urllib3``'s `Retry` mechanism.
-URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION = 3
+URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION = 1
 
 #: int: Default number of retries on exceptions raised while streaming the request content.
 REQUESTS_RETRIES_ON_STREAM_EXCEPTION = 10
 
 #: float: Default retry backoff factor.
 RETRY_BACKOFF_FACTOR = 0.1
 
@@ -148,15 +148,15 @@
     Notes:
         This function has an external dependency on the global variable :data:`_requests_extended_retries_factor`, whose
         value can be changed through the function :func:`set_requests_retries_factor`. Also, it should be greater than
         ``0``, thus allowing the decorated method to retry at least once to cover the edge cases of exceptions and bad
         status codes.
 
     References:
-         [1] http://www.saltycrane.com/blog/2009/11/trying-out-retry-decorator-python/
+         [1] https://www.saltycrane.com/blog/2009/11/trying-out-retry-decorator-python/
 
          [2] https://en.wikipedia.org/wiki/Exponential_backoff
     """
     if logger is None:
         logger = logging.getLogger(__name__)
 
     random.seed()
@@ -268,22 +268,24 @@
 
         Returns:
             ``requests.Response``: The response to the HTTP ``GET`` request.
 
         Raises:
             :class:`BDownloaderException`: Raised when the termination or cancellation flag has been set, for example,
                 if :attr:`RequestsSessionWrapper.requester_cb` is initialized to :meth:`BDownloader.raise_on_interrupted`.
+            ``requests.RequestException``: Raised when any of ``requests``'s exceptions occurred or bad status codes were
+                received and retries have been exhausted.
             ExceptionByRequesterCB: Same exception(s) as that raised by :attr:`RequestsSessionWrapper.requester_cb`, if any.
         """
         if self.requester_cb:
             self.requester_cb()  # e.g. jump instantly out of the retries when interrupted by user
 
         kwargs.setdefault('timeout', self.timeout)
 
-        if self.referrer and self.referrer == '*':
+        if self.referrer == '*':
             self.headers.update({'Referer': url})
 
         return super(RequestsSessionWrapper, self).get(url, **kwargs)
 
     @staticmethod
     def _build_cookiejar_from_kvp(key_values):
         """Build a CookieJar from cookies in the form of key/value pairs.
@@ -326,15 +328,15 @@
 
     which applies to all the exceptions and those status codes that fall into the `status_forcelist`. For other status
     codes, the maximum retries shall be :data:`_requests_extended_retries_factor`.
 
     Args:
         builtin_retries (int): Maximum number of retry attempts allowed on errors and interested status codes, which will
             apply to the retry logic of the underlying ``urllib3``. If set to `None` or ``0``, it will default to
-            :const:`URLLIB3_RETRIES_ON_EXCEPTION`.
+            :const:`URLLIB3_BUILTIN_RETRIES_ON_EXCEPTION`.
         backoff_factor (float): The backoff factor to apply between retries.
         status_forcelist (set of int): A set of HTTP status codes that a retry should be enforced on. The default status
             forcelist shall be :const:`URLLIB3_RETRY_STATUS_CODES` if not given.
         session (:obj:`requests.Session`): An instance of the class ``requests.Session`` or its customized subclass.
             When not provided, it will use :class:`RequestsSessionWrapper` to create by default.
         num_pools (int): The number of connection pools to cache, which has the same meaning as `num_pools` in
             ``urllib3.PoolManager`` and will eventually be passed to it.
@@ -563,34 +565,39 @@
         ctx = {
             "total_size": 2000,  # total size of all the to-be-downloaded files, maybe inaccurate due to chunked transfer encoding
             "accurate": True,  # Is `total_size` accurate?
             "orig_path_urls": [('file1', 'url1\turl2\turl3'), ('file2', 'url4\turl5\turl6')],  # originally added downloads,
                 # which don't necessarily correspond to `files` e.g. due to duplicate or interruption
             "file_cnt": 2,  # number of current downloading files
             "alt_files": [("full_path_to_file1", `ctx_file1_obj`), ("full_path_to_file2", `ctx_file2_obj`)],  # flattened `files`
+            "active_files": [("full_path_to_file1", `ctx_file1_obj`)],  # scheduled, in-processing file downloads
+            "active_downloads": 1,  # number of in-processing file downloads
+            "next_download": 1,  # index to the next to schedule to download file
+            "poll_changed": False,  # Have the polled files' states changed?
             "files":{
                 "full_path_to_file1":{
                     "length": 2000,  # 0 means 'unknown', i.e. file size can't be pre-determined through any one of provided URLs
                     "progress": 0,  # `SUCCEEDED` downloaded bytes: initialized to 0, set to the last progress when
                                     # resuming and updated on completion (SUCCEEDED only!) of every task (`Future`)
                     "last_progress": 0,  # CONSTANT: the loaded progress of last run upon resuming from interruption
                     "downloaded": 0, # downloaded bytes: initialized to 0, set to the last progress when resuming
                                      # and updated on completion (SUCCEEDED, FAILED, CANCELLED) of every task (`Future`)
                     "resumable": True,
                     "resuming_from_intr": False,  # Are we resuming from keyboard interruption?
                     "download_state": "inprocess",
-                    "future_aborted": False,  # Some `Future` instance(s) raised exception or got cancelled?
                     "cancelled_on_exception": False,
-                    "futures": [future1, future2],
-                    "tsk_num": 2,  # number of the `ranges` and `futures`
                     "orig_path_url": ('file1', 'url1\turl2\turl3'),  # (path, url) as a subparameter passed to :meth:`downloads`
                     "path_url": ('full_path_to_file1', 'url1\turl2\turl3'),  # (full_pathname, active_URLs)
                     "urls":{"url1":{"accept_ranges": "bytes", "refcnt": 1, "interrupted": 2, "succeeded": -5},
                             "url2":{"accept_ranges": "none", "refcnt": 0, "interrupted": 0, "succeeded": 0},
                             "url3":{"accept_ranges": "bytes", "refcnt": 1, "interrupted": 0, "succeeded": -2}},
+                    "alt_ranges": [("bytes=1000-1999", `ctx_range2_obj`)],  # task ranges stack
+                    "worker_ranges": [("bytes=0-999", `ctx_range1_obj`)],  # active range downloading tasks
+                    "active_workers": 1,  # number of active worker threads on ranges downloading of the file
+                    "ranges_succeeded": 0,  # number of ranges successfully downloaded
                     "ranges":{
                         "bytes=0-999": {
                             "start": 0,  # start byte position
                             "end": 999,  # end byte position, None for 'unkown', see above
                             "offset": 0,  # current pointer position relative to 'start'(i.e. 0)
                             "start_time": 0,
                             "rt_dl_speed": 0,  # x seconds interval
@@ -610,42 +617,38 @@
                             "url": [url3],
                             "alt_urls": {}
                         }
                     }
                 },
                 "full_path_to_file2":{
                 }
-            },
-            "futures": {
-                future1: {"file": "full_path_to_file1", "range": "bytes=0-999"},
-                future2: {"file": "full_path_to_file1", "range": "bytes=1000-1999"}
             }
         }
     """
     INPROCESS_EXT = '.bdl'        # extension for the file in downloading (i.e. not succeeded yet)
     RESUM_PARTS_EXT = '.bdl.par'  # extension for the resumption parts file
 
     # Possible download states of the files and ranges
     PENDING = 'pending'      # submitted but not yet processed
     INPROCESS = 'inprocess'  # in downloading
     FAILED = 'failed'        # aborted with exception raised
     SUCCEEDED = 'succeeded'  # finished without error
     CANCELLED = 'cancelled'  # aborted without being processed
 
-    _COMPLETED = [FAILED, CANCELLED, SUCCEEDED]
+    _COMPLETED = {FAILED, CANCELLED, SUCCEEDED}
 
     _FILE_STATES = [PENDING, INPROCESS, FAILED, CANCELLED, SUCCEEDED]
     _RANGE_STATES = [PENDING, INPROCESS, FAILED, CANCELLED, SUCCEEDED]
 
     # Progress bar styles
     PROGRESS_BS_MILL = 'mill'
     PROGRESS_BS_BAR = 'bar'
     PROGRESS_BS_NONE = 'none'
 
-    _PROGRESS_BAR_STYLES = [PROGRESS_BS_MILL, PROGRESS_BS_BAR, PROGRESS_BS_NONE]
+    _PROGRESS_BAR_STYLES = {PROGRESS_BS_MILL, PROGRESS_BS_BAR, PROGRESS_BS_NONE}
 
     # Default value for `max_workers`
     _MAX_WORKERS = (_cpu_count() or 1) * 5  # In line with `futures`
 
     # Default chunk size for streaming the download
     _STREAM_CHUNK_SIZE = 7168
 
@@ -659,23 +662,28 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
         return False
 
-    def __init__(self, max_workers=None, min_split_size=1024*1024, chunk_size=1024*100, proxy=None, cookies=None,
-                 user_agent=None, logger=None, progress='mill', num_pools=20, pool_maxsize=20, request_timeout=None,
-                 request_retries=None, status_forcelist=None, resumption_retries=None, continuation=True, referrer=None,
-                 check_certificate=True, ca_certificate=None, certificate=None):
+    def __init__(self, max_workers=None, max_parallel_downloads=5, workers_per_download=4, min_split_size=1024*1024,
+                 chunk_size=1024*100, proxy=None, cookies=None, user_agent=None, logger=None, progress='mill',
+                 num_pools=20, pool_maxsize=20, request_timeout=None, request_retries=None, status_forcelist=None,
+                 resumption_retries=None, continuation=True, referrer=None, check_certificate=True, ca_certificate=None,
+                 certificate=None):
         """Create and initialize a :class:`BDownloader` object.
 
         Args:
             max_workers (int): The `max_workers` parameter specifies the number of the parallel downloading threads,
                 whose default value is determined by ``#num_of_processor * 5`` if set to `None`.
+            max_parallel_downloads (int): `max_parallel_downloads` limits the number of files downloading concurrently.
+                It has a default value of 5.
+            workers_per_download (int): `workers_per_download` sets the maximum number of worker threads for every file
+                downloading job, which defaults to 4.
             min_split_size (int): `min_split_size` denotes the size in bytes of file pieces split to be downloaded
                 in parallel, which defaults to 1024*1024 bytes (i.e. 1MB).
             chunk_size (int): The `chunk_size` parameter specifies the chunk size in bytes of every http range request,
                 which will take a default value of 1024*100 (i.e. 100KB) if not provided.
             proxy (str): The `proxy` supports both HTTP and SOCKS proxies in the form of ``'http://[user:pass@]host:port'``
                 and ``'socks5://[user:pass@]host:port'``, respectively.
             cookies (str, dict or CookieJar): If `cookies` needs to be set, it must either take the form of ``'cookie_key=cookie_value'``,
@@ -749,31 +757,35 @@
         session = RequestsSessionWrapper(timeout=request_timeout, proxy=proxy, cookies=cookies, user_agent=user_agent,
                                          referrer=referrer, verify=verify, cert=certificate, requester_cb=self.raise_on_interrupted)
         self.requester = requests_retry_session(session=session, builtin_retries=request_retries,
                                                 backoff_factor=RETRY_BACKOFF_FACTOR,
                                                 status_forcelist=status_forcelist,
                                                 num_pools=num_pools, pool_maxsize=pool_maxsize)
 
-        self.executor = ThreadPoolExecutor(max_workers)
-        self.max_workers = max_workers or self._MAX_WORKERS
+        self.max_parallel_downloads = max_parallel_downloads
+        self.workers_per_download = workers_per_download
+        if max_workers is None:
+            max_workers = self._MAX_WORKERS
+        self.max_workers = max(max_workers, self.max_parallel_downloads * self.workers_per_download)
+        self.executor = ThreadPoolExecutor(self.max_workers)
 
         self.progress_thread = None
         self.mgmnt_thread = None
         self.all_done_event = threading.Event()  # Event signaling the completion of all the download jobs
         self.all_done = False  # Flag denoting the completion of all the download jobs
         # Flag indicating that **all** the download tasks have been submitted, i.e. no more downloads to be added
         self.all_submitted = False
         self.sigint = False  # Received the SIGINT (i.e. `KeyboardInterrupt`) signal, e.g. raised by hitting `Ctrl-C`?
         self.cmdquit = False  # Received the QUIT command, e.g. triggered by pressing `q`?
         # Flag indicating that cancellation of all the tasks have been done on demand, e.g. by pressing `Ctrl-C` or `q`
         self.cancelled_on_interrupt = False
         self.stop = False  # Flag signaling waiting threads to exit
         # The download context that maintains the status of the downloading files and the corresponding chunks
-        self._dl_ctx = {"total_size": 0, "accurate": True, "orig_path_urls": [],
-                        "file_cnt": 0, "alt_files": [], "files": {}, "futures": {}}
+        self._dl_ctx = {'total_size': 0, 'accurate': True, 'orig_path_urls': [], 'file_cnt': 0, 'files': {},
+                        'alt_files': [], 'active_files': [], 'next_download': 0, 'active_downloads': 0, 'poll_changed': False}
 
         # list: A downloadable subset of all the `(path, url)`\ s that were passed to :meth:`BDownloader.download` or
         # :meth:`BDownloader.downloads`.
         self.active_downloads_added = []
         # list: The non-downloadable `(path, url)`\ s that were filtered out before downloading actually begins.
         # Together with :attr:`BDownloader.active_downloads_added`, they form the whole of the input downloads.
         self.failed_downloads_on_addition = []
@@ -1300,57 +1312,54 @@
             file_path = path_name
         else:
             file_name = path_tail
             file_path = path_head
 
         orig_urls = url.split('\t')  # maybe TAB-separated URLs
         ctx_file = {'length': 0, 'progress': 0, 'last_progress': 0, 'downloaded': 0, 'resumable': False,
-                    'resuming_from_intr': False, 'download_state': self.PENDING, 'future_aborted': False,
-                    'cancelled_on_exception': False, 'futures': [], 'tsk_num': 0, 'orig_path_url': orig_path_url,
-                    'urls': {}, 'ranges': {}}
+                    'resuming_from_intr': False, 'download_state': self.PENDING, 'cancelled_on_exception': False,
+                    'orig_path_url': orig_path_url, 'path_url': None, 'urls': {}, 'ranges': {}, 'alt_ranges': [],
+                    'worker_ranges': [], 'active_workers': 0, 'ranges_succeeded': 0}
 
         active_urls = []
         downloadable = False  # Must have at least one active URL to download the file
         for mirror_url in orig_urls:
             try:
-                r = self.requester.get(mirror_url, allow_redirects=True, stream=True)
-                if r.status_code == requests.codes.ok:
-                    file_len = int(r.headers.get('Content-Length', 0))
-                    if file_len:
-                        if not ctx_file['length']:
-                            ctx_file['length'] = file_len
-                        else:
-                            if file_len != ctx_file['length']:
-                                self._logger.error("Error: the size of the file '%s' obtained from '%s' happened to "
-                                                   "mismatch with that from others, download will continue but the "
-                                                   "downloaded file may not be the intended one", file_name, mirror_url)
-
-                                r.close()
-                                continue
-
-                    ctx_url = ctx_file['urls'][mirror_url] = {'accept_ranges': "none", 'refcnt': 0, 'interrupted': 0,
-                                                              'succeeded': 0}
-
-                    accept_ranges = r.headers.get('Accept-Ranges')
-                    if "bytes" == accept_ranges:
-                        ctx_url['accept_ranges'] = accept_ranges
-                        ctx_file['resumable'] = True
-
-                    if not file_name:
-                        content_disposition = r.headers.get('Content-Disposition')
-                        if content_disposition:
-                            file_name = self._get_fname_from_hdr(content_disposition)
-
-                    downloadable = True
-                    active_urls.append(mirror_url)
-                else:
-                    self._logger.warning("Unexpected status code %d: trying to determine the size of the file '%s' "
-                                         "using '%s'", r.status_code, file_name, mirror_url)
+                with self.requester.get(mirror_url, allow_redirects=True, stream=True) as r:
+                    if r.status_code == requests.codes.ok:
+                        file_len = int(r.headers.get('Content-Length', 0))
+                        if file_len:
+                            if not ctx_file['length']:
+                                ctx_file['length'] = file_len
+                            else:
+                                if file_len != ctx_file['length']:
+                                    self._logger.error("Error: the size of the file '%s' obtained from '%s' happened to "
+                                                       "mismatch with that from others, download will continue but the "
+                                                       "downloaded file may not be the intended one", file_name, mirror_url)
+
+                                    continue
+
+                        ctx_url = ctx_file['urls'][mirror_url] = {'accept_ranges': "none", 'refcnt': 0, 'interrupted': 0,
+                                                                  'succeeded': 0}
+
+                        accept_ranges = r.headers.get('Accept-Ranges')
+                        if "bytes" == accept_ranges:
+                            ctx_url['accept_ranges'] = accept_ranges
+                            ctx_file['resumable'] = True
+
+                        if not file_name:
+                            content_disposition = r.headers.get('Content-Disposition')
+                            if content_disposition:
+                                file_name = self._get_fname_from_hdr(content_disposition)
 
-                r.close()
+                        downloadable = True
+                        active_urls.append(mirror_url)
+                    else:
+                        self._logger.warning("Unexpected status code %d: trying to determine the size of the file '%s' "
+                                             "using '%s'", r.status_code, file_name, mirror_url)
             except requests.RequestException as e:
                 self._logger.error("Error while trying to determine the size of the file '%s' using '%s': '%r'",
                                    file_name, mirror_url, e)
 
         if downloadable:
             if not file_name:
                 file_name = self._get_fname_from_url(active_urls[0])
@@ -1416,42 +1425,44 @@
             if not ctx_file['length']:
                 self._dl_ctx['accurate'] = False
 
             iter_url = self._pick_file_url(file_path_name)
 
             if not is_resuming:
                 # calculate request ranges
-                if self._is_parallel_downloadable(file_path_name) and self.max_workers > 1:
+                if self._is_parallel_downloadable(file_path_name) and self.workers_per_download > 1:
                     ranges = self.calc_req_ranges(ctx_file['length'], self.min_split_size, 0)
                 else:
                     ranges = [(0, None)]
 
-                ctx_file['tsk_num'] = len(ranges)  # How many tasks to complete the download job of the file
                 for start, end in ranges:
                     req_range = "bytes={}-{}".format(start, end)
                     ctx_range = ctx_file['ranges'][req_range] = {}
                     ctx_range.update({
                         'start': start,
                         'end': end,
                         'offset': 0,
                         'start_time': 0,
                         'rt_dl_speed': 0,
                         'download_state': self.PENDING,
                         'url': next(iter_url),
                         'alt_urls': {}})
             else:
                 ctx_file['ranges'] = resumption_ctx['failed_ranges']
-                ctx_file['tsk_num'] = len(ctx_file['ranges'])
 
                 for ctx_range in ctx_file['ranges'].values():
                     ctx_range['url'] = next(iter_url)
                     ctx_range['alt_urls'] = {}
 
+            ctx_file['alt_ranges'] = [(req_range, ctx_range) for req_range, ctx_range in ctx_file['ranges'].items()]
+            ctx_file['alt_ranges'].reverse()  # To pop from the range stack and download from the beginning of the file
+
             # make the file visible to the world
             self._dl_ctx['alt_files'].append((file_path_name, ctx_file))
+            self._dl_ctx['file_cnt'] += 1
 
         return downloadable, path_url, orig_path_url
 
     def _build_ctx(self, path_urls):
         """Build the context for downloading the file(s).
 
         Args:
@@ -1479,44 +1490,14 @@
                 existing_orig.append(orig_path_url)
             else:
                 failed.append(path_url)
                 failed_orig.append(orig_path_url)
 
         return active, active_orig, failed, failed_orig, existing, existing_orig
 
-    def _submit_dl_tasks(self, path_urls):
-        """Submit the download tasks of the files to the thread pool.
-
-        Args:
-            path_urls (list of tuple): The meaning and format of the `path_urls` is similar to the parameter for
-                :meth:`downloads`.
-
-        Returns:
-            None.
-        """
-        for path_name, _ in path_urls:
-            ctx_file = self._dl_ctx['files'][path_name]
-
-            if len(ctx_file['ranges']) > 1:
-                tsk = self._get_remote_file_multipart
-            else:
-                tsk = self._get_remote_file_singlewhole
-
-            for req_range, ctx_range in ctx_file['ranges'].items():
-                future = self.executor.submit(tsk, path_name, req_range)
-                ctx_file['futures'].append(future)
-                ctx_range['future'] = future
-                ctx_range['start_time'] = time.time()
-                self._dl_ctx['futures'][future] = {
-                    "file": path_name,
-                    "range": req_range
-                }
-
-            self._dl_ctx['file_cnt'] += 1
-
     def _is_all_done(self):
         """Check if all the tasks have completed.
 
         Returns:
             bool: ``True`` if all the ``Future``\ s have been done, meaning that all the files have finished downloading,
             whether successfully or not; ``False`` otherwise.
         """
@@ -1616,107 +1597,163 @@
             else:
                 self._logger.warning("The download of the file '%s' has been cancelled on demand, but can be resumed "
                                      "by re-running it: '%r'", the_file, ctx_file['orig_path_url'])
         except EnvironmentError as e:
             self._logger.error("Error while operating on '%s': 'Error number %d: %s'", e.filename, e.errno, e.strerror)
 
     def _cancel_all_on_interrupted(self):
-        """Cancel all the downloading tasks when receiving the ``SIGINT`` signal or the QUIT command."""
+        """Cancel all the pending tasks when receiving the ``SIGINT`` signal or the QUIT command."""
         if self.all_submitted and not self.cancelled_on_interrupt:
-            for f in self._dl_ctx['futures']:
-                f.cancel()
+            for fi in range(self._dl_ctx['next_download'], self._dl_ctx['file_cnt']):
+                the_file, ctx_file = self._dl_ctx['alt_files'][fi]
+                ctx_file['download_state'] = self.CANCELLED
+                self._on_cancelled(the_file, ctx_file)
+                self.failed_downloads_in_running.append(ctx_file['orig_path_url'])
 
             self.cancelled_on_interrupt = True
             self._logger.warning("The user terminated the downloads %s!",
                                  "by pressing the interrupt key" if self.sigint else "by typing the QUIT command")
 
     def _finalize_on_interrupted_py2(self):
         """When interrupted under Python2.x, perform state transitions manually and act accordingly."""
         for the_file, ctx_file in self._dl_ctx['files'].items():
             if ctx_file['download_state'] == self.INPROCESS:
                 self._on_failed(the_file, ctx_file)
             elif ctx_file['download_state'] == self.PENDING:
                 self._on_cancelled(the_file, ctx_file)
 
+    def _schedule_dl_tasks(self, path_name, num_tasks):
+        """Arrange the range downloading tasks of the file and assign them to the thread pool executor.
+
+        Args:
+            path_name (str): The full path name of the file being scheduled for.
+            num_tasks (int): The number of the range tasks requested to allocate.
+
+        Returns:
+            list of tuple: The (re-)scheduled range tasks and their corresponding download contexts.
+        """
+        worker_ranges = []
+        ctx_file = self._dl_ctx['files'][path_name]
+
+        if len(ctx_file['ranges']) > 1:
+            tsk = self._get_remote_file_multipart
+        else:
+            tsk = self._get_remote_file_singlewhole
+
+        while ctx_file['alt_ranges'] and len(worker_ranges) < num_tasks:
+            req_range, ctx_range = ctx_file['alt_ranges'].pop()
+            future = self.executor.submit(tsk, path_name, req_range)
+            ctx_range['future'] = future
+            ctx_range['start_time'] = time.time()
+
+            worker_ranges.append((req_range, ctx_range))
+
+        return worker_ranges
+
+    def _schedule_files_downloads(self):
+        """Remove the completed tasks from the files downloading queue and submit new file task assignments."""
+        active_files = []
+
+        for the_file, ctx_file in self._dl_ctx['active_files']:
+            if ctx_file['download_state'] not in self._COMPLETED:
+                active_files.append((the_file, ctx_file))
+            else:
+                self._dl_ctx['active_downloads'] -= 1
+
+        while self._dl_ctx['active_downloads'] < self.max_parallel_downloads and self._dl_ctx['next_download'] < self._dl_ctx['file_cnt']:
+            the_file, ctx_file = self._dl_ctx['alt_files'][self._dl_ctx['next_download']]
+            ctx_file['worker_ranges'] = self._schedule_dl_tasks(the_file, self.workers_per_download)
+            ctx_file['active_workers'] = len(ctx_file['worker_ranges'])
+
+            active_files.append((the_file, ctx_file))
+            self._dl_ctx['active_downloads'] += 1
+            self._dl_ctx['next_download'] += 1
+
+        self._dl_ctx['active_files'] = active_files
+
+    def _schedule_file_download(self, the_file, ctx_file):
+        """Remove the succeeded range tasks, reassign the failed and arrange new for the file downloading."""
+        worker_ranges, raised_ranges = [], []
+
+        for req_range, ctx_range in ctx_file['worker_ranges']:
+            if ctx_range['download_state'] not in self._COMPLETED:
+                worker_ranges.append((req_range, ctx_range))
+            elif ctx_range['download_state'] == self.FAILED:
+                ctx_range['download_state'] = self.PENDING
+                ctx_range['future'] = None
+                raised_ranges.append((req_range, ctx_range))
+
+        ctx_file['alt_ranges'] += raised_ranges
+
+        worker_ranges += self._schedule_dl_tasks(the_file, ctx_file['active_workers'] - len(worker_ranges))
+        ctx_file['worker_ranges'] = worker_ranges
+
     def _state_mgmnt(self):
         """Perform the state-related operations of file downloading.
 
         This method updates the download status of the files and their related chunks when the associated worker threads
         completed, either because of finished without error, raised on exception or cancelled intentionally.
 
         Returns:
             None.
         """
-        # Cancel the downloading tasks repeatedly on the downloading queue when interrupted
-        if self.sigint or self.cmdquit:
+        if not (self.sigint or self.cmdquit):
+            # Assign new file-level downloads and submit their initial range tasks to the thread pool when current downloads' state changed
+            if self._dl_ctx['poll_changed'] or (self._dl_ctx['active_downloads'] < self.max_parallel_downloads and
+                                                self._dl_ctx['next_download'] < self._dl_ctx['file_cnt']):
+                self._schedule_files_downloads()
+                self._dl_ctx['poll_changed'] = False
+        else:
+            # Cancel the pending tasks on the downloading queue when interrupted
             self._cancel_all_on_interrupted()
 
-        for fi in range(self._dl_ctx['file_cnt']):
-            _, ctx_file = self._dl_ctx['alt_files'][fi]
-            if ctx_file['download_state'] not in self._COMPLETED:
-                ranges_all_done = True
-
-                fs = ctx_file['futures']
-                fs_num = len(fs)
-                tsk_num = ctx_file['tsk_num']
-                if fs_num == tsk_num:  # Make sure that all the tasks of the file have been submitted
-                    for ctx_range in ctx_file['ranges'].values():
-                        future = ctx_range['future']
-                        if future.done():
-                            if ctx_range['download_state'] not in self._COMPLETED:
-                                ctx_file['downloaded'] += ctx_range['offset']
+        for the_file, ctx_file in self._dl_ctx['active_files']:
+            ranges_have_dones = False
 
-                                try:
-                                    exception = future.exception()
-                                    if exception is None:
-                                        ctx_range['download_state'] = self.SUCCEEDED
-                                        ctx_file['progress'] += ctx_range['offset']
-
-                                        # Accumulate the download statistics of the source URLs
-                                        for url, ctx_url_range in ctx_range['alt_urls'].items():
-                                            ctx_url_file = ctx_file['urls'][url]
-                                            ctx_url_file['refcnt'] += ctx_url_range.get('refcnt', 0)
-                                            ctx_url_file['interrupted'] += ctx_url_range.get('interrupted', 0)
-                                        # use MINUS for ease of multi-level sorting
-                                        ctx_file['urls'][ctx_range['url'][-1]]['succeeded'] -= 1
-                                    else:  # exception raised
-                                        ctx_range['download_state'] = self.FAILED
-                                        ctx_file['future_aborted'] = True
-
-                                        if not (self.cancelled_on_interrupt or ctx_file['cancelled_on_exception']):
-                                            # Cancel the download of the failed file
-                                            for f in fs:
-                                                f.cancel()
-
-                                            ctx_file['cancelled_on_exception'] = True
-                                except CancelledError:
-                                    ctx_range['download_state'] = self.CANCELLED
-                                    ctx_file['future_aborted'] = True
-                        else:
-                            ranges_all_done = False
-                else:
-                    ranges_all_done = False
+            for _, ctx_range in ctx_file['worker_ranges']:
+                future = ctx_range['future']
+                if future.done():
+                    ranges_have_dones = True
+                    ctx_file['downloaded'] += ctx_range['offset']
 
-                if ranges_all_done:
-                    the_file = ctx_file['path_url'][0]
-
-                    if not ctx_file['future_aborted']:
-                        ctx_file['download_state'] = self.SUCCEEDED
-                        self.succeeded_downloads_in_running.append(ctx_file['orig_path_url'])
-
-                        self._on_succeeded(the_file, ctx_file)
-                    else:
-                        if ctx_file['download_state'] != self.PENDING:
-                            ctx_file['download_state'] = self.FAILED
-                            self._on_failed(the_file, ctx_file)
-                        else:
-                            ctx_file['download_state'] = self.CANCELLED
-                            self._on_cancelled(the_file, ctx_file)
+                    try:
+                        exception = future.exception()
+                        if exception is None:
+                            ctx_range['download_state'] = self.SUCCEEDED
+                            ctx_file['ranges_succeeded'] += 1
+                            ctx_file['progress'] += ctx_range['offset']
+
+                            # Accumulate the download statistics of the source URLs
+                            for url, ctx_url_range in ctx_range['alt_urls'].items():
+                                ctx_url_file = ctx_file['urls'][url]
+                                ctx_url_file['refcnt'] += ctx_url_range.get('refcnt', 0)
+                                ctx_url_file['interrupted'] += ctx_url_range.get('interrupted', 0)
+                            # use MINUS for ease of multi-level sorting
+                            ctx_file['urls'][ctx_range['url'][-1]]['succeeded'] -= 1
+                        else:  # exception raised
+                            ctx_range['download_state'] = self.FAILED
+                            ctx_file['active_workers'] -= 1
+                    except CancelledError:
+                        # could not reach here
+                        ctx_range['download_state'] = self.CANCELLED
+
+            if ctx_file['ranges_succeeded'] == len(ctx_file['ranges']):
+                ctx_file['download_state'] = self.SUCCEEDED
+                self._dl_ctx['poll_changed'] = True
+
+                self.succeeded_downloads_in_running.append(ctx_file['orig_path_url'])
+                self._on_succeeded(the_file, ctx_file)
+            elif ctx_file['active_workers'] == 0:
+                ctx_file['download_state'] = self.FAILED
+                self._dl_ctx['poll_changed'] = True
 
-                        self.failed_downloads_in_running.append(ctx_file['orig_path_url'])
+                self.failed_downloads_in_running.append(ctx_file['orig_path_url'])
+                self._on_failed(the_file, ctx_file)
+            elif ranges_have_dones:
+                self._schedule_file_download(the_file, ctx_file)
 
     def _mgmnt_task(self):
         """The management thread body.
 
         This thread manages the downloading process of the whole job queue, currently including state management only.
         When all the tasks have been done, it signals the waiting thread and exits immediately.
 
@@ -1737,15 +1774,15 @@
     def _calc_completed(self):
         """Calculate the already downloaded bytes of the files.
 
         Returns:
             int: The size in bytes of the downloaded pieces.
         """
         completed = 0
-        for fi in range(self._dl_ctx['file_cnt']):
+        for fi in range(self._dl_ctx['next_download']):
             _, ctx_file = self._dl_ctx['alt_files'][fi]
             if ctx_file['download_state'] not in self._COMPLETED:
                 completed += ctx_file['last_progress']
 
                 ctx_ranges = ctx_file.get('ranges')
                 if ctx_ranges:
                     for ctx_range in ctx_ranges.values():
@@ -1826,15 +1863,14 @@
                     self.progress_thread = threading.Thread(target=self._progress_task)
                     self.progress_thread.start()
 
                 if self.mgmnt_thread is None:
                     self.mgmnt_thread = threading.Thread(target=self._mgmnt_task)
                     self.mgmnt_thread.start()
 
-                self._submit_dl_tasks(active)
                 self.active_downloads_added.extend(active_orig)
 
             if existing_orig:
                 self.succeeded_downloads_on_addition.extend(existing_orig)
 
             if failed_orig:
                 self.failed_downloads_on_addition.extend(failed_orig)
```

### Comparing `bdownload-0.1.7/src/bdownload/utils.py` & `bdownload-0.1.8/src/bdownload/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,26 +51,40 @@
 
 def _update_local_cacert_ver(new_ver):
     with codecs.open(certifi_cacert_ver, 'w+', 'utf-8') as fd:
         fd.write(new_ver)
 
 
 def get_latest_tag_github(owner, repo, key, **kwargs):
+    """Get the latest tag/version of a GitHub repository.
+
+    Args:
+        owner (str): The account owner of the repository.
+        repo (str): The name of the repository.
+        key (func): A function for extracting comparison key from each tag/version.
+        **kwargs: Same arguments as that of :meth:`bdownload.download.RequestsSessionWrapper.__init__()`.
+
+    Returns:
+        str: The name of the latest tag.
+
+    Raises:
+        exception: Same exception as that raised by :meth:`bdownload.download.RequestsSessionWrapper.get()`.
+    """
     rest_api = 'https://api.github.com/repos/%(owner)s/%(repo)s/tags' % {'owner': owner, 'repo': repo}
-    header = {'Accept': 'application/vnd.github.v3+json'}
+    headers = {'Accept': 'application/vnd.github.v3+json'}
     requester = requests_retry_session(**kwargs)
 
     try:
-        r = requester.get(rest_api, headers=header)
-        r.raise_for_status()
+        r = requester.get(rest_api, headers=headers)
         tags = r.json()
         max_tag = max(tags, key=key)
         return max_tag['name']
     except Exception as e:
-        raise Exception("Error while fetching '%s/%s's latest tag: '%s'" % (owner, repo, str(e)))
+        print("Error while fetching '%s/%s's latest tag: '%s'" % (owner, repo, str(e)))
+        raise
 
 
 def _key(tag):
     return tag['name'] if not tag['name'].startswith('v') else '1970.01.01'
 
 
 def _download_certifi(pathname, url, **kwargs):
@@ -115,14 +129,16 @@
 
     parser.add_argument('-p', '--proxy', dest='proxy', help='Proxy of the form "http://[user:pass@]host:port" or "socks5://[user:pass@]host:port" ')
 
     return parser
 
 
 def update_cacert():
+    """Update ``certifi`` to the latest version of certificate authority (CA) bundle on Python2.7.
+    """
     if _py3plus:
         print("This utility only supports updating the CA bundle on Python2. For Python3, please run 'pip install -U certifi' to update it instead.")
         sys.exit(-1)
 
     args = _arg_parser().parse_args()
     kwargs = vars(args)
 
@@ -143,12 +159,12 @@
             cacert_path = '/'.join([certifi_root, 'certifi', CACERT_PEM])
             _extract_cacert(certifi, cacert_path, certifi_cacert)
 
             _update_local_cacert_ver(latest_ver)
 
             print("The certifi CA bundle has been successfully updated to version '%s'." % latest_ver)
         else:
-            print("The certifi CA bundle has already been the latest (%s), so there is nothing to do." % local_ver)
+            print("The certifi CA bundle has already been the latest (%s), so there is nothing left to do." % local_ver)
             sys.exit(-1)
     except Exception as e:
         print("Updating the certifi CA bundle has failed: '%s'" % str(e))
         sys.exit(-1)
```

### Comparing `bdownload-0.1.7/tests/test_bdownloader.py` & `bdownload-0.1.8/tests/test_bdownloader.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/tests/test_cli.py` & `bdownload-0.1.8/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from subprocess import Popen, PIPE
 
 # test vectors that use *raw* URL strings mimicking what the `argparse` actually sees
 FILES = [
             {
                 "file": "gdb-9.2.tar.xz",
                 "url": r"https://mirrors.kernel.org/gnu/gdb/gdb-9.2.tar.xz	"
-                       r"https://mirror.sergal.org/gnu/gdb/gdb-9.2.tar.xz\t"
+                       r"https://ftp.gnu.org/gnu/gdb/gdb-9.2.tar.xz\t"
                        r"https://mirror.ibcp.fr/pub/gnu/gdb/gdb-9.2.tar.xz",
                 "sha1": "356ee474a24bfb2f133894730916557dfea9da2e"
             }
         ]
 
 
 class TestCommandLineTool(unittest.TestCase):
```

### Comparing `bdownload-0.1.7/tests/test_multisource_download.py` & `bdownload-0.1.8/tests/test_multisource_download.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,19 @@
                 "file": "valgrind-3.15.0-11.el7.x86_64.rpm",
                 "url": "https://mirrors.163.com/centos/7/os/x86_64/Packages/valgrind-3.15.0-11.el7.x86_64.rpm	"
                        "https://mirrors.tuna.tsinghua.edu.cn/centos/7/os/x86_64/Packages/valgrind-3.15.0-11.el7.x86_64.rpm\t"
                        "https://mirrors.aliyun.com/centos/7/os/x86_64/Packages/valgrind-3.15.0-11.el7.x86_64.rpm",
                 "sha1": "84866f6c637042297eda09cdd4fed35118c4f507"
             },
             {
-                "file": "eclipse_3.8.1.orig.tar.xz",
-                "url": "http://ftp.us.debian.org/debian/pool/main/e/eclipse/eclipse_3.8.1.orig.tar.xz	"
-                       "http://debian-archive.trafficmanager.net/debian/pool/main/e/eclipse/eclipse_3.8.1.orig.tar.xz\t"
-                       "http://ftp.uk.debian.org/debian/pool/main/e/eclipse/eclipse_3.8.1.orig.tar.xz",
-                "sha1": "9b8bb069eea91ac7f1b7a3295803056e50e31fa1"
+                "file": "eclipse-cdt_9.9.0.orig.tar.xz",
+                "url": "http://ftp.us.debian.org/debian/pool/main/e/eclipse-cdt/eclipse-cdt_9.9.0.orig.tar.xz	"
+                       "http://debian-archive.trafficmanager.net/debian/pool/main/e/eclipse-cdt/eclipse-cdt_9.9.0.orig.tar.xz\t"
+                       "http://ftp.uk.debian.org/debian/pool/main/e/eclipse-cdt/eclipse-cdt_9.9.0.orig.tar.xz",
+                "sha1": "108cfea1b876beb95ab73f2c5a947659f38115b6"
             }
         ]
 
 
 class TestMultiSourceDownload(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
```

### Comparing `bdownload-0.1.7/third_parties/setupext_janitor/janitor.py` & `bdownload-0.1.8/third_parties/setupext_janitor/janitor.py`

 * *Files identical despite different names*

### Comparing `bdownload-0.1.7/third_parties/setupext_janitor/README.rst` & `bdownload-0.1.8/third_parties/setupext_janitor/README.rst`

 * *Files identical despite different names*

