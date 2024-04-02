# Comparing `tmp/pipen_poplog-0.1.0.tar.gz` & `tmp/pipen_poplog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_poplog-0.1.0.tar", max compression
+gzip compressed data, was "pipen_poplog-0.1.1.tar", max compression
```

## Comparing `pipen_poplog-0.1.0.tar` & `pipen_poplog-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-02-05 21:08:25.565387 pipen_poplog-0.1.0/LICENSE
--rw-r--r--   0        0        0     2143 2024-02-05 21:08:25.565387 pipen_poplog-0.1.0/README.md
--rw-r--r--   0        0        0     4348 2024-02-05 21:08:25.565387 pipen_poplog-0.1.0/pipen_poplog.py
--rw-r--r--   0        0        0      828 2024-02-05 21:08:25.565387 pipen_poplog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 pipen_poplog-0.1.0/setup.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 pipen_poplog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-02 20:34:07.724548 pipen_poplog-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2143 2024-04-02 20:34:07.724548 pipen_poplog-0.1.1/README.md
+-rw-r--r--   0        0        0     4460 2024-04-02 20:34:07.724548 pipen_poplog-0.1.1/pipen_poplog.py
+-rw-r--r--   0        0        0      828 2024-04-02 20:34:07.724548 pipen_poplog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 pipen_poplog-0.1.1/setup.py
+-rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 pipen_poplog-0.1.1/PKG-INFO
```

### Comparing `pipen_poplog-0.1.0/LICENSE` & `pipen_poplog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_poplog-0.1.0/README.md` & `pipen_poplog-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pipen_poplog-0.1.0/pipen_poplog.py` & `pipen_poplog-0.1.1/pipen_poplog.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pipen.pluginmgr import plugin
 from pipen.utils import get_logger
 
 if TYPE_CHECKING:
     from pipen import Pipen, Proc
     from pipen.job import Job
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 PATTERN = r'\[PIPEN-POPLOG\]\[(?P<level>\w+?)\] (?P<message>.*)'
 logger = get_logger("poplog")
 levels = {"warn": "warning"}
 
 
 class PipenPoplogPlugin:
     """Populate logs from stdout/stderr to pipen runnning logs"""
@@ -116,15 +116,19 @@
 
     @plugin.impl
     async def on_job_succeeded(self, proc: Proc, job: Job):
         self._poplog(proc, job, end=True)
 
     @plugin.impl
     async def on_job_failed(self, proc: Proc, job: Job):
-        self._poplog(proc, job, end=True)
+        try:
+            self._poplog(proc, job, end=True)
+        except FileNotFoundError:
+            # In case the file is not there
+            pass
 
     @plugin.impl
     async def on_proc_done(self, proc: Proc, succeeded: bool | str):
         for handler in self.handlers.values():
             try:
                 handler.close()
             except Exception:
```

### Comparing `pipen_poplog-0.1.0/pyproject.toml` & `pipen_poplog-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-poplog"
-version = "0.1.0"
+version = "0.1.1"
 description = "Populate logs from jobs to running log of the pipeline"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-poplog"
 repository = "https://github.com/pwwang/pipen-poplog"
```

### Comparing `pipen_poplog-0.1.0/setup.py` & `pipen_poplog-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ['pipen>=0.14,<0.15']
 
 entry_points = \
 {'pipen': ['poplog = pipen_poplog:poplog_plugin']}
 
 setup_kwargs = {
     'name': 'pipen-poplog',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Populate logs from jobs to running log of the pipeline',
     'long_description': '# pipen-poplog\n\nPopulate logs from jobs to running log of the pipeline for [pipen][1].\n\n## Installation\n\n```bash\npip install -U pipen-poplog\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:log2file"]`, or uninstall this plugin.\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Poplog(Proc):\n    input = "var:var"\n    input_data = [0, 1, 2]\n    script = """\n        echo -n "[PIPEN-POPLOG][INFO] Log message "\n        sleep 1  # Simulate message not read in time\n        echo "by {{in.var}} 1"\n        sleep 1\n        echo "[PIPEN-POPLOG][ERROR] Log message by {{in.var}} 2"\n        sleep 1\n        echo "[PIPEN-POPLOG][INFO] Log message by {{in.var}} 3"\n    """\n\n\nif __name__ == "__main__":\n    Pipen().run()\n```\n\n```\n01-12 11:23:52 I core    ╭═══════════════ PoplogDefault ═════════════════╮\n01-12 11:23:52 I core    ║ A default poplog proc                         ║\n01-12 11:23:52 I core    ╰═══════════════════════════════════════════════╯\n01-12 11:23:52 I core    PoplogDefault: Workdir: \'.pipen/Pipeline/PoplogDefault\'\n01-12 11:23:52 I core    PoplogDefault: <<< [START]\n01-12 11:23:52 I core    PoplogDefault: >>> [END]\n01-12 11:23:56 I poplog  PoplogDefault: [0/2] Log message by 0 1\n01-12 11:23:59 E poplog  PoplogDefault: [0/2] Log message by 0 2\n01-12 11:24:02 I poplog  PoplogDefault: [0/2] Log message by 0 3\n```\n\n## Configuration\n\n- `plugin_opts.poplog_loglevel`: The log level for poplog. Default: `info`.\n- `plugin_opts.poplog_pattern`: The pattern to match the log message. Default: `r\'\\[PIPEN-POPLOG\\]\\[(?P<level>\\w+)\\] (?P<message>.*)\'`.\n- `plugin_opts.poplog_jobs`: The job indices to be populated. Default: `[0]` (the first job).\n- `plugin_opts.poplog_max`: The total max number of the log message to be poplutated. Default: `99`.\n- `plugin_opts.poplog_source`: The source of the log message. Default: `stdout`.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-poplog',
```

### Comparing `pipen_poplog-0.1.0/PKG-INFO` & `pipen_poplog-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-poplog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Populate logs from jobs to running log of the pipeline
 Home-page: https://github.com/pwwang/pipen-poplog
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

