# Comparing `tmp/neon-skill-speed_test-1.0.2a1.tar.gz` & `tmp/neon-skill-speed_test-1.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-speed_test-1.0.2a1.tar", last modified: Mon Feb  5 23:34:01 2024, max compression
+gzip compressed data, was "neon-skill-speed_test-1.0.2a2.tar", last modified: Tue Apr  2 20:54:34 2024, max compression
```

## Comparing `neon-skill-speed_test-1.0.2a1.tar` & `neon-skill-speed_test-1.0.2a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.338983 neon-skill-speed_test-1.0.2a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.338983 neon-skill-speed_test-1.0.2a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/locale/en-us/dialog/notify_testing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/locale/en-us/dialog/results.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/locale/en-us/dialog/start_test.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/locale/en-us/intent/run_speed_test.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-05 23:34:01.000000 neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:34:01.342983 neon-skill-speed_test-1.0.2a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 23:33:58.000000 neon-skill-speed_test-1.0.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/notify_testing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/results.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/dialog/start_test.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/locale/en-us/intent/run_speed_test.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 20:54:34.000000 neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:34.575796 neon-skill-speed_test-1.0.2a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 20:54:24.000000 neon-skill-speed_test-1.0.2a2/version.py
```

### Comparing `neon-skill-speed_test-1.0.2a1/LICENSE.md` & `neon-skill-speed_test-1.0.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/PKG-INFO` & `neon-skill-speed_test-1.0.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed_test
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.2a1/README.md` & `neon-skill-speed_test-1.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/__init__.py` & `neon-skill-speed_test-1.0.2a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/neon_skill_speed_test.egg-info/PKG-INFO` & `neon-skill-speed_test-1.0.2a2/neon_skill_speed_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speed-test
-Version: 1.0.2a1
+Version: 1.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-speed_test
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-speed_test-1.0.2a1/setup.py` & `neon-skill-speed_test-1.0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/skill.json` & `neon-skill-speed_test-1.0.2a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/test/test_skill.py` & `neon-skill-speed_test-1.0.2a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speed_test-1.0.2a1/version.py` & `neon-skill-speed_test-1.0.2a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.2a1"
+__version__ = "1.0.2a2"
```

