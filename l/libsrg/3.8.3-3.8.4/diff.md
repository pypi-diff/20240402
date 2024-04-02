# Comparing `tmp/libsrg-3.8.3-py3-none-any.whl.zip` & `tmp/libsrg-3.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,29 @@
-Zip file size: 36980 bytes, number of entries: 27
+Zip file size: 37449 bytes, number of entries: 27
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
--rw-r--r--  2.0 unx     1889 b- defN 23-Dec-10 17:14 libsrg/ElapsedTime.py
--rw-r--r--  2.0 unx     5015 b- defN 24-Mar-07 01:14 libsrg/Info.py
+-rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
+-rw-r--r--  2.0 unx     6514 b- defN 24-Apr-02 15:00 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
--rw-r--r--  2.0 unx     6093 b- defN 24-Mar-09 01:08 libsrg/LoggingAppBase.py
--rw-r--r--  2.0 unx     5891 b- defN 24-Feb-08 14:25 libsrg/LoggingCounter.py
+-rw-r--r--  2.0 unx     6093 b- defN 24-Apr-02 15:52 libsrg/LoggingAppBase.py
+-rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
 -rw-r--r--  2.0 unx     1376 b- defN 23-Jan-08 15:03 libsrg/LoggingWatcher.py
 -rw-r--r--  2.0 unx     2680 b- defN 23-Jan-31 15:30 libsrg/NagiosBase.py
 -rw-r--r--  2.0 unx    15682 b- defN 24-Feb-24 19:36 libsrg/ReZFS.py
--rw-r--r--  2.0 unx     5094 b- defN 24-Mar-08 15:58 libsrg/Runner.py
+-rw-r--r--  2.0 unx     5865 b- defN 24-Apr-02 15:44 libsrg/Runner.py
 -rw-r--r--  2.0 unx     4035 b- defN 23-May-22 23:46 libsrg/Runner2.py
 -rw-r--r--  2.0 unx     7024 b- defN 23-Oct-05 17:56 libsrg/Stage0.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 16:52 libsrg/__init__.py
--rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:35 libsrg/temp.py
+-rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:35 libsrg/template.py
 -rw-r--r--  2.0 unx    26527 b- defN 24-Jan-08 17:22 libsrg/ztool.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Mar-09 01:32 libsrg-3.8.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Mar-09 01:32 libsrg-3.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 01:32 libsrg-3.8.3.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Mar-09 01:32 libsrg-3.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2088 b- defN 24-Mar-09 01:32 libsrg-3.8.3.dist-info/RECORD
-27 files, 112178 bytes uncompressed, 33680 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2092 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/RECORD
+27 files, 114425 bytes uncompressed, 34141 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -39,15 +39,15 @@
 
 Filename: libsrg/Stage0.py
 Comment: 
 
 Filename: libsrg/__init__.py
 Comment: 
 
-Filename: libsrg/temp.py
+Filename: libsrg/template.py
 Comment: 
 
 Filename: libsrg/ztool.py
 Comment: 
 
 Filename: libsrg/TKGUI/GuiBase.py
 Comment: 
@@ -60,23 +60,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-3.8.3.dist-info/LICENSE.txt
+Filename: libsrg-3.8.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-3.8.3.dist-info/METADATA
+Filename: libsrg-3.8.4.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-3.8.3.dist-info/WHEEL
+Filename: libsrg-3.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-3.8.3.dist-info/top_level.txt
+Filename: libsrg-3.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-3.8.3.dist-info/RECORD
+Filename: libsrg-3.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/ElapsedTime.py

```diff
@@ -23,15 +23,15 @@
         self.start()
 
     def elapsed_asc(self) -> str:
         td = timedelta(seconds=self._elapsed)
         return str(td)
 
     def __str__(self):
-        return f"{self.name=} {self._starttime=} {self._endtime=} {self._elapsed=}"
+        return f"ET({self.name!r},{self.elapsed_asc()},{self._elapsed})"
 
     """records start time and zeros elapsed
     if called more than once, last call wipes any previous data"""
 
     def start(self):
         self._starttime = time()
         self._endtime = self._starttime
```

## libsrg/Info.py

