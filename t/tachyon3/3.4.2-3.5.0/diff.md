# Comparing `tmp/tachyon3-3.4.2.tar.gz` & `tmp/tachyon3-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tachyon3-3.4.2.tar", last modified: Tue Feb 15 17:39:43 2022, max compression
+gzip compressed data, was "tachyon3-3.5.0.tar", last modified: Tue Apr  2 19:54:40 2024, max compression
```

## Comparing `tachyon3-3.4.2.tar` & `tachyon3-3.5.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.166911 tachyon3-3.4.2/
--rw-rw-r--   0 lph       (1000) lph       (1000)      205 2022-02-15 17:39:43.166911 tachyon3-3.4.2/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)     3398 2021-09-02 14:41:30.000000 tachyon3-3.4.2/README.md
--rw-rw-r--   0 lph       (1000) lph       (1000)      108 2022-02-15 17:39:43.166911 tachyon3-3.4.2/setup.cfg
--rw-rw-r--   0 lph       (1000) lph       (1000)      549 2021-09-02 14:41:30.000000 tachyon3-3.4.2/setup.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/
--rw-rw-r--   0 lph       (1000) lph       (1000)      953 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)    13352 2022-02-15 17:31:06.000000 tachyon3-3.4.2/tachyon/__main__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      911 2022-02-15 17:36:36.000000 tachyon3-3.4.2/tachyon/__version__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1434 2022-02-15 17:31:06.000000 tachyon3-3.4.2/tachyon/conf.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5766 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/config.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/data/
--rw-rw-r--   0 lph       (1000) lph       (1000)    45377 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/data/files.json
--rw-rw-r--   0 lph       (1000) lph       (1000)    29008 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/data/paths.json
--rw-rw-r--   0 lph       (1000) lph       (1000)     1286 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/database.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1880 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/dbutils.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2493 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/directoryfetcher.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2814 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/filefetcher.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5207 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/generator.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      989 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/har.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/heuristics/
--rw-rw-r--   0 lph       (1000) lph       (1000)     1152 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/heuristics/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1358 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/heuristics/logbehaviorchange.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1673 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/heuristics/matchstring.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3804 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/heuristics/rejectignoredquery.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      337 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/heuristics/striptag.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1933 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/loaders.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3330 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/output.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/plugins/
--rw-rw-r--   0 lph       (1000) lph       (1000)      851 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/__init__.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/plugins/file/
--rw-rw-r--   0 lph       (1000) lph       (1000)      893 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/file/__init__.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.162911 tachyon3-3.4.2/tachyon/plugins/host/
--rw-rw-r--   0 lph       (1000) lph       (1000)     3581 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/HostProcessor.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2693 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/PathGenerator.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2506 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/Robots.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3131 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/SitemapXML.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     4739 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/Svn.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      956 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/plugins/host/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3274 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/result.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1467 2021-09-02 14:41:30.000000 tachyon3-3.4.2/tachyon/textutils.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2022-02-15 17:39:43.166911 tachyon3-3.4.2/tachyon3.egg-info/
--rw-rw-r--   0 lph       (1000) lph       (1000)      205 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)     1010 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/SOURCES.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        1 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/dependency_links.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       51 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/entry_points.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       67 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/requires.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        8 2022-02-15 17:39:43.000000 tachyon3-3.4.2/tachyon3.egg-info/top_level.txt
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/
+-rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2021-09-02 14:41:30.000000 tachyon3-3.5.0/LICENSE.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      219 2024-04-02 19:54:40.991845 tachyon3-3.5.0/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3398 2021-09-02 14:41:30.000000 tachyon3-3.5.0/README.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      108 2024-04-02 19:54:40.991845 tachyon3-3.5.0/setup.cfg
+-rw-rw-r--   0 lph       (1000) lph       (1000)      549 2024-04-02 19:52:39.000000 tachyon3-3.5.0/setup.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      953 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)    13352 2022-02-15 17:31:06.000000 tachyon3-3.5.0/tachyon/__main__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      911 2024-04-02 19:53:00.000000 tachyon3-3.5.0/tachyon/__version__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1434 2022-02-15 17:31:06.000000 tachyon3-3.5.0/tachyon/conf.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5766 2024-04-02 19:52:39.000000 tachyon3-3.5.0/tachyon/config.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/data/
+-rw-rw-r--   0 lph       (1000) lph       (1000)    45377 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/data/files.json
+-rw-rw-r--   0 lph       (1000) lph       (1000)    29008 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/data/paths.json
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1286 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/database.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1880 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/dbutils.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2493 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/directoryfetcher.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2814 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/filefetcher.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5207 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/generator.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      989 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/har.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/heuristics/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1152 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/heuristics/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1358 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/heuristics/logbehaviorchange.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1673 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/heuristics/matchstring.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3804 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/heuristics/rejectignoredquery.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      337 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/heuristics/striptag.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1933 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/loaders.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3330 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/output.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/plugins/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      851 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/__init__.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/plugins/file/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      893 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/file/__init__.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon/plugins/host/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3581 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/HostProcessor.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2693 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/PathGenerator.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2506 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/Robots.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3131 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/SitemapXML.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     4739 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/Svn.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      956 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/plugins/host/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3274 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/result.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1467 2021-09-02 14:41:30.000000 tachyon3-3.5.0/tachyon/textutils.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2024-04-02 19:54:40.991845 tachyon3-3.5.0/tachyon3.egg-info/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      219 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1021 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/SOURCES.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        1 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/dependency_links.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       51 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/entry_points.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       67 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/requires.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        8 2024-04-02 19:54:40.000000 tachyon3-3.5.0/tachyon3.egg-info/top_level.txt
```

### Comparing `tachyon3-3.4.2/README.md` & `tachyon3-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/setup.py` & `tachyon3-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/__init__.py` & `tachyon3-3.5.0/tachyon/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/__main__.py` & `tachyon3-3.5.0/tachyon/__main__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/__version__.py` & `tachyon3-3.5.0/tachyon/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 59 Temple
 # Place, Suite 330, Boston, MA  02111-1307  USA
 
