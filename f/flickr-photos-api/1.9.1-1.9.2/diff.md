# Comparing `tmp/flickr-photos-api-1.9.1.tar.gz` & `tmp/flickr-photos-api-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr-photos-api-1.9.1.tar", last modified: Tue Mar 26 11:18:23 2024, max compression
+gzip compressed data, was "flickr-photos-api-1.9.2.tar", last modified: Tue Apr  2 13:08:20 2024, max compression
```

## Comparing `flickr-photos-api-1.9.1.tar` & `flickr-photos-api-1.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-03-26 11:18:23.723028 flickr-photos-api-1.9.1/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr-photos-api-1.9.1/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr-photos-api-1.9.1/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-03-26 11:18:23.722864 flickr-photos-api-1.9.1/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2448 2023-12-27 10:54:19.000000 flickr-photos-api-1.9.1/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1810 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.1/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-03-26 11:18:23.723068 flickr-photos-api-1.9.1/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-03-26 11:18:23.719584 flickr-photos-api-1.9.1/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-03-26 11:18:23.721285 flickr-photos-api-1.9.1/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1002 2024-03-26 11:17:52.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    32693 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/api.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1632 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2063 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr-photos-api-1.9.1/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-03-26 11:18:23.722679 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-03-26 11:18:23.000000 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      526 2024-03-26 11:18:23.000000 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-03-26 11:18:23.000000 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-03-26 11:18:23.000000 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-03-26 11:18:23.000000 flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-03-26 11:18:23.722401 flickr-photos-api-1.9.1/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    21130 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.1/tests/test_api.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     7091 2024-03-26 10:37:52.000000 flickr-photos-api-1.9.1/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr-photos-api-1.9.1/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612800 flickr-photos-api-1.9.2/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr-photos-api-1.9.2/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr-photos-api-1.9.2/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-04-02 13:08:20.612619 flickr-photos-api-1.9.2/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2448 2023-12-27 10:54:19.000000 flickr-photos-api-1.9.2/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1810 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.2/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-02 13:08:20.612843 flickr-photos-api-1.9.2/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.607174 flickr-photos-api-1.9.2/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.609266 flickr-photos-api-1.9.2/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1002 2024-04-02 13:08:13.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    32718 2024-04-02 13:08:13.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/api.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1632 2024-01-04 12:06:41.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2063 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr-photos-api-1.9.2/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612403 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3346 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      526 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-02 13:08:20.000000 flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-02 13:08:20.612145 flickr-photos-api-1.9.2/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    21130 2024-03-26 11:13:22.000000 flickr-photos-api-1.9.2/tests/test_api.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     7091 2024-03-26 10:37:52.000000 flickr-photos-api-1.9.2/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr-photos-api-1.9.2/tests/test_utils.py
```

### Comparing `flickr-photos-api-1.9.1/LICENSE-APACHE` & `flickr-photos-api-1.9.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/LICENSE-MIT` & `flickr-photos-api-1.9.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/PKG-INFO` & `flickr-photos-api-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 1.9.1
+Version: 1.9.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr-photos-api-1.9.1/README.md` & `flickr-photos-api-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/pyproject.toml` & `flickr-photos-api-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api/__init__.py` & `flickr-photos-api-1.9.2/src/flickr_photos_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     PhotosInGroup,
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
 )
 
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 
 
 __all__ = [
     "FlickrPhotosApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
```

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api/api.py` & `flickr-photos-api-1.9.2/src/flickr_photos_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     find_required_text,
 )
 from tenacity import (
     retry,
     retry_if_exception,
     RetryError,
     stop_after_attempt,
-    wait_fixed,
+    wait_random_exponential,
 )
 
 from .exceptions import (
     FlickrApiException,
     InvalidApiKey,
     InvalidXmlException,
     LicenseNotFound,
@@ -103,16 +103,16 @@
         try:
             return self._call_api(method=method, params=params)
         except RetryError as retry_err:
             retry_err.reraise()
 
     @retry(
         retry=retry_if_exception(is_retryable),
-        stop=stop_after_attempt(3),
-        wait=wait_fixed(1),
+        stop=stop_after_attempt(5),
+        wait=wait_random_exponential(),
     )
     def _call_api(self, *, method: str, params: dict[str, str] | None) -> ET.Element:
         if params is not None:
             get_params = {"method": method, **params}
         else:
             get_params = {"method": method}
```

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api/exceptions.py` & `flickr-photos-api-1.9.2/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api/types.py` & `flickr-photos-api-1.9.2/src/flickr_photos_api/types.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api/utils.py` & `flickr-photos-api-1.9.2/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 1.9.1
+Version: 1.9.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr-photos-api-1.9.1/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr-photos-api-1.9.2/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/tests/test_api.py` & `flickr-photos-api-1.9.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `flickr-photos-api-1.9.1/tests/test_errors.py` & `flickr-photos-api-1.9.2/tests/test_errors.py`

 * *Files identical despite different names*