```diff
@@ -1,56 +1,82 @@
 #! /usr/bin/env python3
 import configparser
 import logging
 import os
 import platform
 from importlib.metadata import version
 
+from libsrg.LoggingCounter import LoggingCounter
+from libsrg.Runner import ElapsedTime
 from libsrg.Runner import Runner
 
 
 class Info:
-    def __init__(self, hostname: str = None):
+    def __init__(self, hostname: str = None, timeout: int = 10, retries: int = 0):
         self.logger = logging.getLogger(self.__class__.__name__)
-
-        self.libsrg_ver = version('libsrg')
-        self.local_node = platform.node()
-        self.local_node_short = self.local_node.split('.')[0]
-        self.config = configparser.ConfigParser()
-        self.like_fedora=False
-        self.like_rhel=False
-        self.like_redhat=False
-        self.like_debian=False
-        self.userat=None
-        if hostname:
-            self.userat = f"root@{hostname}"
-            self.hostname = hostname
-        else:
+        self.kernel_dnf = None
+        self.boot_mode = None
+        self.uid = None
+        self.pretty_name = None
+        self.id_like = None
+        self.id = None
+        self.osrelease = None
+        self.ip = None
+        self.short = None
+        self.fqdn = None
+        self.kernel = None
+        self.machine = None
+        self.runtime = ElapsedTime("Info_runtime")
+        with self.runtime:
+            self.retries = retries
+            self.libsrg_ver = version('libsrg')
+            self.local_node = platform.node()
+            self.local_node_short = self.local_node.split('.')[0]
+            self.config = configparser.ConfigParser()
+            self.like_fedora = False
+            self.like_rhel = False
+            self.like_redhat = False
+            self.like_debian = False
             self.userat = None
-            self.hostname = self.local_node_short
-        rm = Runner("uname -m",userat=self.userat,rethrow=True,timeout=10,throw=True)
-        if not rm.success:
-            raise Exception(f"Command Failed {rm}")
-        self.machine= rm.so_lines[-1]
+            self.success = True
+            if hostname:
+                self.userat = f"root@{hostname}"
+                self.hostname = hostname
+            else:
+                self.userat = None
+                self.hostname = self.local_node_short
+            try:
+                self.inner(timeout=timeout, retries=retries)
+            except Exception as e:
+                self.success = False
+                self.logger.exception(e)
+
+    def inner(self, timeout: int = 10, retries: int = 0):
+        # return
+        rh = Runner(f"host {self.hostname}")
+        if not rh.success:
+            raise Exception(f"Failed name lookup for host {self.hostname}")
 
-        rk = Runner("uname -r",userat=self.userat,rethrow=True,timeout=10,throw=True)
-        self.kernel= rk.so_lines[-1]
+        rm = Runner("uname -m", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
+        self.machine = rm.so_lines[-1]
 
-        rfqdn = Runner("hostname -f", userat=self.userat,rethrow=True,timeout=10,throw=True)
+        rk = Runner("uname -r", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
+        self.kernel = rk.so_lines[-1]
+
+        rfqdn = Runner("hostname -f", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.fqdn = rfqdn.so_lines[-1]
 
-        rshort = Runner("hostname -s", userat=self.userat,rethrow=True,timeout=10,throw=True)
+        rshort = Runner("hostname -s", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.short = rshort.so_lines[-1]
 
-        rip = Runner("hostname -i", userat=self.userat,rethrow=True,timeout=10,throw=True)
+        rip = Runner("hostname -i", userat=self.userat, rethrow=True, timeout=timeout, throw=True, retries=retries)
         self.ip = rip.so_lines[-1]
 
-        r = Runner("cat /etc/os-release", userat=self.userat,rethrow=True,timeout=10,throw=True)
-        if not r.success:
-            raise Exception(f"os-release failed for {self.userat}")
+        r = Runner("cat /etc/os-release", userat=self.userat, rethrow=True, timeout=timeout, throw=True,
+                   retries=retries)
         data = r.so_lines
         # add a section header
         data.insert(0, "[osrelease]")
         self.config.read_string("\n".join(data))
         # for key in self.config:
         #     self.logger.info(key)
         osrelease = self.config['osrelease']
@@ -89,53 +115,59 @@
             self.like_debian = True
 
         self.like_redhat = self.like_fedora or self.like_rhel
 
         self.uid = os.getuid()
         bios = "ARM" if "aarch64" in self.machine else "BIOS"
         # These next few Runner calls may return non zero status
-        rhow = Runner(f"test -d /sys/firmware/efi", userat=self.userat,rethrow=True,timeout=10,throw=False)
-        self.uefi = "UEFI" if rhow.success else bios
+        rhow = Runner(f"test -d /sys/firmware/efi", userat=self.userat, rethrow=True, timeout=timeout, throw=True,
+                      retries=retries)
+        self.boot_mode = "UEFI" if rhow.success else bios
 
-        r2 = Runner("grep 'exclude=kernel' /etc/dnf/dnf.conf", userat=self.userat,rethrow=True,timeout=10,throw=False)
+        r2 = Runner("grep 'exclude=kernel' /etc/dnf/dnf.conf", userat=self.userat, rethrow=False, timeout=timeout,
+                    throw=False, retries=retries)
         ret = r2.ret
         if ret == 0:
-            self.kernel_dnf="locked"
+            self.kernel_dnf = "locked"
         elif ret == 1:
-            self.kernel_dnf="unlocked"
+            self.kernel_dnf = "unlocked"
         else:
-            self.kernel_dnf="NA"
+            self.kernel_dnf = "NA"
 
     def __str__(self):
         return f"Info({self.hostname=} {self.id=} {self.id_like=} {self.pretty_name=} {self.machine=})"
 
-    def is_root(self) ->bool:
+    def is_root(self) -> bool:
         return self.uid == 0
 
     def exit_if_not_root(self):
         if not self.is_root():
             self.logger.critical("Must run as root, uid={self.uid}, hostname={self.hostname}")
             exit(-1)
 
     def is_x86_64(self) -> bool:
         return self.machine == "x86_64"
 
     def dump(self):
-        #print(self)
-        for k, v in info.__dict__.items():
-            if k not in ["logger","config","osrelease"]:
+        # print(self)
+        for k, v in self.__dict__.items():
+            if k not in ["logger", "config", "osrelease"]:
                 print(f"{k}={v}")
-        for k,v in info.osrelease.items():
-            print(f"osrelease.{k}={v}")
+        if "osrelease" in self.__dict__ and self.__dict__["osrelease"]:
+            for k, v in self.osrelease.items():
+                print(f"osrelease.{k}={v}")
         print("-----------------------------------------------")
 
 
 if __name__ == '__main__':
     # info = Info("nas0")
-    info = Info()
-    info.dump()
-    # info = Info(hostname="nas0")
-    # info.dump()
-    # info = Info(hostname="nas1")
-    # info.dump()
-    err=Info("xxx")
-
+    LoggingCounter.config_and_attach()
+    for name in [None, "nas1", "web", "nowhere"]:
+        logging.info(f"start {name}")
+        t1 = ElapsedTime(f"Outer {name}")
+        print(name, "*" * 80)
+        with t1:
+            info = Info(name)
+        logging.info(f"returned {name} {info} {t1}")
+        with t1:
+            info.dump()
+        logging.info(f"dump complete {name} {t1}")
```

