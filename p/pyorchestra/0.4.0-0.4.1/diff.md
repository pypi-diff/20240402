# Comparing `tmp/pyorchestra-0.4.0.tar.gz` & `tmp/pyorchestra-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.4.0.tar", max compression
+gzip compressed data, was "pyorchestra-0.4.1.tar", max compression
```

## Comparing `pyorchestra-0.4.0.tar` & `pyorchestra-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     7652 2024-03-21 10:26:06.977153 pyorchestra-0.4.0/LICENSE
--rwxr-xr-x   0        0        0    25622 2024-03-21 10:26:06.977153 pyorchestra-0.4.0/README.md
--rwxr-xr-x   0        0        0       62 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     1045 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      208 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1170 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/main.py
--rwxr-xr-x   0        0        0     7208 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      519 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/backend.py
--rwxr-xr-x   0        0        0    19034 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/formatting.py
--rwxr-xr-x   0        0        0     1455 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/models.py
--rwxr-xr-x   0        0        0    10731 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-03-21 10:26:06.981153 pyorchestra-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/LICENSE
+-rwxr-xr-x   0        0        0    25622 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     1045 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      208 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1170 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/main.py
+-rwxr-xr-x   0        0        0     7208 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      519 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/backend.py
+-rwxr-xr-x   0        0        0    19098 2024-04-02 14:27:21.441410 pyorchestra-0.4.1/orchestra/core.py
+-rwxr-xr-x   0        0        0      873 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/formatting.py
+-rwxr-xr-x   0        0        0     1455 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/models.py
+-rwxr-xr-x   0        0        0    10731 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-02 14:27:21.445410 pyorchestra-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.4.1/PKG-INFO
```

### Comparing `pyorchestra-0.4.0/LICENSE` & `pyorchestra-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/README.md` & `pyorchestra-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/dto/job.py` & `pyorchestra-0.4.1/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/dto/run.py` & `pyorchestra-0.4.1/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/dto/task.py` & `pyorchestra-0.4.1/orchestra/api/dto/task.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/main.py` & `pyorchestra-0.4.1/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/routers/jobs.py` & `pyorchestra-0.4.1/orchestra/api/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/routers/tags.py` & `pyorchestra-0.4.1/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/api/routers/tasks.py` & `pyorchestra-0.4.1/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/backend.py` & `pyorchestra-0.4.1/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/core.py` & `pyorchestra-0.4.1/orchestra/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
                 scheduler_log = Run(
                     job=job_name,
                     module=module_name,
                     task=task_name,
                     task_id=task_meta.id,
                     schedule=job.type.name if job.max_attempts != 1 else "ONCE",
-                    timezone=job.datetime.tzname(),
+                    timezone=job.datetime.tzinfo.zone,
                     triggered_date=trigger_timestamp,
                 )
                 session.add(scheduler_log)
                 session.commit()
 
         celery_task.__name__ = task.name
         return celery_task
@@ -278,15 +278,16 @@
         return set([self.set_job_state_property(job, is_paused=True if job in self.paused_jobs else False) for job in jobs])
 
     def get_jobs(self, tags: set[str], any_tag: bool, include_paused: bool = True):
         # contrary to what get_jobs' docstring says, get_job will not return all jobs when tag is an empty set
         if len(tags) == 0:
             active_jobs = self.scheduler.get_jobs()
         else:
-            active_jobs = self.scheduler.get_jobs(tags, any_tag=any_tag)
+            active_jobs = set(filter(lambda job: job.tags.intersection(tags) if any_tag else job.tags == tags, self.scheduler.jobs))
+
         paused_jobs = set()
         if include_paused:
             paused_jobs = self.get_paused_jobs(tags, any_tag=any_tag)
 
         return self.apply_state_to_jobs(active_jobs.union(paused_jobs))
 
     def job_exists(self, job_name: str):
```

### Comparing `pyorchestra-0.4.0/orchestra/formatting.py` & `pyorchestra-0.4.1/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/models.py` & `pyorchestra-0.4.1/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/orchestra/scheduling.py` & `pyorchestra-0.4.1/orchestra/scheduling.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.4.0/pyproject.toml` & `pyorchestra-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.4.0"
+version = "0.4.1"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.4.0/PKG-INFO` & `pyorchestra-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.4.0
+Version: 0.4.1
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
```