-__version__ = "3.4.2"
+__version__ = "3.5.0"
```

### Comparing `tachyon3-3.4.2/tachyon/conf.py` & `tachyon3-3.5.0/tachyon/conf.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/config.py` & `tachyon3-3.5.0/tachyon/config.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/data/files.json` & `tachyon3-3.5.0/tachyon/data/files.json`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/data/paths.json` & `tachyon3-3.5.0/tachyon/data/paths.json`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/database.py` & `tachyon3-3.5.0/tachyon/database.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/dbutils.py` & `tachyon3-3.5.0/tachyon/dbutils.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/directoryfetcher.py` & `tachyon3-3.5.0/tachyon/directoryfetcher.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/filefetcher.py` & `tachyon3-3.5.0/tachyon/filefetcher.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/generator.py` & `tachyon3-3.5.0/tachyon/generator.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/har.py` & `tachyon3-3.5.0/tachyon/har.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/heuristics/__init__.py` & `tachyon3-3.5.0/tachyon/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/heuristics/logbehaviorchange.py` & `tachyon3-3.5.0/tachyon/heuristics/logbehaviorchange.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/heuristics/matchstring.py` & `tachyon3-3.5.0/tachyon/heuristics/matchstring.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/heuristics/rejectignoredquery.py` & `tachyon3-3.5.0/tachyon/heuristics/rejectignoredquery.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/loaders.py` & `tachyon3-3.5.0/tachyon/loaders.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/output.py` & `tachyon3-3.5.0/tachyon/output.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/__init__.py` & `tachyon3-3.5.0/tachyon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/file/__init__.py` & `tachyon3-3.5.0/tachyon/plugins/file/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/HostProcessor.py` & `tachyon3-3.5.0/tachyon/plugins/host/HostProcessor.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/PathGenerator.py` & `tachyon3-3.5.0/tachyon/plugins/host/PathGenerator.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/Robots.py` & `tachyon3-3.5.0/tachyon/plugins/host/Robots.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/SitemapXML.py` & `tachyon3-3.5.0/tachyon/plugins/host/SitemapXML.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/Svn.py` & `tachyon3-3.5.0/tachyon/plugins/host/Svn.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/plugins/host/__init__.py` & `tachyon3-3.5.0/tachyon/plugins/host/__init__.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/result.py` & `tachyon3-3.5.0/tachyon/result.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon/textutils.py` & `tachyon3-3.5.0/tachyon/textutils.py`

 * *Files identical despite different names*

### Comparing `tachyon3-3.4.2/tachyon3.egg-info/SOURCES.txt` & `tachyon3-3.5.0/tachyon3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.cfg
 setup.py
 tachyon/__init__.py
 tachyon/__main__.py
 tachyon/__version__.py
 tachyon/conf.py
```