## libsrg/LoggingAppBase.py

```diff
@@ -116,17 +116,17 @@
             self.logger.info("^^^^^ that was supposed to throw an exception")
 
     def demo_final_checks(self):
         ctr = LoggingCounter.get_instance()
         self.logger.info("Asserts check actual versus expected logging counts as logged at end of run (atexit)")
         self.logger.info("  note that counters are frozen in atexit code, so atexit output does not change counts\n\n")
         assert ctr.count_for_level(logging.DEBUG) == 1
-        assert ctr.count_for_level(logging.INFO) == 21
+        assert ctr.count_for_level(logging.INFO) == 15
         assert ctr.count_for_level(logging.WARNING) == 1
-        assert ctr.count_for_level(logging.ERROR) == 3
+        assert ctr.count_for_level(logging.ERROR) == 2
         assert ctr.count_for_level(logging.CRITICAL) == 1
 
     @classmethod
     def demo(cls):
         app = SampleApp()
         app.demo_levels()
         app.demo_runner()
```

## libsrg/LoggingCounter.py

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env  python3
 
 import atexit
-import datetime
 import logging
 import sys
 import time
 from collections import Counter
 from importlib.metadata import version
 from typing import List
```

## libsrg/Runner.py

```diff
@@ -3,14 +3,15 @@
 import subprocess
 from pathlib import Path
 from typing import List, Optional, Union, Dict
 
 from libsrg.ElapsedTime import ElapsedTime
 
 
