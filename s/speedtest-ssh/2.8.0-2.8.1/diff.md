# Comparing `tmp/speedtest_ssh-2.8.0.tar.gz` & `tmp/speedtest_ssh-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtest_ssh-2.8.0.tar", last modified: Fri Jan 19 15:15:55 2024, max compression
+gzip compressed data, was "speedtest_ssh-2.8.1.tar", last modified: Tue Apr  2 10:06:52 2024, max compression
```

## Comparing `speedtest_ssh-2.8.0.tar` & `speedtest_ssh-2.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:15:55.344837 speedtest_ssh-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-19 15:15:55.340837 speedtest_ssh-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 15:15:55.344837 speedtest_ssh-2.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:15:55.340837 speedtest_ssh-2.8.0/speedtest_ssh/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/sftp_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/speedtest_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-19 15:15:47.000000 speedtest_ssh-2.8.0/speedtest_ssh/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:15:55.340837 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 15:15:55.000000 speedtest_ssh-2.8.0/speedtest_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:52.668882 speedtest_ssh-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-02 10:06:52.668882 speedtest_ssh-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:06:52.668882 speedtest_ssh-2.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:52.668882 speedtest_ssh-2.8.1/speedtest_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/sftp_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/speedtest_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 10:06:46.000000 speedtest_ssh-2.8.1/speedtest_ssh/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:52.668882 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 10:06:52.000000 speedtest_ssh-2.8.1/speedtest_ssh.egg-info/top_level.txt
```

### Comparing `speedtest_ssh-2.8.0/LICENSE` & `speedtest_ssh-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtest_ssh-2.8.0/PKG-INFO` & `speedtest_ssh-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtest_ssh
-Version: 2.8.0
+Version: 2.8.1
 Summary: A tool meant to check inter-device speeds via ssh
 License: GPL
 Project-URL: Homepage, https://github.com/zwimer/speedtest_ssh
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `speedtest_ssh-2.8.0/README.md` & `speedtest_ssh-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `speedtest_ssh-2.8.0/pyproject.toml` & `speedtest_ssh-2.8.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -54,7 +54,14 @@
 target-version = ["py312"]
 
 [tool.ruff]
 ignore = ["E731"]
 line-length = 120
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
+
+[tool.bandit]
+skips = ["B404", "B108"]
+
+[tool.vulture]
+ignore_names = ["cli"]
+paths = ["speedtest_ssh"]
```

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh/data_transfer.py` & `speedtest_ssh-2.8.1/speedtest_ssh/data_transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 if TYPE_CHECKING:
     from paramiko import SFTPClient
 
 
 __all__ = ("DataTransfer", "SFTP", "Rsync")
 
 
+_dict = string.ascii_uppercase + string.ascii_lowercase + string.digits
+
+
+def _rand_str(size: int) -> str:
+    return "".join(random.choice(_dict) for _ in range(size))  # nosec B311
+
+
 class ProgressBar(tqdm):
     """
     A small tqdm wrapper for paramiko's SFTP callbacks to use
     """
 
     def __init__(self, desc: str):
         super().__init__(desc=desc, unit="B", unit_scale=True, unit_divisor=1024, dynamic_ncols=True)
@@ -39,27 +46,26 @@
         if self.total is None:
             self.total = bytes_remaining
         self.update(bytes_done - self.n)
 
 
 class DataTransfer:
     """
-    A context mananger used to send and receive data to and from the remote client
+    A context manager used to send and receive data to and from the remote client
     This class is a context manager; on exit will remove the remote file on deletion
     """
 
     _LOG = "DataTransfer"
 
     def __init__(self, config: Config):
         """
         :param config: The Config object the DataTransfer instance should use
         """
         self._l = getLogger(self._LOG)
-        rand = lambda: random.choice(string.ascii_uppercase + string.ascii_lowercase + string.digits)
-        self._remote_f: str = f"/tmp/speedtest-ssh_{datetime.now()}_{''.join(rand() for _ in range(8))}.tmp"
+        self._remote_f: str = f"/tmp/speedtest-ssh_{datetime.now()}_{_rand_str(8)}.tmp"
         self._remote_f = self._remote_f.replace(":", "-").replace(" ", "_")
         # We promise that _remote_f components match: ^[a-zA-Z\d_.-]+$ (old rsync args suck)
         self._l.debug("Parsing ssh config and loading keys...")
         self._sftp_cm = sftp_wrapper(config)
         self._sftp: SFTPClient  # Defined in __enter__
 
     def __enter__(self) -> DataTransfer:
```

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh/ping.py` & `speedtest_ssh-2.8.1/speedtest_ssh/ping.py`

 * *Files identical despite different names*

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh/sftp_wrapper.py` & `speedtest_ssh-2.8.1/speedtest_ssh/sftp_wrapper.py`

 * *Files identical despite different names*

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh/speedtest_ssh.py` & `speedtest_ssh-2.8.1/speedtest_ssh/speedtest_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .config import Config
 from .data_transfer import DataTransfer, SFTP, Rsync
 from .ping import ping as ping_test
 from ._version import __version__
 
 
 base_size = 2 * (1024**2)
-_password_env_name = "SPEEDTEST_SSH_PASSWORD"
+_password_env_name = "SPEEDTEST_SSH_PASSWORD"  # nosec B105
 _LOG = "speedtest_ssh"
 
 
 def _iteration(temp: Path, client: DataTransfer, size: int) -> tuple[int, int]:
     """
     Time uploading and downloading a file of size bytes
     :param temp: A temporary file we have ownership of
```

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh/util.py` & `speedtest_ssh-2.8.1/speedtest_ssh/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,28 +39,28 @@
     """
     :param cmd: The command to run
     :param args: The arguments of cmd
     :param kwargs: Fowarded to subprocess.Popen
     :return: Completed process
     """
     _log_cmd(cmd, args)
-    return subprocess.run((cmd, *args), **kwargs)
+    return subprocess.run((cmd, *args), **kwargs)  # nosec B603
 
 
 def tee_cmd(cmd: Path, *args: str | Path, level: int, **kwargs) -> tuple[subprocess.Popen, str]:
     """
     :param cmd: The command to run (and info log the output of)
     :param args: The arguments of cmd
     :param level: The log level to use
     :param kwargs: Fowarded to subprocess.Popen aside from test and stdout
     :return: Completed process, stdout (do not read stdout from CompletedProcess)
     """
-    assert "text" not in kwargs
-    assert "stdout" not in kwargs
+    assert "text" not in kwargs  # nosec B101
+    assert "stdout" not in kwargs  # nosec B101
     log = getLogger(_LOG)
     _log_cmd(cmd, args)
-    p = subprocess.Popen((cmd, *args), text=True, stdout=subprocess.PIPE, **kwargs)
+    p = subprocess.Popen((cmd, *args), text=True, stdout=subprocess.PIPE, **kwargs)  # nosec B603
     stdout = ""
     for line in p.stdout:  # type: ignore
         log.log(level, line[:-1])
         stdout += line
     return p, stdout
```

### Comparing `speedtest_ssh-2.8.0/speedtest_ssh.egg-info/PKG-INFO` & `speedtest_ssh-2.8.1/speedtest_ssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtest_ssh
-Version: 2.8.0
+Version: 2.8.1
 Summary: A tool meant to check inter-device speeds via ssh
 License: GPL
 Project-URL: Homepage, https://github.com/zwimer/speedtest_ssh
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