+
 class Runner:
     """
     Runner is a utility class to run a command as a subprocess and return results
     * command is passed as a list of program followed by zero or more arguments
       * if provided as a single string, call split to make it a list
     * Runner objects are single use
       * command executed by constructor
@@ -29,15 +30,17 @@
     """
 
     def __init__(self, cmd: Union[List[str], str], timeout=None, rethrow=False, verbose=False, throw=False,
                  cwd: Optional[Union[str, Path]] = None,
                  userat: Optional[str] = None,
                  env: Optional[Dict[str, str]] = None,
                  inherit_env: bool = False,
-                 logger: Optional[logging.Logger] = None
+                 logger: Optional[logging.Logger] = None,
+                 retries: int = 0,
+
                  ):
         """
         Run the given command and return results
 
         :param cmd: A list of strings, or a single string which Runner will str.split()
         :param timeout: If positive, number of seconds before a timeout exception is raised
         :param rethrow: If true, rethrow any exceptions caught, else success set False
@@ -56,28 +59,29 @@
             self._cmd = cmd.split()
         else:
             self._cmd = cmd
         if userat:
             self._cmd = ["ssh", userat] + self._cmd
         # timeout (if specified) is a timeout to communicate in seconds
         self.env = os.environ if inherit_env else env
-
+        self.allowed_tries = retries + 1
+        self.try_number = 0
         self.timeout = timeout
         self.userat = userat
         self.success = False
         self.so_bytes: bytearray
         self.se_bytes: bytearray
         self.verbose = verbose
         self.cwd = cwd
         self.ret: int = -1
         self.so_lines: List[str] = []
         self.se_lines: List[str] = []
         self.caught: Optional[Exception] = None
         self.p = None
-        self.throw=throw
+        self.throw = throw
         self.rethrow = rethrow
         with self.runtime:
             self._run_subprocess()
         if throw and not self.success:
             self.log()
             raise Exception(f"Runner failed {self}")
         if verbose:
@@ -96,31 +100,50 @@
             if throw:
                 raise ChildProcessError(str(self))
 
     def raise_if_failed(self, lgr: logging.Logger = None, ):
         self.log(lgr=lgr, throw=True)
 
     def _run_subprocess(self):
-        if self.verbose:
-            self.logger.debug(self._cmd)
-        try:
-            self.p = subprocess.Popen(self._cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=self.cwd,
-                                      env=self.env
-                                      )
-            (self.so_bytes, self.se_bytes) = self.p.communicate(timeout=self.timeout)
-            self.ret = self.p.wait()
-            so_str0 = self.so_bytes.decode("utf-8")
-            self.so_lines = so_str0.splitlines(keepends=False)
-            se_str0 = self.se_bytes.decode("utf-8")
-            self.se_lines = se_str0.splitlines(keepends=False)
-            self.success = self.ret == 0
-        except Exception as ex:
-            self.logger.error(ex)
-            self.success = False
-            self.caught = ex
-            if self.rethrow:
-                raise ex
+        for self.try_number in range(self.allowed_tries):
+            if self.verbose:
+                self.logger.debug(self._cmd)
+            try:
+                self.p = subprocess.Popen(self._cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=self.cwd,
+                                          env=self.env
+                                          )
+                (self.so_bytes, self.se_bytes) = self.p.communicate(timeout=self.timeout)
+                self.ret = self.p.wait()
+                so_str0 = self.so_bytes.decode("utf-8")
+                self.so_lines = so_str0.splitlines(keepends=False)
+                se_str0 = self.se_bytes.decode("utf-8")
+                self.se_lines = se_str0.splitlines(keepends=False)
+                self.success = self.ret == 0
+                if self.success:
+                    return
+            except Exception as ex:
+                self.logger.error(ex)
+                self.success = False
+                self.caught = ex
+        if self.rethrow and self.caught:
+            raise self.caught
 
     def __str__(self):
         # noinspection PyPep8
         cstr = " ".join(self._cmd)
         return f'Runner(success={self.success} ret={self.ret} cstr="{cstr}" runtime={self.runtime.elapsed():5.3f} so_lines={self.so_lines} se_lines={self.se_lines} userat={self.userat})'
+
+if __name__ == "__main__":
+    from libsrg.LoggingCounter import LoggingCounter
+    LoggingCounter.config_and_attach()
+
+    runner = Runner("sleep 5",timeout=10)
+    print(runner)
+    print(runner.try_number,runner.allowed_tries)
+
+    runner = Runner("sleep 5",timeout=3)
+    print(runner)
+    print(runner.try_number,runner.allowed_tries)
+
+    runner = Runner("sleep 5",timeout=3,retries=2)
+    print(runner)
+    print(runner.try_number,runner.allowed_tries)
```

## Comparing `libsrg/temp.py` & `libsrg/template.py`

 * *Files identical despite different names*

## Comparing `libsrg-3.8.3.dist-info/LICENSE.txt` & `libsrg-3.8.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-3.8.3.dist-info/METADATA` & `libsrg-3.8.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 3.8.3
+Version: 3.8.4
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-3.8.3.dist-info/RECORD` & `libsrg-3.8.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
-libsrg/ElapsedTime.py,sha256=-rkCEvfq_lY3qxKWcWV7ItjKzXt8mylcbneJsDdbC_E,1889
-libsrg/Info.py,sha256=TycGz2J8NjqAOqpuwYk_4qGk7U289TOch7ofU0dlFJE,5015
+libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
+libsrg/Info.py,sha256=0b5hU-Hc8Vut-04fppvPAMwGCWhMKWLkBc7wVsf3QH4,6514
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
-libsrg/LoggingAppBase.py,sha256=YLt8xC0Auautv2zyTnuSHhvS33cYTWfOgOile-IxYMk,6093
-libsrg/LoggingCounter.py,sha256=goyWtieXpkI0aSqkYQfmJ_ojkQR1mq0upyEgklxNalM,5891
+libsrg/LoggingAppBase.py,sha256=7-eaWR0QyPbpG7MSb_56lEsYREbQnKpJFypRM3o0fcQ,6093
+libsrg/LoggingCounter.py,sha256=42YlyNOvebDk9c1kXhSzklPD-nlzxDz6DkwfApw8p80,5875
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
 libsrg/LoggingWatcher.py,sha256=tZ803wbw_qvW8tSRDwAbBRQSCrMzhz-FIJsf_hCNIFo,1376
 libsrg/NagiosBase.py,sha256=5FniCUJ8ywFX8oM2q0gKQX2Wvz6J6yt0HT_WYfPniik,2680
 libsrg/ReZFS.py,sha256=zyWTZVehgq2ibQrBEz8tCnei6KdjS9KXdpSjQSSRJ6M,15682
-libsrg/Runner.py,sha256=Pkf2vwNCZfTiwzOjRGF_4vwN_cH8QW6pIc4fV-s2YZU,5094
+libsrg/Runner.py,sha256=oqA-b5CEp9n6mc2Oq2wiIk337yMNAVZuhK-m9X-XwpM,5865
 libsrg/Runner2.py,sha256=UDgEAku-g5y9xRrAmr5ZYc4FpZ8rbxSTVX03DV07J8Q,4035
 libsrg/Stage0.py,sha256=xK8a5mCAlwXzpOgSvnj0elD65cT3RYYb3ubCkAGp8nw,7024
 libsrg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-libsrg/temp.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
+libsrg/template.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
 libsrg/ztool.py,sha256=vnBTbN6cTqaTF6JukVeoOBrXJ3eCu1uIv3qhBrUAGzo,26527
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=A2XBTtlvtNwnxFlw8xTkHkuCITxvgZlQfWjWeaAmejQ,10692
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-3.8.3.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-3.8.3.dist-info/METADATA,sha256=veKBGXaL-5MGHL8yLWOCP8XcFf88ykksbEn8W6eQhU8,3357
-libsrg-3.8.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-libsrg-3.8.3.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-3.8.3.dist-info/RECORD,,
+libsrg-3.8.4.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-3.8.4.dist-info/METADATA,sha256=2TM0LxGU-EKv5ck5lC4NwxfO0V8nd-A-bFJfc1YTb_c,3357
+libsrg-3.8.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-3.8.4.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-3.8.4.dist-info/RECORD,,
```

